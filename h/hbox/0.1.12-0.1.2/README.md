# Comparing `tmp/hbox-0.1.12.tar.gz` & `tmp/hbox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbox-0.1.12.tar", max compression
+gzip compressed data, was "hbox-0.1.2.tar", max compression
```

## Comparing `hbox-0.1.12.tar` & `hbox-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2024-05-02 05:07:28.118439 hbox-0.1.12/LICENSE
--rw-r--r--   0        0        0     6331 2024-05-02 05:07:28.118439 hbox-0.1.12/README.md
--rw-r--r--   0        0        0     6635 2024-05-02 05:07:28.118439 hbox-0.1.12/hbox/commands.py
--rw-r--r--   0        0        0     2212 2024-05-02 05:07:28.118439 hbox-0.1.12/hbox/config.py
--rw-r--r--   0        0        0      684 2024-05-02 05:07:28.118439 hbox-0.1.12/hbox/logger.py
--rw-r--r--   0        0        0     3094 2024-05-02 05:07:28.118439 hbox-0.1.12/hbox/main.py
--rw-r--r--   0        0        0     2292 2024-05-02 05:07:28.118439 hbox-0.1.12/hbox/utils.py
--rw-r--r--   0        0        0      428 2024-05-02 05:07:28.118439 hbox-0.1.12/pyproject.toml
--rw-r--r--   0        0        0     6802 1970-01-01 00:00:00.000000 hbox-0.1.12/PKG-INFO
+-rw-r--r--   0        0        0     6820 2024-05-02 00:30:53.471090 hbox-0.1.2/hbox/commands.py
+-rw-r--r--   0        0        0     2212 2024-05-01 23:08:08.455225 hbox-0.1.2/hbox/config.py
+-rw-r--r--   0        0        0      713 2024-05-02 00:12:58.356957 hbox-0.1.2/hbox/logger.py
+-rw-r--r--   0        0        0     3170 2024-05-02 00:36:33.736473 hbox-0.1.2/hbox/main.py
+-rw-r--r--   0        0        0     2366 2024-05-02 00:14:33.310882 hbox-0.1.2/hbox/utils.py
+-rw-r--r--   0        0        0     1098 2024-05-01 14:02:10.452353 hbox-0.1.2/LICENSE
+-rw-r--r--   0        0        0      445 2024-05-02 00:38:24.696258 hbox-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5855 2024-05-02 00:37:35.237764 hbox-0.1.2/README.md
+-rw-r--r--   0        0        0     6126 1970-01-01 00:00:00.000000 hbox-0.1.2/PKG-INFO
```

### Comparing `hbox-0.1.12/README.md` & `hbox-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,22 @@
-# hbox
+Metadata-Version: 2.1
+Name: hbox
+Version: 0.1.2
+Summary: CLI tool that leverages container technology to manage packages.
+License: MIT
+Author: Helton Carlos de Souza
+Author-email: heltoncarlossouza@gmail.com
+Requires-Python: >=3.12,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Description-Content-Type: text/markdown
 
-[![CI](https://img.shields.io/github/actions/workflow/status/helton/hbox/production.yml?branch=main&logo=github&label=CI)](https://github.com/helton/hbox/actions?query=event%3Apush+branch%3Amain+workflow%3ACI)
-[![pypi](https://img.shields.io/pypi/v/hbox.svg)](https://pypi.python.org/pypi/hbox)
-[![versions](https://img.shields.io/pypi/pyversions/hbox.svg)](https://github.com/helton/hbox)
-[![license](https://img.shields.io/github/license/helton/hbox.svg)](https://github.com/helton/hbox/blob/main/LICENSE)
+# hbox
 
 hbox is a Command Line Interface (CLI) that leverages container technology to manage packages.
 
 ## Features
 
 hbox offers the following features:
 
@@ -35,23 +44,14 @@
     run                 Run the package.
     use (set)           Set current version of a package.
 
 options:
   -h, --help            show this help message and exit
 ```
 
-## Installation
-
-You can install hbox via `pip` or your preferred package manager.
-To install hbox via `pip`, run the following command:
-
-```sh
-pip install hbox
-```
-
 ## Setup
 
 ### Shims and Shell Configuration
 
 hbox utilizes shims and a configuration file to effectively manage your installed packages. For the successful addition of `$HBOX_DIR/shims` at the correct priority level to your path, these lines of code should be added to your `.bashrc` or `.zshrc` file:
 
 ```sh
@@ -207,7 +207,8 @@
 - [Experimental] Identify paths in `hbox run` to map them via container volumes automatically
 - Separate `packages.json` from `config.json`
   - Allow use to override `packages.json` retrieved from centralized index/repo
 - Add `hbox update` to update index
 - Add `hbox register` to register a package, even with custom image
 - Add option to remove images when removing packages
 - Add support to colors in `hbox run` output when possible (*nix only?)
+
```

### Comparing `hbox-0.1.12/hbox/commands.py` & `hbox-0.1.2/hbox/commands.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-import os
-import platform
-import subprocess
-from typing import Optional
-
-import hbox.config as config
-from hbox.logger import get_logger
-from hbox.utils import execute_command, resolve_path
-
-log = get_logger(__name__)
-
-
-def add_shim(name: str):
-    shims_file_path = resolve_path(os.path.join(config.shims_path, name))
-    if not os.path.exists(shims_file_path):
-        os.makedirs(os.path.dirname(shims_file_path), exist_ok=True)
-        with open(shims_file_path, 'w') as shim_file:
-            shim_file.write('#!/bin/sh\n')
-            shim_file.write('hbox run ' + name + ' "$@"\n')
-
-        # Set the permissions of the new shim script to be executable (0o755 gives rwx for user and rx for group/others)
-        os.chmod(shims_file_path, 0o755)
-
-
-def remove_shim(name: str):
-    shims_file_path = resolve_path(os.path.join(config.shims_path, name))
-    if os.path.exists(shims_file_path):
-        os.remove(shims_file_path)
-
-
-def get_container_image_url(name: str, version: str, set_as_default: bool):
-    cfg = config.load_config()
-    versions_cfg = config.load_versions()
-    found = False
-    for current_package in versions_cfg.packages:
-        if current_package.name == name:
-            if version in current_package.versions:
-                log.info(f"'{name}' version {version} already exists.")
-                return None, versions_cfg
-            else:
-                current_package.versions.append(version)
-                if set_as_default:
-                    log.info(f"'{name}' version {version} set as default.")
-                    current_package.current = version
-                found = True
-            break
-    if not found:
-        package = config.Package(name=name, versions=[version], current=version)
-        versions_cfg.packages.append(package)
-
-    if name in cfg.packages:
-        image = cfg.packages[name].image
-    else:
-        image = name
-
-    return f"{image}:{version}", versions_cfg
-
-
-def add_package(name, version: Optional[str] = "latest", set_as_default: Optional[bool] = False):
-    image_url, versions_cfg = get_container_image_url(name, version, set_as_default)
-    if image_url:
-        full_command = ["docker", "pull", image_url]
-        exit_code = execute_command(full_command)
-        if exit_code and exit_code != 0:
-            log.error(f"Failed to add package '{name}' at version {version}.")
-        else:
-            config.save_versions(versions_cfg)
-            log.info(f"Added '{name}' version {version}.")
-            add_shim(name)
-
-
-def remove_package(name: str, version: Optional[str] = None):
-    versions_cfg = config.load_versions()
-    for current_package in versions_cfg.packages:
-        if current_package.name == name:
-            if version:
-                if version in current_package.versions:
-                    # Check if version to be removed is the current one and if there are multiple versions
-                    if version == current_package.current and len(current_package.versions) > 1:
-                        log.error(
-                            f"Cannot remove the current active version '{version}' of '{name}'.")
-                        return
-                    current_package.versions.remove(version)
-                    log.info(f"Removed version '{version}' of '{name}'.")
-                else:
-                    log.error(f"Version '{version}' of '{name}' does not exist.")
-
-            if not version or not current_package.versions:
-                versions_cfg.packages.remove(current_package)
-                remove_shim(name)
-                log.info(f"Removed package '{name}'.")
-            break
-    else:
-        log.error(f"Package '{name}' does not exist.")
-
-    config.save_versions(versions_cfg)
-
-
-def run_package(name: str, command: list):
-    cfg = config.load_config()
-    versions_cfg = config.load_versions()
-
-    image = name
-    version = "latest"
-
-    volumes_command = []
-    if name in cfg.packages:
-        package = cfg.packages[name]
-        image = package.image
-        for volume in package.volumes:
-            source = resolve_path(volume.source)
-            target = volume.target
-            if os.path.exists(source):
-                log.debug(f"Mounting volume {source} to {target}")
-                volumes_command.extend(["-v", f"{source}:{target}"])
-            else:
-                log.debug(f"Volume {source} not found. Skipping.")
-    else:
-        log.debug(f"No configuration found for package '{name}'. Using {name} as the image name.")
-
-    for current_package in versions_cfg.packages:
-        if current_package.name == name:
-            version = current_package.current
-
-    full_image_url = f"{image}:{version}"
-
-    full_command = ["docker", "run", "--rm", full_image_url] + volumes_command + command
-    try:
-        execute_command(full_command, can_be_interactive=True)
-    except subprocess.CalledProcessError as e:
-        log.debug(f"Failed to run command {' '.join(full_command)}")
-
-
-def set_package_version(name: str, version: str):
-    versions_cfg = config.load_versions()
-    for current_package in versions_cfg.packages:
-        if current_package.name == name:
-            if version in current_package.versions:
-                current_package.current = version
-                config.save_versions(versions_cfg)
-                log.info(f"'{name}' set to version {version}")
-            else:
-                log.error(f"'{name}' version {version} not found. Add the version first via 'add' command.")
-
-
-def show_info():
-    log.info("OS:")
-    os_info = ' '.join(platform.uname())
-    log.info(os_info)
-
-    log.info("\nHBOX VERSION:")
-    log.info(config.get_library_version())
-
-    log.info("\nHBOX ENVIRONMENT VARIABLES:")
-    log.info(f"HBOX_DIR={config.base_dir}")
-
-
-def show_version():
-    log.info(config.get_library_version())
-
-
-def print_package(package):
-    log.info(f"- {package.name}:")
-    sorted_versions = sorted(package.versions)
-    for version in sorted_versions:
-        msg = f"  - {version}"
-        if version == package.current:
-            msg += " ✔"
-        log.info(msg)
-
-
-def list_packages(name: Optional[str] = None):
-    versions_cfg = config.load_versions()
-    if name:
-        found = False
-        for package in versions_cfg.packages:
-            if package.name == name:
-                print_package(package)
-                found = True
-                break
-        if not found:
-            log.error(f"Package '{name}' was not found. Add the package first via 'add' command.")
-    else:
-        for package in sorted(versions_cfg.packages, key=lambda pkg: pkg.name):
-            print_package(package)
+import os
+import platform
+import subprocess
+from typing import Optional
+
+import hbox.config as config
+from hbox.logger import get_logger
+from hbox.utils import execute_command, resolve_path
+
+log = get_logger(__name__)
+
+
+def add_shim(name: str):
+    shims_file_path = resolve_path(os.path.join(config.shims_path, name))
+    if not os.path.exists(shims_file_path):
+        os.makedirs(os.path.dirname(shims_file_path), exist_ok=True)
+        with open(shims_file_path, 'w') as shim_file:
+            shim_file.write('#!/bin/sh\n')
+            shim_file.write('hbox run ' + name + ' "$@"\n')
+
+        # Set the permissions of the new shim script to be executable (0o755 gives rwx for user and rx for group/others)
+        os.chmod(shims_file_path, 0o755)
+
+
+def remove_shim(name: str):
+    shims_file_path = resolve_path(os.path.join(config.shims_path, name))
+    if os.path.exists(shims_file_path):
+        os.remove(shims_file_path)
+
+
+def get_container_image_url(name: str, version: str, set_as_default: bool):
+    cfg = config.load_config()
+    versions_cfg = config.load_versions()
+    found = False
+    for current_package in versions_cfg.packages:
+        if current_package.name == name:
+            if version in current_package.versions:
+                log.info(f"'{name}' version {version} already exists.")
+                return None, versions_cfg
+            else:
+                current_package.versions.append(version)
+                if set_as_default:
+                    log.info(f"'{name}' version {version} set as default.")
+                    current_package.current = version
+                found = True
+            break
+    if not found:
+        package = config.Package(name=name, versions=[version], current=version)
+        versions_cfg.packages.append(package)
+
+    if name in cfg.packages:
+        image = cfg.packages[name].image
+    else:
+        image = name
+
+    return f"{image}:{version}", versions_cfg
+
+
+def add_package(name, version: Optional[str] = "latest", set_as_default: Optional[bool] = False):
+    image_url, versions_cfg = get_container_image_url(name, version, set_as_default)
+    if image_url:
+        full_command = ["docker", "pull", image_url]
+        exit_code = execute_command(full_command)
+        if exit_code and exit_code != 0:
+            log.error(f"Failed to add package '{name}' at version {version}.")
+        else:
+            config.save_versions(versions_cfg)
+            log.info(f"Added '{name}' version {version}.")
+            add_shim(name)
+
+
+def remove_package(name: str, version: Optional[str] = None):
+    versions_cfg = config.load_versions()
+    for current_package in versions_cfg.packages:
+        if current_package.name == name:
+            if version:
+                if version in current_package.versions:
+                    # Check if version to be removed is the current one and if there are multiple versions
+                    if version == current_package.current and len(current_package.versions) > 1:
+                        log.error(
+                            f"Cannot remove the current active version '{version}' of '{name}'.")
+                        return
+                    current_package.versions.remove(version)
+                    log.info(f"Removed version '{version}' of '{name}'.")
+                else:
+                    log.error(f"Version '{version}' of '{name}' does not exist.")
+
+            if not version or not current_package.versions:
+                versions_cfg.packages.remove(current_package)
+                remove_shim(name)
+                log.info(f"Removed package '{name}'.")
+            break
+    else:
+        log.error(f"Package '{name}' does not exist.")
+
+    config.save_versions(versions_cfg)
+
+
+def run_package(name: str, command: list):
+    cfg = config.load_config()
+    versions_cfg = config.load_versions()
+
+    image = name
+    version = "latest"
+
+    volumes_command = []
+    if name in cfg.packages:
+        package = cfg.packages[name]
+        image = package.image
+        for volume in package.volumes:
+            source = resolve_path(volume.source)
+            target = volume.target
+            if os.path.exists(source):
+                log.debug(f"Mounting volume {source} to {target}")
+                volumes_command.extend(["-v", f"{source}:{target}"])
+            else:
+                log.debug(f"Volume {source} not found. Skipping.")
+    else:
+        log.debug(f"No configuration found for package '{name}'. Using {name} as the image name.")
+
+    for current_package in versions_cfg.packages:
+        if current_package.name == name:
+            version = current_package.current
+
+    full_image_url = f"{image}:{version}"
+
+    full_command = ["docker", "run", "--rm", full_image_url] + volumes_command + command
+    try:
+        execute_command(full_command, can_be_interactive=True)
+    except subprocess.CalledProcessError as e:
+        log.debug(f"Failed to run command {' '.join(full_command)}")
+
+
+def set_package_version(name: str, version: str):
+    versions_cfg = config.load_versions()
+    for current_package in versions_cfg.packages:
+        if current_package.name == name:
+            if version in current_package.versions:
+                current_package.current = version
+                config.save_versions(versions_cfg)
+                log.info(f"'{name}' set to version {version}")
+            else:
+                log.error(f"'{name}' version {version} not found. Add the version first via 'add' command.")
+
+
+def show_info():
+    log.info("OS:")
+    os_info = ' '.join(platform.uname())
+    log.info(os_info)
+
+    log.info("\nHBOX VERSION:")
+    log.info(config.get_library_version())
+
+    log.info("\nHBOX ENVIRONMENT VARIABLES:")
+    log.info(f"HBOX_DIR={config.base_dir}")
+
+
+def show_version():
+    log.info(config.get_library_version())
+
+
+def print_package(package):
+    log.info(f"- {package.name}:")
+    sorted_versions = sorted(package.versions)
+    for version in sorted_versions:
+        msg = f"  - {version}"
+        if version == package.current:
+            msg += " ✔"
+        log.info(msg)
+
+
+def list_packages(name: Optional[str] = None):
+    versions_cfg = config.load_versions()
+    if name:
+        found = False
+        for package in versions_cfg.packages:
+            if package.name == name:
+                print_package(package)
+                found = True
+                break
+        if not found:
+            log.error(f"Package '{name}' was not found. Add the package first via 'add' command.")
+    else:
+        for package in sorted(versions_cfg.packages, key=lambda pkg: pkg.name):
+            print_package(package)
```

### Comparing `hbox-0.1.12/hbox/config.py` & `hbox-0.1.2/hbox/config.py`

 * *Files identical despite different names*

