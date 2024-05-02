# Comparing `tmp/dsi_cocoa-0.1.2.tar.gz` & `tmp/dsi_cocoa-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.1.2.tar", last modified: Wed May  1 18:02:13 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.1.3.tar", last modified: Thu May  2 21:32:15 2024, max compression
```

## Comparing `dsi_cocoa-0.1.2.tar` & `dsi_cocoa-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.037971 dsi_cocoa-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.037971 dsi_cocoa-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-01 18:02:08.000000 dsi_cocoa-0.1.2/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:02:13.041971 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 18:02:13.000000 dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:15.124621 dsi_cocoa-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:15.116621 dsi_cocoa-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:15.120621 dsi_cocoa-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-02 21:32:15.124621 dsi_cocoa-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 21:32:15.124621 dsi_cocoa-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:15.116621 dsi_cocoa-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:15.120621 dsi_cocoa-0.1.3/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 21:32:11.000000 dsi_cocoa-0.1.3/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 21:32:15.124621 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-02 21:32:15.000000 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-02 21:32:15.000000 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 21:32:15.000000 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-02 21:32:15.000000 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 21:32:15.000000 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 21:32:15.000000 dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.1.2/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.1.3/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.1.3/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/.gitignore` & `dsi_cocoa-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/.pre-commit-config.yaml` & `dsi_cocoa-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/PKG-INFO` & `dsi_cocoa-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.2
+Version: 0.1.3
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.2/README.md` & `dsi_cocoa-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/pyproject.toml` & `dsi_cocoa-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.1.3/src/cocoa/evaluate_repo.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,17 +20,19 @@
     is_code_in_functions_or_main,
     pyflakes_notebook,
     pyflakes_python_file,
 )
 from cocoa.notebooks import process_notebook
 from cocoa.repo import (
     check_branch_names,
+    clone_repo,
     files_after_date,
     get_current_branch,
     get_remote_branches_info,
+    is_git_remote_repo,
     is_git_repo,
 )
 
 
 def walk_and_process(
     dir_path, no_filter_flag, lint_flag, start_date=None, verbose=False
 ):
@@ -120,37 +122,44 @@
             print(f"{tool_name} found {len(results)} issues:")
             for result in results[:5]:
                 print(f"  {result}")
             if len(results) > 5:
                 print(f"  ...and {len(results) - 5} more issues.")
 
 
-def evaluate_repo(dir_path, lint_flag, start_date=None, verbose=False):
+def evaluate_repo(path_or_url, lint_flag, start_date=None, verbose=False):
     """
-    This is the entry point to running the automated code review
-    It should be called from inside the docker container.
+    This is the entry point to running the automated code review.
     """
 
-    if not os.path.isdir(dir_path):
-        print(f"Error: {dir_path} is not a valid directory.")
-        exit(1)
-
-    if not is_git_repo(dir_path):
-        print(f"Error: {dir_path} is not a Git repository.")
+    if os.path.isdir(path_or_url):
+        if not is_git_repo(path_or_url):
+            print(f"Error: {path_or_url} is not a Git repository.")
+            exit(1)
+
+        check_branch_names(path_or_url)
+        get_remote_branches_info(path_or_url)
+        walk_and_process(
+            path_or_url,
+            None,
+            lint_flag=lint_flag,
+            start_date=start_date,
+            verbose=verbose,
+        )
+    elif is_git_remote_repo(path_or_url):
+        repo_path = clone_repo(path_or_url)
+        evaluate_repo(
+            repo_path,
+            lint_flag=lint_flag,
+            start_date=start_date,
+            verbose=verbose,
+        )
+    else:
+        print(f"Error: {path_or_url} is not a Git repository URL.")
         exit(1)
-
-    check_branch_names(dir_path)
-    get_remote_branches_info(dir_path)
-    walk_and_process(
-        dir_path,
-        None,
-        lint_flag=lint_flag,
-        start_date=start_date,
-        verbose=verbose,
-    )
     return 0
 
 
 def main():
     parser = argparse.ArgumentParser(description="COCOA CLI")
 
     parser.add_argument("repo", help="Path to a repository root directory")
```

### Comparing `dsi_cocoa-0.1.2/src/cocoa/linting.py` & `dsi_cocoa-0.1.3/src/cocoa/linting.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,34 +40,36 @@
 
 def pyflakes_notebook(path_to_notebook):
     """
     Run pyflakes on a Jupyter notebook.
     :param path_to_notebook: path to the notebook file.
     :return: list of warnings and errors from pyflakes.
     """
-    # Convert notebook to Python script
-    exporter = PythonExporter()
-    script, _ = exporter.from_filename(path_to_notebook)
-
-    with tempfile.NamedTemporaryFile(
-        mode="w", delete=False, suffix=".py"
-    ) as temp:
-        temp_name = temp.name
-        temp.write(script)
-
-    errors_and_warnings = pyflakes_python_file(temp_name)
-    reformatted_errors_and_warnings = convert_temp_names_to_originals(
-        errors_and_warnings,
-        path_to_notebook,
-    )
-
-    # Delete temporary file
-    os.remove(temp_name)
-    return reformatted_errors_and_warnings
-
+    try:
+        # Convert notebook to Python script
+        exporter = PythonExporter()
+        script, _ = exporter.from_filename(path_to_notebook)
+
+        with tempfile.NamedTemporaryFile(
+            mode="w", delete=False, suffix=".py"
+        ) as temp:
+            temp_name = temp.name
+            temp.write(script)
+
+        errors_and_warnings = pyflakes_python_file(temp_name)
+        reformatted_errors_and_warnings = convert_temp_names_to_originals(
+            errors_and_warnings,
+            path_to_notebook,
+        )
+
+        # Delete temporary file
+        os.remove(temp_name)
+        return reformatted_errors_and_warnings
+    except Exception as e:
+        print(f"An error occurred while running pyflakes: {e}")
 
 def pyflakes_python_file(file_path):
     """
     Run a python file through pyflakes. returns the number of warnings raised.
     """
     # Prepare StringIO object for capturing pyflakes output
     error_stream = StringIO()
```

### Comparing `dsi_cocoa-0.1.2/src/cocoa/notebooks.py` & `dsi_cocoa-0.1.3/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/src/cocoa/repo.py` & `dsi_cocoa-0.1.3/src/cocoa/repo.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 import os
 import tempfile
 from datetime import datetime
 
 import git
+import requests
 from git import GitCommandError, Repo
 
 
 def is_git_repo(repo_path):
     """
     Return a boolean if the directory supplied is a git repo.
     """
@@ -179,7 +180,22 @@
         commit_date = datetime.fromtimestamp(commit.committed_date)
         if commit_date > since_date:
             for entry in commit.stats.files.keys():
                 file_path = os.path.join(repo.working_dir, entry)
                 if file_path not in files_modified:
                     files_modified.append(file_path)
     return files_modified
+
+
+def is_git_remote_repo(url):
+    # Normalize the URL by ensuring it ends with '.git'
+    if not url.endswith(".git"):
+        url += ".git"
+
+    try:
+        response = requests.get(url)
+        if response.ok:
+            return True
+    except requests.RequestException as e:
+        print(f"Failed to access {url}: {e}")
+
+    return False
```

### Comparing `dsi_cocoa-0.1.2/src/cocoa/spring2024.py` & `dsi_cocoa-0.1.3/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.2
+Version: 0.1.3
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dsi_cocoa-0.1.2/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.1.3/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

