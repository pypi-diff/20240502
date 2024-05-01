# Comparing `tmp/bitbucket_pipeline_runner-0.4.1.tar.gz` & `tmp/bitbucket_pipeline_runner-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket_pipeline_runner-0.4.1.tar", max compression
+gzip compressed data, was "bitbucket_pipeline_runner-0.4.2.tar", max compression
```

## Comparing `bitbucket_pipeline_runner-0.4.1.tar` & `bitbucket_pipeline_runner-0.4.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1070 2024-04-15 21:35:07.074115 bitbucket_pipeline_runner-0.4.1/LICENSE
--rw-r--r--   0        0        0     1046 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/README.md
--rw-r--r--   0        0        0       29 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/__init__.py
--rw-r--r--   0        0        0       61 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/__main__.py
--rw-r--r--   0        0        0     3057 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/artifacts.py
--rw-r--r--   0        0        0    10673 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/cache.py
--rw-r--r--   0        0        0     5267 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/cli.py
--rw-r--r--   0        0        0     3227 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/config.py
--rw-r--r--   0        0        0    17315 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/container.py
--rw-r--r--   0        0        0     5831 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/context.py
--rw-r--r--   0        0        0      608 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/errors.py
--rw-r--r--   0        0        0    14998 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/models.py
--rw-r--r--   0        0        0      357 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/parse.py
--rw-r--r--   0        0        0        0 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/py.typed
--rw-r--r--   0        0        0     4193 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/repository.py
--rw-r--r--   0        0        0    15676 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/runner.py
--rw-r--r--   0        0        0     9283 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/service.py
--rw-r--r--   0        0        0        0 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/__init__.py
--rw-r--r--   0        0        0     1665 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/known_hosts
--rwxr-xr-x   0        0        0      451 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/runit.sh
--rw-r--r--   0        0        0     4331 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pipeline_runner/utils.py
--rw-r--r--   0        0        0     2844 2024-04-15 21:35:07.078115 bitbucket_pipeline_runner-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1046 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/README.md
+-rw-r--r--   0        0        0       29 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/__main__.py
+-rw-r--r--   0        0        0     3057 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/artifacts.py
+-rw-r--r--   0        0        0    10673 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/cache.py
+-rw-r--r--   0        0        0     5267 2024-05-01 22:12:59.144712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/cli.py
+-rw-r--r--   0        0        0     3227 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/config.py
+-rw-r--r--   0        0        0    18041 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/container.py
+-rw-r--r--   0        0        0     5831 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/context.py
+-rw-r--r--   0        0        0      608 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/errors.py
+-rw-r--r--   0        0        0    14998 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/models.py
+-rw-r--r--   0        0        0      357 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/parse.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/py.typed
+-rw-r--r--   0        0        0     4193 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/repository.py
+-rw-r--r--   0        0        0    15676 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/runner.py
+-rw-r--r--   0        0        0     9283 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/service.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/__init__.py
+-rw-r--r--   0        0        0     1665 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/known_hosts
+-rwxr-xr-x   0        0        0      451 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/runit.sh
+-rw-r--r--   0        0        0     4331 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pipeline_runner/utils.py
+-rw-r--r--   0        0        0     2844 2024-05-01 22:12:59.148712 bitbucket_pipeline_runner-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2308 1970-01-01 00:00:00.000000 bitbucket_pipeline_runner-0.4.2/PKG-INFO
```

### Comparing `bitbucket_pipeline_runner-0.4.1/LICENSE` & `bitbucket_pipeline_runner-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/README.md` & `bitbucket_pipeline_runner-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/artifacts.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/artifacts.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/cache.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/cache.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/cli.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/cli.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/config.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/config.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/container.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/container.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,18 +140,19 @@
 
         volumes = self._get_volumes()
         environment = self._environment.copy()
 
         opts = {"cpu_period": 100000, "cpu_quota": 400000, "cpu_shares": 4096} if config.cpu_limits else {}
 
         if config.expose_ssh_agent:
-            if ssh_sock_path := os.environ.get("SSH_AUTH_SOCK"):
+            ssh_agent_socket_path = get_ssh_agent_socket_path(self._client)
+
+            if ssh_agent_socket_path:
                 logger.info("Mounting ssh agent in container")
-                ssh_sock_path = os.path.realpath(os.path.expanduser(ssh_sock_path))
-                volumes[ssh_sock_path] = {"bind": "/ssh-agent"}
+                volumes[ssh_agent_socket_path] = {"bind": "/ssh-agent"}
                 environment["SSH_AUTH_SOCK"] = "/ssh-agent"
             else:
                 logger.warning("No running ssh agent available")
 
         container = self._client.containers.run(
             self._image.name,
             name=self._name,
@@ -466,15 +467,15 @@
     except docker.errors.NotFound:
         if client.images.get(image.name):
             logger.warning("Image not found on remote, but exists locally: %s", image.name)
         else:
             raise
     except docker.errors.APIError:
         if client.images.get(image.name):
-            logger.warning("Error fetching new version of image, falling back to curent one: %s", image.name)
+            logger.warning("Error fetching new version of image, falling back to current one: %s", image.name)
         else:
             raise
 
     _pulled_images.add(image.name)
 
 
 def get_image_authentication(image: Image) -> dict[str, str] | None:
@@ -505,7 +506,32 @@
     if image.username and image.password:
         return {
             "username": image.username,
             "password": image.password,
         }
 
     return None
+
+
+def get_ssh_agent_socket_path(client: DockerClient) -> str | None:
+    ssh_sock_path: str | None
+
+    if docker_is_docker_desktop(client):
+        logger.debug("Using docker desktop's host service ssh agent")
+        ssh_sock_path = "/run/host-services/ssh-auth.sock"
+    elif ssh_sock_path := os.environ.get("SSH_AUTH_SOCK"):
+        logger.debug("Using ssh agent specified by $SSH_AUTH_SOCK")
+    else:
+        return None
+
+    return os.path.realpath(os.path.expanduser(ssh_sock_path))
+
+
+def docker_is_docker_desktop(client: DockerClient) -> bool:
+    platform_name: str
+
+    try:
+        platform_name = client.version()["Platform"]["Name"]
+    except KeyError:
+        platform_name = ""
+
+    return platform_name.startswith("Docker Desktop ")
```

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/context.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/context.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/errors.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/errors.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/models.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/models.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/repository.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/repository.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/runner.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/runner.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/service.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/service.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/static/known_hosts` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/static/known_hosts`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pipeline_runner/utils.py` & `bitbucket_pipeline_runner-0.4.2/pipeline_runner/utils.py`

 * *Files identical despite different names*

### Comparing `bitbucket_pipeline_runner-0.4.1/pyproject.toml` & `bitbucket_pipeline_runner-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bitbucket-pipeline-runner"
-version = "0.4.1"
+version = "0.4.2"
 description = "Run a bitbucket pipeline locally"
 authors = ["Mathieu Lemay <acidrain1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mathieu-lemay/pipeline-runner"
 packages = [
     {include = "pipeline_runner"}
```

### Comparing `bitbucket_pipeline_runner-0.4.1/PKG-INFO` & `bitbucket_pipeline_runner-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbucket-pipeline-runner
-Version: 0.4.1
+Version: 0.4.2
 Summary: Run a bitbucket pipeline locally
 Home-page: https://github.com/mathieu-lemay/pipeline-runner
 License: MIT
 Author: Mathieu Lemay
 Author-email: acidrain1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

