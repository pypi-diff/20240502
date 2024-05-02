# Comparing `tmp/mike-2.0.0.tar.gz` & `tmp/mike-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mike-2.0.0.tar", last modified: Thu Nov  2 21:34:01 2023, max compression
+gzip compressed data, was "mike-2.1.0.tar", last modified: Thu May  2 00:49:36 2024, max compression
```

## Comparing `mike-2.0.0.tar` & `mike-2.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.298873 mike-2.0.0/
--rw-rw-r--   0 jim       (1000) jim       (1000)     6596 2023-11-02 21:31:50.000000 mike-2.0.0/CHANGES.md
--rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-03-02 23:32:07.000000 mike-2.0.0/LICENSE
--rw-rw-r--   0 jim       (1000) jim       (1000)       97 2021-03-01 03:43:15.000000 mike-2.0.0/MANIFEST.in
--rw-rw-r--   0 jim       (1000) jim       (1000)    19650 2023-11-02 21:34:01.298873 mike-2.0.0/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)    15710 2023-11-02 04:50:21.000000 mike-2.0.0/README.md
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.290873 mike-2.0.0/mike/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.0.0/mike/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)       18 2023-11-02 21:31:41.000000 mike-2.0.0/mike/app_version.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1239 2023-11-02 00:12:32.000000 mike-2.0.0/mike/arguments.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    11861 2023-11-02 00:12:32.000000 mike-2.0.0/mike/commands.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    18593 2023-11-02 04:42:06.000000 mike-2.0.0/mike/driver.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    13389 2023-03-13 21:45:58.000000 mike-2.0.0/mike/git_utils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4278 2023-11-02 04:41:55.000000 mike-2.0.0/mike/jsonpath.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2716 2023-07-05 17:42:05.000000 mike-2.0.0/mike/mkdocs_plugin.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2356 2023-05-11 19:44:14.000000 mike-2.0.0/mike/mkdocs_utils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2367 2023-03-02 23:32:07.000000 mike-2.0.0/mike/server.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.294873 mike-2.0.0/mike/templates/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.0.0/mike/templates/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      378 2023-03-02 23:32:07.000000 mike-2.0.0/mike/templates/redirect.html
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.294873 mike-2.0.0/mike/themes/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.0.0/mike/themes/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.294873 mike-2.0.0/mike/themes/mkdocs/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.0.0/mike/themes/mkdocs/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.294873 mike-2.0.0/mike/themes/mkdocs/css/
--rw-rw-r--   0 jim       (1000) jim       (1000)      376 2020-02-24 00:26:03.000000 mike-2.0.0/mike/themes/mkdocs/css/version-select.css
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.294873 mike-2.0.0/mike/themes/mkdocs/js/
--rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2023-11-02 00:12:32.000000 mike-2.0.0/mike/themes/mkdocs/js/version-select.js
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.298873 mike-2.0.0/mike/themes/readthedocs/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.0.0/mike/themes/readthedocs/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.298873 mike-2.0.0/mike/themes/readthedocs/css/
--rw-rw-r--   0 jim       (1000) jim       (1000)       86 2017-12-04 03:10:10.000000 mike-2.0.0/mike/themes/readthedocs/css/version-select.css
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.298873 mike-2.0.0/mike/themes/readthedocs/js/
--rw-rw-r--   0 jim       (1000) jim       (1000)     2178 2023-11-02 00:12:32.000000 mike-2.0.0/mike/themes/readthedocs/js/version-select.js
--rw-rw-r--   0 jim       (1000) jim       (1000)     6729 2023-11-02 04:35:40.000000 mike-2.0.0/mike/versions.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-11-02 21:34:01.294873 mike-2.0.0/mike.egg-info/
--rw-rw-r--   0 jim       (1000) jim       (1000)    19650 2023-11-02 21:34:00.000000 mike-2.0.0/mike.egg-info/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)      774 2023-11-02 21:34:00.000000 mike-2.0.0/mike.egg-info/SOURCES.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2023-11-02 21:34:00.000000 mike-2.0.0/mike.egg-info/dependency_links.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)     1341 2023-11-02 21:34:00.000000 mike-2.0.0/mike.egg-info/entry_points.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2017-12-04 03:12:13.000000 mike-2.0.0/mike.egg-info/not-zip-safe
--rw-rw-r--   0 jim       (1000) jim       (1000)      195 2023-11-02 21:34:00.000000 mike-2.0.0/mike.egg-info/requires.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        5 2023-11-02 21:34:00.000000 mike-2.0.0/mike.egg-info/top_level.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      423 2023-11-02 21:34:01.298873 mike-2.0.0/setup.cfg
--rw-rw-r--   0 jim       (1000) jim       (1000)     5159 2023-11-02 00:12:32.000000 mike-2.0.0/setup.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6994 2024-05-02 00:47:02.000000 mike-2.1.0/CHANGES.md
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-03-02 23:32:07.000000 mike-2.1.0/LICENSE
+-rw-rw-r--   0 jim       (1000) jim       (1000)       97 2021-03-01 03:43:15.000000 mike-2.1.0/MANIFEST.in
+-rw-rw-r--   0 jim       (1000) jim       (1000)    20375 2024-05-02 00:49:36.269359 mike-2.1.0/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)    16331 2024-02-29 18:47:52.000000 mike-2.1.0/README.md
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.249349 mike-2.1.0/mike/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)       18 2024-05-02 00:49:26.000000 mike-2.1.0/mike/app_version.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1239 2023-11-02 00:12:32.000000 mike-2.1.0/mike/arguments.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    11924 2024-02-29 18:47:52.000000 mike-2.1.0/mike/commands.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    19178 2024-03-01 00:08:45.000000 mike-2.1.0/mike/driver.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    13389 2023-03-13 21:45:58.000000 mike-2.1.0/mike/git_utils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4278 2023-11-02 04:41:55.000000 mike-2.1.0/mike/jsonpath.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2716 2023-07-05 17:42:05.000000 mike-2.1.0/mike/mkdocs_plugin.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3199 2024-04-05 00:45:27.000000 mike-2.1.0/mike/mkdocs_utils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2367 2023-03-02 23:32:07.000000 mike-2.1.0/mike/server.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/templates/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/templates/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      378 2023-03-02 23:32:07.000000 mike-2.1.0/mike/templates/redirect.html
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/mkdocs/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/mkdocs/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/mkdocs/css/
+-rw-rw-r--   0 jim       (1000) jim       (1000)      376 2020-02-24 00:26:03.000000 mike-2.1.0/mike/themes/mkdocs/css/version-select.css
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike/themes/mkdocs/js/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2023-11-02 00:12:32.000000 mike-2.1.0/mike/themes/mkdocs/js/version-select.js
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/mike/themes/readthedocs/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/readthedocs/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/mike/themes/readthedocs/css/
+-rw-rw-r--   0 jim       (1000) jim       (1000)       86 2017-12-04 03:10:10.000000 mike-2.1.0/mike/themes/readthedocs/css/version-select.css
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.269359 mike-2.1.0/mike/themes/readthedocs/js/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2178 2023-11-02 00:12:32.000000 mike-2.1.0/mike/themes/readthedocs/js/version-select.js
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6729 2023-11-02 04:35:40.000000 mike-2.1.0/mike/versions.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2024-05-02 00:49:36.265357 mike-2.1.0/mike.egg-info/
+-rw-rw-r--   0 jim       (1000) jim       (1000)    20375 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)      774 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/SOURCES.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        1 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/dependency_links.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1341 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/entry_points.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        1 2017-12-04 03:12:13.000000 mike-2.1.0/mike.egg-info/not-zip-safe
+-rw-rw-r--   0 jim       (1000) jim       (1000)      195 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/requires.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        5 2024-05-02 00:49:35.000000 mike-2.1.0/mike.egg-info/top_level.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)      423 2024-05-02 00:49:36.269359 mike-2.1.0/setup.cfg
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5159 2023-11-02 00:12:32.000000 mike-2.1.0/setup.py
```

### Comparing `mike-2.0.0/CHANGES.md` & `mike-2.1.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 # Changes
 
+## v2.1.0 (2024-05-01)
+
+### New features
+- When calling `set-default`, you can now pass `--allow-undefined` to set the
+  default to a version that doesn't exist yet
+- Add global-level `-q` / `--quiet` option to suppress warning messages
+- Add support for handling `!relative` in `mkdocs.yml`
+
+### Bug fixes
+- When loading an MkDocs config, mike now runs the `startup` and `shutdown`
+  events
+
+---
+
 ## v2.0.0 (2023-11-02)
 
 ### New features
 
 - Add support for applying arbitrary properties to documentation versions
 - Add support for hiding specific versions from the selector when using the
   default themes
```

### Comparing `mike-2.0.0/LICENSE` & `mike-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/PKG-INFO` & `mike-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mike
-Version: 2.0.0
+Version: 2.1.0
 Summary: Manage multiple versions of your MkDocs-powered documentation
 Home-page: https://github.com/jimporter/mike
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
 License: BSD-3-Clause
 Description: # mike
         **mike** is a Python utility that makes it easy to deploy multiple versions of
@@ -150,24 +150,33 @@
         You can also specify many of these options via your `mkdocs.yml` configuration
         as shown above. For example, `--alias-type` can also be specified via
         `plugins.mike.alias_type`. (For `--branch` and `--remote`, you can use the
         built-in MkDocs fields `remote_branch` and `remote_name`.)
         
         ### Viewing Your Docs
         
-        To test that your docs have been built as expected, you can serve them locally
-        from a dev server:
+        When editing your documentation, you can usually just use the ordinary [`mkdocs
+        serve`][mkdocs-serve] to show the genereated results. This serves the current
+        version of your documentation without forcing you to create a Git commit first
+        via `mike deploy`.
+        
+        If you want to test all the versions of your documentation as you'd see on your
+        production server, you can serve them locally via:
         
         ```sh
         mike serve
         ```
         
-        By default, this serves the docs on `http://localhost:8000`, but you can
-        change this with `-a`/`--dev-addr`. Remember though, *this is for testing only*.
-        To host your docs for real, you should use a real web server.
+        This serves your current documentation as committed to your `gh-pages` branch.
+        By default, it serves the docs at `http://localhost:8000`, but you can change
+        this with `-a`/`--dev-addr`.
+        
+        > [!CAUTION]
+        > `mike serve` and `mkdocs serve` should be used *for testing only*. To host
+        > your docs for real, use a real web server.
         
         ### Deleting Docs
         
         Sometimes you need to delete an old version of your docs, either because you
         made a mistake or you're pruning unsupported versions. You can do this via the
         `delete` subcommand:
         
@@ -207,14 +216,18 @@
         so that people going to the root of your site are redirected to the latest
         version of the docs:
         
         ```sh
         mike set-default [identifier]
         ```
         
+        Normally, this command will return an error if `identifier` doesn't exist. If
+        you want to set the default to a version that doesn't exist yet, you can pass
+        `--allow-undefined`.
+        
         If you want to use a different template from the default, you can pass
         `-T`/`--template`; this takes a path to a [Jinja][jinja] template that accepts
         an `{{href}}` variable. (Note that this page *always* uses a redirect, no matter
         the setting of `alias_type`/`--alias-type`.)
         
         Like `deploy` and `delete` above, you can specify `--branch`, `--push`,
         etc to control how the commit is handled.
@@ -309,16 +322,15 @@
         
         ## Staying in Sync
         
         mike will do its best to stay in-sync with your remote repository and will
         automatically update your local branch to match the remote's if possible (note
         that mike *won't* automatically `git fetch` anything). If your local branch has
         diverged from your remote, mike will leave it as-is and ask you what to do. To
-        ignore the remote's state, just pass `--ignore`; to update to the remote's
-        state, pass `--rebase`.
+        ignore the remote's state, just pass `--ignore-remote-status`.
         
         ## `CNAME` (and Other Special Files)
         
         Some special files that you'd like to deploy along with your documentation (such
         as `CNAME`) aren't related to a particular version of the docs, and instead need
         to go in the root directory of your site. There's no special handling for this
         in mike, but since your built docs live on a Git branch, it's still easy to
@@ -384,24 +396,25 @@
         
         ## License
         
         This project is licensed under the [BSD 3-clause license](LICENSE).
         
         [pypi-image]: https://img.shields.io/pypi/v/mike.svg
         [pypi-link]: https://pypi.python.org/pypi/mike
-        [ci-image]: https://github.com/jimporter/mike/workflows/build/badge.svg
-        [ci-link]: https://github.com/jimporter/mike/actions?query=branch%3Amaster+workflow%3Abuild
+        [ci-image]: https://github.com/jimporter/mike/actions/workflows/build.yml/badge.svg
+        [ci-link]: https://github.com/jimporter/mike/actions/workflows/build.yml?query=branch%3Amaster
         [codecov-image]: https://codecov.io/gh/jimporter/mike/branch/master/graph/badge.svg
         [codecov-link]: https://codecov.io/gh/jimporter/mike
         
         [bfg9000]: https://jimporter.github.io/bfg9000
         [setuptools]: https://pythonhosted.org/setuptools/
         [shtab]: https://github.com/iterative/shtab
         [shtab-setup]: https://github.com/iterative/shtab#cli-usage
         [jinja]: https://jinja.palletsprojects.com/
+        [mkdocs-serve]: https://www.mkdocs.org/user-guide/cli/#mkdocs-serve
         [gh-action-commit]: https://github.com/actions/checkout#push-a-commit-using-the-built-in-token
         
 Keywords: mkdocs multiple versions
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
```

### Comparing `mike-2.0.0/README.md` & `mike-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -147,24 +147,33 @@
 You can also specify many of these options via your `mkdocs.yml` configuration
 as shown above. For example, `--alias-type` can also be specified via
 `plugins.mike.alias_type`. (For `--branch` and `--remote`, you can use the
 built-in MkDocs fields `remote_branch` and `remote_name`.)
 
 ### Viewing Your Docs
 
-To test that your docs have been built as expected, you can serve them locally
-from a dev server:
+When editing your documentation, you can usually just use the ordinary [`mkdocs
+serve`][mkdocs-serve] to show the genereated results. This serves the current
+version of your documentation without forcing you to create a Git commit first
+via `mike deploy`.
+
+If you want to test all the versions of your documentation as you'd see on your
+production server, you can serve them locally via:
 
 ```sh
 mike serve
 ```
 
-By default, this serves the docs on `http://localhost:8000`, but you can
-change this with `-a`/`--dev-addr`. Remember though, *this is for testing only*.
-To host your docs for real, you should use a real web server.
+This serves your current documentation as committed to your `gh-pages` branch.
+By default, it serves the docs at `http://localhost:8000`, but you can change
+this with `-a`/`--dev-addr`.
+
+> [!CAUTION]
+> `mike serve` and `mkdocs serve` should be used *for testing only*. To host
+> your docs for real, use a real web server.
 
 ### Deleting Docs
 
 Sometimes you need to delete an old version of your docs, either because you
 made a mistake or you're pruning unsupported versions. You can do this via the
 `delete` subcommand:
 
@@ -204,14 +213,18 @@
 so that people going to the root of your site are redirected to the latest
 version of the docs:
 
 ```sh
 mike set-default [identifier]
 ```
 
+Normally, this command will return an error if `identifier` doesn't exist. If
+you want to set the default to a version that doesn't exist yet, you can pass
+`--allow-undefined`.
+
 If you want to use a different template from the default, you can pass
 `-T`/`--template`; this takes a path to a [Jinja][jinja] template that accepts
 an `{{href}}` variable. (Note that this page *always* uses a redirect, no matter
 the setting of `alias_type`/`--alias-type`.)
 
 Like `deploy` and `delete` above, you can specify `--branch`, `--push`,
 etc to control how the commit is handled.
@@ -306,16 +319,15 @@
 
 ## Staying in Sync
 
 mike will do its best to stay in-sync with your remote repository and will
 automatically update your local branch to match the remote's if possible (note
 that mike *won't* automatically `git fetch` anything). If your local branch has
 diverged from your remote, mike will leave it as-is and ask you what to do. To
-ignore the remote's state, just pass `--ignore`; to update to the remote's
-state, pass `--rebase`.
+ignore the remote's state, just pass `--ignore-remote-status`.
 
 ## `CNAME` (and Other Special Files)
 
 Some special files that you'd like to deploy along with your documentation (such
 as `CNAME`) aren't related to a particular version of the docs, and instead need
 to go in the root directory of your site. There's no special handling for this
 in mike, but since your built docs live on a Git branch, it's still easy to
@@ -381,18 +393,19 @@
 
 ## License
 
 This project is licensed under the [BSD 3-clause license](LICENSE).
 
 [pypi-image]: https://img.shields.io/pypi/v/mike.svg
 [pypi-link]: https://pypi.python.org/pypi/mike
-[ci-image]: https://github.com/jimporter/mike/workflows/build/badge.svg
-[ci-link]: https://github.com/jimporter/mike/actions?query=branch%3Amaster+workflow%3Abuild
+[ci-image]: https://github.com/jimporter/mike/actions/workflows/build.yml/badge.svg
+[ci-link]: https://github.com/jimporter/mike/actions/workflows/build.yml?query=branch%3Amaster
 [codecov-image]: https://codecov.io/gh/jimporter/mike/branch/master/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/jimporter/mike
 
 [bfg9000]: https://jimporter.github.io/bfg9000
 [setuptools]: https://pythonhosted.org/setuptools/
 [shtab]: https://github.com/iterative/shtab
 [shtab-setup]: https://github.com/iterative/shtab#cli-usage
 [jinja]: https://jinja.palletsprojects.com/
+[mkdocs-serve]: https://www.mkdocs.org/user-guide/cli/#mkdocs-serve
 [gh-action-commit]: https://github.com/actions/checkout#push-a-commit-using-the-built-in-token
```

### Comparing `mike-2.0.0/mike/arguments.py` & `mike-2.1.0/mike/arguments.py`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/commands.py` & `mike-2.1.0/mike/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,28 +268,29 @@
     except KeyError:
         raise ValueError('identifier {!r} does not exist'.format(identifier))
 
     with git_utils.Commit(branch, message, allow_empty=allow_empty) as commit:
         commit.add_file(versions_to_file_info(all_versions, deploy_prefix))
 
 
-def set_default(identifier, template=None, *, branch='gh-pages', message=None,
-                allow_empty=False, deploy_prefix=''):
+def set_default(identifier, template=None, allow_undefined=False, *,
+                branch='gh-pages', message=None, allow_empty=False,
+                deploy_prefix=''):
     if message is None:
         message = (
             'Set default version to {doc_identifier}{deploy_prefix} with ' +
             'mike {mike_version}'
         ).format(
             doc_identifier=identifier,
             deploy_prefix=_format_deploy_prefix(deploy_prefix),
             mike_version=app_version
         )
 
     all_versions = list_versions(branch, deploy_prefix)
-    if not all_versions.find(identifier):
+    if not allow_undefined and not all_versions.find(identifier):
         raise ValueError('identifier {!r} does not exist'.format(identifier))
 
     t = _redirect_template(template)
     with git_utils.Commit(branch, message, allow_empty=allow_empty) as commit:
         commit.add_file(git_utils.FileInfo(
             os.path.join(deploy_prefix, 'index.html'),
             t.render(href=identifier + '/')
```

### Comparing `mike-2.0.0/mike/driver.py` & `mike-2.1.0/mike/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 import sys
+import warnings
 from contextlib import contextmanager
 
 from . import arguments
 from . import commands
 from . import git_utils
 from . import jsonpath
 from . import mkdocs_utils
@@ -73,14 +74,18 @@
 
 generate_completion_desc = """
 Generate shell-completion functions for bfg9000 and write them to standard
 output. This requires the Python package `shtab`.
 """
 
 
+def showwarning(message, category, filename, lineno, file=None, line=None):
+    sys.stderr.write('warning: {}\n'.format(message))
+
+
 def add_git_arguments(parser, *, commit=True, deploy_prefix=True):
     # Add this whenever we add git arguments since we pull the remote and
     # branch from mkdocs.yml.
     parser.add_argument('-F', '--config-file', metavar='FILE', complete='file',
                         help='the MkDocs configuration file to use')
 
     git = parser.add_argument_group('git arguments')
@@ -170,39 +175,39 @@
     try:
         git_utils.update_from_upstream(args.remote, args.branch)
     except (git_utils.GitBranchDiverged, git_utils.GitRevUnrelated) as e:
         if strict:
             raise ValueError(str(e) + "\n  If you're sure this is intended, " +
                              'retry with --ignore-remote-status')
         else:
-            sys.stderr.write('warning: {}\n'.format(e))
+            warnings.warn(str(e))
 
 
 @contextmanager
 def handle_empty_commit():
     try:
         yield
     except git_utils.GitEmptyCommit as e:
-        sys.stderr.write(('warning: {}\n  To create a commit anyway, retry ' +
-                          'with --allow-empty\n').format(e))
+        warnings.warn(str(e) + '\n  To create a commit anyway, retry with ' +
+                      '--allow-empty')
 
 
 def deploy(parser, args):
     cfg = load_mkdocs_config(args, strict=True)
     check_remote_status(args, strict=True)
     with handle_empty_commit():
         alias_type = commands.AliasType[args.alias_type]
         with commands.deploy(cfg, args.version, args.title, args.aliases,
                              args.update_aliases, alias_type, args.template,
                              branch=args.branch, message=args.message,
                              allow_empty=args.allow_empty,
                              deploy_prefix=args.deploy_prefix,
                              set_props=args.set_props or []), \
              mkdocs_utils.inject_plugin(args.config_file) as config_file:
-            mkdocs_utils.build(config_file, args.version)
+            mkdocs_utils.build(config_file, args.version, quiet=args.quiet)
         if args.push:
             git_utils.push_branch(args.remote, args.branch)
 
 
 def delete(parser, args):
     load_mkdocs_config(args)
     check_remote_status(args, strict=True)
@@ -295,15 +300,16 @@
 
 
 def set_default(parser, args):
     load_mkdocs_config(args)
     check_remote_status(args, strict=True)
     with handle_empty_commit():
         commands.set_default(args.identifier, args.template,
-                             branch=args.branch, message=args.message,
+                             args.allow_undefined, branch=args.branch,
+                             message=args.message,
                              allow_empty=args.allow_empty,
                              deploy_prefix=args.deploy_prefix)
         if args.push:
             git_utils.push_branch(args.remote, args.branch)
 
 
 def serve(parser, args):
@@ -322,20 +328,24 @@
         print(shtab.complete(parser, shell=args.shell))
     except ImportError:  # pragma: no cover
         print('shtab not found; install via `pip install shtab`')
         return 1
 
 
 def main():
+    warnings.showwarning = showwarning
+
     parser = arguments.ArgumentParser(prog='mike', description=description)
     subparsers = parser.add_subparsers(metavar='COMMAND')
     subparsers.required = True
 
     parser.add_argument('--version', action='version',
                         version='%(prog)s ' + app_version)
+    parser.add_argument('-q', '--quiet', action='store_true',
+                        help='silence warnings')
     parser.add_argument('--debug', action='store_true',
                         help='report extra information for debugging mike')
 
     deploy_p = subparsers.add_parser(
         'deploy', description=deploy_desc,
         help='build docs and deploy them to a branch'
     )
@@ -420,14 +430,17 @@
     set_default_p = subparsers.add_parser(
         'set-default', description=set_default_desc,
         help='set the default version for your docs'
     )
     set_default_p.set_defaults(func=set_default)
     set_default_p.add_argument('-T', '--template', complete='file',
                                help='template file to use')
+    set_default_p.add_argument('--allow-undefined', action='store_true',
+                               help=('allow setting undefined versions as ' +
+                                     'default'))
     add_git_arguments(set_default_p)
     set_default_p.add_argument('identifier', metavar='IDENTIFIER',
                                help='version or alias to set as default')
 
     serve_p = subparsers.add_parser(
         'serve', description=serve_desc, help='serve docs locally for testing'
     )
@@ -452,13 +465,16 @@
     completion_p.set_defaults(func=generate_completion)
     shell = (os.path.basename(os.environ['SHELL'])
              if 'SHELL' in os.environ else None)
     completion_p.add_argument('-s', '--shell', metavar='SHELL', default=shell,
                               help='shell type (default: %(default)s)')
 
     args = parser.parse_args()
+    if args.quiet:
+        warnings.filterwarnings('ignore')
+
     try:
         return args.func(parser, args)
     except Exception as e:
         if args.debug:  # pragma: no cover
             raise
         parser.exit(1, 'error: {}\n'.format(e))
```

### Comparing `mike-2.0.0/mike/git_utils.py` & `mike-2.1.0/mike/git_utils.py`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/jsonpath.py` & `mike-2.1.0/mike/jsonpath.py`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/mkdocs_plugin.py` & `mike-2.1.0/mike/mkdocs_plugin.py`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/mkdocs_utils.py` & `mike-2.1.0/mike/mkdocs_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,46 @@
 import mkdocs.config
+import mkdocs.plugins
 import mkdocs.utils
 import os
 import re
 import subprocess
 import yaml
 from collections.abc import Iterable, Mapping
 from contextlib import contextmanager
 from tempfile import NamedTemporaryFile
 
 docs_version_var = 'MIKE_DOCS_VERSION'
 
 
+class RoundTrippableTag:
+    def __init__(self, node):
+        self.node = node
+
+    def __repr__(self):
+        return repr(self.node)
+
+    @staticmethod
+    def constructor(loader, suffix, node):
+        return RoundTrippableTag(node)
+
+    @staticmethod
+    def representer(dumper, data):
+        return data.node
+
+
+class RoundTripLoader(yaml.Loader):
+    pass
+
+
+yaml.add_multi_constructor('!', RoundTrippableTag.constructor,
+                           Loader=RoundTripLoader)
+yaml.add_multi_representer(RoundTrippableTag, RoundTrippableTag.representer)
+
+
 def _open_config(config_file=None):
     if config_file is None:
         config_file = ['mkdocs.yml', 'mkdocs.yaml']
     elif not isinstance(config_file, Iterable) or isinstance(config_file, str):
         config_file = [config_file]
 
     exc = None
@@ -26,22 +52,29 @@
                 exc = e
     raise exc
 
 
 def load_config(config_file=None, **kwargs):
     with _open_config(config_file) as f:
         cfg = mkdocs.config.load_config(f, **kwargs)
-        return cfg['plugins'].run_event('config', cfg)
+
+        if 'startup' in mkdocs.plugins.EVENTS:
+            cfg['plugins'].run_event('startup', command='mike', dirty=False)
+        cfg = cfg['plugins'].run_event('config', cfg)
+        if 'shutdown' in mkdocs.plugins.EVENTS:
+            cfg['plugins'].run_event('shutdown')
+
+        return cfg
 
 
 @contextmanager
 def inject_plugin(config_file):
     with _open_config(config_file) as f:
         config_file = f.name
-        config = mkdocs.utils.yaml_load(f)
+        config = mkdocs.utils.yaml_load(f, loader=RoundTripLoader)
 
     plugins = config.setdefault('plugins', ['search'])
     for i in plugins:
         if ( (isinstance(i, str) and i == 'mike') or
              (isinstance(i, dict) and 'mike' in i) ):
             yield config_file
             return
@@ -59,24 +92,23 @@
 
     try:
         yield f.name
     finally:
         os.remove(f.name)
 
 
-def build(config_file, version, verbose=True):
+def build(config_file, version, *, quiet=False, output=None):
     command = (
-        ['mkdocs', 'build', '--clean'] +
+        ['mkdocs'] + (['--quiet'] if quiet else []) + ['build', '--clean'] +
         (['--config-file', config_file] if config_file else [])
     )
 
     env = os.environ.copy()
     env[docs_version_var] = version
 
-    output = None if verbose else subprocess.DEVNULL
     subprocess.run(command, check=True, env=env, stdout=output, stderr=output)
 
 
 def version():
     output = subprocess.run(
         ['mkdocs', '--version'],
         check=True, stdout=subprocess.PIPE, universal_newlines=True
```

### Comparing `mike-2.0.0/mike/server.py` & `mike-2.1.0/mike/server.py`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/themes/mkdocs/js/version-select.js` & `mike-2.1.0/mike/themes/mkdocs/js/version-select.js`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/themes/readthedocs/js/version-select.js` & `mike-2.1.0/mike/themes/readthedocs/js/version-select.js`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike/versions.py` & `mike-2.1.0/mike/versions.py`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike.egg-info/PKG-INFO` & `mike-2.1.0/mike.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mike
-Version: 2.0.0
+Version: 2.1.0
 Summary: Manage multiple versions of your MkDocs-powered documentation
 Home-page: https://github.com/jimporter/mike
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
 License: BSD-3-Clause
 Description: # mike
         **mike** is a Python utility that makes it easy to deploy multiple versions of
@@ -150,24 +150,33 @@
         You can also specify many of these options via your `mkdocs.yml` configuration
         as shown above. For example, `--alias-type` can also be specified via
         `plugins.mike.alias_type`. (For `--branch` and `--remote`, you can use the
         built-in MkDocs fields `remote_branch` and `remote_name`.)
         
         ### Viewing Your Docs
         
-        To test that your docs have been built as expected, you can serve them locally
-        from a dev server:
+        When editing your documentation, you can usually just use the ordinary [`mkdocs
+        serve`][mkdocs-serve] to show the genereated results. This serves the current
+        version of your documentation without forcing you to create a Git commit first
+        via `mike deploy`.
+        
+        If you want to test all the versions of your documentation as you'd see on your
+        production server, you can serve them locally via:
         
         ```sh
         mike serve
         ```
         
-        By default, this serves the docs on `http://localhost:8000`, but you can
-        change this with `-a`/`--dev-addr`. Remember though, *this is for testing only*.
-        To host your docs for real, you should use a real web server.
+        This serves your current documentation as committed to your `gh-pages` branch.
+        By default, it serves the docs at `http://localhost:8000`, but you can change
+        this with `-a`/`--dev-addr`.
+        
+        > [!CAUTION]
+        > `mike serve` and `mkdocs serve` should be used *for testing only*. To host
+        > your docs for real, use a real web server.
         
         ### Deleting Docs
         
         Sometimes you need to delete an old version of your docs, either because you
         made a mistake or you're pruning unsupported versions. You can do this via the
         `delete` subcommand:
         
@@ -207,14 +216,18 @@
         so that people going to the root of your site are redirected to the latest
         version of the docs:
         
         ```sh
         mike set-default [identifier]
         ```
         
+        Normally, this command will return an error if `identifier` doesn't exist. If
+        you want to set the default to a version that doesn't exist yet, you can pass
+        `--allow-undefined`.
+        
         If you want to use a different template from the default, you can pass
         `-T`/`--template`; this takes a path to a [Jinja][jinja] template that accepts
         an `{{href}}` variable. (Note that this page *always* uses a redirect, no matter
         the setting of `alias_type`/`--alias-type`.)
         
         Like `deploy` and `delete` above, you can specify `--branch`, `--push`,
         etc to control how the commit is handled.
@@ -309,16 +322,15 @@
         
         ## Staying in Sync
         
         mike will do its best to stay in-sync with your remote repository and will
         automatically update your local branch to match the remote's if possible (note
         that mike *won't* automatically `git fetch` anything). If your local branch has
         diverged from your remote, mike will leave it as-is and ask you what to do. To
-        ignore the remote's state, just pass `--ignore`; to update to the remote's
-        state, pass `--rebase`.
+        ignore the remote's state, just pass `--ignore-remote-status`.
         
         ## `CNAME` (and Other Special Files)
         
         Some special files that you'd like to deploy along with your documentation (such
         as `CNAME`) aren't related to a particular version of the docs, and instead need
         to go in the root directory of your site. There's no special handling for this
         in mike, but since your built docs live on a Git branch, it's still easy to
@@ -384,24 +396,25 @@
         
         ## License
         
         This project is licensed under the [BSD 3-clause license](LICENSE).
         
         [pypi-image]: https://img.shields.io/pypi/v/mike.svg
         [pypi-link]: https://pypi.python.org/pypi/mike
-        [ci-image]: https://github.com/jimporter/mike/workflows/build/badge.svg
-        [ci-link]: https://github.com/jimporter/mike/actions?query=branch%3Amaster+workflow%3Abuild
+        [ci-image]: https://github.com/jimporter/mike/actions/workflows/build.yml/badge.svg
+        [ci-link]: https://github.com/jimporter/mike/actions/workflows/build.yml?query=branch%3Amaster
         [codecov-image]: https://codecov.io/gh/jimporter/mike/branch/master/graph/badge.svg
         [codecov-link]: https://codecov.io/gh/jimporter/mike
         
         [bfg9000]: https://jimporter.github.io/bfg9000
         [setuptools]: https://pythonhosted.org/setuptools/
         [shtab]: https://github.com/iterative/shtab
         [shtab-setup]: https://github.com/iterative/shtab#cli-usage
         [jinja]: https://jinja.palletsprojects.com/
+        [mkdocs-serve]: https://www.mkdocs.org/user-guide/cli/#mkdocs-serve
         [gh-action-commit]: https://github.com/actions/checkout#push-a-commit-using-the-built-in-token
         
 Keywords: mkdocs multiple versions
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Documentation
```

### Comparing `mike-2.0.0/mike.egg-info/SOURCES.txt` & `mike-2.1.0/mike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/mike.egg-info/entry_points.txt` & `mike-2.1.0/mike.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mike-2.0.0/setup.py` & `mike-2.1.0/setup.py`

 * *Files identical despite different names*

