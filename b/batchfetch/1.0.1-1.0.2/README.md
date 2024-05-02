# Comparing `tmp/batchfetch-1.0.1.tar.gz` & `tmp/batchfetch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.0.1.tar", last modified: Thu May  2 17:21:33 2024, max compression
+gzip compressed data, was "batchfetch-1.0.2.tar", last modified: Thu May  2 18:07:13 2024, max compression
```

## Comparing `batchfetch-1.0.1.tar` & `batchfetch-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 17:21:33.183903 batchfetch-1.0.1/
--rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-02 12:24:09.000000 batchfetch-1.0.1/.gitignore
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-02 12:24:09.000000 batchfetch-1.0.1/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     2739 2024-05-02 17:21:33.180570 batchfetch-1.0.1/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     1866 2024-05-02 16:02:49.000000 batchfetch-1.0.1/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 17:21:33.180570 batchfetch-1.0.1/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      883 2024-05-02 12:24:09.000000 batchfetch-1.0.1/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5541 2024-05-02 12:24:09.000000 batchfetch-1.0.1/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     8249 2024-05-02 12:24:09.000000 batchfetch-1.0.1/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    11874 2024-05-02 12:24:09.000000 batchfetch-1.0.1/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-02 12:24:09.000000 batchfetch-1.0.1/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 17:21:33.180570 batchfetch-1.0.1/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     2739 2024-05-02 17:21:33.000000 batchfetch-1.0.1/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-02 17:21:33.000000 batchfetch-1.0.1/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-02 17:21:33.000000 batchfetch-1.0.1/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       74 2024-05-02 17:21:33.000000 batchfetch-1.0.1/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-02 17:21:33.000000 batchfetch-1.0.1/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-02 17:21:33.000000 batchfetch-1.0.1/batchfetch.egg-info/top_level.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-02 12:24:09.000000 batchfetch-1.0.1/run_tests.sh
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-02 17:21:33.183903 batchfetch-1.0.1/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2023 2024-05-02 17:18:56.000000 batchfetch-1.0.1/setup.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 17:21:33.180570 batchfetch-1.0.1/tests/
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 17:21:33.180570 batchfetch-1.0.1/tests/data/
--rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-02 12:24:09.000000 batchfetch-1.0.1/tests/data/test-md5sum.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-02 12:24:09.000000 batchfetch-1.0.1/tests/data/test-run_simple.sh
--rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-02 12:24:09.000000 batchfetch-1.0.1/tests/test_helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.742270 batchfetch-1.0.2/
+-rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-02 12:24:09.000000 batchfetch-1.0.2/.gitignore
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-02 12:24:09.000000 batchfetch-1.0.2/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     3408 2024-05-02 18:07:13.738936 batchfetch-1.0.2/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     2535 2024-05-02 18:06:03.000000 batchfetch-1.0.2/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      883 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5541 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     8655 2024-05-02 18:05:39.000000 batchfetch-1.0.2/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    11874 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     3408 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       74 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/top_level.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-02 12:24:09.000000 batchfetch-1.0.2/run_tests.sh
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-02 18:07:13.742270 batchfetch-1.0.2/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2023 2024-05-02 18:06:46.000000 batchfetch-1.0.2/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/tests/
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/tests/data/
+-rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-02 12:24:09.000000 batchfetch-1.0.2/tests/data/test-md5sum.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-02 12:24:09.000000 batchfetch-1.0.2/tests/data/test-run_simple.sh
+-rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-02 12:24:09.000000 batchfetch-1.0.2/tests/test_helpers.py
```

### Comparing `batchfetch-1.0.1/.gitignore` & `batchfetch-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/LICENSE` & `batchfetch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/PKG-INFO` & `batchfetch-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,17 +27,19 @@
 ## Introduction
 
 Efficiently clone or pull multiple Git repositories in parallel. Ideal for developers managing multiple projects or for downloading plugins or packages in bulk.
 
 ## Installation
 
 ```
-sudo pip install git+https://github.com/jamescherti/batchfetch
+pip install --user batchfetch
 ```
 
+The pip command above will install the `batchfetch` executable in the directory `~/.local/bin/`.
+
 ## Example
 
 Here is an example of a `batchfetch.yaml` file:
 
 ```yaml
 ---
 
@@ -59,20 +61,38 @@
   # Delete './impatient-mode'
   - git: https://github.com/skeeto/impatient-mode
     delete: true
 ```
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
 
+## Usage
+
+Here are the various options that `batchfetch` provides, along with descriptions of their usage:
+
+```sh
+usage: batchfetch [--option] [args]
+
+Command line interface.
+
+options:
+  -h, --help            show this help message and exit
+  -p MAX_PROCS, --max-procs MAX_PROCS
+                        Run up to N Number of parallel git processes (Default: 3).
+  -v, --verbose         Enable verbose mode.
+  -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
+                        Specify the batchfetch YAML file (default: './batchfetch.yaml').
+```
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.
 
 ## Links
 
-- [The batchfetch Git repository](https://github.com/jamescherti/batchfetch)
+- [batchfetch @GitHub](https://github.com/jamescherti/batchfetch)
+- [batchfetch @Pypi](https://pypi.org/project/batchfetch/)
```

### Comparing `batchfetch-1.0.1/README.md` & `batchfetch-1.0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 ## Introduction
 
 Efficiently clone or pull multiple Git repositories in parallel. Ideal for developers managing multiple projects or for downloading plugins or packages in bulk.
 
 ## Installation
 
 ```
-sudo pip install git+https://github.com/jamescherti/batchfetch
+pip install --user batchfetch
 ```
 
+The pip command above will install the `batchfetch` executable in the directory `~/.local/bin/`.
+
 ## Example
 
 Here is an example of a `batchfetch.yaml` file:
 
 ```yaml
 ---
 
@@ -35,20 +37,38 @@
   # Delete './impatient-mode'
   - git: https://github.com/skeeto/impatient-mode
     delete: true
 ```
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
 
+## Usage
+
+Here are the various options that `batchfetch` provides, along with descriptions of their usage:
+
+```sh
+usage: batchfetch [--option] [args]
+
+Command line interface.
+
+options:
+  -h, --help            show this help message and exit
+  -p MAX_PROCS, --max-procs MAX_PROCS
+                        Run up to N Number of parallel git processes (Default: 3).
+  -v, --verbose         Enable verbose mode.
+  -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
+                        Specify the batchfetch YAML file (default: './batchfetch.yaml').
+```
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.
 
 ## Links
 
-- [The batchfetch Git repository](https://github.com/jamescherti/batchfetch)
+- [batchfetch @GitHub](https://github.com/jamescherti/batchfetch)
+- [batchfetch @Pypi](https://pypi.org/project/batchfetch/)
```

### Comparing `batchfetch-1.0.1/batchfetch/__init__.py` & `batchfetch-1.0.2/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/batchfetch/batchfetch_base.py` & `batchfetch-1.0.2/batchfetch/batchfetch_base.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/batchfetch/batchfetch_cli.py` & `batchfetch-1.0.2/batchfetch/batchfetch_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <https://www.gnu.org/licenses/>.
 #
 """Command line interface."""
 
 import argparse
 import logging
+import os
 import subprocess
 import sys
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from typing import Set
 
 import colorama
@@ -197,47 +198,61 @@
     #     pass
 
 
 def parse_args():
     """Parse the command line arguments."""
     desc = __doc__
     usage = "%(prog)s [--option] [args]"
-    parser = argparse.ArgumentParser(description=desc,
-                                     usage=usage)
+    parser = argparse.ArgumentParser(description=desc, usage=usage)
+
     parser.add_argument(
         "-p", "--max-procs", default="3", required=False,
-        help="Run up to N Number of parallel git fetch processes.",
+        help="Run up to N Number of parallel git processes (Default: 3).",
     )
 
     parser.add_argument(
         "-v", "--verbose", action="store_true", default=False,
-        help="Verbose mode.",
+        help="Enable verbose mode.",
+    )
+
+    parser.add_argument(
+        "-f",
+        "--batchfetch-file",
+        default="./batchfetch.yaml",
+        required=False,
+        help="Specify the batchfetch YAML file (default: './batchfetch.yaml').",
     )
 
     args = parser.parse_args()
+
+    if not Path(args.batchfetch_file).is_file():
+        print(f"Error: File not found: {args.batchfetch_file}",
+              file=sys.stderr)
+        sys.exit(1)
+
     return args
 
 
 def command_line_interface():
     """Command line interface."""
     errno = 0
     logging.basicConfig(level=logging.INFO, stream=sys.stdout,
                         format="%(asctime)s %(name)s: %(message)s")
 
     colorama.init()
-    setproctitle(subprocess.list2cmdline(
-        [Path(sys.argv[0]).name] + sys.argv[1:]
-    ))
+    setproctitle(subprocess.list2cmdline([Path(sys.argv[0]).name] +
+                                         sys.argv[1:]))
 
     args = parse_args()
-
-    path_batchfetch_yaml = "batchfetch.yaml"
     downloader_cli = BatchFetchCli(verbose=args.verbose,
                                    max_workers=int(args.max_procs))
-    downloader_cli.load(path_batchfetch_yaml)
+
+    downloader_cli.load(args.batchfetch_file)
+    os.chdir(os.path.dirname(args.batchfetch_file))
+
     try:
         if not downloader_cli.download():
             errno = 1
     except KeyboardInterrupt:
         print("Interrupted.", file=sys.stderr)
         errno = 1
     except BatchFetchError as err:
```

### Comparing `batchfetch-1.0.1/batchfetch/batchfetch_git.py` & `batchfetch-1.0.2/batchfetch/batchfetch_git.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/batchfetch/helpers.py` & `batchfetch-1.0.2/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/batchfetch.egg-info/PKG-INFO` & `batchfetch-1.0.2/batchfetch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchfetch
-Version: 1.0.1
+Version: 1.0.2
 Summary: Efficiently clone and pull multiple Git repositories.
 Home-page: https://github.com/jamescherti/batchfetch
 Author: James Cherti
 License: GPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -27,17 +27,19 @@
 ## Introduction
 
 Efficiently clone or pull multiple Git repositories in parallel. Ideal for developers managing multiple projects or for downloading plugins or packages in bulk.
 
 ## Installation
 
 ```
-sudo pip install git+https://github.com/jamescherti/batchfetch
+pip install --user batchfetch
 ```
 
+The pip command above will install the `batchfetch` executable in the directory `~/.local/bin/`.
+
 ## Example
 
 Here is an example of a `batchfetch.yaml` file:
 
 ```yaml
 ---
 
@@ -59,20 +61,38 @@
   # Delete './impatient-mode'
   - git: https://github.com/skeeto/impatient-mode
     delete: true
 ```
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
 
+## Usage
+
+Here are the various options that `batchfetch` provides, along with descriptions of their usage:
+
+```sh
+usage: batchfetch [--option] [args]
+
+Command line interface.
+
+options:
+  -h, --help            show this help message and exit
+  -p MAX_PROCS, --max-procs MAX_PROCS
+                        Run up to N Number of parallel git processes (Default: 3).
+  -v, --verbose         Enable verbose mode.
+  -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
+                        Specify the batchfetch YAML file (default: './batchfetch.yaml').
+```
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.
 
 ## Links
 
-- [The batchfetch Git repository](https://github.com/jamescherti/batchfetch)
+- [batchfetch @GitHub](https://github.com/jamescherti/batchfetch)
+- [batchfetch @Pypi](https://pypi.org/project/batchfetch/)
```

### Comparing `batchfetch-1.0.1/run_tests.sh` & `batchfetch-1.0.2/run_tests.sh`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.1/setup.py` & `batchfetch-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

### Comparing `batchfetch-1.0.1/tests/test_helpers.py` & `batchfetch-1.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

