# Comparing `tmp/gouge-2.2.2.tar.gz` & `tmp/gouge-2.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gouge-2.2.2.tar", last modified: Thu Apr 25 11:21:07 2024, max compression
+gzip compressed data, was "gouge-2.2.2.post1.tar", last modified: Thu May  2 06:54:55 2024, max compression
```

## Comparing `gouge-2.2.2.tar` & `gouge-2.2.2.post1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-25 11:21:00.000000 gouge-2.2.2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-25 11:21:00.000000 gouge-2.2.2/.devcontainer/init.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-25 11:21:00.000000 gouge-2.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-25 11:21:00.000000 gouge-2.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-25 11:21:00.000000 gouge-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 11:21:00.000000 gouge-2.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-25 11:21:00.000000 gouge-2.2.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 11:21:00.000000 gouge-2.2.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-25 11:21:00.000000 gouge-2.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 11:21:07.064050 gouge-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-25 11:21:00.000000 gouge-2.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/pre-formatter-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/pre-formatter-not-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_static/snapshot1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-25 11:21:00.000000 gouge-2.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-25 11:21:00.000000 gouge-2.2.2/fabfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-25 11:21:00.000000 gouge-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:21:07.064050 gouge-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.060050 gouge-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/src/gouge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/parseable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/preformatters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:00.000000 gouge-2.2.2/src/gouge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/src/gouge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-25 11:21:07.000000 gouge-2.2.2/src/gouge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:21:07.064050 gouge-2.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_caplog.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_preformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-25 11:21:00.000000 gouge-2.2.2/test/test_shifting_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.devcontainer/init.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/pre-formatter-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/pre-formatter-not-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_static/snapshot1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.196269 gouge-2.2.2.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.200269 gouge-2.2.2.post1/src/gouge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/parseable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/preformatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/src/gouge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/src/gouge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 06:54:55.000000 gouge-2.2.2.post1/src/gouge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:54:55.204269 gouge-2.2.2.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_caplog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_preformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-05-02 06:54:49.000000 gouge-2.2.2.post1/test/test_shifting_filter.py
```

### Comparing `gouge-2.2.2/.devcontainer/devcontainer.json` & `gouge-2.2.2.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/.github/workflows/main.yml` & `gouge-2.2.2.post1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/.gitignore` & `gouge-2.2.2.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/.pre-commit-config.yaml` & `gouge-2.2.2.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/PKG-INFO` & `gouge-2.2.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.2.2
+Version: 2.2.2.post1
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.2.2/README.rst` & `gouge-2.2.2.post1/README.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/docs/Makefile` & `gouge-2.2.2.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/docs/_static/pre-formatter-applied.png` & `gouge-2.2.2.post1/docs/_static/pre-formatter-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/docs/_static/pre-formatter-not-applied.png` & `gouge-2.2.2.post1/docs/_static/pre-formatter-not-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/docs/_static/snapshot1.png` & `gouge-2.2.2.post1/docs/_static/snapshot1.png`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/docs/changelog.rst` & `gouge-2.2.2.post1/docs/changelog.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 * [2.2.1] - fix: If the message or traceback contained Python string-template
   variables the output could either break or cause incorrect output. This is
   now fixed.
 
 * [2.2.2] - fix: Correctly initialise the "highlighted_path" value
 
+* [2.2.2post1] - fix: Corrected the "preformatters" example from the
+  documentation
+
 Version 2.1
 -----------
 
 * Added support for pre-formatters.
 * Provide bundled pre-formatter for ``uvicorn.access`` via
   ``gouge.preformatters``
```

### Comparing `gouge-2.2.2/docs/conf.py` & `gouge-2.2.2.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/docs/index.rst` & `gouge-2.2.2.post1/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -227,42 +227,65 @@
         return message.upper()
 
     my_log_formatter = Simple(pre_formatters={"my.logger": [my_preformatter]})
 
 Using Pre-Formatters With dictConfig
 -------------------------------------
 
+This example demostrates the use of the builtin ``uvicorn_access``
+pre-formatter.
+
 When using :py:func:`logging.config.dictConfig`, you can provide a subclass of
 ``Simple()`` as so:
 
 .. code-block:: python
     :caption: Pre-Formatter for log-config files
 
+    from gouge.preformatters import uvicorn_access
+
     class MyFormatter(Simple):
         def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs, pre_formatters={...})
+            super().__init__(
+                *args,
+                pre_formatters={
+                    "uvicorn.access": [uvicorn_access]
+                },
+                **kwargs,
+            )
 
 
 and then use it in the log-config as so:
 
 .. code-block:: yaml
     :caption: Example config for dictConfig
 
+    ---
     version: 1
-    handlers:
     root:
       level: DEBUG
       handlers:
         - console
-    console:
-      class : logging.StreamHandler
-      formatter: gouge
+    loggers:
+      # uvicorn loggers are pretty silent by default. We set some of them to INFO.
+      # This will make the messages (which are usfeul during development) appear in
+      # the console.
+      # uvicorn.error contains startup messages.
+      uvicorn.error:
+        level: INFO
+      # uvicorn.access contains access logs.
+      uvicorn.access:
+        level: INFO
+    handlers:
+      console:
+        class : logging.StreamHandler
+        formatter: gouge
     formatters:
       gouge:
-        class: "my.module.MyFormatter"
+        class: "powonline.logging.LogFormatter"
+
 
 
 Module Contents
 ===============
 
 .. toctree::
    :maxdepth: 4
```

### Comparing `gouge-2.2.2/fabfile.py` & `gouge-2.2.2.post1/fabfile.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/pyproject.toml` & `gouge-2.2.2.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gouge"
-version = "2.2.2"
+version = "2.2.2post1"
 authors = [
     {name = "Michel Albert", email = "michel@albert.lu"},
 ]
 description = "Collection of logging formatters."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {text = "BSD-3-Clause"}
```

### Comparing `gouge-2.2.2/src/gouge/colourcli.py` & `gouge-2.2.2.post1/src/gouge/colourcli.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/src/gouge/filters.py` & `gouge-2.2.2.post1/src/gouge/filters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/src/gouge/parseable.py` & `gouge-2.2.2.post1/src/gouge/parseable.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/src/gouge/preformatters.py` & `gouge-2.2.2.post1/src/gouge/preformatters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/src/gouge.egg-info/PKG-INFO` & `gouge-2.2.2.post1/src/gouge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.2.2
+Version: 2.2.2.post1
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.2.2/src/gouge.egg-info/SOURCES.txt` & `gouge-2.2.2.post1/src/gouge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/test/test_coloring.py` & `gouge-2.2.2.post1/test/test_coloring.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/test/test_colourcli.py` & `gouge-2.2.2.post1/test/test_colourcli.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/test/test_preformatter.py` & `gouge-2.2.2.post1/test/test_preformatter.py`

 * *Files identical despite different names*

### Comparing `gouge-2.2.2/test/test_shifting_filter.py` & `gouge-2.2.2.post1/test/test_shifting_filter.py`

 * *Files identical despite different names*

