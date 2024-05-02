# Comparing `tmp/batchfetch-1.0.2.tar.gz` & `tmp/batchfetch-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchfetch-1.0.2.tar", last modified: Thu May  2 18:07:13 2024, max compression
+gzip compressed data, was "batchfetch-1.0.3.tar", last modified: Thu May  2 18:41:01 2024, max compression
```

## Comparing `batchfetch-1.0.2.tar` & `batchfetch-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.742270 batchfetch-1.0.2/
--rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-02 12:24:09.000000 batchfetch-1.0.2/.gitignore
--rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-02 12:24:09.000000 batchfetch-1.0.2/LICENSE
--rw-r--r--   0 dev        (455) work      (1000)     3408 2024-05-02 18:07:13.738936 batchfetch-1.0.2/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)     2535 2024-05-02 18:06:03.000000 batchfetch-1.0.2/README.md
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/batchfetch/
--rw-r--r--   0 dev        (455) work      (1000)      883 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/__init__.py
--rw-r--r--   0 dev        (455) work      (1000)     5541 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/batchfetch_base.py
--rw-r--r--   0 dev        (455) work      (1000)     8655 2024-05-02 18:05:39.000000 batchfetch-1.0.2/batchfetch/batchfetch_cli.py
--rw-r--r--   0 dev        (455) work      (1000)    11874 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/batchfetch_git.py
--rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-02 12:24:09.000000 batchfetch-1.0.2/batchfetch/helpers.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/batchfetch.egg-info/
--rw-r--r--   0 dev        (455) work      (1000)     3408 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/PKG-INFO
--rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/SOURCES.txt
--rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/dependency_links.txt
--rw-r--r--   0 dev        (455) work      (1000)       74 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/entry_points.txt
--rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/requires.txt
--rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-02 18:07:13.000000 batchfetch-1.0.2/batchfetch.egg-info/top_level.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-02 12:24:09.000000 batchfetch-1.0.2/run_tests.sh
--rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-02 18:07:13.742270 batchfetch-1.0.2/setup.cfg
--rwxr-xr-x   0 dev        (455) work      (1000)     2023 2024-05-02 18:06:46.000000 batchfetch-1.0.2/setup.py
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/tests/
-drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:07:13.738936 batchfetch-1.0.2/tests/data/
--rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-02 12:24:09.000000 batchfetch-1.0.2/tests/data/test-md5sum.txt
--rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-02 12:24:09.000000 batchfetch-1.0.2/tests/data/test-run_simple.sh
--rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-02 12:24:09.000000 batchfetch-1.0.2/tests/test_helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:41:01.747427 batchfetch-1.0.3/
+-rw-r--r--   0 dev        (455) work      (1000)     2034 2024-05-02 12:24:09.000000 batchfetch-1.0.3/.gitignore
+-rw-r--r--   0 dev        (455) work      (1000)    35149 2024-05-02 12:24:09.000000 batchfetch-1.0.3/LICENSE
+-rw-r--r--   0 dev        (455) work      (1000)     4483 2024-05-02 18:41:01.744093 batchfetch-1.0.3/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)     3610 2024-05-02 18:37:55.000000 batchfetch-1.0.3/README.md
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:41:01.744093 batchfetch-1.0.3/batchfetch/
+-rw-r--r--   0 dev        (455) work      (1000)      883 2024-05-02 12:24:09.000000 batchfetch-1.0.3/batchfetch/__init__.py
+-rw-r--r--   0 dev        (455) work      (1000)     5541 2024-05-02 12:24:09.000000 batchfetch-1.0.3/batchfetch/batchfetch_base.py
+-rw-r--r--   0 dev        (455) work      (1000)     8662 2024-05-02 18:39:20.000000 batchfetch-1.0.3/batchfetch/batchfetch_cli.py
+-rw-r--r--   0 dev        (455) work      (1000)    11874 2024-05-02 12:24:09.000000 batchfetch-1.0.3/batchfetch/batchfetch_git.py
+-rw-r--r--   0 dev        (455) work      (1000)     4081 2024-05-02 12:24:09.000000 batchfetch-1.0.3/batchfetch/helpers.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:41:01.744093 batchfetch-1.0.3/batchfetch.egg-info/
+-rw-r--r--   0 dev        (455) work      (1000)     4483 2024-05-02 18:41:01.000000 batchfetch-1.0.3/batchfetch.egg-info/PKG-INFO
+-rw-r--r--   0 dev        (455) work      (1000)      468 2024-05-02 18:41:01.000000 batchfetch-1.0.3/batchfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 dev        (455) work      (1000)        1 2024-05-02 18:41:01.000000 batchfetch-1.0.3/batchfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 dev        (455) work      (1000)       74 2024-05-02 18:41:01.000000 batchfetch-1.0.3/batchfetch.egg-info/entry_points.txt
+-rw-r--r--   0 dev        (455) work      (1000)       36 2024-05-02 18:41:01.000000 batchfetch-1.0.3/batchfetch.egg-info/requires.txt
+-rw-r--r--   0 dev        (455) work      (1000)       11 2024-05-02 18:41:01.000000 batchfetch-1.0.3/batchfetch.egg-info/top_level.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      916 2024-05-02 12:24:09.000000 batchfetch-1.0.3/run_tests.sh
+-rw-r--r--   0 dev        (455) work      (1000)       38 2024-05-02 18:41:01.747427 batchfetch-1.0.3/setup.cfg
+-rwxr-xr-x   0 dev        (455) work      (1000)     2023 2024-05-02 18:40:12.000000 batchfetch-1.0.3/setup.py
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:41:01.744093 batchfetch-1.0.3/tests/
+drwxr-xr-x   0 dev        (455) work      (1000)        0 2024-05-02 18:41:01.744093 batchfetch-1.0.3/tests/data/
+-rw-r--r--   0 dev        (455) work      (1000)       24 2024-05-02 12:24:09.000000 batchfetch-1.0.3/tests/data/test-md5sum.txt
+-rwxr-xr-x   0 dev        (455) work      (1000)      117 2024-05-02 12:24:09.000000 batchfetch-1.0.3/tests/data/test-run_simple.sh
+-rw-r--r--   0 dev        (455) work      (1000)     1870 2024-05-02 12:24:09.000000 batchfetch-1.0.3/tests/test_helpers.py
```

### Comparing `batchfetch-1.0.2/.gitignore` & `batchfetch-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/LICENSE` & `batchfetch-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/PKG-INFO` & `batchfetch-1.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,22 @@
-Metadata-Version: 2.1
-Name: batchfetch
-Version: 1.0.2
-Summary: Efficiently clone and pull multiple Git repositories.
-Home-page: https://github.com/jamescherti/batchfetch
-Author: James Cherti
-License: GPLv3
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Environment :: Console
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: POSIX :: Other
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: Utilities
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: colorama
-Requires-Dist: schema
-Requires-Dist: setproctitle
-Requires-Dist: PyYAML
-
-# Batchfetch - Efficiently clone or pull multiple Git repositories.
+# Batchfetch - Efficiently clone or pull multiple Git repositories in parallel
 
 ## Introduction
 
-Efficiently clone or pull multiple Git repositories in parallel. Ideal for developers managing multiple projects or for downloading plugins or packages in bulk.
+Batchfetch is a command-line tool designed to clone, fetch, and merge multiple Git repositories simultaneously.
+
+With Batchfetch, you no longer need to manually manage each repository one by one. It automates the tedious aspects of repository management, freeing you up to focus on what truly matters: your workflow.
+
+Batchfetch is ideal for quickly cloning or pulling multiple Git repositories. It is also useful for cloning various addons, such as Vim plugins, Emacs packages, Ansible roles, Ansible collections, and other addons available on websites like GitHub, Codeberg, and GitLab.
+
+## Features:
+- Git Clone and Fetch/Merge: Clones the repositories and their submodules, ensuring that all the repositories are always up-to-date by fetching and merging changes.
+- Parallel Operations: Utilizes threads to simultaneously Git clone or pull multiple repositories, dramatically reducing wait times.
+- User-Friendly Interface: Provides simple and straightforward command-line options that make it easy to get started and effectively manage your repositories.
+- Custom Configuration: Allows the use of a YAML configuration file to specify and manage the repositories you interact with, enabling repeatable setups and consistent environments.
 
 ## Installation
 
 ```
 pip install --user batchfetch
 ```
 
@@ -65,23 +51,23 @@
 
 Execute the `batchfetch` command from the same directory as `batchfetch.yml` to make it clone or update the local copies of the repositories above.
 
 ## Usage
 
 Here are the various options that `batchfetch` provides, along with descriptions of their usage:
 
-```sh
+```
 usage: batchfetch [--option] [args]
 
 Command line interface.
 
 options:
   -h, --help            show this help message and exit
-  -p MAX_PROCS, --max-procs MAX_PROCS
-                        Run up to N Number of parallel git processes (Default: 3).
+  -j JOBS, --jobs JOBS
+                        Run up to N Number of parallel git processes (Default: 5).
   -v, --verbose         Enable verbose mode.
   -f BATCHFETCH_FILE, --batchfetch-file BATCHFETCH_FILE
                         Specify the batchfetch YAML file (default: './batchfetch.yaml').
 ```
 ## License
 
 Copyright (c) [James Cherti](https://www.jamescherti.com)
```

### Comparing `batchfetch-1.0.2/batchfetch/__init__.py` & `batchfetch-1.0.3/batchfetch/__init__.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/batchfetch/batchfetch_base.py` & `batchfetch-1.0.3/batchfetch/batchfetch_base.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/batchfetch/batchfetch_cli.py` & `batchfetch-1.0.3/batchfetch/batchfetch_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             else:
                 print("Failed.")
 
             return False
         else:
             if num_success == 0:
                 print("Already up to date.")
-            else:
+            elif not self.verbose:
                 print("Success.")
 
         return True
 
     # def check_managed_directories(self):
     #     # managed_downloads = {Path(item).resolve()
     #     #                      for item in self.managed_filenames}
@@ -201,16 +201,16 @@
 def parse_args():
     """Parse the command line arguments."""
     desc = __doc__
     usage = "%(prog)s [--option] [args]"
     parser = argparse.ArgumentParser(description=desc, usage=usage)
 
     parser.add_argument(
-        "-p", "--max-procs", default="3", required=False,
-        help="Run up to N Number of parallel git processes (Default: 3).",
+        "-j", "--jobs", default="5", required=False,
+        help="Run up to N Number of parallel git processes (Default: 5).",
     )
 
     parser.add_argument(
         "-v", "--verbose", action="store_true", default=False,
         help="Enable verbose mode.",
     )
 
@@ -240,15 +240,15 @@
 
     colorama.init()
     setproctitle(subprocess.list2cmdline([Path(sys.argv[0]).name] +
                                          sys.argv[1:]))
 
     args = parse_args()
     downloader_cli = BatchFetchCli(verbose=args.verbose,
-                                   max_workers=int(args.max_procs))
+                                   max_workers=int(args.jobs))
 
     downloader_cli.load(args.batchfetch_file)
     os.chdir(os.path.dirname(args.batchfetch_file))
 
     try:
         if not downloader_cli.download():
             errno = 1
```

### Comparing `batchfetch-1.0.2/batchfetch/batchfetch_git.py` & `batchfetch-1.0.3/batchfetch/batchfetch_git.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/batchfetch/helpers.py` & `batchfetch-1.0.3/batchfetch/helpers.py`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/run_tests.sh` & `batchfetch-1.0.3/run_tests.sh`

 * *Files identical despite different names*

### Comparing `batchfetch-1.0.2/setup.py` & `batchfetch-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 setup(
     name="batchfetch",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     description="Efficiently clone and pull multiple Git repositories.",
     license="GPLv3",
     long_description=((Path(__file__).parent.resolve().joinpath("README.md"))
                       .read_text(encoding="utf-8")),
     long_description_content_type="text/markdown",
     url="https://github.com/jamescherti/batchfetch",
```

### Comparing `batchfetch-1.0.2/tests/test_helpers.py` & `batchfetch-1.0.3/tests/test_helpers.py`

 * *Files identical despite different names*

