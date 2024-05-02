# Comparing `tmp/easy_fossy-2.0.9.tar.gz` & `tmp/easy_fossy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fossy-2.0.9.tar", max compression
+gzip compressed data, was "easy_fossy-2.1.0.tar", max compression
```

## Comparing `easy_fossy-2.0.9.tar` & `easy_fossy-2.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1089 2024-02-13 20:02:56.662156 easy_fossy-2.0.9/LICENSE
--rwxr-xr-x   0        0        0     7135 2024-02-13 20:23:00.389925 easy_fossy-2.0.9/README.md
--rwxr-xr-x   0        0        0    52272 2024-02-13 21:42:14.060276 easy_fossy-2.0.9/easy_fossy/__init__.py
--rwxr-xr-x   0        0        0    19105 2024-02-13 21:37:08.139628 easy_fossy-2.0.9/easy_fossy/models.py
--rwxr-xr-x   0        0        0      612 2024-02-13 21:42:32.847998 easy_fossy-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     7735 1970-01-01 00:00:00.000000 easy_fossy-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0    59768 2024-05-02 12:09:07.500706 easy_fossy-2.1.0/easy_fossy/__init__.py
+-rw-r--r--   0        0        0    19249 2024-05-02 11:50:30.050210 easy_fossy-2.1.0/easy_fossy/models.py
+-rw-r--r--   0        0        0     1089 2024-02-13 20:02:56.662156 easy_fossy-2.1.0/LICENSE
+-rw-r--r--   0        0        0      612 2024-05-02 11:04:05.326773 easy_fossy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7135 2024-02-13 20:23:00.389925 easy_fossy-2.1.0/README.md
+-rw-r--r--   0        0        0     7735 1970-01-01 00:00:00.000000 easy_fossy-2.1.0/PKG-INFO
```

### Comparing `easy_fossy-2.0.9/LICENSE` & `easy_fossy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.0.9/README.md` & `easy_fossy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `easy_fossy-2.0.9/easy_fossy/__init__.py` & `easy_fossy-2.1.0/easy_fossy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     Public,
     Findings,
     ClearingStatus,
     Action,
     Action1,
     Agent,
     ApiInfo,
+    Copyright,
     File,
     Folder,
     Group,
     Hash,
     HeathInfo,
     Info,
     Job,
@@ -131,14 +132,50 @@
             case {**info}:
                 report_info = Info(**info)
                 print(f"{report_info.message}")
                 return new_group_name
             case _:
                 print(response.text)
 
+    def get_token_by_uname_pwd(self) -> str:
+        """Get the token via user name and password in the config"""
+        payload = {
+            "username": self.config.get("uname"),
+            "password": self.config.get("pwd"),
+            "token_name": str("created_viaapi_on_")
+            + str(self.now.strftime(self.dt_format)),
+            "token_scope": self.config.get("access"),
+            "token_expire": str(self.token_expire_yyyy_mm_dd),
+        }
+        headers = {
+            "accept": "application/json",
+            "Content-Type": "application/json",
+        }
+
+        response = requests.request(
+            "POST", self.url + str("tokens"), json=payload, headers=headers
+        )
+
+        match response.json():
+            case {"Authorization": self.bearer_token}:
+                self.config["bearer_token"] = self.bearer_token
+                self.config["token_expire"] = str(self.token_expire_yyyy_mm_dd)
+                with open(self.config_file, "w") as cf:
+                    self.config_parser.write(cf)
+                self.bearer_token = self.config.get("bearer_token")
+                if self.bearer_token != "":
+                    print(
+                        f"Added token to bearer_token param of your config {self.bearer_token}"
+                    )
+                return self.bearer_token
+            case _:
+                print("Error while getting token")
+                print(response.text)
+                sys.exit(1)
+
     def get_all_users(self) -> List[User]:
         """List of users present in the given instance"""
         payload = ""
         headers = {
             "accept": "application/json",
             "limit": "1000",
             "page": "1",
@@ -148,15 +185,16 @@
 
         response = requests.request(
             "GET", self.url + str("users"), data=payload, headers=headers
         )
 
         match response.json():
             case [*args]:
-                users = [print(user) and User(**user) for user in args]
+                # users = [print(user) and User(**user) for user in args]
+                users = [User(**user) for user in args]
                 # for j in jobs:
                 #     print(jobs)
                 return users
             case _:
                 print(response.text)
 
     # get_all_users()
@@ -194,57 +232,22 @@
         response = requests.request(
             "GET", self.url + str(f"users/{user_id}"), data=payload, headers=headers
         )
 
         match response.json():
             case {**user}:
                 user = User(**user)
-                print(user)
+                # print(user)
                 return user
             case _:
                 print(response.text)
 
         # get_user_by_id(user_id=3)
-                
-    def get_token_by_uname_pwd(self) -> str:
-        """Get the token via user name and password in the config"""
-        payload = {
-            "username": self.config.get("uname"),
-            "password": self.config.get("pwd"),
-            "token_name": str("created_viaapi_on_")
-            + str(self.now.strftime(self.dt_format)),
-            "token_scope": self.config.get("access"),
-            "token_expire": str(self.token_expire_yyyy_mm_dd),
-        }
-        headers = {
-            "accept": "application/json",
-            "Content-Type": "application/json",
-        }
-
-        response = requests.request(
-            "POST", self.url + str("tokens"), json=payload, headers=headers
-        )
-
-        match response.json():
-            case {"Authorization": self.bearer_token}:
-                self.config["bearer_token"] = self.bearer_token
-                self.config["token_expire"] = str(self.token_expire_yyyy_mm_dd)
-                with open(self.config_file, "w") as cf:
-                    self.config_parser.write(cf)
-                self.bearer_token = self.config.get("bearer_token")
-                if self.bearer_token != "":
-                    print(
-                        f"Added token to bearer_token param of your config {self.bearer_token}"
-                    )
-                return self.bearer_token
-            case _:
-                print("Error while getting token")
-                print(response.text)
-                sys.exit(1)
 
+    # get_user_by_id(user_id=)
     def get_all_jobs(self) -> List[Job]:
         """List of jobs present in the given instance"""
         payload = ""
         headers = {
             "accept": "application/json",
             "limit": "1000",
             "page": "1",
@@ -326,14 +329,120 @@
                 print(job)
                 return job
             case _:
                 print(response.text)
 
     # get_job_info_by_upload_id(job_id=3)
 
+    def get_upload_tree_id_by_upload_id(self, upload_id: int) -> Info:
+        """give the upload_id to get the upload_tree_id
+        {
+            "code": 200,
+            "message": 18852769,
+            "type": "INFO"
+        }
+        """
+        payload = ""
+        headers = {"accept": "application/json", "Authorization": self.bearer_token}
+
+        response = requests.request(
+            "GET",
+            self.url + str(f"uploads/{upload_id}/topitem"),
+            data=payload,
+            headers=headers,
+        )
+
+        match response.json():
+            case {**info}:
+                info = Info(**info)
+                # print(info)
+                return info
+            case _:
+                print(response.text)
+
+    # get_upload_tree_id_by_upload_id(upload_id=3)
+
+    def get_copyrights_by_upload_id_uploadtree_id(
+        self, upload_id: int, upload_tree_id: int
+    ) -> List[Copyright]:
+        """give the upload_id to get the upload_tree_id
+        [{
+            "content": "Copyright (C) 2008 dinesh Inc.",
+            "hash": "7414e55329991506a99fe2fb3383bbee",
+            "count": 28
+        },
+        {
+            "content": "Copyright (C) 2009 ravi Inc.",
+            "hash": "5c1af30f2523e1257bf8b7dba3e79776",
+            "count": 4
+        }]
+        """
+        payload = ""
+        headers = {"accept": "application/json", "Authorization": self.bearer_token}
+
+        response = requests.request(
+            "GET",
+            self.url + str(f"uploads/{upload_id}/item/{upload_tree_id}/copyrights"),
+            data=payload,
+            headers=headers,
+        )
+
+        match response.json():
+            case [*args]:
+                copyrights = [Copyright(**copyright) for copyright in args]
+                # for j in jobs:
+                #     print(jobs)
+                return copyrights
+            case _:
+                print(response.text)
+
+    # get_copyrights_by_upload_id_uploadtree_id(upload_id=3)
+
+    def get_copyrights_by_upload_id(self, upload_id: int) -> List[Copyright]:
+        """give the upload_id to get the upload_tree_id
+        [{
+            "content": "Copyright (C) 2008 dinesh Inc.",
+            "hash": "7414e55329991506a99fe2fb3383bbee",
+            "count": 28
+        },
+        {
+            "content": "Copyright (C) 2009 ravi Inc.",
+            "hash": "5c1af30f2523e1257bf8b7dba3e79776",
+            "count": 4
+        }]
+        """
+        payload = ""
+        headers = {"accept": "application/json", "Authorization": self.bearer_token}
+
+        upload_tree_id_info: Info = self.get_upload_tree_id_by_upload_id(
+            upload_id=upload_id
+        )
+        upload_tree_id = upload_tree_id_info.message
+
+        response = requests.request(
+            "GET",
+            self.url
+            + str(
+                f"uploads/{upload_id}/item/{upload_tree_id}/copyrights?status=active"
+            ),
+            data=payload,
+            headers=headers,
+        )
+
+        match response.json():
+            case [*args]:
+                copyrights = [Copyright(**copyright) for copyright in args]
+                # for j in jobs:
+                #     print(jobs)
+                return copyrights
+            case _:
+                print(response.text)
+
+    # get_copyrights_by_upload_id(upload_id=3)
+
     def generate_and_get_desired_report_for_uploadid(
         self, upload_id: int, report_format: ReportFormat
     ):
         """For given upload_id generate the report job to get report id and use to download desired Report Format
 
         class ReportFormat(Enum):
             dep5 = 'dep5'
@@ -639,17 +748,20 @@
         limit: int,
     ) -> List[Upload]:
         """get_all_uploads_based_on(folder_id: int, is_recursive: bool, search_pattern_key: str, upload_status: ClearingStatus, assignee: str, since_yyyy_mm_dd: str, page: int, limit: int) -> List[Upload]"""
         querystring = {
             "folderId": folder_id,
             "recursive": is_recursive,
             "name": search_pattern_key,
-            "status": upload_status.name,
+            "status": upload_status,
             "assignee": assignee,
             "since": since_yyyy_mm_dd,
+            "page": page,
+            "limit": limit,
+            "groupName": self.group_name,
         }
 
         payload = ""
         headers = {
             "accept": "application/json",
             "groupName": self.group_name,
             "page": str(page),
@@ -673,14 +785,64 @@
                 return uploads
             case _:
                 print(response.text)
 
     # get_all_uploads_based_on(folder_id=1, is_recursive=True,
     #                          search_pattern_key='', upload_status=ClearingStatus.Open, assignee='', since_yyyy_mm_dd='', page=1, limit=1000)
 
+    def get_all_uploads_based_on_common_assignee(
+        self,
+        folder_id: int,
+        is_recursive: bool,
+        search_pattern_key: str,
+        upload_status: ClearingStatus,
+        # assignee: str,
+        since_yyyy_mm_dd: str,
+        page: int,
+        limit: int,
+    ) -> List[Upload]:
+        """get_all_uploads_based_on(folder_id: int, is_recursive: bool, search_pattern_key: str, upload_status: ClearingStatus, assignee: str, since_yyyy_mm_dd: str, page: int, limit: int) -> List[Upload]"""
+        querystring = {
+            "folderId": folder_id,
+            "recursive": is_recursive,
+            "name": search_pattern_key,
+            "status": upload_status.name,
+            # "assignee": assignee,
+            "since": since_yyyy_mm_dd,
+        }
+
+        payload = ""
+        headers = {
+            "accept": "application/json",
+            "groupName": self.group_name,
+            "page": str(page),
+            "limit": str(limit),
+            "Authorization": self.bearer_token,
+        }
+
+        response = requests.request(
+            "GET",
+            self.url + str("uploads"),
+            data=payload,
+            headers=headers,
+            params=querystring,
+        )
+
+        match response.json():
+            case [*args]:
+                uploads = [Upload(**upload) for upload in args]
+                # for upload in uploads:
+                #     print(upload)
+                return uploads
+            case _:
+                print(response.text)
+
+    # get_all_uploads_based_on_common_assignee(folder_id=1, is_recursive=True,
+    #                          search_pattern_key='', upload_status=ClearingStatus.Open, since_yyyy_mm_dd='', page=1, limit=1000)
+
     def get_licenses_found_by_agents_for_uploadid(
         self, upload_id: int, agents: List[str], show_directories: bool
     ) -> UploadLicenses | Info:
         """get licenses acc to agent
         class Agent(Enum):
             nomos = 'nomos'
             monk = 'monk'
@@ -777,15 +939,15 @@
                 print(f"upload id is {report_info.message}")
                 return report_info.message
             case _:
                 print(response.text)
 
     # get_upload_id_by_local_package_upload(
     #     file_path='uploads/commons-io-2.11.0-src.zip', folder_id=1, upload_desc='commons-io-2.11.0', visibility=Public.public)
-
+    @staticmethod
     def check_url_exists(url: str):
         """
         Checks if a url exists
         :param url: url to check
         :return: True if the url exists, false otherwise.
         """
         return requests.head(url, allow_redirects=True).status_code == 200
@@ -984,29 +1146,34 @@
     #     upload_id=4, folder_id=1, group_name=group_name)
 
     def trigger_analysis_for_upload_package(self, file_path: str, folder_id: int):
         """trigger_analysis_for_upload_package(file_path: str, folder_id: int)"""
         if not Path(file_path).exists():
             print(f"File path {file_path} doesn't exist")
 
-        uploads: List[Upload] = self.get_all_uploads_based_on(
+        uploads: List[Upload] = self.get_all_uploads_based_on_common_assignee(
             folder_id=folder_id,
             is_recursive=True,
             search_pattern_key="",
             upload_status=ClearingStatus.Open,
-            assignee="",
+            # assignee="",
             since_yyyy_mm_dd="",
             page=1,
             limit=1000,
-            group_name=self.group_name,
+            # group_name=self.group_name,
         )
         file_name = file_path.split("/").pop()
 
-        upload_id = [u.id for u in uploads if file_name == u.uploadname]
-        size = len(upload_id)
+        # if folder is empty uploads will be None
+        size = 0
+        if uploads == None:
+            size = 0
+        else:
+            upload_id = [u.id for u in uploads if file_name == u.uploadname]
+            size = len(upload_id)
         is_present_uploadID = False
         if size > 1:
             is_present_uploadID = True
             print(f"{size} no of duplicates are there with ids {upload_id}")
             print(
                 "exiting.. please comeback after deleting duplicates via delete_uploads_by_upload_id(upload_id=upload_id, group_name=group_name)"
             )
@@ -1017,93 +1184,125 @@
         else:
             # no upload_id is there
             upload_id = self.get_upload_id_by_local_package_upload(
                 file_path=file_path,
                 folder_id=folder_id,
                 upload_desc=file_name,
                 visibility=Public.protected,
-                group_name=group_name,
+                # group_name=group_name,
             )
 
         if is_present_uploadID:
-            jobs: List[Job] = [
-                j for j in self.get_all_jobs(self.group_name) if j.uploadId == upload_id
-            ]
-
-            if len(jobs) >= 1:
-                print(f"Multiple jobs exists for same upload_id: {upload_id}")
-                job = jobs.pop()
-                print(f" Returning Existing Job ID :{job.id}")
-                return job.id
+            # get_all_jobs() is very slow because of huge size so just returning message
+            # jobs: List[Job] = [
+            #     j for j in self.get_all_jobs() if j.uploadId == upload_id
+            # ]
+
+            # if len(jobs) >= 1:
+            #     print(f"Multiple jobs exists for same upload_id: {upload_id}")
+            #     job = jobs.pop()
+            #     print(f" Returning Existing Job ID :{job.id}")
+            #     return job.id
+            # else:
+            #     job = jobs.pop()
+            #     print(f" Returning Existing Job ID :{job.id}")
+            #     return job.id
+            print(f"File {file_name} already present in folder id {folder_id}")
         else:
             info = self.trigger_analysis_for_upload_id(
-                upload_id=upload_id, folder_id=folder_id, group_name=self.group_name
+                upload_id=upload_id,
+                folder_id=folder_id,
+                # group_name=self.group_name
             )
             print(f"Computed new Job ID is :{info.message}")
             return info.message
 
     # trigger_analysis_for_upload_package(
     #     file_path='uploads/commons-lang3-3.12.0-src.zip', folder_id=1, group_name=group_name)
 
     def trigger_analysis_for_url_upload_package(
         self, file_download_url: str, file_name: str, branch_name: str, folder_id: int
     ):
         """trigger_analysis_for_url_upload_package(file_download_url: str, file_name: str, branch_name: str, folder_id: int)"""
         if not self.check_url_exists(file_download_url):
             print(f"git url {file_download_url} is malformed")
 
-        uploads: List[Upload] = self.get_all_uploads_based_on(
+        uploads: List[Upload] = self.get_all_uploads_based_on_common_assignee(
             folder_id=folder_id,
             is_recursive=True,
             search_pattern_key="",
             upload_status=ClearingStatus.Open,
-            assignee="",
+            # assignee="",
             since_yyyy_mm_dd="",
             page=1,
             limit=1000,
-            group_name=self.group_name,
+            # group_name=self.group_name,
         )
+        # if folder is empty uploads will be None
+        size = 0
+        upload_id: any
+        if uploads == None:
+            print("uploads is None")
+            size = 0
+        else:
+            upload_id = [u.id for u in uploads if file_name == u.uploadname]
+            # upload_id = []
+            # for u in uploads:
+            #     if file_name == u.uploadname:
+            #         # print(
+            #         #     f"Comparing file_name: {file_name} == u.uploadname: {u.uploadname}"
+            #         # )
+            #         upload_id.append(u.id)
 
-        upload_id = [u.id for u in uploads if file_name == u.uploadname]
-        size = len(upload_id)
+            size = len(upload_id)
+            # print(f"Existing upload size: {size}")
         is_present_uploadID = False
         if size > 1:
+            # print("section size > 1")
             is_present_uploadID = True
             print(f"{size} no of duplicates are there with ids {upload_id}")
             print(
                 "exiting.. please comeback after deleting duplicates via delete_uploads_by_upload_id(upload_id=upload_id, group_name=group_name)"
             )
             sys.exit(1)
         elif size == 1:
+            # print("section size ==  1")
             is_present_uploadID = True
             upload_id = upload_id[0]
         else:
+            # print("section else size ")
             # no upload_id is there
             upload_id = self.get_upload_id_by_download_url_package_upload(
                 file_download_url=file_download_url,
                 file_name=file_name,
-                folder_id=1,
+                folder_id=folder_id,
                 upload_desc=file_name,
                 visibility=Public.public,
-                group_name=group_name,
+                # group_name=self.group_name,
             )
 
         if is_present_uploadID:
-            jobs: List[Job] = [
-                j for j in self.get_all_jobs(self.group_name) if j.uploadId == upload_id
-            ]
-
-            if len(jobs) >= 1:
-                print(f"Multiple jobs exists for same upload_id: {upload_id}")
-                job = jobs.pop()
-                print(f" Returning Existing Job ID :{job.id}")
-                return job.id
+            # get_all_jobs() is very slow because of huge size so just returning message
+            # jobs: List[Job] = [
+            #     j for j in self.get_all_jobs() if j.uploadId == upload_id
+            # ]
+
+            # if len(jobs) >= 1:
+            #     print(f"Multiple jobs exists for same upload_id: {upload_id}")
+            #     job = jobs.pop()
+            #     print(f" Returning Existing Job ID :{job.id}")
+            #     return job.id
+            # else:
+            #     job = jobs.pop()
+            #     print(f" Returning Existing Job ID :{job.id}")
+            #     return job.id
+            print(f"File {file_name} already present in folder id {folder_id}")
         else:
             info = self.trigger_analysis_for_upload_id(
-                upload_id=upload_id, folder_id=folder_id, group_name=group_name
+                upload_id=upload_id, folder_id=folder_id
             )
             print(f"Computed new Job ID is :{info.message}")
             return info.message
 
     # trigger_analysis_for_url_upload_package(
     #     file_download_url='https://github.com/dineshr93/pageres/archive/refs/heads/master.zip', file_name='pageres.zip', branch_name='', folder_id=1)
 
@@ -1113,28 +1312,33 @@
         """trigger_analysis_for_git_upload_package(git_url: str, branch_name: str, folder_id: int)"""
         if not self.check_url_exists(git_url):
             print(f"git url {git_url} is malformed")
 
         file_name = git_url.split("/").pop()
         print(file_name)
 
-        uploads: List[Upload] = self.get_all_uploads_based_on(
+        uploads: List[Upload] = self.get_all_uploads_based_on_common_assignee(
             folder_id=folder_id,
             is_recursive=True,
             search_pattern_key="",
             upload_status=ClearingStatus.Open,
-            assignee="",
+            # assignee="",
             since_yyyy_mm_dd="",
             page=1,
             limit=1000,
-            group_name=self.group_name,
+            # group_name=self.group_name,
         )
 
-        upload_id = [u.id for u in uploads if file_name == u.uploadname]
-        size = len(upload_id)
+        # if folder is empty uploads will be None
+        size = 0
+        if uploads == None:
+            size = 0
+        else:
+            upload_id = [u.id for u in uploads if file_name == u.uploadname]
+            size = len(upload_id)
         is_present_uploadID = False
         if size > 1:
             is_present_uploadID = True
             print(f"{size} no of duplicates are there with ids {upload_id}")
             print(
                 "exiting.. please comeback after deleting duplicates via delete_uploads_by_upload_id(upload_id=upload_id, group_name=group_name)"
             )
@@ -1144,33 +1348,41 @@
             upload_id = upload_id[0]
         else:
             # no upload_id is there
             upload_id = self.get_upload_id_by_giturl_package_upload(
                 git_url=git_url,
                 branch_name=branch_name,
                 upload_name=file_name,
-                folder_id=1,
+                folder_id=folder_id,
                 upload_desc="",
                 visibility=Public.public,
-                group_name=self.group_name,
+                # group_name=self.group_name,
             )
 
         if is_present_uploadID:
-            jobs: List[Job] = [
-                j for j in self.get_all_jobs(self.group_name) if j.uploadId == upload_id
-            ]
-
-            if len(jobs) >= 1:
-                print(f"Multiple jobs exists for same upload_id: {upload_id}")
-                job = jobs.pop()
-                print(f" Returning Existing Job ID :{job.id}")
-                return job.id
+            # get_all_jobs() is very slow because of huge size so just returning message
+            # jobs: List[Job] = [
+            #     j for j in self.get_all_jobs() if j.uploadId == upload_id
+            # ]
+
+            # if len(jobs) >= 1:
+            #     print(f"Multiple jobs exists for same upload_id: {upload_id}")
+            #     job = jobs.pop()
+            #     print(f" Returning Existing Job ID :{job.id}")
+            #     return job.id
+            # else:
+            #     job = jobs.pop()
+            #     print(f" Returning Existing Job ID :{job.id}")
+            #     return job.id
+            print(f"File {file_name} already present in folder id {folder_id}")
         else:
             info = self.trigger_analysis_for_upload_id(
-                upload_id=upload_id, folder_id=folder_id, group_name=self.group_name
+                upload_id=upload_id,
+                folder_id=folder_id,
+                # group_name=self.group_name
             )
             print(f"Computed new Job ID is :{info.message}")
             return info.message
 
     # trigger_analysis_for_git_upload_package(
     #     git_url='https://github.com/dineshr93/pageres', branch_name='master', folder_id=1)
```

### Comparing `easy_fossy-2.0.9/easy_fossy/models.py` & `easy_fossy-2.1.0/easy_fossy/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,633 +10,621 @@
 
 from pydantic import BaseModel, Field, SecretStr, constr
 
 
 class LicenseDecider(BaseModel):
     nomos_monk: Optional[bool] = Field(
         None,
-        description='Scanners matches if all Nomos findings are within the Monk findings.',
+        description="Scanners matches if all Nomos findings are within the Monk findings.",
     )
     bulk_reused: Optional[bool] = Field(
-        None, description='Bulk phrases from reused packages.'
+        None, description="Bulk phrases from reused packages."
     )
     new_scanner: Optional[bool] = Field(
         None,
-        description='New scanner results, i.e., decisions were marked as work in progress if new scanner finds additional licenses.',
+        description="New scanner results, i.e., decisions were marked as work in progress if new scanner finds additional licenses.",
     )
     ojo_decider: Optional[bool] = Field(
         None,
-        description='Scanners matches if Ojo or REUSE.Software findings are no contradiction with other findings.',
+        description="Scanners matches if Ojo or REUSE.Software findings are no contradiction with other findings.",
     )
 
 
 class ClearingStatus(Enum):
-    Open = 'Open'
-    InProgress = 'InProgress'
-    Closed = 'Closed'
-    Rejected = 'Rejected'
+    Open = "Open"
+    InProgress = "InProgress"
+    Closed = "Closed"
+    Rejected = "Rejected"
 
 
 class UploadSummary(BaseModel):
-    id: Optional[int] = Field(None, description='Upload id of the upload.')
-    uploadName: Optional[str] = Field(
-        None, description='Display name of the upload.')
-    assignee: Optional[int] = Field(
-        None, description='assignee id of the upload.')
+    id: Optional[int] = Field(None, description="Upload id of the upload.")
+    uploadName: Optional[str] = Field(None, description="Display name of the upload.")
+    assignee: Optional[int] = Field(None, description="assignee id of the upload.")
     mainLicense: Optional[str] = Field(
-        None, description='Main license selected on the upload.'
+        None, description="Main license selected on the upload."
     )
     uniqueLicenses: Optional[int] = Field(
-        None, description='No. of unique licenses found.'
+        None, description="No. of unique licenses found."
     )
     totalLicenses: Optional[int] = Field(
-        None, description='Total no. of licenses found.'
+        None, description="Total no. of licenses found."
     )
     uniqueConcludedLicenses: Optional[int] = Field(
-        None, description='Unique licenses concluded.'
+        None, description="Unique licenses concluded."
     )
     totalConcludedLicenses: Optional[int] = Field(
-        None, description='Total concluded licenses.'
+        None, description="Total concluded licenses."
     )
     filesToBeCleared: Optional[int] = Field(
-        None, description='Files without clearing decisions.'
+        None, description="Files without clearing decisions."
     )
     filesCleared: Optional[int] = Field(
-        None, description='Files with clearing decisions.'
+        None, description="Files with clearing decisions."
     )
     clearingStatus: Optional[ClearingStatus] = Field(
-        None, description='Upload is clearing status.'
+        None, description="Upload is clearing status."
     )
     copyrightCount: Optional[int] = Field(
-        None, description='No. of copyrights found in the upload.'
+        None, description="No. of copyrights found in the upload."
     )
 
 
 class Status(Enum):
-    Completed = 'Completed'
-    Failed = 'Failed'
-    Queued = 'Queued'
-    Processing = 'Processing'
+    Completed = "Completed"
+    Failed = "Failed"
+    Queued = "Queued"
+    Processing = "Processing"
 
 
 class Job(BaseModel):
-    id: Optional[int] = Field(None, description='ID of the job')
-    name: Optional[str] = Field(None, description='Name of the job')
-    queueDate: Optional[str] = Field(
-        None, description='When the job was queued')
+    id: Optional[int] = Field(None, description="ID of the job")
+    name: Optional[str] = Field(None, description="Name of the job")
+    queueDate: Optional[str] = Field(None, description="When the job was queued")
     uploadId: Optional[int] = Field(
-        None, description='Upload for which the job was scheduled'
+        None, description="Upload for which the job was scheduled"
     )
-    userId: Optional[int] = Field(
-        None, description='User who scheduled the job')
+    userId: Optional[int] = Field(None, description="User who scheduled the job")
     groupId: Optional[int] = Field(
-        None, description='Group under which the job was scheduled'
+        None, description="Group under which the job was scheduled"
     )
-    eta: Optional[int] = Field(
-        None, description='ETA of job to finish in seconds')
+    eta: Optional[int] = Field(None, description="ETA of job to finish in seconds")
     status: Optional[Status] = Field(
-        None, description='Denotes the current status of the job in the queue'
+        None, description="Denotes the current status of the job in the queue"
     )
 
 
 class Type(Enum):
-    INFO = 'INFO'
-    ERROR = 'ERROR'
+    INFO = "INFO"
+    ERROR = "ERROR"
 
 
 class Info(BaseModel):
-    code: Optional[int] = Field(
-        None, description='HTTP status code', example=200)
-    message: Optional[str] = Field(None, description='Message in the info')
+    code: Optional[int] = Field(None, description="HTTP status code", example=200)
+    message: Optional[str] = Field(None, description="Message in the info")
     type: Optional[Type] = Field(
-        None, description='Denotes if info was created on error'
+        None, description="Denotes if info was created on error"
+    )
+
+
+class Copyright(BaseModel):
+    content: Optional[str] = Field(
+        None, description="actual copyright", example="copyright (c) Dinesh Ravi"
+    )
+    hash: Optional[str] = Field(None, description="hash value of copyright")
+    count: Optional[int] = Field(
+        None, description="No. of files with same copyrights found in the package."
     )
 
 
 class AccessLevel(Enum):
-    none = 'none'
-    read_only = 'read_only'
-    clearing_admin = 'clearing_admin'
-    read_write = 'read_write'
-    admin = 'admin'
+    none = "none"
+    read_only = "read_only"
+    clearing_admin = "clearing_admin"
+    read_write = "read_write"
+    admin = "admin"
 
 
 class Analysis(BaseModel):
     bucket: Optional[bool] = Field(
-        None, description='Should bucket analysis be run on this upload'
+        None, description="Should bucket analysis be run on this upload"
     )
     copyright_email_author: Optional[bool] = Field(
         None,
-        description='Should Copyright/Email/URL/Author Analysis be run on this upload.',
+        description="Should Copyright/Email/URL/Author Analysis be run on this upload.",
     )
     ecc: Optional[bool] = Field(
-        None, description='Should ECC Analysis be run on this upload.'
+        None, description="Should ECC Analysis be run on this upload."
     )
     keyword: Optional[bool] = Field(
-        None, description='Should keyword Analysis be run on this upload.'
+        None, description="Should keyword Analysis be run on this upload."
     )
     mime: Optional[bool] = Field(
-        None, description='Should MIME Analysis be run on this upload.'
+        None, description="Should MIME Analysis be run on this upload."
     )
     monk: Optional[bool] = Field(
-        None, description='Should Monk Analysis be run on this upload.'
+        None, description="Should Monk Analysis be run on this upload."
     )
     nomos: Optional[bool] = Field(
-        None, description='Should Nomos Analysis be run on this upload.'
+        None, description="Should Nomos Analysis be run on this upload."
     )
     ojo: Optional[bool] = Field(
-        None, description='Should OJO Analysis be run on this upload.'
+        None, description="Should OJO Analysis be run on this upload."
     )
     package: Optional[bool] = Field(
-        None, description='Should Package Analysis be run on this upload.'
+        None, description="Should Package Analysis be run on this upload."
     )
     reso: Optional[bool] = Field(
-        None, description='Should REUSE.Software Analysis be run on this upload.'
+        None, description="Should REUSE.Software Analysis be run on this upload."
     )
 
 
 class Reuser(BaseModel):
-    reuse_upload: Optional[int] = Field(
-        None, description='The UploadID to reuse.')
-    reuse_group: str = Field(..., description='The group of the reused upload')
+    reuse_upload: Optional[int] = Field(None, description="The UploadID to reuse.")
+    reuse_group: str = Field(..., description="The group of the reused upload")
     reuse_main: Optional[bool] = Field(
-        None, description='Copy the main license from reused package?'
+        None, description="Copy the main license from reused package?"
     )
     reuse_enhanced: Optional[bool] = Field(
-        None, description='Run enhanced reuser with diff tool (slow)'
+        None, description="Run enhanced reuser with diff tool (slow)"
     )
     reuse_report: Optional[bool] = Field(
-        None, description='Copy all report configuration from conf page.'
+        None, description="Copy all report configuration from conf page."
     )
     reuse_copyright: Optional[bool] = Field(
-        None, description='Copy the copyright deactivation and edits.'
+        None, description="Copy the copyright deactivation and edits."
     )
 
 
 class Folder(BaseModel):
-    id: Optional[int] = Field(None, description='Id of the folder.')
-    name: Optional[str] = Field(None, description='Name of the folder.')
-    description: Optional[str] = Field(
-        None, description='Description of the folder.')
+    id: Optional[int] = Field(None, description="Id of the folder.")
+    name: Optional[str] = Field(None, description="Name of the folder.")
+    description: Optional[str] = Field(None, description="Description of the folder.")
     parent: Optional[int] = Field(
-        None, description='Id of the parent folder (if any, null otherwise).'
+        None, description="Id of the parent folder (if any, null otherwise)."
     )
 
 
 class TokenScope(Enum):
-    read = 'read'
-    write = 'write'
+    read = "read"
+    write = "write"
 
 
 class TokenRequest(BaseModel):
-    username: str = Field(..., description='Username of the login user.')
+    username: str = Field(..., description="Username of the login user.")
     password: SecretStr = Field(
-        ..., description='Password of the user trying to login.'
+        ..., description="Password of the user trying to login."
     )
     token_name: constr(max_length=40) = Field(
-        ..., description='Friendly name of the token'
+        ..., description="Friendly name of the token"
     )
-    token_scope: TokenScope = Field(..., description='The scope of the token.')
+    token_scope: TokenScope = Field(..., description="The scope of the token.")
     token_expire: date = Field(
-        ..., description='Date when the token must expire (default max 30 days).'
+        ..., description="Date when the token must expire (default max 30 days)."
     )
 
 
 class VcsType(Enum):
-    svn = 'svn'
-    git = 'git'
+    svn = "svn"
+    git = "git"
 
 
 class VcsUpload(BaseModel):
-    vcsType: VcsType = Field(..., description='VCS type')
-    vcsUrl: str = Field(..., description='URL of the repository')
+    vcsType: VcsType = Field(..., description="VCS type")
+    vcsUrl: str = Field(..., description="URL of the repository")
     vcsBranch: Optional[str] = Field(
-        None, description='Branch to checkout for analysis (for Git only)'
+        None, description="Branch to checkout for analysis (for Git only)"
     )
-    vcsName: Optional[str] = Field(
-        None, description='Display name of the upload')
-    vcsUsername: Optional[str] = Field(
-        None, description='Username for the VCS')
-    vcsPassword: Optional[str] = Field(
-        None, description='Password for the VCS')
+    vcsName: Optional[str] = Field(None, description="Display name of the upload")
+    vcsUsername: Optional[str] = Field(None, description="Username for the VCS")
+    vcsPassword: Optional[str] = Field(None, description="Password for the VCS")
 
 
 class UrlUpload(BaseModel):
-    url: str = Field(..., description='URL for file/folder to be uploaded')
+    url: str = Field(..., description="URL for file/folder to be uploaded")
     name: Optional[str] = Field(
-        None, description='Viewable name for this file or directory'
+        None, description="Viewable name for this file or directory"
     )
     accept: Optional[str] = Field(
         None,
-        description='Comma-separated lists of file name suffixes or patterns to accpet\n',
+        description="Comma-separated lists of file name suffixes or patterns to accpet\n",
     )
     reject: Optional[str] = Field(
         None,
-        description='Comma-separated lists of file name suffixes or patterns to reject\n',
+        description="Comma-separated lists of file name suffixes or patterns to reject\n",
     )
     maxRecursionDepth: Optional[int] = Field(
-        None, description='Maximum recursion depth for folders (0 for infinite)'
+        None, description="Maximum recursion depth for folders (0 for infinite)"
     )
 
 
 class ServerUpload(BaseModel):
     path: str = Field(
-        ..., description='File path to be uploaded (reccursive, support *)'
+        ..., description="File path to be uploaded (reccursive, support *)"
     )
     name: Optional[str] = Field(
-        None, description='Viewable name for this file or directory'
+        None, description="Viewable name for this file or directory"
     )
 
 
 class Hash(BaseModel):
     sha1: Optional[str] = Field(
         None,
-        description='SHA1 checksum of the file',
-        example='81fe8bfe87576c3ecb22426f8e57847382917acf',
+        description="SHA1 checksum of the file",
+        example="81fe8bfe87576c3ecb22426f8e57847382917acf",
     )
     md5: Optional[str] = Field(
         None,
-        description='MD5 checksum of the file',
-        example='e2fc714c4727ee9395f324cd2e7f331f',
+        description="MD5 checksum of the file",
+        example="e2fc714c4727ee9395f324cd2e7f331f",
     )
     sha256: Optional[str] = Field(
         None,
-        description='SHA256 checksum of the file',
-        example='88d4266fd4e6338d13b845fcf289579d209c897823b9217da3e161936f031589',
+        description="SHA256 checksum of the file",
+        example="88d4266fd4e6338d13b845fcf289579d209c897823b9217da3e161936f031589",
     )
-    size: Optional[int] = Field(None, description='Size of the file in bytes')
+    size: Optional[int] = Field(None, description="Size of the file in bytes")
 
 
 class Message(Enum):
-    Not_found = 'Not found'
-    Invalid_keys = 'Invalid keys'
+    Not_found = "Not found"
+    Invalid_keys = "Invalid keys"
 
 
 class Findings(BaseModel):
     scanner: Optional[List[str]] = Field(
-        None, description='Licenses finding by scanner', example=['MIT', 'BSD-3-Clause']
+        None, description="Licenses finding by scanner", example=["MIT", "BSD-3-Clause"]
     )
     conclusion: Optional[List[str]] = Field(
         None,
-        description='Licenses concluded by user or main license in case of package\n',
-        example=['MIT', 'GPL-2.0'],
+        description="Licenses concluded by user or main license in case of package\n",
+        example=["MIT", "GPL-2.0"],
     )
     copyright: Optional[List[str]] = Field(
         None,
-        description='Copyright findings for the file\n',
+        description="Copyright findings for the file\n",
         example=[
-            'Copyright (C) 2017-2020 Free Software Foundation, Inc.',
-            'Copyright (C) 1991-2020 Free Software Foundation, Inc.',
+            "Copyright (C) 2017-2020 Free Software Foundation, Inc.",
+            "Copyright (C) 1991-2020 Free Software Foundation, Inc.",
         ],
     )
 
 
 class License(BaseModel):
-    shortName: Optional[str] = Field(
-        None, description='Short name', example='MIT')
+    shortName: Optional[str] = Field(None, description="Short name", example="MIT")
     fullName: Optional[str] = Field(
-        None, description='Full name', example='MIT License'
+        None, description="Full name", example="MIT License"
     )
     text: Optional[str] = Field(
         None,
-        description='License text',
-        example='MIT License Copyright (c) <year> <copyright holders> ...',
+        description="License text",
+        example="MIT License Copyright (c) <year> <copyright holders> ...",
     )
     url: Optional[str] = Field(
         None,
-        description='URL of the license text',
-        example='https://opensource.org/licenses/MIT',
+        description="URL of the license text",
+        example="https://opensource.org/licenses/MIT",
     )
-    risk: Optional[int] = Field(None, description='Risk level', example=3)
-    isCandidate: Optional[bool] = Field(
-        None, description='Is the license a candidate?')
+    risk: Optional[int] = Field(None, description="Risk level", example=3)
+    isCandidate: Optional[bool] = Field(None, description="Is the license a candidate?")
 
 
 class Group(BaseModel):
-    id: Optional[int] = Field(None, description='Id key', example=126)
+    id: Optional[int] = Field(None, description="Id key", example=126)
     name: Optional[str] = Field(
-        None, description='Name of a group', example='Main group'
+        None, description="Name of a group", example="Main group"
     )
 
 
 class Classification(Enum):
-    green = 'green'
-    white = 'white'
-    yellow = 'yellow'
-    red = 'red'
+    green = "green"
+    white = "white"
+    yellow = "yellow"
+    red = "red"
 
 
 class Obligation(BaseModel):
-    id: Optional[int] = Field(None, description='Id key', example=126)
+    id: Optional[int] = Field(None, description="Id key", example=126)
     topic: Optional[str] = Field(
-        None, description='Obligation topic', example='Should preserve notice'
+        None, description="Obligation topic", example="Should preserve notice"
     )
     type: Optional[str] = Field(
-        None, description='Type of obligation', example='Obligation'
+        None, description="Type of obligation", example="Obligation"
     )
     text: Optional[str] = Field(
         None,
-        description='Obligation text',
-        example='All notices from the package should be preserved.',
+        description="Obligation text",
+        example="All notices from the package should be preserved.",
     )
     classification: Optional[Classification] = Field(
         None,
-        description='Level of attention this obligation should raise in the clearing process\n',
+        description="Level of attention this obligation should raise in the clearing process\n",
     )
     comment: Optional[str] = Field(
         None,
-        description='Comments for the obligation',
-        example='Please respect the obligation',
+        description="Comments for the obligation",
+        example="Please respect the obligation",
     )
 
 
 class License1(BaseModel):
-    name: Optional[str] = Field(None, description='Name of license')
-    url: Optional[str] = Field(None, description='Link to license')
+    name: Optional[str] = Field(None, description="Name of license")
+    url: Optional[str] = Field(None, description="Link to license")
 
 
 class ApiInfo(BaseModel):
-    name: Optional[str] = Field(None, description='Name of the API service')
-    description: Optional[str] = Field(
-        None, description='Additional information')
+    name: Optional[str] = Field(None, description="Name of the API service")
+    description: Optional[str] = Field(None, description="Additional information")
     version: Optional[str] = Field(
-        None, description='Current API version as per documentation'
+        None, description="Current API version as per documentation"
     )
-    security: Optional[List[str]] = Field(
-        None, description='Security methods allowed')
-    contact: Optional[str] = Field(
-        None, description='Contact email from API docs')
-    license: Optional[License1] = Field(None, description='Licensing of API')
+    security: Optional[List[str]] = Field(None, description="Security methods allowed")
+    contact: Optional[str] = Field(None, description="Contact email from API docs")
+    license: Optional[License1] = Field(None, description="Licensing of API")
 
 
 class Status1(Enum):
-    OK = 'OK'
-    WARN = 'WARN'
-    ERROR = 'ERROR'
+    OK = "OK"
+    WARN = "WARN"
+    ERROR = "ERROR"
 
 
 class Status2(Enum):
-    OK = 'OK'
-    ERROR = 'ERROR'
+    OK = "OK"
+    ERROR = "ERROR"
 
 
 class Scheduler(BaseModel):
-    status: Optional[Status2] = Field(
-        None, description='Health status of scheduler')
+    status: Optional[Status2] = Field(None, description="Health status of scheduler")
 
 
 class Status3(Enum):
-    OK = 'OK'
-    ERROR = 'ERROR'
+    OK = "OK"
+    ERROR = "ERROR"
 
 
 class Db(BaseModel):
     status: Optional[Status3] = Field(
-        None, description='Health status of DB connection'
+        None, description="Health status of DB connection"
     )
 
 
 class HeathInfo(BaseModel):
-    status: Optional[Status1] = Field(None, description='Status of service')
-    scheduler: Optional[Scheduler] = Field(
-        None, description='Scheduler information')
-    db: Optional[Db] = Field(None, description='DB connection status')
+    status: Optional[Status1] = Field(None, description="Status of service")
+    scheduler: Optional[Scheduler] = Field(None, description="Scheduler information")
+    db: Optional[Db] = Field(None, description="DB connection status")
 
 
 class TokensPostResponse(BaseModel):
     header: Optional[str] = None
 
 
 class Status4(Enum):
-    Open = 'Open'
-    InProgress = 'InProgress'
-    Closed = 'Closed'
-    Rejected = 'Rejected'
+    Open = "Open"
+    InProgress = "InProgress"
+    Closed = "Closed"
+    Rejected = "Rejected"
 
 
 class Status5(Enum):
-    Open = 'Open'
-    InProgress = 'InProgress'
-    Closed = 'Closed'
-    Rejected = 'Rejected'
+    Open = "Open"
+    InProgress = "InProgress"
+    Closed = "Closed"
+    Rejected = "Rejected"
 
 
 class UploadType(Enum):
-    vcs = 'vcs'
-    url = 'url'
-    server = 'server'
+    vcs = "vcs"
+    url = "url"
+    server = "server"
 
 
 class UploadsPostRequest(BaseModel):
     __root__: Union[VcsUpload, UrlUpload, ServerUpload]
 
 
 class UploadsPostRequest1(BaseModel):
     fileInput: Optional[bytes] = None
 
 
 class Public(Enum):
-    private = 'private'
-    protected = 'protected'
-    public = 'public'
+    private = "private"
+    protected = "protected"
+    public = "public"
 
 
 class UploadType1(Enum):
-    vcs = 'vcs'
-    url = 'url'
-    server = 'server'
+    vcs = "vcs"
+    url = "url"
+    server = "server"
 
 
 class UploadType2(Enum):
-    vcs = 'vcs'
-    url = 'url'
-    server = 'server'
+    vcs = "vcs"
+    url = "url"
+    server = "server"
 
 
 class AgentEnum(Enum):
-    nomos = 'nomos'
-    monk = 'monk'
-    ninka = 'ninka'
-    ojo = 'ojo'
-    reportImport = 'reportImport'
-    reso = 'reso'
+    nomos = "nomos"
+    monk = "monk"
+    ninka = "ninka"
+    ojo = "ojo"
+    reportImport = "reportImport"
+    reso = "reso"
 
 
 class Agent(Enum):
-    nomos = 'nomos'
-    monk = 'monk'
-    ninka = 'ninka'
-    ojo = 'ojo'
-    reportImport = 'reportImport'
-    reso = 'reso'
+    nomos = "nomos"
+    monk = "monk"
+    ninka = "ninka"
+    ojo = "ojo"
+    reportImport = "reportImport"
+    reso = "reso"
 
 
 class SearchType(Enum):
-    directory = 'directory'
-    containers = 'containers'
-    allfiles = 'allfiles'
+    directory = "directory"
+    containers = "containers"
+    allfiles = "allfiles"
 
 
 class SearchType1(Enum):
-    directory = 'directory'
-    containers = 'containers'
-    allfiles = 'allfiles'
+    directory = "directory"
+    containers = "containers"
+    allfiles = "allfiles"
 
 
 class SearchType2(Enum):
-    directory = 'directory'
-    containers = 'containers'
-    allfiles = 'allfiles'
+    directory = "directory"
+    containers = "containers"
+    allfiles = "allfiles"
 
 
 class Action(Enum):
-    copy = 'copy'
-    move = 'move'
+    copy = "copy"
+    move = "move"
 
 
 class Action1(Enum):
-    copy = 'copy'
-    move = 'move'
+    copy = "copy"
+    move = "move"
 
 
 class ReportFormat(Enum):
-    dep5 = 'dep5'
-    spdx2 = 'spdx2'
-    spdx2tv = 'spdx2tv'
-    readmeoss = 'readmeoss'
-    unifiedreport = 'unifiedreport'
+    dep5 = "dep5"
+    spdx2 = "spdx2"
+    spdx2tv = "spdx2tv"
+    readmeoss = "readmeoss"
+    unifiedreport = "unifiedreport"
 
 
 class ReportFormat1(Enum):
-    dep5 = 'dep5'
-    spdx2 = 'spdx2'
-    spdx2tv = 'spdx2tv'
-    readmeoss = 'readmeoss'
-    unifiedreport = 'unifiedreport'
+    dep5 = "dep5"
+    spdx2 = "spdx2"
+    spdx2tv = "spdx2tv"
+    readmeoss = "readmeoss"
+    unifiedreport = "unifiedreport"
 
 
 class ReportFormat2(Enum):
-    dep5 = 'dep5'
-    spdx2 = 'spdx2'
-    spdx2tv = 'spdx2tv'
-    readmeoss = 'readmeoss'
-    unifiedreport = 'unifiedreport'
+    dep5 = "dep5"
+    spdx2 = "spdx2"
+    spdx2tv = "spdx2tv"
+    readmeoss = "readmeoss"
+    unifiedreport = "unifiedreport"
 
 
 class Kind(Enum):
-    candidate = 'candidate'
-    main = 'main'
-    all = 'all'
+    candidate = "candidate"
+    main = "main"
+    all = "all"
 
 
 class LicenseGetResponse(License):
-    id: Optional[int] = Field(None, description='Id key', example=125)
+    id: Optional[int] = Field(None, description="Id key", example=125)
 
 
 class Kind1(Enum):
-    candidate = 'candidate'
-    main = 'main'
-    all = 'all'
+    candidate = "candidate"
+    main = "main"
+    all = "all"
 
 
 class LicensePostRequest(License):
     mergeRequest: Optional[bool] = Field(
-        False, description='Open a merge request for candidate license?'
+        False, description="Open a merge request for candidate license?"
     )
 
 
 class LicenseShortnameGetResponse(License):
-    id: Optional[int] = Field(None, description='Id key', example=125)
+    id: Optional[int] = Field(None, description="Id key", example=125)
     obligations: Optional[List[Obligation]] = Field(
-        None, description='Obligations associated with the license'
+        None, description="Obligations associated with the license"
     )
 
 
 class LicenseShortnamePatchRequest(BaseModel):
     fullName: Optional[str] = Field(
-        None, description='New fullname', example='Updated license name'
+        None, description="New fullname", example="Updated license name"
     )
     text: Optional[str] = Field(
         None,
-        description='New license text',
-        example='Updated and corrected license text',
+        description="New license text",
+        example="Updated and corrected license text",
     )
     url: Optional[str] = Field(
         None,
-        description='New URL for license',
-        example='https://opensource.org/licenses/MIT',
+        description="New URL for license",
+        example="https://opensource.org/licenses/MIT",
     )
-    risk: Optional[int] = Field(None, description='New risk value', example=2)
+    risk: Optional[int] = Field(None, description="New risk value", example=2)
 
 
 class ScanOptions(BaseModel):
     analysis: Optional[Analysis] = None
     decider: Optional[LicenseDecider] = None
     reuse: Optional[Reuser] = None
 
 
 class Upload(BaseModel):
     folderid: Optional[int] = Field(
-        None, description='The folder id, where the upload is located'
+        None, description="The folder id, where the upload is located"
     )
     foldername: Optional[str] = Field(
-        None, description='The name of the folder where the upload is located'
+        None, description="The name of the folder where the upload is located"
     )
-    id: Optional[int] = Field(None, description='Upload id of the upload.')
-    description: Optional[str] = Field(
-        None, description='Description of the upload.')
-    uploadname: Optional[str] = Field(
-        None, description='Display name of the upload.')
+    id: Optional[int] = Field(None, description="Upload id of the upload.")
+    description: Optional[str] = Field(None, description="Description of the upload.")
+    uploadname: Optional[str] = Field(None, description="Display name of the upload.")
     uploaddate: Optional[str] = Field(
-        None, description='Date, when the file was uploaded.'
+        None, description="Date, when the file was uploaded."
     )
-    assignee: Optional[int] = Field(
-        None, description='assignee id of the upload.')
+    assignee: Optional[int] = Field(None, description="assignee id of the upload.")
     hash: Optional[Hash] = None
 
 
 class User(BaseModel):
-    id: int = Field(..., description='ID of the user')
-    name: str = Field(..., description='Unique username')
-    description: str = Field(..., description='Description of the user')
+    id: int = Field(..., description="ID of the user")
+    name: str = Field(..., description="Unique username")
+    description: str = Field(..., description="Description of the user")
     email: Optional[str] = Field(
-        None, description='Email of the user, needs to be unique and is required'
+        None, description="Email of the user, needs to be unique and is required"
     )
     accessLevel: Optional[AccessLevel] = None
     rootFolderId: Optional[float] = Field(
-        None, description='root folder id of the user'
+        None, description="root folder id of the user"
     )
-    emailNotification: Optional[bool] = Field(
-        None, description='enable email notification when upload scan completes'
+    emailNotification: Optional[str] = Field(
+        None, description="enable email notification when upload scan completes"
     )
     agents: Optional[Analysis] = None
 
 
 class UploadLicense(BaseModel):
     filePath: Optional[str] = Field(
-        None, description='Relative file path', example='path/to/LICENSE'
+        None, description="Relative file path", example="path/to/LICENSE"
     )
     findings: Optional[Findings] = None
 
 
 class UploadLicenses(BaseModel):
     __root__: List[UploadLicense]
 
 
 class File(BaseModel):
     hash: Hash
     findings: Optional[Findings] = None
     uploads: Optional[List[int]] = Field(
-        None, description='Upload ID if the file was uploaded as a package'
+        None, description="Upload ID if the file was uploaded as a package"
     )
     message: Optional[Message] = Field(
         None,
-        description='Message in case provided hash not found or error',
-        example='Not found',
+        description="Message in case provided hash not found or error",
+        example="Not found",
     )
 
 
 class SearchResults(BaseModel):
     upload: Optional[Upload] = None
-    uploadTreeId: Optional[int] = Field(None, description='Upload tree ID')
-    filename: Optional[str] = Field(
-        None, description='Filename of the treeItem')
+    uploadTreeId: Optional[int] = Field(None, description="Upload tree ID")
+    filename: Optional[str] = Field(None, description="Filename of the treeItem")
```

### Comparing `easy_fossy-2.0.9/pyproject.toml` & `easy_fossy-2.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_fossy"
-version = "2.0.9"
+version = "2.1.0"
 description = "fossology API wrapper in python 3.10"
 authors = ["dinesh_ravi"]
 license = "MIT License"
 readme = "README.md"
 
 [tool.poetry.scripts]
 easy_fossy = 'easy_fossy:easy_fossy'
```

### Comparing `easy_fossy-2.0.9/PKG-INFO` & `easy_fossy-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fossy
-Version: 2.0.9
+Version: 2.1.0
 Summary: fossology API wrapper in python 3.10
 License: MIT
 Author: dinesh_ravi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

