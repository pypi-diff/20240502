# Comparing `tmp/kubernator-1.0.8.tar.gz` & `tmp/kubernator-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernator-1.0.8.tar", last modified: Wed Dec 20 19:31:11 2023, max compression
+gzip compressed data, was "kubernator-1.0.9.tar", last modified: Sun Dec 24 17:40:59 2023, max compression
```

## Comparing `kubernator-1.0.8.tar` & `kubernator-1.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 19:31:11.152113 kubernator-1.0.8/
--rw-rw-r--   0 runner    (1001) docker     (127)       27 2023-12-20 19:24:36.000000 kubernator-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2023-12-20 19:31:11.152113 kubernator-1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 19:31:11.148113 kubernator-1.0.8/kubernator/
--rw-r--r--   0 runner    (1001) docker     (127)    11387 2023-12-20 19:24:36.000000 kubernator-1.0.8/kubernator/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-20 19:24:36.000000 kubernator-1.0.8/kubernator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24820 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 19:31:11.152113 kubernator-1.0.8/kubernator/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/awscli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/eks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/istio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20248 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)    26000 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/k8s_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/kops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/minikube.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/plugins/terragrunt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2023-12-20 19:23:55.000000 kubernator-1.0.8/kubernator/proc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 19:31:11.148113 kubernator-1.0.8/kubernator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 19:31:11.000000 kubernator-1.0.8/kubernator.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 19:31:11.152113 kubernator-1.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)    11700 2023-12-20 19:24:36.000000 kubernator-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 17:40:59.614107 kubernator-1.0.9/
+-rw-rw-r--   0 runner    (1001) docker     (127)       27 2023-12-24 17:30:28.000000 kubernator-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2023-12-24 17:40:59.614107 kubernator-1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 17:40:59.610107 kubernator-1.0.9/kubernator/
+-rw-r--r--   0 runner    (1001) docker     (127)    11387 2023-12-24 17:30:28.000000 kubernator-1.0.9/kubernator/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2023-12-24 17:30:28.000000 kubernator-1.0.9/kubernator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24951 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 17:40:59.614107 kubernator-1.0.9/kubernator/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/awscli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/eks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10525 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/istio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20248 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26000 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/k8s_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/kops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10147 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/minikube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/plugins/terragrunt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2023-12-24 17:29:45.000000 kubernator-1.0.9/kubernator/proc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-24 17:40:59.614107 kubernator-1.0.9/kubernator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-24 17:40:59.000000 kubernator-1.0.9/kubernator.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-24 17:40:59.614107 kubernator-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11834 2023-12-24 17:30:28.000000 kubernator-1.0.9/setup.py
```

### Comparing `kubernator-1.0.8/PKG-INFO` & `kubernator-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Kubernator is the a pluggable framework for K8S provisioning
 Home-page: https://github.com/karellen/kubernator
 Author: Express Systems USA, Inc.
 Author-email: 
 Maintainer: Karellen, Inc., Arcadiy Ivanov
 Maintainer-email: supervisor@karellen.co,arcadiy@karellen.co
 License: Apache License, Version 2.0
@@ -78,14 +78,22 @@
 ## Using Kubernator with Docker
 
 A simple example is as follows:
 ```
 $ docker run --mount type=bind,source="$(pwd)",target=/root,readonly -t ghcr.io/karellen/kubernator:latest
 ```
 
+## Using Kubernator on MacOS
+
+```
+$ brew install python3.11
+$ pip3.11 install `kubernator~=1.0.9`
+$ kubernator --version
+```
+
 Please note, that some plugins (e.g. `awscli`, `eks`) may require additional volume mounts or environmental
 variables to be passed for credentials and other external configuration.
 
 ## Mode of Operation
 
 Kubernator is a command line utility. Upon startup and processing of the command line arguments and initializing
 logging, Kubernator initializes plugins. Current plugins include:
```

### Comparing `kubernator-1.0.8/kubernator/LICENSE` & `kubernator-1.0.9/kubernator/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/__init__.py` & `kubernator-1.0.9/kubernator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 
 def _main():
     from kubernator import app
     return app.main() or 0
```

### Comparing `kubernator-1.0.8/kubernator/__main__.py` & `kubernator-1.0.9/kubernator/__main__.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/api.py` & `kubernator-1.0.9/kubernator/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,16 +231,17 @@
 def install_python_k8s_client(run, package_major, logger_stdout, logger_stderr):
     cache_dir = get_cache_dir("python")
     package_major_dir = cache_dir / str(package_major)
 
     if not package_major_dir.exists():
         package_major_dir.mkdir(parents=True, exist_ok=True)
 
-        run(["pip", "install", "--no-deps", "--no-cache-dir", "--no-input", "--target", str(package_major_dir),
-             f"kubernetes~={package_major}.0"], logger_stdout, logger_stderr).wait()
+        run([sys.executable, "-m", "pip", "install", "--no-deps", "--no-cache-dir", "--no-input", "--pre",
+             "--root-user-action=ignore", "--break-system-packages", "--disable-pip-version-check",
+             "--target", str(package_major_dir), f"kubernetes~={package_major}.0"], logger_stdout, logger_stderr).wait()
 
     return package_major_dir
 
 
 class _PropertyList(MutableSequence):
 
     def __init__(self, seq, read_parent, name):
```

### Comparing `kubernator-1.0.8/kubernator/app.py` & `kubernator-1.0.9/kubernator/app.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/__init__.py` & `kubernator-1.0.9/kubernator/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/awscli.py` & `kubernator-1.0.9/kubernator/plugins/awscli.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/eks.py` & `kubernator-1.0.9/kubernator/plugins/eks.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/helm.py` & `kubernator-1.0.9/kubernator/plugins/helm.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
 
         if version:
             # Download and use specific version
             helm_url = f"https://get.helm.sh/helm-v{version}-{get_golang_os()}-{get_golang_machine()}.tar.gz"
             helm_file_dl, _ = context.app.download_remote_file(logger, helm_url, "bin")
             helm_file_dl = str(helm_file_dl)
             self.helm_dir = tempfile.TemporaryDirectory()
+            context.app.register_cleanup(self.helm_dir)
 
             helm_file = str(Path(self.helm_dir.name) / "helm")
             helm_tar = tarfile.open(helm_file_dl)
             helm_tar.extractall(self.helm_dir.name)
 
             copy(Path(self.helm_dir.name)/f"{get_golang_os()}-{get_golang_machine()}"/"helm", helm_file)
```

### Comparing `kubernator-1.0.8/kubernator/plugins/istio.py` & `kubernator-1.0.9/kubernator/plugins/istio.py`

 * *Files 15% similar despite different names*

```diff
@@ -62,19 +62,30 @@
     def register(self, version=None):
         context = self.context
         context.app.register_plugin("kubeconfig")
         context.app.register_plugin("k8s")
 
         if version:
             # Download and use specific version
+            istioctl_os = get_golang_os()
+            if istioctl_os == "darwin":
+                istioctl_os = "osx"
+                istioctl_machine = get_golang_machine()
+                if istioctl_machine == "amd64":
+                    istioctl_platform = istioctl_os
+                else:
+                    istioctl_platform = f"{istioctl_os}-{istioctl_machine}"
+            else:
+                istioctl_platform = f"{istioctl_os}-{get_golang_machine()}"
             istioctl_url = (f"https://github.com/istio/istio/releases/download/{version}/"
-                            f"istioctl-{version}-{get_golang_os()}-{get_golang_machine()}.tar.gz")
+                            f"istioctl-{version}-{istioctl_platform}.tar.gz")
             istioctl_file_dl, _ = context.app.download_remote_file(logger, istioctl_url, "bin")
             istioctl_file_dl = str(istioctl_file_dl)
             self.istioctl_dir = tempfile.TemporaryDirectory()
+            context.app.register_cleanup(self.istioctl_dir)
 
             istioctl_file = str(Path(self.istioctl_dir.name) / "istioctl")
             istio_tar = tarfile.open(istioctl_file_dl)
             istio_tar.extractall(self.istioctl_dir.name)
 
             os.chmod(istioctl_file, 0o500)
             prepend_os_path(self.istioctl_dir.name)
```

### Comparing `kubernator-1.0.8/kubernator/plugins/k8s.py` & `kubernator-1.0.9/kubernator/plugins/k8s.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/k8s_api.py` & `kubernator-1.0.9/kubernator/plugins/k8s_api.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/kops.py` & `kubernator-1.0.9/kubernator/plugins/kops.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/kubeconfig.py` & `kubernator-1.0.9/kubernator/plugins/kubeconfig.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/kubectl.py` & `kubernator-1.0.9/kubernator/plugins/kubectl.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,47 +47,50 @@
         super().__init__()
 
     def set_context(self, context):
         self.context = context
 
     def stanza(self):
         context = self.context.kubectl
-        return [context.kubectl_file, f"--kubeconfig={context.kubeconfig}"]
+        return [context.kubectl_file, f"--kubeconfig={self.context.kubeconfig.kubeconfig}"]
 
     def register(self,
                  version=None,
                  kubeconfig=None):
         context = self.context
 
+        context.app.register_plugin("kubeconfig")
 
-        kubeconfig = kubeconfig or os.environ.get("KUBECONFIG", os.path.expanduser("~/.kube/config"))
+        if not version and "k8s" in context:
+            version = ".".join(context.k8s.server_version)
+            logger.info("Kubernetes plugin is running with server version %s - will use it", version)
 
         if version:
             # Download and use specific version
             kubectl_url = f"https://dl.k8s.io/release/v{version}/bin/" \
                           f"{get_golang_os()}/" \
                           f"{get_golang_machine()}/kubectl"
             kubectl_file_dl, _ = context.app.download_remote_file(logger, kubectl_url, "bin")
             kubectl_file_dl = str(kubectl_file_dl)
             self.kubectl_dir = tempfile.TemporaryDirectory()
+            context.app.register_cleanup(self.kubectl_dir)
 
             kubectl_file = str(Path(self.kubectl_dir.name) / "kubectl")
             copy(kubectl_file_dl, kubectl_file)
             os.chmod(kubectl_file, 0o500)
             prepend_os_path(self.kubectl_dir.name)
         else:
             # Use current version
             kubectl_file = which("kubectl")
             if not kubectl_file:
                 raise RuntimeError("`kubectl` cannot be found and no version has been specified")
 
             logger.debug("Found kubectl in %r", kubectl_file)
 
         context.globals.kubectl = dict(version=version,
-                                       kubeconfig=kubeconfig,
                                        kubectl_file=kubectl_file,
                                        stanza=self.stanza,
                                        test=self.test_kubectl
                                        )
 
         context.globals.kubectl.version = context.kubectl.test()
```

### Comparing `kubernator-1.0.8/kubernator/plugins/minikube.py` & `kubernator-1.0.9/kubernator/plugins/minikube.py`

 * *Files 18% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         env = dict(os.environ)
         env["MINIKUBE_HOME"] = str(self.minikube_home_dir)
         env["KUBECONFIG"] = str(minikube.kubeconfig)
         return stanza, env
 
     def register(self, minikube_version=None, profile="default", k8s_version=None,
                  keep_running=False, start_fresh=False,
-                 nodes=1, driver="docker", cpus="no-limit", extra_args=None):
+                 nodes=1, driver=None, cpus="no-limit", extra_args=None):
         context = self.context
 
         context.app.register_plugin("kubeconfig")
 
         if not k8s_version:
             msg = "No Kubernetes version is specified for Minikube"
             logger.critical(msg)
@@ -107,28 +107,55 @@
                                                                f"https://github.com/kubernetes/minikube/releases"
                                                                f"/download/v{minikube_version}/"
                                                                f"minikube-{get_golang_os()}-{get_golang_machine()}",
                                                                "bin")
 
         os.chmod(minikube_dl_file, 0o500)
         self.minikube_dir = tempfile.TemporaryDirectory()
+        context.app.register_cleanup(self.minikube_dir)
+
         minikube_file = Path(self.minikube_dir.name) / "minikube"
         minikube_file.symlink_to(minikube_dl_file)
         prepend_os_path(self.minikube_dir.name)
         version_out: str = self.context.app.run_capturing_out([minikube_file, "version", "--short"],
                                                               stderr_logger).strip()
         version = version_out[1:]
         logger.info("Found minikube %s in %s", version, minikube_file)
 
         profile_dir = get_cache_dir("minikube")
         self.minikube_home_dir = profile_dir
         self.minikube_home_dir.mkdir(parents=True, exist_ok=True)
         self.kubeconfig_dir = profile_dir / ".kube"
         self.kubeconfig_dir.mkdir(parents=True, exist_ok=True)
 
+        if not driver:
+            driver = "docker"
+            if get_golang_os() == "darwin":
+                logger.debug("Auto-detecting Minikube driver on MacOS...")
+                cmd_debug_logger = StripNL(proc_logger.debug)
+                try:
+                    context.app.run(["docker", "info"], cmd_debug_logger, cmd_debug_logger).wait()
+                    logger.info("Docker is functional, selecting 'docker' as the driver for Minikube")
+                except (FileNotFoundError, CalledProcessError) as e:
+                    logger.trace("Docker is NOT functional", exc_info=e)
+                    driver = "hyperkit"
+                    try:
+                        context.app.run(["hyperkit", "-v"], cmd_debug_logger, cmd_debug_logger).wait()
+                        logger.info("Hyperkit is functional, selecting 'hyperkit' as the driver for Minikube")
+                    except (FileNotFoundError, CalledProcessError) as e:
+                        logger.trace("Hyperkit is NOT functional", exc_info=e)
+                        driver = "podman"
+                        try:
+                            context.app.run(["podman", "info"], cmd_debug_logger, cmd_debug_logger).wait()
+                            logger.info("Podman is functional, selecting 'podman' as the driver for Minikube")
+                        except (FileNotFoundError, CalledProcessError) as e:
+                            logger.trace("Podman is NOT functional", exc_info=e)
+                            raise RuntimeError("No Minikube driver is functional on MacOS. "
+                                               "Tried 'docker', 'hyperkit' and 'podman'!")
+
         context.globals.minikube = dict(version=version,
                                         minikube_file=str(minikube_file),
                                         profile=profile,
                                         k8s_version=k8s_version,
                                         start_fresh=start_fresh,
                                         keep_running=keep_running,
                                         nodes=nodes,
@@ -155,20 +182,24 @@
                         e.output.strip())
             return False
 
     def minikube_start(self):
         minikube = self.context.minikube
         if not self.minikube_is_running():
             logger.info("Starting minikube profile %r...", minikube.profile)
-            self.cmd("start",
-                     "--driver", str(minikube.driver),
-                     "--nodes", str(minikube.nodes),
-                     "--cpus", str(minikube.cpus),
-                     "--kubernetes-version", str(minikube.k8s_version),
-                     "--wait", "apiserver")
+            args = ["start",
+                    "--driver", str(minikube.driver),
+                    "--kubernetes-version", str(minikube.k8s_version),
+                    "--wait", "apiserver",
+                    "--nodes", str(minikube.nodes)]
+
+            if minikube.driver == "docker":
+                args.extend(["--cpus", str(minikube.cpus)])
+
+            self.cmd(*args)
         else:
             logger.warning("Minikube profile %r is already running!", minikube.profile)
 
         logger.info("Updating minikube profile %r context", minikube.profile)
         self.cmd("update-context")
 
     def minikube_stop(self):
```

### Comparing `kubernator-1.0.8/kubernator/plugins/template.py` & `kubernator-1.0.9/kubernator/plugins/template.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator/plugins/terraform.py` & `kubernator-1.0.9/kubernator/plugins/terraform.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             # Download and use specific version
 
             tf_url = f"https://releases.hashicorp.com/terraform/{version}/terraform_" \
                      f"{version}_{get_golang_os()}_{get_golang_machine()}.zip"
             tf_file_dl, _ = context.app.download_remote_file(logger, tf_url, "bin")
             tf_file_dl = str(tf_file_dl)
             self.tf_dir = tempfile.TemporaryDirectory()
+            context.app.register_cleanup(self.tf_dir)
 
             tf_file = str(Path(self.tf_dir.name) / "terraform")
             tf_zip = zipfile.ZipFile(tf_file_dl)
             tf_zip.extractall(self.tf_dir.name)
 
             os.chmod(tf_file, 0o500)
             prepend_os_path(self.tf_dir.name)
```

### Comparing `kubernator-1.0.8/kubernator/plugins/terragrunt.py` & `kubernator-1.0.9/kubernator/plugins/terragrunt.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         if version:
             # Download and use specific version
             tg_url = (f"https://github.com/gruntwork-io/terragrunt/releases/download/v{version}/"
                       f"terragrunt_{get_golang_os()}_{get_golang_machine()}")
             tg_file_cache, _ = context.app.download_remote_file(logger, tg_url, "bin")
 
             self.tg_dir = tempfile.TemporaryDirectory()
+            context.app.register_cleanup(self.tg_dir)
+
             tg_file = Path(self.tg_dir.name) / "terragrunt"
             copy(tg_file_cache, tg_file)
             os.chmod(tg_file, 0o500)
             prepend_os_path(self.tg_dir.name)
         else:
             # Use current version
             tg_file = which("terragrunt")
```

### Comparing `kubernator-1.0.8/kubernator/proc.py` & `kubernator-1.0.9/kubernator/proc.py`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/kubernator.egg-info/PKG-INFO` & `kubernator-1.0.9/kubernator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubernator
-Version: 1.0.8
+Version: 1.0.9
 Summary: Kubernator is the a pluggable framework for K8S provisioning
 Home-page: https://github.com/karellen/kubernator
 Author: Express Systems USA, Inc.
 Author-email: 
 Maintainer: Karellen, Inc., Arcadiy Ivanov
 Maintainer-email: supervisor@karellen.co,arcadiy@karellen.co
 License: Apache License, Version 2.0
@@ -78,14 +78,22 @@
 ## Using Kubernator with Docker
 
 A simple example is as follows:
 ```
 $ docker run --mount type=bind,source="$(pwd)",target=/root,readonly -t ghcr.io/karellen/kubernator:latest
 ```
 
+## Using Kubernator on MacOS
+
+```
+$ brew install python3.11
+$ pip3.11 install `kubernator~=1.0.9`
+$ kubernator --version
+```
+
 Please note, that some plugins (e.g. `awscli`, `eks`) may require additional volume mounts or environmental
 variables to be passed for credentials and other external configuration.
 
 ## Mode of Operation
 
 Kubernator is a command line utility. Upon startup and processing of the command line arguments and initializing
 logging, Kubernator initializes plugins. Current plugins include:
```

### Comparing `kubernator-1.0.8/kubernator.egg-info/SOURCES.txt` & `kubernator-1.0.9/kubernator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubernator-1.0.8/setup.py` & `kubernator-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'kubernator',
-        version = '1.0.8',
+        version = '1.0.9',
         description = 'Kubernator is the a pluggable framework for K8S provisioning',
-        long_description = '# Kubernator\n\nKubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,\nprocessing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,\ntransforming them and then applying against the Kubernetes cluster.\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/kubernator/kubernator.yml?branch=master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)\n\n[![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n\n## Notices\n\n### Beta Software\n\nWhile fully functional in the current state and used in production, this software is in **BETA**. A lot of things\nare expected to change rapidly, including main APIs, initialization procedures and some core features. Documentation at\nthis stage is basically non-existent.\n\n### License\n\nThe product is licensed under the Apache License, Version 2.0. Please see LICENSE for further details.\n\n### Warranties and Liability\n\nKubernator and its plugins are provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either\nexpress or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,\nMERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of\nusing or redistributing Kubernator and assume any risks associated with doing so.\n\n### Trademarks\n\n"Kubernator" and "Ktor" are trademarks or registered trademarks of Express Systems USA, Inc and Karellen, Inc. All other\ntrademarks are property of their respective owners.\n\n## Problem Statement\n\n## Solution\n\n## Using Kubernator with Docker\n\nA simple example is as follows:\n```\n$ docker run --mount type=bind,source="$(pwd)",target=/root,readonly -t ghcr.io/karellen/kubernator:latest\n```\n\nPlease note, that some plugins (e.g. `awscli`, `eks`) may require additional volume mounts or environmental\nvariables to be passed for credentials and other external configuration.\n\n## Mode of Operation\n\nKubernator is a command line utility. Upon startup and processing of the command line arguments and initializing\nlogging, Kubernator initializes plugins. Current plugins include:\n\n0. Kubernator App\n1. Terraform\n2. kOps\n3. Kubernetes\n4. Helm\n5. Template\n\nThe order of initialization matters as it\'s the order the plugin handlers are executed!\n\nThe entire application operates in the following stages by invoking each plugin\'s stage handler in sequence:\n\n1. Plugin Init Stage\n2. Pre-start script (if specified)\n3. Plugin Start Stage\n4. For each directory in the pipeline:\n    1. Plugin Before Directory Stage\n    2. If `.kubernator.py` is present in the directory:\n        1. Plugin Before Script Stage\n        2. `.kubernator.py` script\n        3. Plugin After Script Stage\n    3. Plugin After Directory Stage\n5. Plugin End Stage\n\nEach plugin individually plays a specific role and performs a specific function which will be described in a later\nsection.\n\n## State/Context\n\nThere is a global state that is carried through as the application is running. It is a hierarchy of objects (`context`)\nthat follows the parent-child relationship as the application traverses the directory structure. For example, given the\ndirectory structure `/a/b`, `/a/c`, and `/a/c/d` any value of the context set or modified in context scoped to\ndirectory `/a` is visible in directories `/a/b`, `/a/c` and `/a/c/d`, while the same modified or set in `/a/b` is only\nvisible there, while one in `/a/c` is visible in `/a/c` and in `/a/c/d` but not `/a` or `/a/b`.\n\nAdditionally, there is a `context.globals` which is the top-most context that is available in all stages that are not\nassociated with the directory structure.\n\nNote, that in cases where the directory structure traversal moves to remote directories (that are actualized by local\ntemporary directories), such remote directory structure enters the context hierarchy as a child of the directory in\nwhich remote was registered.\n\nAlso note, that context carries not just data by references to essential functions.\n\nIn pre-start and `.kubernator.py` scripts the context is fully available as a global variable `ktor`.\n\n### Plugins\n\n#### Kubernator App Plugin\n\nThe role of the Kubernator App Plugin is to traverse the directory structure, expose essential functions through context\nand to run Kubernator scripts.\n\nIn the *After Directory Stage* Kubernator app scans the directories immediately available in the current, sorts them in\nthe alphabetic order, excludes those matching any of the patterns in `context.app.excludes` and then queues up the\nremaining directories in the order the match the patterns in `context.app.includes`.\n\nThus, for a directory content `/a/foo`, `/a/bal`, `/a/bar`, `/a/baz`, excludes `f*`, and includes `baz` and `*`, the\nresulting queue of directories to traverse will be `/a/baz`, `/a/bal`, `/a/bar`.\n\nNotice, that user can further interfere with processing order of the directory queue by asking Kubernator to walk\narbitrary paths, both local and remote.\n\n##### Context\n\n* `ktor.app.args`\n  > Namespace containing command line argument values\n* `ktor.app.walk_local(*paths: Union[Path, str, bytes])`\n  > Immediately schedules the paths to be traversed after the current directory by adding them to the queue\n  > Relative path is relative to the current directory\n* `ktor.app.walk_remote(repo, *path_prefixes: Union[Path, str, bytes])`\n  > Immediately schedules the path prefixes under the remote repo URL to be traversed after the current directory by\n  > adding them to the queue. Only Git URLs are currently supported.\n  > All absolute path prefixes are relativized based on the repository.\n* `ktor.app.repository_credentials_provider(func: Callable)`\n  > Sets a repository credentials provider function `func` that sets/overwrites credentials for URLs being specified by\n  > `walk_remote`. The callable `func` accepts a single argument containing a parsed URL in a form of tuple. The `func`\n  > is expected to return a tuple of three elements representing URL schema, username and password. If the value should\n  > not be changed it should be None. To convert from `git://repo.com/hello` to HTTPS authentication one should write\n  > a function returning `("https", "username", "password")`. The best utility is achieved by logic that allows running\n  > the plan both in CI and local environments using different authentication mechanics in different environments.\n\n#### Terraform\n\nThis is exclusively designed to pull the configuration options out of Terraform and to allow scripts and plugins to\nutilize that data.\n\n##### Context\n\n* `ktor.tf`\n  > A dictionary containing the values from Terraform output\n\n#### Kops\n\n##### Context\n\n#### Kubernetes\n\n##### Context\n\n#### Helm\n\n##### Context\n\n#### Templates\n\n##### Context\n\n## Examples\n\n### Adding Remote Directory\n\n```python\nktor.app.repository_credentials_provider(lambda r: ("ssh", "git", None))\nktor.app.walk_remote("git://repo.example.com/org/project?ref=dev", "/project")\n```\n\n### Adding Local Directory\n\n```python\nktor.app.walk_local("/home/username/local-dir")\n```\n\n### Using Transformers\n\n```python\ndef remove_replicas(resources, r: "K8SResource"):\n    if (r.group == "apps" and r.kind in ("StatefulSet", "Deployment")\n            and "replicas" in r.manifest["spec"]):\n        logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",\n                       r, r.source)\n        del r.manifest["spec"]["replicas"]\n\n\nktor.k8s.add_transformer(remove_replicas)\n```\n',
+        long_description = '# Kubernator\n\nKubernator™ (Ktor™) is an integrated solution for the Kubernetes state management. It operates on directories,\nprocessing their content via a collection of plugins, generating Kubernetes resources in the process, validating them,\ntransforming them and then applying against the Kubernetes cluster.\n\n[![Gitter](https://img.shields.io/gitter/room/karellen/lobby?logo=gitter)](https://gitter.im/karellen/Lobby)\n[![Build Status](https://img.shields.io/github/actions/workflow/status/karellen/kubernator/kubernator.yml?branch=master)](https://github.com/karellen/kubernator/actions/workflows/kubernator.yml)\n[![Coverage Status](https://img.shields.io/coveralls/github/karellen/kubernator/master?logo=coveralls)](https://coveralls.io/r/karellen/kubernator?branch=master)\n\n[![Kubernator Version](https://img.shields.io/pypi/v/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Python Versions](https://img.shields.io/pypi/pyversions/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Day](https://img.shields.io/pypi/dd/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Week](https://img.shields.io/pypi/dw/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n[![Kubernator Downloads Per Month](https://img.shields.io/pypi/dm/kubernator?logo=pypi)](https://pypi.org/project/kubernator/)\n\n## Notices\n\n### Beta Software\n\nWhile fully functional in the current state and used in production, this software is in **BETA**. A lot of things\nare expected to change rapidly, including main APIs, initialization procedures and some core features. Documentation at\nthis stage is basically non-existent.\n\n### License\n\nThe product is licensed under the Apache License, Version 2.0. Please see LICENSE for further details.\n\n### Warranties and Liability\n\nKubernator and its plugins are provided on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either\nexpress or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT,\nMERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of\nusing or redistributing Kubernator and assume any risks associated with doing so.\n\n### Trademarks\n\n"Kubernator" and "Ktor" are trademarks or registered trademarks of Express Systems USA, Inc and Karellen, Inc. All other\ntrademarks are property of their respective owners.\n\n## Problem Statement\n\n## Solution\n\n## Using Kubernator with Docker\n\nA simple example is as follows:\n```\n$ docker run --mount type=bind,source="$(pwd)",target=/root,readonly -t ghcr.io/karellen/kubernator:latest\n```\n\n## Using Kubernator on MacOS\n\n```\n$ brew install python3.11\n$ pip3.11 install `kubernator~=1.0.9`\n$ kubernator --version\n```\n\nPlease note, that some plugins (e.g. `awscli`, `eks`) may require additional volume mounts or environmental\nvariables to be passed for credentials and other external configuration.\n\n## Mode of Operation\n\nKubernator is a command line utility. Upon startup and processing of the command line arguments and initializing\nlogging, Kubernator initializes plugins. Current plugins include:\n\n0. Kubernator App\n1. Terraform\n2. kOps\n3. Kubernetes\n4. Helm\n5. Template\n\nThe order of initialization matters as it\'s the order the plugin handlers are executed!\n\nThe entire application operates in the following stages by invoking each plugin\'s stage handler in sequence:\n\n1. Plugin Init Stage\n2. Pre-start script (if specified)\n3. Plugin Start Stage\n4. For each directory in the pipeline:\n    1. Plugin Before Directory Stage\n    2. If `.kubernator.py` is present in the directory:\n        1. Plugin Before Script Stage\n        2. `.kubernator.py` script\n        3. Plugin After Script Stage\n    3. Plugin After Directory Stage\n5. Plugin End Stage\n\nEach plugin individually plays a specific role and performs a specific function which will be described in a later\nsection.\n\n## State/Context\n\nThere is a global state that is carried through as the application is running. It is a hierarchy of objects (`context`)\nthat follows the parent-child relationship as the application traverses the directory structure. For example, given the\ndirectory structure `/a/b`, `/a/c`, and `/a/c/d` any value of the context set or modified in context scoped to\ndirectory `/a` is visible in directories `/a/b`, `/a/c` and `/a/c/d`, while the same modified or set in `/a/b` is only\nvisible there, while one in `/a/c` is visible in `/a/c` and in `/a/c/d` but not `/a` or `/a/b`.\n\nAdditionally, there is a `context.globals` which is the top-most context that is available in all stages that are not\nassociated with the directory structure.\n\nNote, that in cases where the directory structure traversal moves to remote directories (that are actualized by local\ntemporary directories), such remote directory structure enters the context hierarchy as a child of the directory in\nwhich remote was registered.\n\nAlso note, that context carries not just data by references to essential functions.\n\nIn pre-start and `.kubernator.py` scripts the context is fully available as a global variable `ktor`.\n\n### Plugins\n\n#### Kubernator App Plugin\n\nThe role of the Kubernator App Plugin is to traverse the directory structure, expose essential functions through context\nand to run Kubernator scripts.\n\nIn the *After Directory Stage* Kubernator app scans the directories immediately available in the current, sorts them in\nthe alphabetic order, excludes those matching any of the patterns in `context.app.excludes` and then queues up the\nremaining directories in the order the match the patterns in `context.app.includes`.\n\nThus, for a directory content `/a/foo`, `/a/bal`, `/a/bar`, `/a/baz`, excludes `f*`, and includes `baz` and `*`, the\nresulting queue of directories to traverse will be `/a/baz`, `/a/bal`, `/a/bar`.\n\nNotice, that user can further interfere with processing order of the directory queue by asking Kubernator to walk\narbitrary paths, both local and remote.\n\n##### Context\n\n* `ktor.app.args`\n  > Namespace containing command line argument values\n* `ktor.app.walk_local(*paths: Union[Path, str, bytes])`\n  > Immediately schedules the paths to be traversed after the current directory by adding them to the queue\n  > Relative path is relative to the current directory\n* `ktor.app.walk_remote(repo, *path_prefixes: Union[Path, str, bytes])`\n  > Immediately schedules the path prefixes under the remote repo URL to be traversed after the current directory by\n  > adding them to the queue. Only Git URLs are currently supported.\n  > All absolute path prefixes are relativized based on the repository.\n* `ktor.app.repository_credentials_provider(func: Callable)`\n  > Sets a repository credentials provider function `func` that sets/overwrites credentials for URLs being specified by\n  > `walk_remote`. The callable `func` accepts a single argument containing a parsed URL in a form of tuple. The `func`\n  > is expected to return a tuple of three elements representing URL schema, username and password. If the value should\n  > not be changed it should be None. To convert from `git://repo.com/hello` to HTTPS authentication one should write\n  > a function returning `("https", "username", "password")`. The best utility is achieved by logic that allows running\n  > the plan both in CI and local environments using different authentication mechanics in different environments.\n\n#### Terraform\n\nThis is exclusively designed to pull the configuration options out of Terraform and to allow scripts and plugins to\nutilize that data.\n\n##### Context\n\n* `ktor.tf`\n  > A dictionary containing the values from Terraform output\n\n#### Kops\n\n##### Context\n\n#### Kubernetes\n\n##### Context\n\n#### Helm\n\n##### Context\n\n#### Templates\n\n##### Context\n\n## Examples\n\n### Adding Remote Directory\n\n```python\nktor.app.repository_credentials_provider(lambda r: ("ssh", "git", None))\nktor.app.walk_remote("git://repo.example.com/org/project?ref=dev", "/project")\n```\n\n### Adding Local Directory\n\n```python\nktor.app.walk_local("/home/username/local-dir")\n```\n\n### Using Transformers\n\n```python\ndef remove_replicas(resources, r: "K8SResource"):\n    if (r.group == "apps" and r.kind in ("StatefulSet", "Deployment")\n            and "replicas" in r.manifest["spec"]):\n        logger.warning("Resource %s in %s contains `replica` specification that will be removed. Use HPA!!!",\n                       r, r.source)\n        del r.manifest["spec"]["replicas"]\n\n\nktor.k8s.add_transformer(remove_replicas)\n```\n',
         long_description_content_type = 'text/markdown',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             'Operating System :: MacOS :: MacOS X',
```

