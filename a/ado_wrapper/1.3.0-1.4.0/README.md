# Comparing `tmp/ado_wrapper-1.3.0.tar.gz` & `tmp/ado_wrapper-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.3.0.tar", max compression
+gzip compressed data, was "ado_wrapper-1.4.0.tar", max compression
```

## Comparing `ado_wrapper-1.3.0.tar` & `ado_wrapper-1.4.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.3.0/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.3.0/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.3.0/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.3.0/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2187 2024-04-21 14:56:46.791867 ado_wrapper-1.3.0/ado_wrapper/client.py
--rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.3.0/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.3.0/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.3.0/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.3.0/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.3.0/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.3.0/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.3.0/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      976 2024-04-20 14:42:40.468814 ado_wrapper-1.3.0/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4787 2024-04-23 11:10:12.040702 ado_wrapper-1.3.0/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.3.0/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14817 2024-04-23 08:38:52.982381 ado_wrapper-1.3.0/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6583 2024-04-21 14:56:46.795412 ado_wrapper-1.3.0/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.3.0/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.3.0/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15041 2024-04-21 14:56:46.796903 ado_wrapper-1.3.0/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-04-21 14:56:46.797268 ado_wrapper-1.3.0/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    13959 2024-04-21 14:56:46.797627 ado_wrapper-1.3.0/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.3.0/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10226 2024-04-22 10:44:14.335216 ado_wrapper-1.3.0/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.3.0/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.3.0/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.3.0/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.3.0/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9380 2024-04-23 09:03:14.872165 ado_wrapper-1.3.0/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     7881 2024-04-23 11:05:52.742242 ado_wrapper-1.3.0/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4782 2024-04-23 08:38:52.967534 ado_wrapper-1.3.0/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-04-23 11:10:50.239802 ado_wrapper-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.4.0/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.4.0/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.4.0/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.4.0/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2187 2024-04-21 14:56:46.791867 ado_wrapper-1.4.0/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.4.0/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3271 2024-05-02 09:19:09.438484 ado_wrapper-1.4.0/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.4.0/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.4.0/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.4.0/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.4.0/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.4.0/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.4.0/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1026 2024-04-29 12:13:21.212309 ado_wrapper-1.4.0/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.4.0/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.4.0/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14817 2024-04-23 08:38:52.982381 ado_wrapper-1.4.0/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6583 2024-04-21 14:56:46.795412 ado_wrapper-1.4.0/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.4.0/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.4.0/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15274 2024-04-29 10:16:27.641099 ado_wrapper-1.4.0/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.4.0/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    13959 2024-04-21 14:56:46.797627 ado_wrapper-1.4.0/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.4.0/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10226 2024-04-22 10:44:14.335216 ado_wrapper-1.4.0/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.4.0/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.4.0/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.4.0/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.4.0/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.4.0/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9380 2024-04-23 09:03:14.872165 ado_wrapper-1.4.0/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     7881 2024-04-23 11:05:52.742242 ado_wrapper-1.4.0/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4782 2024-04-23 08:38:52.967534 ado_wrapper-1.4.0/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-02 09:20:31.602343 ado_wrapper-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.4.0/PKG-INFO
```

### Comparing `ado_wrapper-1.3.0/LICENSE` & `ado_wrapper-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/README.md` & `ado_wrapper-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/__main__.py` & `ado_wrapper-1.4.0/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/client.py` & `ado_wrapper-1.4.0/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/dumps.py` & `ado_wrapper-1.4.0/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.4.0/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.4.0/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.4.0/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,11 +9,12 @@
     MergePolicies,
     MergePolicyDefaultReviewer,
 )
 from ado_wrapper.resources.projects import Project
 from ado_wrapper.resources.pull_requests import PullRequest
 from ado_wrapper.resources.releases import Release, ReleaseDefinition
 from ado_wrapper.resources.repo import BuildRepository, Repo
+from ado_wrapper.resources.searches import Search
 from ado_wrapper.resources.service_endpoint import ServiceEndpoint
 from ado_wrapper.resources.teams import Team
 from ado_wrapper.resources.users import AdoUser, Member, Reviewer, TeamMember
 from ado_wrapper.resources.variable_groups import VariableGroup
```

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/annotated_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,26 @@
         ado_client.state_manager.remove_resource_from_state(cls.__name__, object_id)  # type: ignore[arg-type]
 
     # # ============ End of requirement set by all state managed resources ================== #
     # # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_all_by_repo(cls, ado_client: AdoClient, repo_name_or_id: str) -> list[AnnotatedTag]:
+    def get_all_by_repo(cls, ado_client: AdoClient, repo_id: str) -> list[AnnotatedTag]:
         """Unofficial API. Also doesn't return a repo_id"""
         request = ado_client.session.post(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_git/{repo_name_or_id}/tags/?api-version=7.1-preview.1"
+            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_git/{repo_id}/tags/?api-version=7.1-preview.1"
         )
         assert request.status_code == 200
         second_half = request.text.split("ms.vss-code-web.git-tags-data-provider")[1].removeprefix('":')
         trimmed_second_half = second_half.split("ms.vss-code-web.navigation-data-provider")[0].removesuffix(',"')
         json_data = json.loads(trimmed_second_half)["tags"]
         # ===
         return [
-            cls(x["objectId"], repo_name_or_id, x["name"], x["comment"],
+            cls(x["objectId"], repo_id, x["name"], x["comment"],
                 Member(x["tagger"]["name"], x["tagger"]["email"], "UNKNOWN"),
                 from_ado_date_string(x["tagger"]["date"]))
             for x in json_data if "comment" in x  # fmt: skip
         ]
 
     @classmethod
     def get_by_name(cls, ado_client: AdoClient, repo_id: str, tag_name: str) -> AnnotatedTag | None:
```

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/branches.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/builds.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/commits.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/environment.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/groups.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/merge_policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,18 @@
                    "dataProviderContext": {"properties": {"projectId": ado_client.ado_project_id, "repositoryId": repo_id, "refName": f"refs/heads/{branch_name}"}}}  # fmt: skip
         request = ado_client.session.post(
             f"https://dev.azure.com/{ado_client.ado_org}/_apis/Contribution/HierarchyQuery?api-version=7.1-preview.1",
             json=payload,
         ).json()
         if request is None:
             return []
+        if "ms.vss-code-web.branch-policies-data-provider" not in request["dataProviders"]:
+            print(f"No default reviewers found for repo {repo_id}! Most likely it's disabled.")
+            return []
+        # ===
         all_reviewers = [Reviewer(x["displayName"], x["uniqueName"], x["id"], 0, False) for x in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["identities"]]  # fmt: skip
         for policy_group in request["dataProviders"]["ms.vss-code-web.branch-policies-data-provider"]["policyGroups"].values():
             if policy_group["currentScopePolicies"] is None:
                 continue
             is_required = policy_group["currentScopePolicies"][0]["isBlocking"]
             if is_required and "requiredReviewerIds" in policy_group["currentScopePolicies"][0]["settings"]:
                 reviewers = policy_group["currentScopePolicies"][0]["settings"]["requiredReviewerIds"]
@@ -124,15 +128,15 @@
             data["id"], settings["scope"][0]["repositoryId"], (branch_name.removeprefix("refs/heads/") if branch_name else None),
             settings["minimumApproverCount"], settings["creatorVoteCounts"], settings["blockLastPusherVote"], settings["allowDownvotes"],
             when_new_changes_are_pushed, from_ado_date_string(data["createdDate"]),  # type: ignore[arg-type]
             is_inherited  # fmt: skip
         )
 
     @classmethod
-    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str) -> MergeBranchPolicy | None:
+    def get_branch_policy(cls, ado_client: AdoClient, repo_id: str, branch_name: str = "main") -> MergeBranchPolicy | None:
         """Gets the latest merge requirements for a pull request."""
         policy = MergePolicies.get_all_branch_policies_by_repo_id(ado_client, repo_id, branch_name)
         return policy[0] if policy else None
 
     @staticmethod
     def set_branch_policy(ado_client: AdoClient, repo_id: str, minimum_approver_count: int,
                           creator_vote_counts: bool, prohibit_last_pushers_vote: bool, allow_completion_with_rejects: bool,
```

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/projects.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/releases.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/repo.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/teams.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/users.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/users.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.4.0/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.4.0/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/state_manager.py` & `ado_wrapper-1.4.0/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/ado_wrapper/utils.py` & `ado_wrapper-1.4.0/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.3.0/pyproject.toml` & `ado_wrapper-1.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.3.0"
+version = "1.4.0"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.3.0/PKG-INFO` & `ado_wrapper-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.3.0
+Version: 1.4.0
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

