# Comparing `tmp/gouge-2.2.2.post1.tar.gz` & `tmp/gouge-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gouge-2.2.2.post1.tar", last modified: Thu May  2 06:54:55 2024, max compression
+gzip compressed data, was "gouge-2.2.3.tar", last modified: Thu May  2 07:07:18 2024, max compression
```

## Comparing `gouge-2.2.2.post1.tar` & `gouge-2.2.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.devcontainer/init.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/pre-formatter-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/pre-formatter-not-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/snapshot1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/fabfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/src/gouge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/parseable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/preformatters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/src/gouge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_caplog.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_preformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_shifting_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.065598 gouge-2.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-02 07:07:11.000000 gouge-2.2.3/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 07:07:11.000000 gouge-2.2.3/.devcontainer/init.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 07:07:11.000000 gouge-2.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-02 07:07:11.000000 gouge-2.2.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-02 07:07:11.000000 gouge-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-02 07:07:11.000000 gouge-2.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 07:07:11.000000 gouge-2.2.3/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 07:07:11.000000 gouge-2.2.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 07:07:11.000000 gouge-2.2.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-02 07:07:18.065598 gouge-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 07:07:11.000000 gouge-2.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/_static/pre-formatter-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/_static/pre-formatter-not-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/_static/snapshot1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.061598 gouge-2.2.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-02 07:07:11.000000 gouge-2.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 07:07:11.000000 gouge-2.2.3/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-02 07:07:11.000000 gouge-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:07:18.065598 gouge-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.057598 gouge-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.065598 gouge-2.2.3/src/gouge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:11.000000 gouge-2.2.3/src/gouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-02 07:07:11.000000 gouge-2.2.3/src/gouge/colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-02 07:07:11.000000 gouge-2.2.3/src/gouge/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-02 07:07:11.000000 gouge-2.2.3/src/gouge/parseable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 07:07:11.000000 gouge-2.2.3/src/gouge/preformatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:11.000000 gouge-2.2.3/src/gouge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.065598 gouge-2.2.3/src/gouge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-02 07:07:18.000000 gouge-2.2.3/src/gouge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-02 07:07:18.000000 gouge-2.2.3/src/gouge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:07:18.000000 gouge-2.2.3/src/gouge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 07:07:18.000000 gouge-2.2.3/src/gouge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 07:07:18.000000 gouge-2.2.3/src/gouge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:07:18.065598 gouge-2.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 07:07:11.000000 gouge-2.2.3/test/test_caplog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 07:07:11.000000 gouge-2.2.3/test/test_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-02 07:07:11.000000 gouge-2.2.3/test/test_colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 07:07:11.000000 gouge-2.2.3/test/test_preformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-02 07:07:11.000000 gouge-2.2.3/test/test_shifting_filter.py
```

### Comparing `gouge-2.2.2.post1/.devcontainer/devcontainer.json` & `gouge-2.2.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/.github/workflows/main.yml` & `gouge-2.2.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/.gitignore` & `gouge-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/.pre-commit-config.yaml` & `gouge-2.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/PKG-INFO` & `gouge-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.2.2.post1
+Version: 2.2.3
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.2.2.post1/README.rst` & `gouge-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/docs/Makefile` & `gouge-2.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/docs/_static/pre-formatter-applied.png` & `gouge-2.2.3/docs/_static/pre-formatter-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/docs/_static/pre-formatter-not-applied.png` & `gouge-2.2.3/docs/_static/pre-formatter-not-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/docs/_static/snapshot1.png` & `gouge-2.2.3/docs/_static/snapshot1.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/docs/changelog.rst` & `gouge-2.2.3/docs/changelog.rst`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,17 @@
   now fixed.
 
 * [2.2.2] - fix: Correctly initialise the "highlighted_path" value
 
 * [2.2.2post1] - fix: Corrected the "preformatters" example from the
   documentation
 
+* [2.2.3] - fix: Path highlighting in exception messages should now work with
+  absolute paths
+
 Version 2.1
 -----------
 
 * Added support for pre-formatters.
 * Provide bundled pre-formatter for ``uvicorn.access`` via
   ``gouge.preformatters``
```

### Comparing `gouge-2.2.2.post1/docs/conf.py` & `gouge-2.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/docs/index.rst` & `gouge-2.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/fabfile.py` & `gouge-2.2.3/fabfile.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/pyproject.toml` & `gouge-2.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gouge"
-version = "2.2.2post1"
+version = "2.2.3"
 authors = [
     {name = "Michel Albert", email = "michel@albert.lu"},
 ]
 description = "Collection of logging formatters."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {text = "BSD-3-Clause"}
```

### Comparing `gouge-2.2.2.post1/src/gouge/colourcli.py` & `gouge-2.2.3/src/gouge/colourcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         super().__init__(fmt, datefmt, style, **python_310_args)
         self.show_threads = show_threads
         self.show_exc = show_exc
         self.force_styling = force_styling
         self.show_pid = show_pid
         self.pre_formatters = pre_formatters or {}
         if (Path.cwd() / "src").exists():
-            self.highlighted_path = Path.cwd() / "src"
+            self.highlighted_path = (Path.cwd() / "src").absolute()
         else:
-            self.highlighted_path = highlighted_path
+            self.highlighted_path = (highlighted_path).absolute()
 
     def format(self, record: LogRecord) -> str:
         if record.levelno <= logging.DEBUG:
             colorize = clr.Style.BRIGHT + clr.Fore.BLACK
         elif record.levelno <= logging.INFO:
             colorize = clr.Fore.CYAN
         elif record.levelno <= logging.WARNING:
@@ -173,15 +173,15 @@
             exc_text = exc_text.replace("{", "{{").replace("}", "}}")
         if self.highlighted_path is None:
             return exc_text
 
         pth = self.highlighted_path
 
         def highlight_local_filenames(match: re.Match) -> str:
-            filename = Path(match.group(1))
+            filename = Path(match.group(1)).absolute()
             if filename.is_relative_to(pth):
                 return match.group(0).replace(
                     match.group(1),
                     f"{clr.Fore.YELLOW}{match.group(1)}{clr.Fore.RED}",
                 )
             return match.group(0)
```

### Comparing `gouge-2.2.2.post1/src/gouge/filters.py` & `gouge-2.2.3/src/gouge/filters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/src/gouge/parseable.py` & `gouge-2.2.3/src/gouge/parseable.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/src/gouge/preformatters.py` & `gouge-2.2.3/src/gouge/preformatters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/src/gouge.egg-info/PKG-INFO` & `gouge-2.2.3/src/gouge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.2.2.post1
+Version: 2.2.3
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.2.2.post1/src/gouge.egg-info/SOURCES.txt` & `gouge-2.2.3/src/gouge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/test/test_coloring.py` & `gouge-2.2.3/test/test_coloring.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/test/test_colourcli.py` & `gouge-2.2.3/test/test_colourcli.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/test/test_preformatter.py` & `gouge-2.2.3/test/test_preformatter.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2.post1/test/test_shifting_filter.py` & `gouge-2.2.3/test/test_shifting_filter.py`

 * *Files identical despite different names*

