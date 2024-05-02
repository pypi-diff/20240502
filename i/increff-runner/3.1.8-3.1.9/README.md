# Comparing `tmp/increff_runner-3.1.8-py3-none-any.whl.zip` & `tmp/increff_runner-3.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 13184 bytes, number of entries: 16
+Zip file size: 13208 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-05 05:14 increff_runner/__init__.py
 -rw-r--r--  2.0 unx     9762 b- defN 24-Apr-30 04:29 increff_runner/function.py
 -rw-r--r--  2.0 unx     4143 b- defN 24-Feb-22 04:41 increff_runner/commons/algo_block_downloader.py
--rw-r--r--  2.0 unx     2817 b- defN 24-May-02 06:39 increff_runner/commons/callback_helper.py
+-rw-r--r--  2.0 unx     2909 b- defN 24-May-02 09:14 increff_runner/commons/callback_helper.py
 -rw-r--r--  2.0 unx      351 b- defN 24-Feb-15 07:21 increff_runner/commons/constants.py
 -rw-r--r--  2.0 unx     3385 b- defN 24-Apr-30 04:29 increff_runner/commons/db_helper.py
 -rw-r--r--  2.0 unx      905 b- defN 24-Feb-22 04:41 increff_runner/commons/db_service.py
 -rw-r--r--  2.0 unx      349 b- defN 24-Apr-30 04:29 increff_runner/commons/event_helper.py
 -rw-r--r--  2.0 unx     8303 b- defN 24-Apr-30 04:29 increff_runner/commons/graphdb_helper.py
 -rw-r--r--  2.0 unx     4177 b- defN 24-May-02 06:39 increff_runner/commons/mse_helper.py
 -rw-r--r--  2.0 unx      687 b- defN 24-Feb-22 04:41 increff_runner/commons/setup.py
 -rw-r--r--  2.0 unx     2104 b- defN 24-Feb-22 04:41 increff_runner/commons/utils.py
--rw-r--r--  2.0 unx      612 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1424 b- defN 24-May-02 06:42 increff_runner-3.1.8.dist-info/RECORD
-16 files, 39126 bytes uncompressed, 10790 bytes compressed:  72.4%
+-rw-r--r--  2.0 unx      612 b- defN 24-May-02 09:15 increff_runner-3.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 09:15 increff_runner-3.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-May-02 09:15 increff_runner-3.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1424 b- defN 24-May-02 09:15 increff_runner-3.1.9.dist-info/RECORD
+16 files, 39218 bytes uncompressed, 10814 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: increff_runner/commons/setup.py
 Comment: 
 
 Filename: increff_runner/commons/utils.py
 Comment: 
 
-Filename: increff_runner-3.1.8.dist-info/METADATA
+Filename: increff_runner-3.1.9.dist-info/METADATA
 Comment: 
 
-Filename: increff_runner-3.1.8.dist-info/WHEEL
+Filename: increff_runner-3.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: increff_runner-3.1.8.dist-info/top_level.txt
+Filename: increff_runner-3.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: increff_runner-3.1.8.dist-info/RECORD
+Filename: increff_runner-3.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## increff_runner/commons/callback_helper.py

```diff
@@ -47,14 +47,15 @@
     update_job(job)
     response = requests.post(url, data=json.dumps(body))
 
 
 def send_failure_webhook(url, task_id, error, job):
     # interim_task = get_interim_tasks(INTERIM_TASK_TABLE, task_id, job["data"]["algo_name"], job["data"]["level"])
     node = get_task_node(job["data"]["algo_name"],task_id,job["data"]["level"])
+    add_error_logs(job["id"], "Hitting Failure WebHook Callback with error -> "+str(error))
     data = {"status": "FAILED", "taskId": task_id, "subtaskName":  node['parent_task'],"reason":str(error)}
 
     # TODO @jaynit to move this config at the client level
     headers = {
         "Content-Type": "application/json",
         "authUsername":"caas-user@increff.com",
         "authPassword":"caasuser@123",
```

## Comparing `increff_runner-3.1.8.dist-info/METADATA` & `increff_runner-3.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increff-runner
-Version: 3.1.8
+Version: 3.1.9
 Summary: Algo Runner For Increff CaaS
 Author: Jaynit Patel
 Author-email: jaynitpatel11062001@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytz ==2023.3.post1
 Requires-Dist: requests ==2.31.0
 Requires-Dist: azure-functions ==1.12.0
```

## Comparing `increff_runner-3.1.8.dist-info/RECORD` & `increff_runner-3.1.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 increff_runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 increff_runner/function.py,sha256=Kk2mSezi3ypvYkjbSrMtxXoO5qwc29uYHAoTk_-W_Yo,9762
 increff_runner/commons/algo_block_downloader.py,sha256=JSZLYpIuWhybRD13sHPu_05X4KoeMApa5qELLkqA9R4,4143
-increff_runner/commons/callback_helper.py,sha256=RjcgLjo4z3slHD9dH7lcoBhQ9ffzoMVoiVWOydd1Kc4,2817
+increff_runner/commons/callback_helper.py,sha256=IJGZ_xyYZLXmC5CH6wTJshkYY6iLnn2gU9Dk4nsESOw,2909
 increff_runner/commons/constants.py,sha256=dJRawPQQduTe1BqN6SrLYYpzI5bVqS6AbuYwj6Qa6is,351
 increff_runner/commons/db_helper.py,sha256=NW4PMZwRM4s636nFrvLOfj7VkarS8EOc2MsZg1YLg2Y,3385
 increff_runner/commons/db_service.py,sha256=5PtU_AQCwm5FVmRXjJprysNoIy_vKt06vN1IlnxuH-c,905
 increff_runner/commons/event_helper.py,sha256=MN1XR6yielNYXLbLxi3uuiDyXZ-lmVKszL9DOL4swBY,349
 increff_runner/commons/graphdb_helper.py,sha256=a4sXvF1NwT2YMolyl2SnrMmmyO-FNhJ6GZrhuT8qXV0,8303
 increff_runner/commons/mse_helper.py,sha256=m2JNRs72goahs3s3OSwwWvsoP_SWjRbOPfW-MEBP4lA,4177
 increff_runner/commons/setup.py,sha256=iwg58X1DKaSP8hKlXLvH5OXSEW8N_UuRMDb2CocaAfY,687
 increff_runner/commons/utils.py,sha256=PUKWRMYzTTWK7pTK2S5DM0szru4zGmmVKfPpXhnmPUM,2104
-increff_runner-3.1.8.dist-info/METADATA,sha256=ge510UqMaWe6zbnKUIXTtMhZ91rT_DRcGZPxH4hwNZo,612
-increff_runner-3.1.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-increff_runner-3.1.8.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
-increff_runner-3.1.8.dist-info/RECORD,,
+increff_runner-3.1.9.dist-info/METADATA,sha256=rKaSTagEDUz5MUhIaKB6ETr6eGuqDYP74WzLXPi7TRg,612
+increff_runner-3.1.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+increff_runner-3.1.9.dist-info/top_level.txt,sha256=pL8Rxzd3TVe5jhZdPB1tmORoBiwmdtiDgfNAvJtCl1s,15
+increff_runner-3.1.9.dist-info/RECORD,,
```

