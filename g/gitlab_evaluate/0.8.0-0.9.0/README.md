# Comparing `tmp/gitlab_evaluate-0.8.0.tar.gz` & `tmp/gitlab_evaluate-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab_evaluate-0.8.0.tar", max compression
+gzip compressed data, was "gitlab_evaluate-0.9.0.tar", max compression
```

## Comparing `gitlab_evaluate-0.8.0.tar` & `gitlab_evaluate-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1122 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/LICENSE
--rw-r--r--   0        0        0     5078 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/README.md
--rw-r--r--   0        0        0        0 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/__init__.py
--rw-r--r--   0        0        0        0 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/ci_readiness/__init__.py
--rw-r--r--   0        0        0     5730 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/ci_readiness/test_engine.py
--rw-r--r--   0        0        0      684 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/ci_readiness/yaml_reader.py
--rw-r--r--   0        0        0       67 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/data/ci-readiness-report.yml
--rw-r--r--   0        0        0    14625 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/data/default-rules-config.yml
--rw-r--r--   0        0        0      309 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/data/migration-report.yml
--rw-r--r--   0        0        0     2628 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/evaluate_ci.py
--rw-r--r--   0        0        0        0 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/__init__.py
--rw-r--r--   0        0        0     7992 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/api.py
--rw-r--r--   0        0        0      336 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/cmd.py
--rw-r--r--   0        0        0     1075 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/filetree.py
--rw-r--r--   0        0        0     4782 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/flag_remediation.py
--rw-r--r--   0        0        0      198 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/git.py
--rw-r--r--   0        0        0     2584 2022-10-31 18:53:05.890735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/human_bytes.py
--rw-r--r--   0        0        0      284 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/limits.py
--rw-r--r--   0        0        0     2468 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/lib/utils.py
--rw-r--r--   0        0        0     2895 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/main.py
--rw-r--r--   0        0        0        0 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/migration_readiness/__init__.py
--rw-r--r--   0        0        0     8576 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/migration_readiness/report_generator.py
--rw-r--r--   0        0        0        0 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/models/__init__.py
--rw-r--r--   0        0        0      311 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/models/ci_rules.py
--rw-r--r--   0        0        0      427 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/gitlab_evaluate/models/test_results.py
--rw-r--r--   0        0        0      861 2022-10-31 18:53:05.891735 gitlab_evaluate-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     6525 1970-01-01 00:00:00.000000 gitlab_evaluate-0.8.0/setup.py
--rw-r--r--   0        0        0     6029 1970-01-01 00:00:00.000000 gitlab_evaluate-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1122 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5113 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/ci_readiness/__init__.py
+-rw-r--r--   0        0        0     5730 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/ci_readiness/test_engine.py
+-rw-r--r--   0        0        0      684 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/ci_readiness/yaml_reader.py
+-rw-r--r--   0        0        0       67 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/data/ci-readiness-report.yml
+-rw-r--r--   0        0        0    14625 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/data/default-rules-config.yml
+-rw-r--r--   0        0        0      309 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/data/migration-report.yml
+-rw-r--r--   0        0        0     2628 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/evaluate_ci.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/__init__.py
+-rw-r--r--   0        0        0     7906 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/api.py
+-rw-r--r--   0        0        0      336 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/cmd.py
+-rw-r--r--   0        0        0     1075 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/filetree.py
+-rw-r--r--   0        0        0     4782 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/flag_remediation.py
+-rw-r--r--   0        0        0      198 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/git.py
+-rw-r--r--   0        0        0     2584 2023-05-10 07:16:20.031494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/human_bytes.py
+-rw-r--r--   0        0        0      288 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/limits.py
+-rw-r--r--   0        0        0     2443 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/lib/utils.py
+-rw-r--r--   0        0        0     2895 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/main.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/migration_readiness/__init__.py
+-rw-r--r--   0        0        0     8576 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/migration_readiness/report_generator.py
+-rw-r--r--   0        0        0        0 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/models/__init__.py
+-rw-r--r--   0        0        0      311 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/models/ci_rules.py
+-rw-r--r--   0        0        0      427 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/gitlab_evaluate/models/test_results.py
+-rw-r--r--   0        0        0      861 2023-05-10 07:16:20.032494 gitlab_evaluate-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6064 1970-01-01 00:00:00.000000 gitlab_evaluate-0.9.0/PKG-INFO
```

### Comparing `gitlab_evaluate-0.8.0/LICENSE` & `gitlab_evaluate-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/README.md` & `gitlab_evaluate-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 - Instance
 - Group (including sub-groups)
 
 This information is useful to the GitLab Professional Services (PS) team to accurately scope migration services.
 
 ## Use Case
 
-GitLab PS plans to share this script with a Customer to run against their GitLab instance or group. Then the customer can send back the output files to enable GitLab engagement managers to scope engagements accurately. There are 3 output files.
-
-The one to send back is the `report.txt` which lists config and project/group data possibly needing some special attention based on these [limits](#project-thresholds)
+GitLab PS plans to share this script with a Customer to run against their GitLab instance or group. Then the customer can send back the output files to enable GitLab engagement managers to scope engagements accurately. There are [3 output files](reading-the-output.md).
 
 ## Install Method
 
 - [pip Install](#pip-install)
 - [Docker Container](#docker-container)
   - [Bash](#local-usage)
 
@@ -39,16 +37,21 @@
 
     For evaluating a GitLab group (including sub-groups)
 
     ```bash
     evaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com -g 42
     ```
 
-4. This should create a file called `evaluate_output.csv`
-5. If you're coordinating a GitLab PS engagement, email this file to the GitLab account team.
+4. This should create three files:
+   - `evaluate_output.csv`
+   - `flags_evaluate_output.csv`
+   - `report.txt`
+
+   For more information on these files, see [reading the output](reading-the-output.md)
+5. If you're coordinating a GitLab PS engagement, email these files to the GitLab account team.
 
 ### To gather CI data from a single repo
 
 ```bash
 # For evaluating a single git repo's CI readiness
 evaluate-ci-readiness -r|--repo <git-repo-url>
 ```
@@ -123,19 +126,20 @@
 
 ## Project Thresholds
 
 _Below are the thresholds we will use to determine whether a project can be considered for normal migration or needs to have special steps taken in order to migrate_
 
 ### Project Data
 
+- Project Size - 20GB
 - Pipelines - 5,000 max
-- Issues - 1,500 total (not just open)
-- Merge Requests - 1,500 total (not just merged)
+- Issues - 5,000 total (not just open)
+- Merge Requests - 5,000 total (not just merged)
 - Container images - 20GB per project
 - Packages - Any packages present
 
-### Repo Data
+### Repository Data
 
-- commits - 20K
-- branches - 1K
-- tags - 1K
-- Disk Size - 10GB
+- Repository Size - 5GB
+- Commits - 50K
+- Branches - 1K
+- Tags - 5K
```

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/ci_readiness/test_engine.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/ci_readiness/test_engine.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/ci_readiness/yaml_reader.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/ci_readiness/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/data/default-rules-config.yml` & `gitlab_evaluate-0.9.0/gitlab_evaluate/data/default-rules-config.yml`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/evaluate_ci.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/evaluate_ci.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/lib/api.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/lib/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             # wiki_size = stats.get['wiki_size']
             # lfs_objects_size = stats.get['lfs_objects_size']
             # job_artifacts_size = stats.get['job_artifacts_size']
             # snippets_size = stats.get['snippets_size']
             # packages_size = stats.get['packages_size']
             export_total = 0
             for k, v in stats.items():
-                updated_dict_entry = { k: hb.HumanBytes.format(v, True) if k != "commit_count" else v, k + "_over": utils.check_size(k, v)}
+                updated_dict_entry = { k: v, k + "_over": utils.check_size(k, v)}
                 my_dict.update(updated_dict_entry)
 
                 # If k an item that would be part of the export, add to running total
                 if k in [
                     "repository_size",
                     "wiki_size",
                     "lfs_objects_size",
@@ -110,15 +110,15 @@
 
                 # my_dict[k] = {
                 #     "value": hb.HumanBytes.format(v, True) if k != 'commit_count' else v,
                 #     "over": utils.check_size(k, v)
                 # }
             
             # Write running total to my_dict
-            my_dict.update({"Estimated Export Size": hb.HumanBytes.format(export_total, True)})
+            my_dict.update({"Estimated Export Size": export_total})
             export_total = 0
             # reset running total? Not loop, so maybe not
         else:
             print(f"Could not extracts stats for project {project.get('path_with_namepsace')}.\n")
     else:
         print(f"Could not retrieve project with stats for project id: {project.get('id')}")
```

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/lib/filetree.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/lib/filetree.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/lib/flag_remediation.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/lib/flag_remediation.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/lib/human_bytes.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/lib/human_bytes.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/lib/utils.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/lib/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,42 +18,41 @@
         with open(file_path, file_action) as cf:
             writer = csv.DictWriter(cf, fieldnames=headers)
             if not append:
                 writer.writeheader()
             for entry in data:
                 writer.writerow(entry)
     except IOError:
-          print(f"\nI/O error. Cannot create {file_path}")
-          print(f"Ensure you have the proper permissions to create {file_path}.\n")
-          sys.exit()
+        print(f"\nI/O error. Cannot create {file_path}")
+        print(f"Ensure you have the proper permissions to create {file_path}.\n")
+        sys.exit()
 
 def check_size(k, v):
     # TODO: Dictionary of function pointers
     if k == "storage_size":
         return check_storage_size(v)
-    elif k == "commit_count":
+    if k == "commit_count":
         return check_num_commits(v)
-    elif k == "repository_size":
+    if k == "repository_size":
         return check_file_size(v)
 
 def check_num_pl(i):
     return i > limits.PIPELINES_COUNT
 
 def check_num_br(i):
     return i > limits.BRANCHES_COUNT
 
 def check_num_commits(i):
     return i > limits.COMMITS_COUNT
 
 def check_storage_size(i):
-    '''Checking storage size against 20 GB'''
+    '''Includes artifacts, repositories, wiki, and other items.'''
     return i > limits.STORAGE_SIZE
 
 def check_registry_size(i):
-    '''Checking registry size against 20 GB'''
     return i > limits.CONTAINERS_SIZE
 
 ### File size limit is 5GB
 def check_file_size(i):
     return i > limits.FILE_SIZE
 
 def check_num_issues(i):
@@ -62,22 +61,22 @@
 def check_num_mr(i):
     return i > limits.MERGE_REQUESTS_COUNT
 
 def check_num_tags(i):
     return i > limits.TAGS_COUNT
 
 def check_proj_type(i):
-    return i 
+    return i
 
 def sizeof_fmt(num, suffix="B"):
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return f"{num:3.1f}{unit}{suffix}"
         num /= 1024.0
     return f"{num:.1f}Yi{suffix}"
 
-"""
-    shameless copy from https://www.w3resource.com/python-exercises/string/python-data-type-string-exercise-96.php
-"""
 def to_camel_case(s):
+    """
+        Shameless copy from https://www.w3resource.com/python-exercises/string/python-data-type-string-exercise-96.php
+    """
     s = sub(r"(_|-)+", " ", s).title().replace(" ", "")
     return ''.join([s[0].lower(), s[1:]])
```

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/main.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/main.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/gitlab_evaluate/migration_readiness/report_generator.py` & `gitlab_evaluate-0.9.0/gitlab_evaluate/migration_readiness/report_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab_evaluate-0.8.0/pyproject.toml` & `gitlab_evaluate-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitlab_evaluate"
-version = "0.8.0"
+version = "0.9.0"
 description = "Scans GitLab instance and ranks projects against a set of criteria. Can be used to identiy projects that may have too much metadata/size to reliably export or import."
 authors = ["GitLab Professional Services <proserv@gitlab.com>", "Jo Marquez <jmarquez@gitlab.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate"
 
 [tool.poetry.dependencies]
```

### Comparing `gitlab_evaluate-0.8.0/setup.py` & `gitlab_evaluate-0.9.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,167 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: gitlab-evaluate
+Version: 0.9.0
+Summary: Scans GitLab instance and ranks projects against a set of criteria. Can be used to identiy projects that may have too much metadata/size to reliably export or import.
+Home-page: https://gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate
+License: MIT
+Author: GitLab Professional Services
+Author-email: proserv@gitlab.com
+Requires-Python: >=3.8.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: gitlab-ps-utils (>=0.5.0,<0.6.0)
+Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['gitlab_evaluate',
- 'gitlab_evaluate.ci_readiness',
- 'gitlab_evaluate.lib',
- 'gitlab_evaluate.migration_readiness',
- 'gitlab_evaluate.models']
-
-package_data = \
-{'': ['*'], 'gitlab_evaluate': ['data/*']}
-
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'gitlab-ps-utils>=0.5.0,<0.6.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'requests>=2.26.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['evaluate-ci-readiness = gitlab_evaluate.evaluate_ci:main',
-                     'evaluate-gitlab = gitlab_evaluate.main:main']}
-
-setup_kwargs = {
-    'name': 'gitlab-evaluate',
-    'version': '0.8.0',
-    'description': 'Scans GitLab instance and ranks projects against a set of criteria. Can be used to identiy projects that may have too much metadata/size to reliably export or import.',
-    'long_description': "# Evaluate\n\nEvaluate is a script that can be run to gather information about all projects of a GitLab\n\n- Instance\n- Group (including sub-groups)\n\nThis information is useful to the GitLab Professional Services (PS) team to accurately scope migration services.\n\n## Use Case\n\nGitLab PS plans to share this script with a Customer to run against their GitLab instance or group. Then the customer can send back the output files to enable GitLab engagement managers to scope engagements accurately. There are 3 output files.\n\nThe one to send back is the `report.txt` which lists config and project/group data possibly needing some special attention based on these [limits](#project-thresholds)\n\n## Install Method\n\n- [pip Install](#pip-install)\n- [Docker Container](#docker-container)\n  - [Bash](#local-usage)\n\n## Usage\n\n### System level data gathering\n\nEvaluate is meant to be run by an **OWNER** (ideally system **ADMINISTRATOR**) of a GitLab instance to gather data about every project on the instance or group (including sub-groups).\n\n1. A GitLab **OWNER** (ideally system **ADMINISTRATOR**) should provision an access token with `api` scope:\n   - [Personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#create-a-personal-access-token) for instance\n   - [Group access token](https://docs.gitlab.com/ee/user/group/settings/group_access_tokens.html#create-a-group-access-token-using-ui) for group\n2. Install `gitlab-evaluate` from the [Install](#install) section above,\n3. Run :point_down:\n\n    For evaluating a GitLab instance\n\n    ```bash\n    evaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com\n    ```\n\n    For evaluating a GitLab group (including sub-groups)\n\n    ```bash\n    evaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com -g 42\n    ```\n\n4. This should create a file called `evaluate_output.csv`\n5. If you're coordinating a GitLab PS engagement, email this file to the GitLab account team.\n\n### To gather CI data from a single repo\n\n```bash\n# For evaluating a single git repo's CI readiness\nevaluate-ci-readiness -r|--repo <git-repo-url>\n```\n\n### Command help screen\n\n```text\nusage: evaluate-gitlab [-h] [-t TOKEN] [-s SOURCE] [-f FILENAME] [-o] [-i] [-p PROCESSES] [-g GROUP_ID]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -t TOKEN, --token TOKEN\n                        Personal Access Token: REQ'd\n  -s SOURCE, --source SOURCE\n                        Source URL: REQ'd\n  -f FILENAME, --filename FILENAME\n                        CSV Output File Name. If not set, will default to 'evaluate_output.csv'\n  -o, --output          Output Per Project Stats to screen\n  -i, --insecure        Set to ignore SSL warnings.\n  -p PROCESSES, --processes PROCESSES\n                        Number of processes. Defaults to number of CPU cores\n  -g GROUP_ID, --group GROUP_ID\n                        Group ID. Evaluate all group projects (including sub-groups)\n```\n\n```text\nusage: evaluate-ci-readiness [-h] [-r REPO]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -r REPO, --repo REPO  Git Repository To Clone (ex: https://username:password@repo.com\n```\n\n### pip Install\n\n```bash\npip install gitlab-evaluate\n```\n\n## Docker Container\n\n[Docker containers with evaluate installed](https://gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate/container_registry) are also available to use.\n\n### Local Usage\n\n```bash\n# Spin up container\ndocker run --name evaluate -it registry.gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate:latest /bin/bash\n\n# In docker shell\nevaluate-ci-readiness -r|--repo <git-repo-url>\nevaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com\n```\n\n### Example GitLab CI job using evaluate ci readiness script\n\n```yaml\nevaluate node-js:\n  stage: test\n  script:\n    - evaluate-ci-readiness --repo=https://github.com/nodejs/node.git\n  artifacts:\n    paths:\n      - node.csv\n```\n\nTo **test**, consider standing up a local docker container of GitLab. Provision an access token with `api` scope and **OWNER** (ideally system **ADMINISTRATOR**) privileges. Create multiple projects with varying number of commits, pipelines, merge requests, issues. Consider importing an open source repo or using [GPT](https://gitlab.com/gitlab-org/quality/performance) to add projects to the system.\n\n## Design\n\nDesign for the script can be found [here](https://gitlab.com/gitlab-com/customer-success/professional-services-group/ps-leadership-team/ps-practice-management/-/issues/83)\n\n## Project Thresholds\n\n_Below are the thresholds we will use to determine whether a project can be considered for normal migration or needs to have special steps taken in order to migrate_\n\n### Project Data\n\n- Pipelines - 5,000 max\n- Issues - 1,500 total (not just open)\n- Merge Requests - 1,500 total (not just merged)\n- Container images - 20GB per project\n- Packages - Any packages present\n\n### Repo Data\n\n- commits - 20K\n- branches - 1K\n- tags - 1K\n- Disk Size - 10GB\n",
-    'author': 'GitLab Professional Services',
-    'author_email': 'proserv@gitlab.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.0',
-}
+# Evaluate
 
+Evaluate is a script that can be run to gather information about all projects of a GitLab
+
+- Instance
+- Group (including sub-groups)
+
+This information is useful to the GitLab Professional Services (PS) team to accurately scope migration services.
+
+## Use Case
+
+GitLab PS plans to share this script with a Customer to run against their GitLab instance or group. Then the customer can send back the output files to enable GitLab engagement managers to scope engagements accurately. There are [3 output files](reading-the-output.md).
+
+## Install Method
+
+- [pip Install](#pip-install)
+- [Docker Container](#docker-container)
+  - [Bash](#local-usage)
+
+## Usage
+
+### System level data gathering
+
+Evaluate is meant to be run by an **OWNER** (ideally system **ADMINISTRATOR**) of a GitLab instance to gather data about every project on the instance or group (including sub-groups).
+
+1. A GitLab **OWNER** (ideally system **ADMINISTRATOR**) should provision an access token with `api` scope:
+   - [Personal access token](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html#create-a-personal-access-token) for instance
+   - [Group access token](https://docs.gitlab.com/ee/user/group/settings/group_access_tokens.html#create-a-group-access-token-using-ui) for group
+2. Install `gitlab-evaluate` from the [Install](#install) section above,
+3. Run :point_down:
+
+    For evaluating a GitLab instance
+
+    ```bash
+    evaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com
+    ```
+
+    For evaluating a GitLab group (including sub-groups)
+
+    ```bash
+    evaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com -g 42
+    ```
+
+4. This should create three files:
+   - `evaluate_output.csv`
+   - `flags_evaluate_output.csv`
+   - `report.txt`
+
+   For more information on these files, see [reading the output](reading-the-output.md)
+5. If you're coordinating a GitLab PS engagement, email these files to the GitLab account team.
+
+### To gather CI data from a single repo
+
+```bash
+# For evaluating a single git repo's CI readiness
+evaluate-ci-readiness -r|--repo <git-repo-url>
+```
+
+### Command help screen
+
+```text
+usage: evaluate-gitlab [-h] [-t TOKEN] [-s SOURCE] [-f FILENAME] [-o] [-i] [-p PROCESSES] [-g GROUP_ID]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -t TOKEN, --token TOKEN
+                        Personal Access Token: REQ'd
+  -s SOURCE, --source SOURCE
+                        Source URL: REQ'd
+  -f FILENAME, --filename FILENAME
+                        CSV Output File Name. If not set, will default to 'evaluate_output.csv'
+  -o, --output          Output Per Project Stats to screen
+  -i, --insecure        Set to ignore SSL warnings.
+  -p PROCESSES, --processes PROCESSES
+                        Number of processes. Defaults to number of CPU cores
+  -g GROUP_ID, --group GROUP_ID
+                        Group ID. Evaluate all group projects (including sub-groups)
+```
+
+```text
+usage: evaluate-ci-readiness [-h] [-r REPO]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -r REPO, --repo REPO  Git Repository To Clone (ex: https://username:password@repo.com
+```
+
+### pip Install
+
+```bash
+pip install gitlab-evaluate
+```
+
+## Docker Container
+
+[Docker containers with evaluate installed](https://gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate/container_registry) are also available to use.
+
+### Local Usage
+
+```bash
+# Spin up container
+docker run --name evaluate -it registry.gitlab.com/gitlab-org/professional-services-automation/tools/utilities/evaluate:latest /bin/bash
+
+# In docker shell
+evaluate-ci-readiness -r|--repo <git-repo-url>
+evaluate-gitlab -t <access-token-with-api-scope> -s https://gitlab.example.com
+```
+
+### Example GitLab CI job using evaluate ci readiness script
+
+```yaml
+evaluate node-js:
+  stage: test
+  script:
+    - evaluate-ci-readiness --repo=https://github.com/nodejs/node.git
+  artifacts:
+    paths:
+      - node.csv
+```
+
+To **test**, consider standing up a local docker container of GitLab. Provision an access token with `api` scope and **OWNER** (ideally system **ADMINISTRATOR**) privileges. Create multiple projects with varying number of commits, pipelines, merge requests, issues. Consider importing an open source repo or using [GPT](https://gitlab.com/gitlab-org/quality/performance) to add projects to the system.
+
+## Design
+
+Design for the script can be found [here](https://gitlab.com/gitlab-com/customer-success/professional-services-group/ps-leadership-team/ps-practice-management/-/issues/83)
+
+## Project Thresholds
+
+_Below are the thresholds we will use to determine whether a project can be considered for normal migration or needs to have special steps taken in order to migrate_
+
+### Project Data
+
+- Project Size - 20GB
+- Pipelines - 5,000 max
+- Issues - 5,000 total (not just open)
+- Merge Requests - 5,000 total (not just merged)
+- Container images - 20GB per project
+- Packages - Any packages present
+
+### Repository Data
+
+- Repository Size - 5GB
+- Commits - 50K
+- Branches - 1K
+- Tags - 5K
 
-setup(**setup_kwargs)
```

