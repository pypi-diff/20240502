# Comparing `tmp/google_cloud_jupyter_config-0.0.7.tar.gz` & `tmp/google_cloud_jupyter_config-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_cloud_jupyter_config-0.0.7.tar", last modified: Fri Apr 26 22:31:49 2024, max compression
+gzip compressed data, was "google_cloud_jupyter_config-0.0.8.tar", last modified: Thu May  2 17:05:52 2024, max compression
```

## Comparing `google_cloud_jupyter_config-0.0.7.tar` & `google_cloud_jupyter_config-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)    11358 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/LICENSE
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       15 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/MANIFEST.in
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/PKG-INFO
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1682 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/README.md
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.428094 google_cloud_jupyter_config-0.0.7/google/
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.428094 google_cloud_jupyter_config-0.0.7/google/cloud/
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      830 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/__init__.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     6495 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/config.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2588 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/config_test.py
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2909 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/tokenrenewer.py
-drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/PKG-INFO
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      467 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/SOURCES.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        1 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/dependency_links.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       43 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/requires.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       12 2024-04-26 22:31:49.000000 google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/top_level.txt
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       67 2024-04-26 22:31:49.429093 google_cloud_jupyter_config-0.0.7/setup.cfg
--rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1216 2024-04-26 22:29:06.000000 google_cloud_jupyter_config-0.0.7/setup.py
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.341249 google_cloud_jupyter_config-0.0.8/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)    11358 2023-08-11 16:50:41.000000 google_cloud_jupyter_config-0.0.8/LICENSE
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       15 2023-08-11 16:50:41.000000 google_cloud_jupyter_config-0.0.8/MANIFEST.in
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-05-02 17:05:52.340249 google_cloud_jupyter_config-0.0.8/PKG-INFO
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1682 2023-08-11 16:50:41.000000 google_cloud_jupyter_config-0.0.8/README.md
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.337249 google_cloud_jupyter_config-0.0.8/google/
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.338249 google_cloud_jupyter_config-0.0.8/google/cloud/
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.340249 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      830 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/__init__.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     5387 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2588 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config_test.py
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2909 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/tokenrenewer.py
+drwxr-xr-x   0 ojarjur   (1000) ojarjur   (1000)        0 2024-05-02 17:05:52.340249 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     2139 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/PKG-INFO
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)      467 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)        1 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       43 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/requires.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       12 2024-05-02 17:05:52.000000 google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/top_level.txt
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)       67 2024-05-02 17:05:52.341249 google_cloud_jupyter_config-0.0.8/setup.cfg
+-rw-r--r--   0 ojarjur   (1000) ojarjur   (1000)     1254 2024-05-02 17:04:51.000000 google_cloud_jupyter_config-0.0.8/setup.py
```

### Comparing `google_cloud_jupyter_config-0.0.7/LICENSE` & `google_cloud_jupyter_config-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.7/PKG-INFO` & `google_cloud_jupyter_config-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-jupyter-config
-Version: 0.0.7
+Version: 0.0.8
 Summary: Jupyter configuration utilities using gcloud
 Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config
 Author: Google, Inc.
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google_cloud_jupyter_config-0.0.7/README.md` & `google_cloud_jupyter_config-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/__init__.py` & `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/__init__.py`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/config.py` & `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -44,79 +44,49 @@
             encoding="UTF-8",
             shell=True,
         )
         t.seek(0)
         return t.read().decode("UTF-8").strip()
 
 
-@cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=60))
+@cachetools.cached(cache=cachetools.TTLCache(maxsize=1024, ttl=(20 * 60)))
 def cached_gcloud_subcommand(subcmd):
     return run_gcloud_subcommand(subcmd)
 
 
 def clear_gcloud_cache():
     """Clear the TTL cache used to cache gcloud subcommand results."""
     cached_gcloud_subcommand.cache_clear()
 
 
 def get_gcloud_config(field):
     """Helper method that invokes the gcloud config helper.
 
     Invoking gcloud commands is a very heavyweight process, so the config is
-    cached for up to 1 minute.
+    cached for up to 20 minutes.
+
+    The config is generated with a minimum credential expiry of 30 minutes, so
+    that we can ensure that the caller can use the cached credentials for at
+    least ~10 minutes even if the cache entry is about to expire.
 
     Args:
         field: A period-separated search path for the config value to return.
                For example, 'configuration.properties.core.project'
     Returns:
         A JSON object whose type depends on the search path for the field within
         the gcloud config.
 
         For example, if the field is `configuration.properties.core.project`,
         then the return value will be a string. In comparison, if the field
         is `configuration.properties.core`, then the return value will be a
         dictionary containing a field named `project` with a string value.
     """
-
-    def validate_credentials(config):
-        """Validate that the credentials in the given config are still valid.
-
-        We require the credentials to have a remaining TTL greater than 60 seconds
-        in order to be considered still valid. This ensures that any caller has
-        a reasonable amount of time remaining to use those credentials.
-        """
-        creds = config.get("credential", None)
-        if not creds:
-            return False
-        access_token = creds.get("access_token", None)
-        if not access_token:
-            return False
-        token_expiry = creds.get("token_expiry", None)
-        if not token_expiry:
-            # If we do not know when the credential expires then just
-            # rely on the cache TTL to refresh the tokens.
-            return True
-        try:
-            expiry_datetime = datetime.datetime.strptime(
-                token_expiry, "%Y-%m-%dT%H:%M:%SZ"
-            )
-            remaining_seconds = (
-                expiry_datetime - datetime.datetime.utcnow()
-            ).total_seconds()
-            return remaining_seconds > 60
-        except ValueError:
-            return False
-
-    subcommand = "config config-helper --format=json"
+    subcommand = "config config-helper --min-expiry=30m --format=json"
     cached_config_str = cached_gcloud_subcommand(subcommand)
     cached_config = json.loads(cached_config_str)
-    if not validate_credentials(cached_config):
-        clear_gcloud_cache()
-        cached_config_str = cached_gcloud_subcommand(subcommand)
-        cached_config = json.loads(cached_config_str)
 
     subconfig = cached_config
     for path_part in field.split("."):
         if path_part:
             subconfig = subconfig.get(path_part, {})
 
     return subconfig
```

### Comparing `google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/config_test.py` & `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/config_test.py`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.7/google/cloud/jupyter_config/tokenrenewer.py` & `google_cloud_jupyter_config-0.0.8/google/cloud/jupyter_config/tokenrenewer.py`

 * *Files identical despite different names*

### Comparing `google_cloud_jupyter_config-0.0.7/google_cloud_jupyter_config.egg-info/PKG-INFO` & `google_cloud_jupyter_config-0.0.8/google_cloud_jupyter_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-jupyter-config
-Version: 0.0.7
+Version: 0.0.8
 Summary: Jupyter configuration utilities using gcloud
 Home-page: https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config
 Author: Google, Inc.
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `google_cloud_jupyter_config-0.0.7/setup.py` & `google_cloud_jupyter_config-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import setuptools
 
 with open("README.md", "r") as fh:
-  long_description = fh.read()
+    long_description = fh.read()
 
 setuptools.setup(
-  name="google-cloud-jupyter-config",
-  author="Google, Inc.",
-  version="0.0.7",
-  description="Jupyter configuration utilities using gcloud",
-  long_description=long_description,
-  long_description_content_type="text/markdown",
-  url="https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config",
-  license="Apache License 2.0",
-  packages=setuptools.find_namespace_packages(),
-  python_requires=">=3.8",
-  install_requires=[
-    "cachetools",
-    "jupyter_server>=2.4.0",
-    "traitlets",
-  ],
+    name="google-cloud-jupyter-config",
+    author="Google, Inc.",
+    version="0.0.8",
+    description="Jupyter configuration utilities using gcloud",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/GoogleCloudPlatform/jupyter-extensions/tree/master/google-cloud-jupyter-config",
+    license="Apache License 2.0",
+    packages=setuptools.find_namespace_packages(),
+    python_requires=">=3.8",
+    install_requires=[
+        "cachetools",
+        "jupyter_server>=2.4.0",
+        "traitlets",
+    ],
 )
```

