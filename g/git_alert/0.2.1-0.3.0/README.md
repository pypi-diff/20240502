# Comparing `tmp/git_alert-0.2.1.tar.gz` & `tmp/git_alert-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_alert-0.2.1.tar", max compression
+gzip compressed data, was "git_alert-0.3.0.tar", max compression
```

## Comparing `git_alert-0.2.1.tar` & `git_alert-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1077 2024-04-28 21:20:43.864705 git_alert-0.2.1/LICENSE
--rw-r--r--   0        0        0     3416 2024-04-28 21:20:43.864705 git_alert-0.2.1/README.md
--rw-r--r--   0        0        0      142 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/__init__.py
--rw-r--r--   0        0        0      393 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/__main__.py
--rw-r--r--   0        0        0     1128 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/argument_parser.py
--rw-r--r--   0        0        0     1285 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/repositories.py
--rw-r--r--   0        0        0      433 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/scripts/git_alert.py
--rw-r--r--   0        0        0     1552 2024-04-28 21:20:43.864705 git_alert-0.2.1/git_alert/traverse.py
--rw-r--r--   0        0        0      657 2024-04-28 21:20:43.864705 git_alert-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3900 1970-01-01 00:00:00.000000 git_alert-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-01 15:01:33.825839 git_alert-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5277 2024-05-01 15:01:33.825839 git_alert-0.3.0/README.md
+-rw-r--r--   0        0        0      142 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/__main__.py
+-rw-r--r--   0        0        0     1348 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/argument_parser.py
+-rw-r--r--   0        0        0     1395 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/configuration.py
+-rw-r--r--   0        0        0     1285 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/repositories.py
+-rw-r--r--   0        0        0      983 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/scripts/git_alert.py
+-rw-r--r--   0        0        0     1552 2024-05-01 15:01:33.825839 git_alert-0.3.0/git_alert/traverse.py
+-rw-r--r--   0        0        0      658 2024-05-01 15:01:33.825839 git_alert-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5761 1970-01-01 00:00:00.000000 git_alert-0.3.0/PKG-INFO
```

### Comparing `git_alert-0.2.1/LICENSE` & `git_alert-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.1/git_alert/argument_parser.py` & `git_alert-0.3.0/git_alert/argument_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,34 @@
         paths_as_pathlibPaths = [Path(path) for path in paths_as_strings]
         return paths_as_pathlibPaths
 
     parser = ArgumentParser(
         epilog="Warning: adding a path to ignore will also ignore all subdirectories of that path."
     )
     parser.add_argument(
+        "-p",
         "--path",
         type=Path,
-        default=Path.cwd(),
         help="top level directory to start the search in",
     )
     parser.add_argument(
         "--only_dirty",
         action="store_true",
         help="only show dirty repositories in the final report",
     )
     parser.add_argument(
+        "-i",
         "--ignore",
         type=ignore_paths,
         default=[],
         help="colon separated list of paths to ignore",
     )
+
+    parser.add_argument("-v", "--version", action="version", version="%(prog)s 0.2.0")
+
+    parser.add_argument(
+        "-c",
+        "--config",
+        type=Path,
+        help="path to the configuration file",
+    )
     return parser.parse_args(args)
```

### Comparing `git_alert-0.2.1/git_alert/repositories.py` & `git_alert-0.3.0/git_alert/repositories.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.1/git_alert/traverse.py` & `git_alert-0.3.0/git_alert/traverse.py`

 * *Files identical despite different names*

### Comparing `git_alert-0.2.1/pyproject.toml` & `git_alert-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "git_alert"
-version = "0.2.1"
+version = "0.3.0"
+
 description = "Checks a given path and its sub-directories for dirty git repositories."
 authors = ["Simon Antonius Lauer <simon.lauer@posteo.de>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "git_alert"}]
 
 [tool.poetry.dependencies]
```

### Comparing `git_alert-0.2.1/PKG-INFO` & `git_alert-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git_alert
-Version: 0.2.1
+Version: 0.3.0
 Summary: Checks a given path and its sub-directories for dirty git repositories.
 License: MIT
 Author: Simon Antonius Lauer
 Author-email: simon.lauer@posteo.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -112,40 +112,85 @@
 After rebuilding, you have git_alert at your fingertips and it gets updated whenever you update your flake.
 
 ## Usage:
 
 You can use _git_alert_ by either calling it as a module (`python -m git_alert`) or by directly using the installed package:
 
 ```
-usage: git_alert [-h] [--path PATH] [--only_dirty] [--ignore IGNORE]
+usage: git_alert [-h] [-p PATH] [--only_dirty] [-i IGNORE] [-v] [-c CONFIG]
 
 options:
-  -h, --help       show this help message and exit
-  --path PATH      top level directory to start the search in
-  --only_dirty     only show dirty repositories in the final report
-  --ignore IGNORE  colon separated list of paths to ignore
+  -h, --help            show this help message and exit
+  -p PATH, --path PATH  top level directory to start the search in
+  --only_dirty          only show dirty repositories in the final report
+  -i IGNORE, --ignore IGNORE
+                        colon separated list of paths to ignore
+  -v, --version         show program's version number and exit
+  -c CONFIG, --config CONFIG
+                        path to the configuration file
 
-Warning: adding a path to ignore will also ignore all subdirectories of that path.
+Warning: adding a path to ignore will also ignore all subdirectories of that
+path.
 ```
 
+It should be noted that all options that require a path require an absolute path. The `-i` option can take multiple paths separated by a colon.
+
+## Configuration:
+
+Git Alert can be configured using a configuration file. The configuration file is expected to be in:
+
+```
+$XDG_CONFIG_HOME/git_alert/config.toml (usually ~/.config/git_alert/config.toml)
+```
+
+This behaviour can be overridden by specifying a path to a configuration file with the `-c` option. The configuration file is in TOML format and can contain the following options:
+
+```toml
+path = "/path/to/start/search/in"
+
+only_dirty = true # only show dirty repositories in the final report
+
+[ignore]
+one_directory = '/path/to/one_directory'
+another_directory = '/path/to/another_directory'
+```
+
+Hence, the configuration file closely resembles the command line options. The command line options will always override the configuration file. However,
+_only_dirty_ is a special case. If it is set to true in the configuration file, it will be applied. The command line flag can only turn it on, not off.
+
 ## Development:
 
 The tool is aimed to be improved and extended going forward. If you have any ideas or want to contribute, feel free to open an issue or a pull request.
 
 ## Goals:
 
 - [ ] more detailed checks (currently it distinguishes only between a repository being clean or not)
 - [ ] speed up the lookup process
 - [ ] enable caching found repositories for faster checking after the first run (maybe utilizing a database)
-- [ ] GUI interface
+- [ ] GUI/ TUI interface
+- [ ] override default configuration file location with command line option
 
 ## Contributing:
 
 This project is under active development, so any contributions are welcome. Feel free to open an issue or a pull request.
 
 In case you want to submit a pull request, please:
 
 - make sure to run the tests before submission
 - use black for code formatting
 
 The project uses pre-commit hooks to ensure code quality, so feel free to use them as well.
+usage: git_alert [-h] [-p PATH] [--only_dirty] [-i IGNORE] [-v] [-c CONFIG]
+
+options:
+-h, --help show this help message and exit
+-p PATH, --path PATH top level directory to start the search in
+--only_dirty only show dirty repositories in the final report
+-i IGNORE, --ignore IGNORE
+colon separated list of paths to ignore
+-v, --version show program's version number and exit
+-c CONFIG, --config CONFIG
+path to the configuration file
+
+Warning: adding a path to ignore will also ignore all subdirectories of that
+path.
```

