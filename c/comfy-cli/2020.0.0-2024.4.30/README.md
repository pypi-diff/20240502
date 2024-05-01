# Comparing `tmp/comfy_cli-2020.0.0.tar.gz` & `tmp/comfy_cli-2024.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfy_cli-2020.0.0.tar", last modified: Sat Apr 13 23:31:18 2024, max compression
+gzip compressed data, was "comfy_cli-2024.4.30.tar", last modified: Wed May  1 22:39:37 2024, max compression
```

## Comparing `comfy_cli-2020.0.0.tar` & `comfy_cli-2024.4.30.tar`

### file list

```diff
@@ -1,14 +1,35 @@
-drwxr-xr-x   0 junhanhuang   (501) staff       (20)        0 2024-04-13 23:31:18.795116 comfy_cli-2020.0.0/
--rw-r--r--   0 junhanhuang   (501) staff       (20)    35823 2024-04-13 23:09:02.000000 comfy_cli-2020.0.0/LICENSE
--rw-r--r--   0 junhanhuang   (501) staff       (20)    43651 2024-04-13 23:31:18.795039 comfy_cli-2020.0.0/PKG-INFO
--rw-r--r--   0 junhanhuang   (501) staff       (20)     2391 2024-04-13 23:09:02.000000 comfy_cli-2020.0.0/README.md
-drwxr-xr-x   0 junhanhuang   (501) staff       (20)        0 2024-04-13 23:31:18.794700 comfy_cli-2020.0.0/comfy_cli.egg-info/
--rw-r--r--   0 junhanhuang   (501) staff       (20)    43651 2024-04-13 23:31:18.000000 comfy_cli-2020.0.0/comfy_cli.egg-info/PKG-INFO
--rw-r--r--   0 junhanhuang   (501) staff       (20)      251 2024-04-13 23:31:18.000000 comfy_cli-2020.0.0/comfy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 junhanhuang   (501) staff       (20)        1 2024-04-13 23:31:18.000000 comfy_cli-2020.0.0/comfy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 junhanhuang   (501) staff       (20)       41 2024-04-13 23:31:18.000000 comfy_cli-2020.0.0/comfy_cli.egg-info/entry_points.txt
--rw-r--r--   0 junhanhuang   (501) staff       (20)       28 2024-04-13 23:31:18.000000 comfy_cli-2020.0.0/comfy_cli.egg-info/requires.txt
--rw-r--r--   0 junhanhuang   (501) staff       (20)        1 2024-04-13 23:31:18.000000 comfy_cli-2020.0.0/comfy_cli.egg-info/top_level.txt
--rw-r--r--   0 junhanhuang   (501) staff       (20)      819 2024-04-13 23:31:16.000000 comfy_cli-2020.0.0/pyproject.toml
--rw-r--r--   0 junhanhuang   (501) staff       (20)      899 2024-04-13 23:31:18.795369 comfy_cli-2020.0.0/setup.cfg
--rw-r--r--   0 junhanhuang   (501) staff       (20)      230 2024-04-13 23:09:02.000000 comfy_cli-2020.0.0/setup.py
+drwxr-xr-x   0 james.kwon   (502) staff       (20)        0 2024-05-01 22:39:37.062274 comfy_cli-2024.4.30/
+-rw-r--r--   0 james.kwon   (502) staff       (20)    35823 2024-04-25 14:45:37.000000 comfy_cli-2024.4.30/LICENSE
+-rw-r--r--   0 james.kwon   (502) staff       (20)    47608 2024-05-01 22:39:37.062008 comfy_cli-2024.4.30/PKG-INFO
+-rw-r--r--   0 james.kwon   (502) staff       (20)     6239 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/README.md
+drwxr-xr-x   0 james.kwon   (502) staff       (20)        0 2024-05-01 22:39:37.058293 comfy_cli-2024.4.30/comfy_cli/
+-rw-r--r--   0 james.kwon   (502) staff       (20)        0 2024-04-25 14:45:37.000000 comfy_cli-2024.4.30/comfy_cli/__init__.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)       93 2024-04-30 01:57:42.000000 comfy_cli-2024.4.30/comfy_cli/__main__.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)    10983 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/cmdline.py
+drwxr-xr-x   0 james.kwon   (502) staff       (20)        0 2024-05-01 22:39:37.059841 comfy_cli-2024.4.30/comfy_cli/command/
+-rw-r--r--   0 james.kwon   (502) staff       (20)       48 2024-04-25 14:45:37.000000 comfy_cli-2024.4.30/comfy_cli/command/__init__.py
+drwxr-xr-x   0 james.kwon   (502) staff       (20)        0 2024-05-01 22:39:37.060353 comfy_cli-2024.4.30/comfy_cli/command/custom_nodes/
+-rw-r--r--   0 james.kwon   (502) staff       (20)       38 2024-04-25 14:45:37.000000 comfy_cli-2024.4.30/comfy_cli/command/custom_nodes/__init__.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)    11101 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/command/custom_nodes/command.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     2800 2024-04-30 23:52:12.000000 comfy_cli-2024.4.30/comfy_cli/command/install.py
+drwxr-xr-x   0 james.kwon   (502) staff       (20)        0 2024-05-01 22:39:37.060540 comfy_cli-2024.4.30/comfy_cli/command/models/
+-rw-r--r--   0 james.kwon   (502) staff       (20)     4684 2024-04-30 03:37:22.000000 comfy_cli-2024.4.30/comfy_cli/command/models/models.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)       83 2024-04-25 14:45:37.000000 comfy_cli-2024.4.30/comfy_cli/command/run.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     2933 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/config_manager.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     1700 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/constants.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     5435 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/env_checker.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)      881 2024-04-28 17:07:48.000000 comfy_cli-2024.4.30/comfy_cli/logging.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     4355 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/meta_data.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     2050 2024-04-30 03:37:22.000000 comfy_cli-2024.4.30/comfy_cli/tracking.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     2738 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/ui.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     1019 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/utils.py
+-rw-r--r--   0 james.kwon   (502) staff       (20)     5397 2024-05-01 13:30:28.000000 comfy_cli-2024.4.30/comfy_cli/workspace_manager.py
+drwxr-xr-x   0 james.kwon   (502) staff       (20)        0 2024-05-01 22:39:37.061624 comfy_cli-2024.4.30/comfy_cli.egg-info/
+-rw-r--r--   0 james.kwon   (502) staff       (20)    47608 2024-05-01 22:39:37.000000 comfy_cli-2024.4.30/comfy_cli.egg-info/PKG-INFO
+-rw-r--r--   0 james.kwon   (502) staff       (20)      709 2024-05-01 22:39:37.000000 comfy_cli-2024.4.30/comfy_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 james.kwon   (502) staff       (20)        1 2024-05-01 22:39:37.000000 comfy_cli-2024.4.30/comfy_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 james.kwon   (502) staff       (20)      121 2024-05-01 22:39:37.000000 comfy_cli-2024.4.30/comfy_cli.egg-info/entry_points.txt
+-rw-r--r--   0 james.kwon   (502) staff       (20)       83 2024-05-01 22:39:37.000000 comfy_cli-2024.4.30/comfy_cli.egg-info/requires.txt
+-rw-r--r--   0 james.kwon   (502) staff       (20)       10 2024-05-01 22:39:37.000000 comfy_cli-2024.4.30/comfy_cli.egg-info/top_level.txt
+-rw-r--r--   0 james.kwon   (502) staff       (20)     1085 2024-04-30 01:57:37.000000 comfy_cli-2024.4.30/pyproject.toml
+-rw-r--r--   0 james.kwon   (502) staff       (20)       38 2024-05-01 22:39:37.062329 comfy_cli-2024.4.30/setup.cfg
```

### Comparing `comfy_cli-2020.0.0/LICENSE` & `comfy_cli-2024.4.30/LICENSE`

 * *Files identical despite different names*

### Comparing `comfy_cli-2020.0.0/PKG-INFO` & `comfy_cli-2024.4.30/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: comfy-cli
-Version: 2020.0.0
+Version: 2024.4.30
 Summary: A CLI tool for installing and using ComfyUI.
-Home-page: https://github.com/???/comfy-cli
-Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>
+Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>, "Dr.Lt.Data" <dr.lt.data@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -680,20 +679,25 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/drip-art/comfy-cli.git
 Keywords: comfyui,stable diffusion
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typer>=0.3.0
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: GitPython
+Requires-Dist: rich
+Requires-Dist: requests
+Requires-Dist: pyyaml
+Requires-Dist: typing-extensions
+Requires-Dist: mixpanel
+Requires-Dist: questionary
 
 # comfy-cli
 
 comfy-cli is a command line tool that helps users easily install and manage [ComfyUI](https://github.com/comfyanonymous/ComfyUI), a powerful open-source machine learning framework. With comfy-cli, you can quickly set up ComfyUI, install packages, and manage custom nodes, all from the convenience of your terminal.
 
 ## Features
 
@@ -703,72 +707,200 @@
 - 💻 Cross-platform compatibility (Windows, macOS, Linux)
 - 📖 Comprehensive documentation and examples
 
 ## Installation
 
 To install comfy-cli, make sure you have Python 3.7 or higher installed on your system. Then, run the following command:
 
-pip install comfy-cli
+`pip install comfy-cli`
+
 
 ## Usage
 
 ### Installing ComfyUI
 
 To install ComfyUI using comfy, simply run:
 
-comfy install
+`comfy install`
+
+This command will download and set up the latest version of ComfyUI and ComfyUI-Manager on your
+system. If you run in a ComfyUI repo that has already been setup. The command
+will simply update the comfy.yaml file to reflect the local setup
+
+  * `comfy install --skip-manager`: Install ComfyUI without ComfyUI-Manager.
+  * `comfy --workspace=<path> install`: Install ComfyUI into `<path>/ComfyUI`.
+  * For `comfy install`, if no path specification like `--workspace, --recent, or --here` is provided, it will be implicitly installed in `<HOME>/comfy`.
+
+
+### Specifying execution path
+
+* You can specify the path of ComfyUI where the command will be applied through path indicators as follows:
+  * `comfy --workspace=<path>`: Run from the ComfyUI installed in the specified workspace.
+  * `comfy --recent`: Run from the recently executed or installed ComfyUI.
+  * `comfy --here`: Run from the ComfyUI located in the current directory.
+* --workspace, --recent, and --here options cannot be used simultaneously.
+* If there is no path indicator, the following priority applies:
+  * Run from the default ComfyUI at the path specified by `comfy set-default <path>`.
+  * Run from the recently executed or installed ComfyUI.
+  * Run from the ComfyUI located in the current directory.
+
+* Example 1: To run the recently executed ComfyUI:
+  * `comfy --recent launch`
+* Example 2: To install a package on the ComfyUI in the current directory:
+  * `comfy --here node install ComfyUI-Impact-Pack`
+* Example 3: To update the automatically selected path of ComfyUI and custom nodes based on priority:
+  * `comfy node update all`
+
+* You can use the `comfy which` command to check the path of the target workspace.
+  * e.g) `comfy --recent which`, `comfy --here which`, `comfy which`, ...
+
+### Launch ComfyUI
+
+Comfy provides commands that allow you to easily run the installed ComfyUI.
+
+  `comfy launch`
 
-This command will download and set up the latest version of ComfyUI on your system.
+- To run with default ComfyUI options:
 
-### Managing Packages
+  `comfy launch -- <extra args...>`
+
+  `comfy launch -- --cpu --listen 0.0.0.0`
+
+- To run background
+
+  `comfy launch --background`
+
+  `comfy --workspace=~/comfy launch --background -- --listen 10.0.0.10 --port 8000`
+  - Instances launched with `--background` are displayed in the "Background ComfyUI" section of `comfy env`, providing management functionalities for a single background instance only. 
+  - Since "Comfy Server Running" in `comfy env` only shows the default port 8188, it doesn't display ComfyUI running on a different port.
+  - Background-running ComfyUI can be stopped with `comfy stop`.
+
+
+### Managing Packages [WIP]
 
 comfy allows you to easily install, update, and remove packages for ComfyUI. Here are some examples:
 
 - Install a package:
 
-  comfy package install package-name
+  `comfy package install package-name`
 
 - Update a package:
 
-  comfy package update package-name
+  `comfy package update package-name`
 
 - Remove a package:
 
-  comfy package remove package-name
+  `comfy package remove package-name`
 
 - List installed packages:
 
-  comfy package list
+  `comfy package list`
+
 
 ### Managing Custom Nodes
 
 comfy provides a convenient way to manage custom nodes for extending ComfyUI's functionality. Here are some examples:
 
-- Create a new custom node:
+- Show custom nodes' information:
+ ```
+comfy node [show|simple-show] [installed|enabled|not-installed|disabled|all|snapshot|snapshot-list] 
+                              ?[--channel <channel name>] 
+                              ?[--mode [remote|local|cache]]
+```
+-
+  `comfy node show all --channel recent`
+
+  `comfy node simple-show installed`
+
+  `comfy node update all`
+
+  `comfy node install ComfyUI-Impact-Pack`
+
 
-  comfy-cli node create node-name
+- Managing snapshot:
 
-- Edit an existing custom node:
+  `comfy node save-snapshot`
 
-  comfy-cli node edit node-name
+  `comfy node restore-snapshot <snapshot name>`
 
-- Remove a custom node:
 
-  comfy-cli node remove node-name
+### Managing Models
 
-- List available custom nodes:
+- Model downloading
 
-  comfy-cli node list
+  `comfy model get`
+
+  *Downloading models that have already been installed will 
+
+- Model remove
+
+  `comfy model enable-gui`
+
+- Model list
+
+  `comfy model list`
+
+
+### Managing ComfyUI-Manager
+
+- disable GUI of ComfyUI-Manager (disable Manager menu and Server)
+
+  `comfy manager disable-gui`
+
+- enable GUI of ComfyUI-Manager
+
+  `comfy manager enable-gui`
+
+- Clear reserved startup action:
+
+  `comfy manager clear`
+
+
+## Format of comfy.yaml (WIP)
+
+```
+basic:
+
+models:
+  - model: [name of the model] 
+    url: [url of the source, e.g. https://huggingface.co/...]
+    paths: [list of paths to the model]
+      - path: [path to the model]
+      - path: [path to the model]
+    hash: [md5hash for the model]
+    type: [type of the model, e.g. diffuser, lora, etc.]
+
+  - model:
+  ...
+
+# compatible with ComfyUI-Manager's .yaml snapshot
+custom_nodes:  
+  comfyui: [commit hash]
+  file_custom_nodes:
+  - disabled: [bool]
+    filename: [.py filename]
+    ...
+  git_custom_nodes:
+    [git-url]:
+      disabled: [bool]
+      hash: [commit hash]
+    ...
+```
 
 ## Contributing
 
-We welcome contributions to comfy-cli! If you have any ideas, suggestions, or bug reports, please open an issue on our [GitHub repository](https://github.com/???/comfy-cli). If you'd like to contribute code, please fork the repository and submit a pull request.
+We welcome contributions to comfy-cli! If you have any ideas, suggestions, or
+bug reports, please open an issue on our [GitHub
+repository](https://github.com/Comfy-Org/comfy-cli/issues). If you'd like to contribute code,
+please fork the repository and submit a pull request.
+
 
 ## License
 
 comfy is released under the [GNU General Public License v3.0](https://github.com/drip-art/comfy-cli/blob/master/LICENSE).
 
 ## Support
 
 If you encounter any issues or have questions about comfy-cli, please [open an issue](https://github.com/comfy-cli/issues) on our GitHub repository. We'll be happy to assist you!
 
 Happy diffusing with ComfyUI and comfy-cli! 🎉
+
```

### Comparing `comfy_cli-2020.0.0/comfy_cli.egg-info/PKG-INFO` & `comfy_cli-2024.4.30/comfy_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: comfy-cli
-Version: 2020.0.0
+Version: 2024.4.30
 Summary: A CLI tool for installing and using ComfyUI.
-Home-page: https://github.com/???/comfy-cli
-Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>
+Maintainer-email: Yoland Yan <yoland@drip.art>, James Kwon <hongilkwon316@gmail.com>, Robin Huang <robin@drip.art>, "Dr.Lt.Data" <dr.lt.data@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -680,20 +679,25 @@
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/drip-art/comfy-cli.git
 Keywords: comfyui,stable diffusion
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typer>=0.3.0
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
+Requires-Dist: GitPython
+Requires-Dist: rich
+Requires-Dist: requests
+Requires-Dist: pyyaml
+Requires-Dist: typing-extensions
+Requires-Dist: mixpanel
+Requires-Dist: questionary
 
 # comfy-cli
 
 comfy-cli is a command line tool that helps users easily install and manage [ComfyUI](https://github.com/comfyanonymous/ComfyUI), a powerful open-source machine learning framework. With comfy-cli, you can quickly set up ComfyUI, install packages, and manage custom nodes, all from the convenience of your terminal.
 
 ## Features
 
@@ -703,72 +707,200 @@
 - 💻 Cross-platform compatibility (Windows, macOS, Linux)
 - 📖 Comprehensive documentation and examples
 
 ## Installation
 
 To install comfy-cli, make sure you have Python 3.7 or higher installed on your system. Then, run the following command:
 
-pip install comfy-cli
+`pip install comfy-cli`
+
 
 ## Usage
 
 ### Installing ComfyUI
 
 To install ComfyUI using comfy, simply run:
 
-comfy install
+`comfy install`
+
+This command will download and set up the latest version of ComfyUI and ComfyUI-Manager on your
+system. If you run in a ComfyUI repo that has already been setup. The command
+will simply update the comfy.yaml file to reflect the local setup
+
+  * `comfy install --skip-manager`: Install ComfyUI without ComfyUI-Manager.
+  * `comfy --workspace=<path> install`: Install ComfyUI into `<path>/ComfyUI`.
+  * For `comfy install`, if no path specification like `--workspace, --recent, or --here` is provided, it will be implicitly installed in `<HOME>/comfy`.
+
+
+### Specifying execution path
+
+* You can specify the path of ComfyUI where the command will be applied through path indicators as follows:
+  * `comfy --workspace=<path>`: Run from the ComfyUI installed in the specified workspace.
+  * `comfy --recent`: Run from the recently executed or installed ComfyUI.
+  * `comfy --here`: Run from the ComfyUI located in the current directory.
+* --workspace, --recent, and --here options cannot be used simultaneously.
+* If there is no path indicator, the following priority applies:
+  * Run from the default ComfyUI at the path specified by `comfy set-default <path>`.
+  * Run from the recently executed or installed ComfyUI.
+  * Run from the ComfyUI located in the current directory.
+
+* Example 1: To run the recently executed ComfyUI:
+  * `comfy --recent launch`
+* Example 2: To install a package on the ComfyUI in the current directory:
+  * `comfy --here node install ComfyUI-Impact-Pack`
+* Example 3: To update the automatically selected path of ComfyUI and custom nodes based on priority:
+  * `comfy node update all`
+
+* You can use the `comfy which` command to check the path of the target workspace.
+  * e.g) `comfy --recent which`, `comfy --here which`, `comfy which`, ...
+
+### Launch ComfyUI
+
+Comfy provides commands that allow you to easily run the installed ComfyUI.
+
+  `comfy launch`
 
-This command will download and set up the latest version of ComfyUI on your system.
+- To run with default ComfyUI options:
 
-### Managing Packages
+  `comfy launch -- <extra args...>`
+
+  `comfy launch -- --cpu --listen 0.0.0.0`
+
+- To run background
+
+  `comfy launch --background`
+
+  `comfy --workspace=~/comfy launch --background -- --listen 10.0.0.10 --port 8000`
+  - Instances launched with `--background` are displayed in the "Background ComfyUI" section of `comfy env`, providing management functionalities for a single background instance only. 
+  - Since "Comfy Server Running" in `comfy env` only shows the default port 8188, it doesn't display ComfyUI running on a different port.
+  - Background-running ComfyUI can be stopped with `comfy stop`.
+
+
+### Managing Packages [WIP]
 
 comfy allows you to easily install, update, and remove packages for ComfyUI. Here are some examples:
 
 - Install a package:
 
-  comfy package install package-name
+  `comfy package install package-name`
 
 - Update a package:
 
-  comfy package update package-name
+  `comfy package update package-name`
 
 - Remove a package:
 
-  comfy package remove package-name
+  `comfy package remove package-name`
 
 - List installed packages:
 
-  comfy package list
+  `comfy package list`
+
 
 ### Managing Custom Nodes
 
 comfy provides a convenient way to manage custom nodes for extending ComfyUI's functionality. Here are some examples:
 
-- Create a new custom node:
+- Show custom nodes' information:
+ ```
+comfy node [show|simple-show] [installed|enabled|not-installed|disabled|all|snapshot|snapshot-list] 
+                              ?[--channel <channel name>] 
+                              ?[--mode [remote|local|cache]]
+```
+-
+  `comfy node show all --channel recent`
+
+  `comfy node simple-show installed`
+
+  `comfy node update all`
+
+  `comfy node install ComfyUI-Impact-Pack`
+
 
-  comfy-cli node create node-name
+- Managing snapshot:
 
-- Edit an existing custom node:
+  `comfy node save-snapshot`
 
-  comfy-cli node edit node-name
+  `comfy node restore-snapshot <snapshot name>`
 
-- Remove a custom node:
 
-  comfy-cli node remove node-name
+### Managing Models
 
-- List available custom nodes:
+- Model downloading
 
-  comfy-cli node list
+  `comfy model get`
+
+  *Downloading models that have already been installed will 
+
+- Model remove
+
+  `comfy model enable-gui`
+
+- Model list
+
+  `comfy model list`
+
+
+### Managing ComfyUI-Manager
+
+- disable GUI of ComfyUI-Manager (disable Manager menu and Server)
+
+  `comfy manager disable-gui`
+
+- enable GUI of ComfyUI-Manager
+
+  `comfy manager enable-gui`
+
+- Clear reserved startup action:
+
+  `comfy manager clear`
+
+
+## Format of comfy.yaml (WIP)
+
+```
+basic:
+
+models:
+  - model: [name of the model] 
+    url: [url of the source, e.g. https://huggingface.co/...]
+    paths: [list of paths to the model]
+      - path: [path to the model]
+      - path: [path to the model]
+    hash: [md5hash for the model]
+    type: [type of the model, e.g. diffuser, lora, etc.]
+
+  - model:
+  ...
+
+# compatible with ComfyUI-Manager's .yaml snapshot
+custom_nodes:  
+  comfyui: [commit hash]
+  file_custom_nodes:
+  - disabled: [bool]
+    filename: [.py filename]
+    ...
+  git_custom_nodes:
+    [git-url]:
+      disabled: [bool]
+      hash: [commit hash]
+    ...
+```
 
 ## Contributing
 
-We welcome contributions to comfy-cli! If you have any ideas, suggestions, or bug reports, please open an issue on our [GitHub repository](https://github.com/???/comfy-cli). If you'd like to contribute code, please fork the repository and submit a pull request.
+We welcome contributions to comfy-cli! If you have any ideas, suggestions, or
+bug reports, please open an issue on our [GitHub
+repository](https://github.com/Comfy-Org/comfy-cli/issues). If you'd like to contribute code,
+please fork the repository and submit a pull request.
+
 
 ## License
 
 comfy is released under the [GNU General Public License v3.0](https://github.com/drip-art/comfy-cli/blob/master/LICENSE).
 
 ## Support
 
 If you encounter any issues or have questions about comfy-cli, please [open an issue](https://github.com/comfy-cli/issues) on our GitHub repository. We'll be happy to assist you!
 
 Happy diffusing with ComfyUI and comfy-cli! 🎉
+
```

### Comparing `comfy_cli-2020.0.0/pyproject.toml` & `comfy_cli-2024.4.30/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "comfy-cli"
 license = {file = "LICENSE"}
-version = "2020.0.0"
-requires-python = ">= 3.7"
+version = "2024.4.30"
+requires-python = ">= 3.8"
 description = "A CLI tool for installing and using ComfyUI."
 readme = "README.md"
 keywords = ["comfyui", "stable diffusion"]
 
 maintainers = [
   {name = "Yoland Yan", email = "yoland@drip.art"},
   {name = "James Kwon", email = "hongilkwon316@gmail.com"},
-  {name = "Robin Huang", email = "robin@drip.art"}
+  {name = "Robin Huang", email = "robin@drip.art"},
+  {name = "Dr.Lt.Data", email = "dr.lt.data@gmail.com"}
 ]
 
 dependencies = [
-    "typer>=0.3.0"
+    "typer>=0.3.0",
+    "GitPython",
+    "rich",
+    "requests",
+    "pyyaml",
+    "typing-extensions",
+    "mixpanel",
+    "questionary",
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
 
 [project.scripts]
-comfy = "comfy.cli:main"
+comfy = "comfy_cli.__main__:main"
+comfy-cli = "comfy_cli.__main__:main"
+comfycli = "comfy_cli.__main__:main"
 
 [project.urls]
-Repository = "https://github.com/drip-art/comfy-cli.git"
+Repository = "https://github.com/drip-art/comfy-cli.git"
+
+
+
```

