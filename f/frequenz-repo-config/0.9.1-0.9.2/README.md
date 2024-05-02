# Comparing `tmp/frequenz-repo-config-0.9.1.tar.gz` & `tmp/frequenz-repo-config-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-repo-config-0.9.1.tar", last modified: Mon Feb 26 15:11:41 2024, max compression
+gzip compressed data, was "frequenz-repo-config-0.9.2.tar", last modified: Thu May  2 08:02:26 2024, max compression
```

## Comparing `frequenz-repo-config-0.9.1.tar` & `frequenz-repo-config-0.9.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.691597 frequenz-repo-config-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-26 15:11:41.691597 frequenz-repo-config-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.683596 frequenz-repo-config-0.9.1/github-rulesets/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/github-rulesets/Disable creation of non-release tags.json
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/github-rulesets/Disable creation of other branches.json
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/github-rulesets/Disallow removal and force-pushes of gh-pages.json
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/github-rulesets/Protect released tags.json
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/github-rulesets/Protect version branches.json
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 15:11:41.691597 frequenz-repo-config-0.9.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.683596 frequenz-repo-config-0.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.683596 frequenz-repo-config-0.9.1/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/
--rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/mike/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/mike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/mike/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/mike/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/mkdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/mkdocs/api_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/mkdocs/mike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/pytest/examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.687597 frequenz-repo-config-0.9.1/src/frequenz/repo/config/setuptools/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/setuptools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/setuptools/grpc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/config/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:26.000000 frequenz-repo-config-0.9.1/src/frequenz/repo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 15:11:41.691597 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-26 15:11:41.000000 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-02-26 15:11:41.000000 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 15:11:41.000000 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-26 15:11:41.000000 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-02-26 15:11:41.000000 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-26 15:11:41.000000 frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.759785 frequenz-repo-config-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-02 08:02:26.759785 frequenz-repo-config-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/github-rulesets/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/github-rulesets/Disable creation of non-release tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/github-rulesets/Disable creation of other branches.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/github-rulesets/Disallow removal and force-pushes of gh-pages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/github-rulesets/Protect released tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/github-rulesets/Protect version branches.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:02:26.759785 frequenz-repo-config-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.751784 frequenz-repo-config-0.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.751784 frequenz-repo-config-0.9.2/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    14547 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/mike/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/mike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/mike/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/mike/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/config/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/mkdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/mkdocs/api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/mkdocs/mike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.755784 frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.759785 frequenz-repo-config-0.9.2/src/frequenz/repo/config/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/pytest/examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.759785 frequenz-repo-config-0.9.2/src/frequenz/repo/config/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/setuptools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/setuptools/grpc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18007 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/config/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:19.000000 frequenz-repo-config-0.9.2/src/frequenz/repo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:02:26.759785 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-02 08:02:26.000000 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-02 08:02:26.000000 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:02:26.000000 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 08:02:26.000000 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-02 08:02:26.000000 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 08:02:26.000000 frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/top_level.txt
```

### Comparing `frequenz-repo-config-0.9.1/LICENSE` & `frequenz-repo-config-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/PKG-INFO` & `frequenz-repo-config-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-repo-config
-Version: 0.9.1
+Version: 0.9.2
 Summary: Frequenz repository setup tools and common configuration
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-repo-config-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-repo-config-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-repo-config-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-repo-config-python
```

### Comparing `frequenz-repo-config-0.9.1/README.md` & `frequenz-repo-config-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/github-rulesets/Disable creation of other branches.json` & `frequenz-repo-config-0.9.2/github-rulesets/Disable creation of other branches.json`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/github-rulesets/Protect released tags.json` & `frequenz-repo-config-0.9.2/github-rulesets/Protect released tags.json`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/github-rulesets/Protect version branches.json` & `frequenz-repo-config-0.9.2/github-rulesets/Protect version branches.json`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/pyproject.toml` & `frequenz-repo-config-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ]
 app = []
 lib = []
 model = []
 extra-lint-examples = [
   "pylint >= 2.17.3, < 4",
   "pytest >= 7.3.0, < 9",
-  "sybil >= 5.0.3, < 7",
+  "sybil >= 5.0.3, < 6.1",
 ]
 dev-flake8 = [
   "flake8 == 6.1.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.3.2",
   "pydocstyle == 6.3.0",
```

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/__init__.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/mike/info.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/mike/info.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/cli/version/mike/sort.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/cli/version/mike/sort.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/github.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/github.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/mkdocs/api_pages.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/mkdocs/api_pages.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/mkdocs/mike.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/mkdocs/mike.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/__init__.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/config.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/config.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/default.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/default.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/session.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/session.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/nox/util.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/nox/util.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/protobuf.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/protobuf.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/pytest/examples.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/pytest/examples.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/setuptools/grpc_tools.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/setuptools/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz/repo/config/version.py` & `frequenz-repo-config-0.9.2/src/frequenz/repo/config/version.py`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/PKG-INFO` & `frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-repo-config
-Version: 0.9.1
+Version: 0.9.2
 Summary: Frequenz repository setup tools and common configuration
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-repo-config-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-repo-config-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-repo-config-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-repo-config-python
```

### Comparing `frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/SOURCES.txt` & `frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-repo-config-0.9.1/src/frequenz_repo_config.egg-info/requires.txt` & `frequenz-repo-config-0.9.2/src/frequenz_repo_config.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 cookiecutter==2.1.1
 jinja2==3.1.2
 sybil==6.0.3
 
 [extra-lint-examples]
 pylint<4,>=2.17.3
 pytest<9,>=7.3.0
-sybil<7,>=5.0.3
+sybil<6.1,>=5.0.3
 
 [lib]
 
 [model]
```

