# Comparing `tmp/aind-behavior-curriculum-0.0.1.tar.gz` & `tmp/aind_behavior_curriculum-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind-behavior-curriculum-0.0.1.tar", last modified: Mon Feb 12 23:06:33 2024, max compression
+gzip compressed data, was "aind_behavior_curriculum-0.0.2.tar", last modified: Thu May  2 17:09:10 2024, max compression
```

## Comparing `aind-behavior-curriculum-0.0.1.tar` & `aind_behavior_curriculum-0.0.2.tar`

### file list

```diff
@@ -1,45 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.269832 aind-behavior-curriculum-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.257832 aind-behavior-curriculum-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.261832 aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.261832 aind-behavior-curriculum-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.github/workflows/init.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-02-12 23:06:33.265832 aind-behavior-curriculum-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.261832 aind-behavior-curriculum-0.0.1/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.261832 aind-behavior-curriculum-0.0.1/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.261832 aind-behavior-curriculum-0.0.1/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/doc_template/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.265832 aind-behavior-curriculum-0.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/examples/task_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/examples/task_instance.json
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/examples/task_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-12 23:06:33.269832 aind-behavior-curriculum-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.257832 aind-behavior-curriculum-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.265832 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum/behavior.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.265832 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6422 2024-02-12 23:06:33.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-12 23:06:33.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-12 23:06:33.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-12 23:06:33.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-12 23:06:33.000000 aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-12 23:06:33.265832 aind-behavior-curriculum-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-02-12 23:06:18.000000 aind-behavior-curriculum-0.0.1/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.670977 aind_behavior_curriculum-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.658977 aind_behavior_curriculum-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.662977 aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.662977 aind_behavior_curriculum-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-02 17:09:10.670977 aind_behavior_curriculum-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.670977 aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-02 17:09:10.000000 aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-02 17:09:10.000000 aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:09:10.000000 aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:09:10.000000 aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-02 17:09:10.000000 aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.662977 aind_behavior_curriculum-0.0.2/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/doc_template/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.662977 aind_behavior_curriculum-0.0.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/examples/example_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/curriculum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/examples/example_project/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    54759 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/diagrams/my_curr_diagram.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/curr_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11108 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/schema_manual_union.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/stage_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/task_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/jsons/task_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/examples/example_project_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/curriculum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.666977 aind_behavior_curriculum-0.0.2/examples/example_project_2/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/diagrams/p_triangle_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40434 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/diagrams/s_triangle_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22657 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/diagrams/track_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30415 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/diagrams/tree_curr_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/examples/example_project_2/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 17:09:10.670977 aind_behavior_curriculum-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.662977 aind_behavior_curriculum-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.670977 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-02 17:09:00.000000 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33412 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/curriculum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13220 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/src/aind_behavior_curriculum/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:09:10.670977 aind_behavior_curriculum-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/tests/test_curriculum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25660 2024-05-02 17:08:59.000000 aind_behavior_curriculum-0.0.2/tests/test_trainer.py
```

### Comparing `aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/.github/ISSUE_TEMPLATE/user-story.md` & `aind_behavior_curriculum-0.0.2/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/.github/workflows/tag_and_publish.yml` & `aind_behavior_curriculum-0.0.2/.github/workflows/tag_and_publish.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 name: Tag and publish
 on:
   push:
     branches:
       - main
-# Remove line 61 to enable automated semantic version bumps.
-# Change line 67 from "if: false" to "if: true" to enable PyPI publishing. 
-# Requires that svc-aindscicomp be added as an admin to repo.
+
 jobs:
   update_badges:
     runs-on: ubuntu-latest
     continue-on-error: true
     steps:
     - uses: actions/checkout@v3
-    - name: Set up Python 3.8
+    - name: Set up Python 3.10
       uses: actions/setup-python@v3
       with:
-        python-version: 3.8
+        python-version: 3.10
     - name: Install dependencies
-      run: | 
+      run: |
         python -m pip install -e .[dev] --no-cache-dir
     - name: Get Python version and Update README.md
       run: |
         python_version=$(grep "requires-python" pyproject.toml | grep -o ">=[^\"]*")
         python_badge=$(grep -o 'python-[^)]*' README.md)
         new_python_badge="python-$python_version-blue?logo=python"
         sed -i "s/$python_badge/$new_python_badge/g" README.md
@@ -38,45 +36,47 @@
         fi
         sed -i "s/$interrogate_badge/$new_interrogate_badge/g" README.md
     - name: Get Coverage values and Update README.md
       run: |
         coverage run -m unittest discover
         coverage_val=$(coverage report | grep "^TOTAL" | grep -o '[0-9]\+%' | grep -o '[0-9]\+')
         coverage_badge=$(grep -o "coverage-[^?]*" README.md)
-        if (( $(echo "$coverage_val >= 90.00" | bc -l) )); then 
+        if (( $(echo "$coverage_val >= 90.00" | bc -l) )); then
             new_coverage_badge="coverage-$coverage_val%25-brightgreen"
         elif (( $(echo "$coverage_val < 80.00" | bc -l) )); then
             new_coverage_badge="coverage-$coverage_val%25-red"
         else
             new_coverage_badge="coverage-$coverage_val%25-yellow"
         fi
         sed -i "s/$coverage_badge/$new_coverage_badge/g" README.md
     - name: Commit changes
       uses: EndBug/add-and-commit@v9
       with:
         default_author: github_actions
         message: "ci: update badges [skip actions]"
         add: '["README.md"]'
+
   tag:
-    needs: update_badges    
+    needs: update_badges
     uses: AllenNeuralDynamics/aind-github-actions/.github/workflows/tag.yml@main
     secrets:
       SERVICE_TOKEN: ${{ secrets.SERVICE_TOKEN }}
+
   publish:
     needs: tag
     if: true
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Pull latest changes
         run: git pull origin main
-      - name: Set up Python 3.8
+      - name: Set up Python 3.11
         uses: actions/setup-python@v2
         with:
-          python-version: 3.8
+          python-version: 3.11
       - name: Install dependencies
         run: |
           pip install --upgrade setuptools wheel twine build
           python -m build
           twine check dist/*
       - name: Publish on PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `aind-behavior-curriculum-0.0.1/.github/workflows/test_and_lint.yml` & `aind_behavior_curriculum-0.0.2/.github/workflows/test_and_lint.yml`

 * *Files 25% similar despite different names*

```diff
@@ -6,21 +6,21 @@
       - main
 
 jobs:
   ci:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
+        python-version: [ '3.11', '3.12' ]
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v3
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
-      run: | 
+      run: |
         python -m pip install -e .[dev]
     - name: Run linter checks
       run: flake8 . && interrogate --verbose .
     - name: Run tests and coverage
       run: coverage run -m unittest discover && coverage report
```

### Comparing `aind-behavior-curriculum-0.0.1/.gitignore` & `aind_behavior_curriculum-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/LICENSE` & `aind_behavior_curriculum-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/PKG-INFO` & `aind_behavior_curriculum-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic==2.6.0
-Requires-Dist: semver==3.0.2
+Requires-Dist: pydantic>2.7
+Requires-Dist: semver>=3.0
+Requires-Dist: jinja2>=3.1.3
+Requires-Dist: boto3>=1.34.95
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
```

### Comparing `aind-behavior-curriculum-0.0.1/README.md` & `aind_behavior_curriculum-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/doc_template/Makefile` & `aind_behavior_curriculum-0.0.2/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/doc_template/make.bat` & `aind_behavior_curriculum-0.0.2/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/doc_template/source/_static/dark-logo.svg` & `aind_behavior_curriculum-0.0.2/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/doc_template/source/_static/favicon.ico` & `aind_behavior_curriculum-0.0.2/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/doc_template/source/_static/light-logo.svg` & `aind_behavior_curriculum-0.0.2/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/doc_template/source/conf.py` & `aind_behavior_curriculum-0.0.2/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/examples/task_creation.py` & `aind_behavior_curriculum-0.0.2/examples/example_project/task.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,50 +3,47 @@
 """
 
 import json
 from typing import Literal
 
 from pydantic import Field, ValidationInfo, field_validator
 
-import aind_behavior_curriculum as abc
+from aind_behavior_curriculum import ModifiableAttr, Task, TaskParameters
 
 
-class ExampleTaskParameters(abc.TaskParameters):
+class ExampleTaskParameters(TaskParameters):
     """
     Example Task Parameters
     """
 
     # Required: Define type annotations for strict type checks.
     # Make fields immutable with Literal type.
-    field_1: int = abc.ModifiableAttr(default=0, ge=0.0)
-    field_2: int = abc.ModifiableAttr(default=0, ge=0.0)
+    field_1: int = ModifiableAttr(default=0, ge=0.0)
+    field_2: int = ModifiableAttr(default=0, ge=0.0)
     field_3: float = Field(default=0.5, ge=0.0, le=1.0)
     field_4: float = Field(default=0.5, ge=0.0, le=1.0)
     field_5: Literal["Immutable Field"] = "Immutable Field"
 
     # Optional: Add additional validation to fields.
     @field_validator("field_1", "field_2")
     @classmethod
     def check_something(cls, v: int, info: ValidationInfo):
         """Your validation code here"""
         return v
 
 
-class ExampleTask(abc.Task):
+class ExampleTask(Task):
     """
     Example Task
     """
 
     name: Literal["TaskName"] = "TaskName"
-    description: str = abc.ModifiableAttr(default="Ex description of task")
-    version: abc.SemVerAnnotation = "0.0.0"
-    # NOTE: '0.0.0' is a placeholder.
-    # Use the version of your task repo package!
+    description: str = ModifiableAttr(default="Ex description of task")
 
-    task_parameters: ExampleTaskParameters = abc.ModifiableAttr(
+    task_parameters: ExampleTaskParameters = ModifiableAttr(
         ..., description=ExampleTaskParameters.__doc__.strip()
     )
 
 
 if __name__ == "__main__":
     # Create task, optionally add parameters
     ex_parameters = ExampleTaskParameters(field_2=50, field_4=0.8)
@@ -64,23 +61,23 @@
         field_2=456,
         field_3=0.8,
         field_4=0.9,
     )
     print(ex_task)
 
     # Export/Serialize Task Schema:
-    with open("examples/task_schema.json", "w") as f:
+    with open("examples/example_project/jsons/task_schema.json", "w") as f:
         json_dict = ExampleTask.model_json_schema()
         json_string = json.dumps(json_dict, indent=4)
         f.write(json_string)
 
     # Export/Serialize Instance:
-    with open("examples/task_instance.json", "w") as f:
+    with open("examples/example_project/jsons/task_instance.json", "w") as f:
         json_dict = ex_task.model_dump()
         json_string = json.dumps(json_dict, indent=4)
         f.write(json_string)
 
     # Import/De-serialize Instance:
-    with open("examples/task_instance.json", "r") as f:
+    with open("examples/example_project/jsons/task_instance.json", "r") as f:
         json_data = f.read()
     task_instance = ExampleTask.model_validate_json(json_data)
     print(task_instance)
```

### Comparing `aind-behavior-curriculum-0.0.1/examples/task_schema.json` & `aind_behavior_curriculum-0.0.2/examples/example_project/jsons/task_schema.json`

 * *Files identical despite different names*

### Comparing `aind-behavior-curriculum-0.0.1/pyproject.toml` & `aind_behavior_curriculum-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,49 +2,53 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aind-behavior-curriculum"
 description = "Generated from aind-library-template"
 license = {text = "MIT"}
-requires-python = ">=3.8"
+requires-python = ">=3.11"
 authors = [
     {name = "Allen Institute for Neural Dynamics"}
 ]
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    "pydantic == 2.6.0",
-    "semver == 3.0.2"
+    "pydantic > 2.7",
+    "semver >= 3.0",
+    "jinja2 >= 3.1.3",
+    "boto3 >= 1.34.95"
 ]
 
 [project.optional-dependencies]
+
 dev = [
     'black',
     'coverage',
     'flake8',
     'interrogate',
     'isort',
     'Sphinx',
     'furo'
 ]
 
+
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src", "examples"]
 
 [tool.setuptools.dynamic]
 version = {attr = "aind_behavior_curriculum.__version__"}
 
 [tool.black]
 line-length = 79
-target_version = ['py36']
+target_version = ['py311']
 exclude = '''
 
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
@@ -71,11 +75,14 @@
     "pragma: no cover"
 ]
 fail_under = 90
 
 [tool.isort]
 line_length = 79
 profile = "black"
+skip = ["src/aind_behavior_curriculum/__init__.py"]
 
 [tool.interrogate]
-exclude = ["setup.py", "docs", "build", "tests/"]
+exclude = ["setup.py", "docs", "build", "tests/", "examples/"]
 fail-under = 100
+
+[tool.poetry]
```

### Comparing `aind-behavior-curriculum-0.0.1/src/aind_behavior_curriculum.egg-info/PKG-INFO` & `aind_behavior_curriculum-0.0.2/aind_behavior_curriculum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: aind-behavior-curriculum
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic==2.6.0
-Requires-Dist: semver==3.0.2
+Requires-Dist: pydantic>2.7
+Requires-Dist: semver>=3.0
+Requires-Dist: jinja2>=3.1.3
+Requires-Dist: boto3>=1.34.95
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: Sphinx; extra == "dev"
```

