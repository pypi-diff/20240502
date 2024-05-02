# Comparing `tmp/increff_runner-3.1.7-py3-none-any.whl.zip` & `tmp/increff_runner-3.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13191 bytes, number of entries: 16
+Zip file size: 13184 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-05 05:14 increff_runner/__init__.py
--rw-r--r--  2.0 unx     9762 b- defN 24-Mar-29 08:33 increff_runner/function.py
+-rw-r--r--  2.0 unx     9762 b- defN 24-Apr-30 04:29 increff_runner/function.py
 -rw-r--r--  2.0 unx     4143 b- defN 24-Feb-22 04:41 increff_runner/commons/algo_block_downloader.py
--rw-r--r--  2.0 unx     2833 b- defN 24-Apr-02 04:36 increff_runner/commons/callback_helper.py
+-rw-r--r--  2.0 unx     2817 b- defN 24-May-02 06:39 increff_runner/commons/callback_helper.py
 -rw-r--r--  2.0 unx      351 b- defN 24-Feb-15 07:21 increff_runner/commons/constants.py
--rw-r--r--  2.0 unx     3385 b- defN 24-Mar-29 07:29 increff_runner/commons/db_helper.py
+-rw-r--r--  2.0 unx     3385 b- defN 24-Apr-30 04:29 increff_runner/commons/db_helper.py
 -rw-r--r--  2.0 unx      905 b- defN 24-Feb-22 04:41 increff_runner/commons/db_service.py
--rw-r--r--  2.0 unx      349 b- defN 24-Feb-22 10:18 increff_runner/commons/event_helper.py
--rw-r--r--  2.0 unx     8303 b- defN 24-Apr-02 04:36 increff_runner/commons/graphdb_helper.py
--rw-r--r--  2.0 unx     4120 b- defN 24-Apr-02 04:29 increff_runner/commons/mse_helper.py
+-rw-r--r--  2.0 unx      349 b- defN 24-Apr-30 04:29 increff_runner/commons/event_helper.py
+-rw-r--r--  2.0 unx     8303 b- defN 24-Apr-30 04:29 increff_runner/commons/graphdb_helper.py
+-rw-r--r--  2.0 unx     4177 b- defN 24-May-02 06:39 increff_runner/commons/mse_helper.py
 -rw-r--r--  2.0 unx      687 b- defN 24-Feb-22 04:41 increff_runner/commons/setup.py
 -rw-r--r--  2.0 unx     2104 b- defN 24-Feb-22 04:41 increff_runner/commons/utils.py
--rw-r--r--  2.0 unx      612 b- defN 24-Apr-02 04:37 increff_runner-3.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 04:37 increff_runner-3.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Apr-02 04:37 increff_runner-3.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1424 b- defN 24-Apr-02 04:37 increff_runner-3.1.7.dist-info/RECORD
-16 files, 39085 bytes uncompressed, 10797 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx      612 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1424 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/RECORD
+16 files, 39126 bytes uncompressed, 10790 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: increff_runner/commons/setup.py
 Comment: 
 
 Filename: increff_runner/commons/utils.py
 Comment: 
 
-Filename: increff_runner-3.1.7.dist-info/METADATA
+Filename: increff_runner-3.1.8.dist-info/METADATA
 Comment: 
 
-Filename: increff_runner-3.1.7.dist-info/WHEEL
+Filename: increff_runner-3.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: increff_runner-3.1.7.dist-info/top_level.txt
+Filename: increff_runner-3.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: increff_runner-3.1.7.dist-info/RECORD
+Filename: increff_runner-3.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## increff_runner/commons/callback_helper.py

```diff
@@ -54,16 +54,16 @@
     data = {"status": "FAILED", "taskId": task_id, "subtaskName":  node['parent_task'],"reason":str(error)}
 
     # TODO @jaynit to move this config at the client level
     headers = {
         "Content-Type": "application/json",
         "authUsername":"caas-user@increff.com",
         "authPassword":"caasuser@123",
-        "authdomainname":"irisx-qc",
-        "project_name":"adidas-or-distribution",
+        "authdomainname":"celio",
+        "project_name":"celio-ars",
         "Conection":"keep-alive"
     }
     add_info_logs(job["id"], f" failure message -> {str(data)}")
     job["webhook_status"] = 400
     update_job(job)
     
     # TODO @jaynit ensure that they are not moved to Success again #cr1_unni
```

## increff_runner/commons/mse_helper.py

```diff
@@ -12,25 +12,27 @@
     extra_blocks = [block for block in next_blocks if block != algo_name]
     for block in extra_blocks:
         del dag[block]
     return dag
 
 
 def create_algo_block_runner_data(
+    client,
     task_id,
     algo_name,
     level,
     block_identifier,
     app,
     app_id,
     masterUri,
     script_info,
     webHookUri,
 ):
     return {
+        "client": client,
         "task_id": task_id,
         "algo_name": algo_name,
         "level": level,
         "block_identifier": block_identifier,
         "app_name": app,
         "app_id": app_id,
         "masterUri": masterUri,
@@ -83,14 +85,15 @@
     #     all_levels = (
     #         [job["data"]["level"]] if job["data"]["level"] in all_levels else all_levels
     #     )
     #     for level in all_levels:
     for next_node in next_nodes:
         change_edge_between_task_nodes(node,next_node)
         data = create_algo_block_runner_data(
+            job["data"]["client"],
             job["data"]["task_id"],
             next_node['name'],
             next_node['level'],
             job["data"]["block_identifier"],
             job["data"]["app_name"],
             job["data"]["app_id"],
             job["data"]["masterUri"],
@@ -107,15 +110,15 @@
     if url == "":
         return
     data = {"status": "SUCCESS", "taskId": task_id, "subtaskName": algo_name,"reason":"Success"}
     headers = {
         "Content-Type": "application/json",
         "authUsername":"caas-user@increff.com",
         "authPassword":"caasuser@123",
-        "authdomainname":"irisx-qc",
-        "project_name":"adidas-or-distribution",
+        "authdomainname":"celio",
+        "project_name":"celio-ars",
         "Conection":"keep-alive"
     }
     add_info_logs(task_id, f"Hitting Success Callback on {url} with data {data} ")
     response = requests.put(url, headers=headers,params=data)
     if response.status_code!=200:
         add_error_logs(task_id, f"Failed to hit the callback with status code {response.text}")
```

## Comparing `increff_runner-3.1.7.dist-info/METADATA` & `increff_runner-3.1.8.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increff-runner
-Version: 3.1.7
+Version: 3.1.8
 Summary: Algo Runner For Increff CaaS
 Author: Jaynit Patel
 Author-email: jaynitpatel11062001@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytz ==2023.3.post1
 Requires-Dist: requests ==2.31.0
 Requires-Dist: azure-functions ==1.12.0
```

## Comparing `increff_runner-3.1.7.dist-info/RECORD` & `increff_runner-3.1.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 increff_runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 increff_runner/function.py,sha256=Kk2mSezi3ypvYkjbSrMtxXoO5qwc29uYHAoTk_-W_Yo,9762
 increff_runner/commons/algo_block_downloader.py,sha256=JSZLYpIuWhybRD13sHPu_05X4KoeMApa5qELLkqA9R4,4143
-increff_runner/commons/callback_helper.py,sha256=-kQdLxmp0kF5w5qhyeF96HliunM4pJLcet_L1LplBX8,2833
+increff_runner/commons/callback_helper.py,sha256=RjcgLjo4z3slHD9dH7lcoBhQ9ffzoMVoiVWOydd1Kc4,2817
 increff_runner/commons/constants.py,sha256=dJRawPQQduTe1BqN6SrLYYpzI5bVqS6AbuYwj6Qa6is,351
 increff_runner/commons/db_helper.py,sha256=NW4PMZwRM4s636nFrvLOfj7VkarS8EOc2MsZg1YLg2Y,3385
 increff_runner/commons/db_service.py,sha256=5PtU_AQCwm5FVmRXjJprysNoIy_vKt06vN1IlnxuH-c,905
 increff_runner/commons/event_helper.py,sha256=MN1XR6yielNYXLbLxi3uuiDyXZ-lmVKszL9DOL4swBY,349
 increff_runner/commons/graphdb_helper.py,sha256=a4sXvF1NwT2YMolyl2SnrMmmyO-FNhJ6GZrhuT8qXV0,8303
-increff_runner/commons/mse_helper.py,sha256=WMDGy9VQpnEu6QALY8Dcm3jeXgQWUtyGGBNCdIuav-s,4120
+increff_runner/commons/mse_helper.py,sha256=m2JNRs72goahs3s3OSwwWvsoP_SWjRbOPfW-MEBP4lA,4177
 increff_runner/commons/setup.py,sha256=iwg58X1DKaSP8hKlXLvH5OXSEW8N_UuRMDb2CocaAfY,687
 increff_runner/commons/utils.py,sha256=PUKWRMYzTTWK7pTK2S5DM0szru4zGmmVKfPpXhnmPUM,2104
-increff_runner-3.1.7.dist-info/METADATA,sha256=_h_ymd9akisrV8pW8ukcwiLnLBDJ_l97rtuDOQNr5kw,612
-increff_runner-3.1.7.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-increff_runner-3.1.7.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
-increff_runner-3.1.7.dist-info/RECORD,,
+increff_runner-3.1.8.dist-info/METADATA,sha256=ge510UqMaWe6zbnKUIXTtMhZ91rT_DRcGZPxH4hwNZo,612
+increff_runner-3.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+increff_runner-3.1.8.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
+increff_runner-3.1.8.dist-info/RECORD,,
```

