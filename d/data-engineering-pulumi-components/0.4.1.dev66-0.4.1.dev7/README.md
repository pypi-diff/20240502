# Comparing `tmp/data_engineering_pulumi_components-0.4.1.dev66.tar.gz` & `tmp/data-engineering-pulumi-components-0.4.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_engineering_pulumi_components-0.4.1.dev66.tar", max compression
+gzip compressed data, was "data-engineering-pulumi-components-0.4.1.dev7.tar", max compression
```

## Comparing `data_engineering_pulumi_components-0.4.1.dev66.tar` & `data-engineering-pulumi-components-0.4.1.dev7.tar`

### file list

```diff
@@ -1,59 +1,41 @@
--rw-r--r--   0        0        0     1089 2024-05-02 12:56:21.516951 data_engineering_pulumi_components-0.4.1.dev66/LICENCE.md
--rw-r--r--   0        0        0        0 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/__init__.py
--rw-r--r--   0        0        0       95 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/auth0/__init__.py
--rw-r--r--   0        0        0     4480 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/auth0/create_application.py
--rw-r--r--   0        0        0     1965 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/__init__.py
--rw-r--r--   0        0        0     5255 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/bucket.py
--rw-r--r--   0        0        0    12040 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/bucket_policy.py
--rw-r--r--   0        0        0    12148 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/bucket_policy_new.py
--rw-r--r--   0        0        0      772 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/cloudtrail_log_bucket.py
--rw-r--r--   0        0        0      880 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/curated_bucket.py
--rw-r--r--   0        0        0     1296 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/fail_bucket.py
--rw-r--r--   0        0        0     1623 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/landing_bucket.py
--rw-r--r--   0        0        0     2182 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py
--rw-r--r--   0        0        0      855 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/raw_history_bucket.py
--rw-r--r--   0        0        0     4274 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py
--rw-r--r--   0        0        0     9017 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/glue/glue_job.py
--rw-r--r--   0        0        0    11261 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/glue/glue_job_new.py
--rw-r--r--   0        0        0    17669 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/glue/glue_move_script.py
--rw-r--r--   0        0        0    14400 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/glue/glue_move_script_new.py
--rw-r--r--   0        0        0     6713 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py
--rw-r--r--   0        0        0     6626 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py
--rw-r--r--   0        0        0     7685 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/copy_object_function_new.py
--rw-r--r--   0        0        0     3465 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py
--rw-r--r--   0        0        0     3241 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/get_fields.py
--rw-r--r--   0        0        0     3440 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py
--rw-r--r--   0        0        0      961 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py
--rw-r--r--   0        0        0     1831 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py
--rw-r--r--   0        0        0     2797 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py
--rw-r--r--   0        0        0     1710 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_fields/get_fields.py
--rw-r--r--   0        0        0     3210 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py
--rw-r--r--   0        0        0     1001 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py
--rw-r--r--   0        0        0     1390 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py
--rw-r--r--   0        0        0      891 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/trigger_dag/trigger_dag_.py
--rw-r--r--   0        0        0     1102 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/trigger_glue/trigger_glue.py
--rw-r--r--   0        0        0     7529 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/unused_presigned_url/unused_presigned_url.py
--rw-r--r--   0        0        0     1844 2024-05-02 12:56:21.520951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/upload_/upload_.py
--rw-r--r--   0        0        0  3005813 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/dependencies.zip
--rw-r--r--   0        0        0    10406 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py
--rw-r--r--   0        0        0     9346 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate_new.py
--rw-r--r--   0        0        0     6722 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/move_object_function.py
--rw-r--r--   0        0        0     8034 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/trigger_dag.py
--rw-r--r--   0        0        0     6150 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/trigger_glue_function.py
--rw-r--r--   0        0        0     5316 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/unused_presigned_url_function.py
--rw-r--r--   0        0        0     3628 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py
--rw-r--r--   0        0        0    10971 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/validate_function.py
--rw-r--r--   0        0        0    12110 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/validate_function_new.py
--rw-r--r--   0        0        0     4858 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/rest_apigateway.py
--rw-r--r--   0        0        0     3117 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/roles/create_get_fields_role.py
--rw-r--r--   0        0        0     3285 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py
--rw-r--r--   0        0        0     2077 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/roles/create_upload_role.py
--rw-r--r--   0        0        0     5140 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/waf.py
--rw-r--r--   0        0        0      213 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/__init__.py
--rw-r--r--   0        0        0     2634 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py
--rw-r--r--   0        0        0     2661 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/landing_to_raw_history_new.py
--rw-r--r--   0        0        0     5625 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py
--rw-r--r--   0        0        0     5563 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/raw_history_to_curated_new.py
--rw-r--r--   0        0        0     8557 2024-05-02 12:56:21.532951 data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/utils.py
--rw-r--r--   0        0        0      825 2024-05-02 12:56:21.536951 data_engineering_pulumi_components-0.4.1.dev66/pyproject.toml
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 data_engineering_pulumi_components-0.4.1.dev66/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/__init__.py
+-rw-r--r--   0        0        0       95 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/auth0/__init__.py
+-rw-r--r--   0        0        0     4454 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/auth0/create_application.py
+-rw-r--r--   0        0        0     1728 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/__init__.py
+-rw-r--r--   0        0        0     4212 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket.py
+-rw-r--r--   0        0        0    10416 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket_policy.py
+-rw-r--r--   0        0        0      772 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/cloudtrail_log_bucket.py
+-rw-r--r--   0        0        0      684 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/curated_bucket.py
+-rw-r--r--   0        0        0     1181 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/fail_bucket.py
+-rw-r--r--   0        0        0     1387 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/landing_bucket.py
+-rw-r--r--   0        0        0     2182 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py
+-rw-r--r--   0        0        0      634 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/raw_history_bucket.py
+-rw-r--r--   0        0        0     4276 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py
+-rw-r--r--   0        0        0     9018 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_job.py
+-rw-r--r--   0        0        0    16667 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_move_script.py
+-rw-r--r--   0        0        0     6713 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py
+-rw-r--r--   0        0        0     6626 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py
+-rw-r--r--   0        0        0     3262 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py
+-rw-r--r--   0        0        0     3236 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py
+-rw-r--r--   0        0        0      962 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py
+-rw-r--r--   0        0        0      933 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py
+-rw-r--r--   0        0        0     2282 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py
+-rw-r--r--   0        0        0     2751 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py
+-rw-r--r--   0        0        0     1001 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py
+-rw-r--r--   0        0        0     1390 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py
+-rw-r--r--   0        0        0     1437 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/upload_/upload_.py
+-rw-r--r--   0        0        0 10008354 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/dependencies.tar.gz
+-rw-r--r--   0        0        0     8773 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py
+-rw-r--r--   0        0        0     6685 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/move_object_function.py
+-rw-r--r--   0        0        0     3155 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py
+-rw-r--r--   0        0        0    10974 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/validate_function.py
+-rw-r--r--   0        0        0     4379 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/rest_apigateway.py
+-rw-r--r--   0        0        0     2766 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py
+-rw-r--r--   0        0        0     2077 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_upload_role.py
+-rw-r--r--   0        0        0      213 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/__init__.py
+-rw-r--r--   0        0        0     2428 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py
+-rw-r--r--   0        0        0     5170 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py
+-rw-r--r--   0        0        0     8557 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/utils.py
+-rw-r--r--   0        0        0      638 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 data-engineering-pulumi-components-0.4.1.dev7/setup.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 data-engineering-pulumi-components-0.4.1.dev7/PKG-INFO
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/auth0/create_application.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/auth0/create_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,37 +25,40 @@
             t="data-engineering-pulumi-components:aws:webapplication",
             opts=opts,
         )
         self._opts = opts
         self._name = name
         self._tagger = tagger
 
-        # Create a tenant (area where all apis + apps are created) manually.
-        # Create a machine-to-machine api manually and use its clientid + client secret
+        # Create a tenant(Area where all api, apps are created) mannually .
+        # Create a machine-to-machine api and use its clientid , client secret
         # to create applications
+
         # create provider. using provider you can create app
         self._auth_provider = provider.Provider(
             resource_name=f"{name}-auth0-provider",
             opts=None,
             domain=auth0_domain,
             client_id=client_id,
             client_secret=client_secret,
             debug=auth0_debug,
         )
+
         self._client = auth0.Client(
             resource_name=f"{name}-web-application",
             app_type="regular_web",
+            custom_login_page=application_url,
             allowed_logout_urls=[
-                "https://localhost:5000/start"
+                "http://localhost:5000/callback"
                 if add_local_host
-                else application_url + "/start",
+                else application_url + "/callback",
             ],
             allowed_origins=[application_url],
             callbacks=[
-                "https://localhost:5000/callback"
+                "http://localhost:5000/callback"
                 if add_local_host
                 else application_url + "/callback",
             ],
             client_secret_rotation_trigger={
                 "triggered_at": "2018-01-02T23:12:01Z",
                 "triggered_by": "auth0",
             },
@@ -83,38 +86,38 @@
                 rotation_type="rotating",
                 token_lifetime=300,
             ),
             token_endpoint_auth_method="client_secret_post",
             web_origins=[
                 "http://localhost:5000" if add_local_host else web_origin,
             ],
-            jwt_configuration=auth0.GlobalClientJwtConfigurationArgs(alg="RS256"),
             opts=ResourceOptions(
                 provider=self._auth_provider, depends_on=self._auth_provider
             ),
         )
+
         self._connection = auth0.Connection(
-            "passwordlessEmail",
+            f"{name}-connection",
             show_as_button=True,
             is_domain_connection=False,
             options=auth0.ConnectionOptionsArgs(
                 from_=f"{name}root@auth0.com",
                 subject="Welcome to {{ application.name }}",
                 syntax="liquid",
                 template=template,
                 brute_force_protection=True,
                 scopes=["openid", "profile", "email"],
                 debug=True,
                 disable_cache=True,
                 disable_signup=True,
                 import_mode=False,
                 totp=auth0.ConnectionOptionsTotpArgs(time_step=300, length=6),
-                name="email",
+                name="Database Connection Opts",
                 tenant_domain=auth0_domain,
-                enabled_database_customization=False,
             ),
             strategy="email",
+            enabled_clients=[self._client.id],
             display_name="Passwordless Connection",
             opts=ResourceOptions(
                 provider=self._auth_provider, depends_on=self._auth_provider
             ),
         )
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/__init__.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,49 +9,43 @@
 
 from .cloud_trail.cloud_trail import CloudTrail
 
 from .glue.glue_job import GlueComponent
 
 from .lambdas.lambda_handlers.get_databases import get_databases
 from .lambdas.lambda_handlers.get_tables import get_tables
-from .lambdas.lambda_handlers.get_fields import get_fields
 
 from .lambdas.authorisation_function import AuthorisationFunction
 from .lambdas.copy_object_function import CopyObjectFunction
 from .lambdas.get_databases_function import GetDatabasesFunction
 from .lambdas.get_tables_function import GetTablesFunction
-from .lambdas.get_fields import GetFieldsLambda
 from .lambdas.move_object_function import MoveObjectFunction
 from .lambdas.upload_object_function import UploadObjectFunction
 from .lambdas.validate_function import ValidateMoveObjectFunction
 
 from .roles.create_list_bucket_role import CreateListBucketRole
 from .roles.create_upload_role import CreateUploadRole
-from .roles.create_get_fields_role import CreateGetFieldsRole
 
 
 __all__ = [
     "AuthorisationFunction",
     "Bucket",
     "BucketPutPermissionsArgs",
     "CopyObjectFunction",
     "CreateListBucketRole",
     "CreateUploadRole",
-    "CreateGetFieldsRole",
     "CuratedBucket",
     "CloudTrailLogBucket",
     "FailBucket",
     "GetDatabasesFunction",
     "GetTablesFunction",
-    "GetFieldsLambda",
     "CloudTrail",
     "GlueComponent",
     "LandingBucket",
     "MoveObjectFunction",
     "PulumiBackendBucket",
     "RawHistoryBucket",
     "UploadObjectFunction",
     "ValidateMoveObjectFunction",
     "get_databases",
     "get_tables",
-    "get_fields",
 ]
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from typing import Optional, Sequence
 import pulumi_aws.s3 as s3
 from pulumi_aws.s3 import BucketCorsRuleArgs
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ComponentResource, ResourceOptions
 from pulumi_aws import Provider
-import pulumi_aws as aws
 
 
 class InvalidBucketNameError(Exception):
     pass
 
 
 def _bucket_name_is_valid(name: str) -> bool:
@@ -93,15 +92,14 @@
             },
             tags=tagger.create_tags(name=name),
             versioning=versioning,
             opts=ResourceOptions(parent=self)
             if provider is None
             else ResourceOptions(parent=self, provider=provider),
         )
-
         self._bucketPublicAccessBlock = s3.BucketPublicAccessBlock(
             resource_name=f"{name}-bucket-public-access-block",
             bucket=self._bucket.id,
             block_public_acls=True,
             block_public_policy=True,
             ignore_public_acls=True,
             restrict_public_buckets=True,
@@ -115,39 +113,14 @@
         }
 
         for name, value in outputs.items():
             setattr(self, name, value)
 
         self.register_outputs(outputs)
 
-    def lifecycle_rules_expiration_days_provided(
-        self, lifecycle_rules_expiration_days, name
-    ):
-        if bool(lifecycle_rules_expiration_days) is False:
-            return None
-        if bool(lifecycle_rules_expiration_days) is True:
-            policies = []
-            for prefix, days in lifecycle_rules_expiration_days.items():
-                policy = aws.s3.BucketLifecycleRuleArgs(
-                    id="bucket-lifecycle-" + name + "-" + prefix,
-                    enabled=True,
-                    prefix=prefix,
-                    expiration=aws.s3.BucketLifecycleRuleExpirationArgs(
-                        days=days, expired_object_delete_marker=True
-                    ),
-                    noncurrent_version_expiration=(
-                        aws.s3.BucketLifecycleRuleNoncurrentVersionExpirationArgs(
-                            days=days,
-                        )
-                    ),
-                )
-                policies.append(policy)
-
-            return policies
-
     def add_cors_rules(
         self,
         cors_allowed_headers: list,
         cors_allowed_origins: list,
     ):
         return [
             BucketCorsRuleArgs(
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/bucket_policy.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket_policy.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,34 +39,44 @@
 
 
 class BucketPolicyBuilder(ComponentResource):
     def __init__(
         self,
         Bucket,
         put_permissions: Optional[Sequence[BucketPutPermissionsArgs]] = None,
-        provider: aws.Provider = None,
+        t: Optional[str] = None,
+        opts: Optional[ResourceOptions] = None,
     ):
         """
         Pass a bucket and some permissions to this object to build a bucket policy and
         attach it to a bucket.
         """
+        if t is None:
+            t = "data-engineering-pulumi-components:aws:BucketPolicyBuilder"
+        self._name = Bucket._name + "_BucketPolicyBuilder"
+        super().__init__(
+            t=t,
+            name=self._name,
+            props=None,
+            opts=opts,
+        )
+
         if getattr(Bucket, "_put_permissions", None) is not None:
             raise Exception("put_permissions are already set")
 
-        self.Bucket_facade = Bucket
+        self.Bucket = Bucket
         self._put_permissions = put_permissions
         self._statements = []
-        self._provider = provider
 
     @property
     def add_basic_access_permissions(
         self,
     ):
         self._statements = Output.all(
-            bucket_arn=self.Bucket_facade._bucket.arn,
+            bucket_arn=self.Bucket._bucket.arn,
             **{str(i): item.__dict__ for i, item in enumerate(self._put_permissions)}
             if self._put_permissions
             else {},
         ).apply(self._get_basic_access_policy)
 
         return self
 
@@ -128,15 +138,15 @@
         )
 
         return statements
 
     @property
     def add_glue_permissions(self):
         self._glue_statements = Output.all(
-            bucket_arn=self.Bucket_facade._bucket.arn,
+            bucket_arn=self.Bucket._bucket.arn,
             **{str(i): item.__dict__ for i, item in enumerate(self._put_permissions)}
             if self._put_permissions
             else {},
         ).apply(self._get_policy_glue)
 
         self._statements = Output.all(
             statements=self._statements,
@@ -175,15 +185,15 @@
             )
 
         return statements
 
     @property
     def add_access_block(self):
         self._access_block_statements = Output.all(
-            bucket_arn=self.Bucket_facade._bucket.arn,
+            bucket_arn=self.Bucket._bucket.arn,
             **{str(i): item.__dict__ for i, item in enumerate(self._put_permissions)}
             if self._put_permissions
             else {},
         ).apply(self._access_block_policy)
 
         self._statements = Output.all(
             statements=self._statements,
@@ -215,15 +225,15 @@
             )
 
         return statements
 
     @property
     def add_cloud_trail_permissions(self):
         self._cloudtrail_statements = Output.all(
-            bucket_arn=self.Bucket_facade._bucket.arn,
+            bucket_arn=self.Bucket._bucket.arn,
         ).apply(self._get_cloudtrail_policy)
 
         self._statements = Output.all(
             statements=self._statements,
             cloudtrail_statements=self._cloudtrail_statements,
         ).apply(lambda args: args.pop("statements") + args.pop("cloudtrail_statements"))
 
@@ -248,86 +258,37 @@
                 "Resource": bucket_arn + "/*",
                 "Condition": {
                     "StringEquals": {"s3:x-amz-acl": "bucket-owner-full-control"}
                 },
             },
         ]
 
-    def _add_ssl_requests_only(self):
-        self._ssl_requests_only_statements = Output.all(
-            bucket_arn=self.Bucket_facade._bucket.arn,
-        ).apply(self._get_ssl_requests_only_policy)
-
-        self._statements = Output.all(
-            statements=self._statements,
-            ssl_requests_only_statements=self._ssl_requests_only_statements,
-        ).apply(
-            lambda args: args.pop("statements")
-            + args.pop("ssl_requests_only_statements")
-        )
-
-        return self
-
-    def _get_ssl_requests_only_policy(self, args):
-        bucket_arn = args.pop("bucket_arn")
-
-        return [
-            {
-                "Sid": "AllowSSLRequestsOnly",
-                "Action": "s3:*",
-                "Effect": "Deny",
-                "Resource": [bucket_arn, bucket_arn + "/*"],
-                "Condition": {"Bool": {"aws:SecureTransport": "false"}},
-                "Principal": "*",
-            }
-        ]
-
     def _get_final_policy_doc(self):
-        # All bucket should deny non SSL requests
-        self._add_ssl_requests_only()
         # Every operation to an Output object needs to be an apply or a Pulumi function
         return self._statements.apply(
             lambda l: json.dumps({"Version": "2012-10-17", "Statement": l})
         )
 
     def _create_bucket_policy(self, policy_doc: Output):
         # Some of the glue outputs aren't compatible with direct reference in the
         # bucket policy creation, so it all needs to be wrapped in an output object.
-
-        # Aas of 2022-08-13 Pulumi can't handle replacing bucket policies
-        # Behaviour has been observed that even with delete_before_replace, Pulumi will
-        # create the new bucket policy first, then delete the old one, resulting in a
-        # blank policy on the attached bucket.
-        # Deleting then creating in separate commands works.
         return Output.all(
-            name=self.Bucket_facade._name,
-            bucket_id=self.Bucket_facade._bucket.id,
+            name=self.Bucket._name,
+            bucket_id=self.Bucket._bucket.id,
             policy_doc=policy_doc,
-            bucket=self.Bucket_facade._bucket,
-            provider=self._provider,
+            bucket=self.Bucket,
         ).apply(
             lambda args: aws.s3.BucketPolicy(
                 resource_name=f"{args['name']}-bucket-policy",
                 bucket=args["bucket_id"],
-                policy=args["policy_doc"],  # needs to be json)
-                opts=ResourceOptions(
-                    parent=args["bucket"],
-                    depends_on=args["bucket"],
-                    delete_before_replace=True,
-                )
-                if args["provider"] is None
-                else ResourceOptions(
-                    parent=args["bucket"],
-                    depends_on=args["bucket"],
-                    provider=args["provider"],
-                    delete_before_replace=True,
-                ),
+                policy=args["policy_doc"],  # needs to be json
+                opts=ResourceOptions(parent=args["bucket"]),
             )
         )
 
     def build(self):
         self._policy_doc = self._get_final_policy_doc()
         self._policy = self._create_bucket_policy(self._policy_doc)
         # Tag the bucket with put permissions so another policy is not added
-        self.Bucket_facade._put_permissions = self._put_permissions
+        self.Bucket._put_permissions = self._put_permissions
 
         return self._policy
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/cloudtrail_log_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/cloudtrail_log_bucket.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/curated_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/curated_bucket.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,22 +6,18 @@
 
 
 class CuratedBucket(Bucket):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
-        lifecycle_rules_expiration_days: dict = {},
         provider: Provider = None,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         super().__init__(
             name=name + "-curated",
             tagger=tagger,
-            lifecycle_rules=self.lifecycle_rules_expiration_days_provided(
-                lifecycle_rules_expiration_days, name
-            ),
             t="data-engineering-pulumi-components:aws:CuratedBucket",
             cors_rules=None,
             provider=provider,
             opts=opts,
         )
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/fail_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/fail_bucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from typing import Optional
 from data_engineering_pulumi_components.aws.buckets.bucket import Bucket
-from data_engineering_pulumi_components.aws.buckets.bucket_policy import (
-    BucketPolicyBuilder,
-)
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ResourceOptions
 import pulumi_aws as aws
 
 
 class FailBucket(Bucket):
     def __init__(
@@ -28,8 +25,8 @@
                             days=14,
                         )
                     ),
                 )
             ],
             opts=opts,
         )
-        self.policy = BucketPolicyBuilder(Bucket=self).build()
+        # Lack of policy is currently intentional
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/landing_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/landing_bucket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 from typing import Optional
 
-from pulumi import ResourceOptions
-
 from data_engineering_pulumi_components.aws.buckets.bucket import Bucket
 from data_engineering_pulumi_components.aws.buckets.bucket_policy import (
-    BucketPolicyBuilder,
     BucketPutPermissionsArgs,
+    BucketPolicyBuilder,
 )
 from data_engineering_pulumi_components.utils import Tagger
+from pulumi import ResourceOptions
 
 
 class LandingBucket(Bucket):
     def __init__(
         self,
         name: str,
         aws_arn_for_put_permission: str,
         tagger: Tagger,
-        lifecycle_rules_expiration_days: dict = {},
         cors_allowed_headers: list = None,
         cors_allowed_origins: list = None,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         super().__init__(
-            name=name if name.endswith("-landing") else name + "-landing",
+            name=name + "-landing",
             t="data-engineering-pulumi-components:aws:LandingBucket",
-            lifecycle_rules=self.lifecycle_rules_expiration_days_provided(
-                lifecycle_rules_expiration_days, name
-            ),
             cors_rules=self.add_cors_rules(
                 cors_allowed_headers=cors_allowed_headers,
                 cors_allowed_origins=cors_allowed_origins,
             )
             if (cors_allowed_headers and cors_allowed_origins) is not None
             else None,
             tagger=tagger,
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self,
         resources_arn_to_monitor: str,
         eventName: str,
         resources_type: str,
         eventCategory: str,
         compare_resource: str = "equals",
     ) -> list:
+
         """
         Function creates the list of TrailAdvancedEventSelectorFieldSelectorArgs
         dynamically
 
         Parameters
           ----------
           resources_arn_to_monitor : str
@@ -94,14 +95,15 @@
                 )
             )
         return _field_selectors
 
     def advanced_event_selector_field_selector(
         self, fieldtype, value, operator
     ) -> cloudtrail.TrailAdvancedEventSelectorFieldSelectorArgs:
+
         equalto_val = [value] if operator == "equals" else None
         notequalto_val = [value] if operator == "not_equals" else None
         starts_withs_val = [value] if operator == "starts_withs" else None
         ends_withs_val = [value] if operator == "ends_withs" else None
         not_starts_withs_val = [value] if operator == "not_starts_withs" else None
         not_ends_withs_val = [value] if operator == "not_not_ends_withsequals" else None
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/glue/glue_job.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         high_memory_worker: bool = False,
         number_of_workers: int = 2,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         """
         Provides a Glue Component that copies objects from a source bucket to a
         destination bucket as a parquet file.
+
         Parameters
         ----------
         destination_bucket : Bucket
             The bucket to copy data to.
         name : str
             The name of the resource.
         source_bucket : Bucket
@@ -176,15 +177,15 @@
                         self._glueJobScript.bucket, self._glueJobScript.key
                     ).apply(lambda o: f"s3://{o[0]}/{o[1]}"),
                 ),
                 role_arn=self._role.arn,
                 default_arguments=glue_inputs,
                 description=f"Populates the {name} curated bucket with parquets",
                 execution_property=JobExecutionPropertyArgs(max_concurrent_runs=1),
-                glue_version="4.0",
+                glue_version="3.0",
                 name=f"{name}-glue-job",
                 number_of_workers=number_of_workers,
                 security_configuration=self._securityConfiguration.name,
                 tags=tagger.create_tags(f"{name}-glue-job"),
                 worker_type="G.2X" if high_memory_worker else "G.1X",
             ),
             opts=ResourceOptions(
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/glue/glue_move_script.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_move_script.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,211 +1,102 @@
 from awsglue.context import GlueContext
 from awsglue.dynamicframe import DynamicFrame
 from awsglue.utils import getResolvedOptions
 from pyspark.context import SparkContext
-from pyspark.sql import SparkSession, DataFrame
+from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql import functions as F
 import sys
 from awsglue.job import Job
-from datetime import datetime as dt
 import boto3
 from string import Template
-import json
-import datetime
-from urllib3 import PoolManager
-import logging
-
-logging.basicConfig(level=logging.INFO)
-root_logger = logging.getLogger()
+import re
 
 
 class InvalidFileType(Exception):
     pass
 
 
 def time_column_converter(dataframe: DataFrame, column: str, format: str):
     non_nulls = dataframe.agg(
         F.sum(F.when(F.col(column).isNotNull(), 1).otherwise(0))
     ).first()[0]
-    if format == "iso":
-        dataframe = dataframe.withColumn(column, F.split(column, r"\.").getItem(0))
-        dataframe = dataframe.withColumn(
-            column, F.to_timestamp(column, "yyyy-MM-dd'T'HH:mm:ss")
-        )
-    else:
-        dataframe = dataframe.withColumn(column, F.to_timestamp(column, format))
+    dataframe = dataframe.withColumn(column, F.to_timestamp(column, format))
     converted = dataframe.agg(
         F.sum(F.when(F.col(column).isNotNull(), 1).otherwise(0))
     ).first()[0]
     if non_nulls != converted:
         print(
             f"Warning! {column} had {non_nulls} timestamps, "
             + f"and now has {converted} non_null timestamps!"
         )
     print("converted column " + column)
     return dataframe
 
 
-def date_finder(input: str):
-    formats = [
-        "%Y%m%d%H%M%SZ",
-        "%d/%m/%Y %H:%M:%S",
-        "%Y-%m-%d",
-        "%Y/%m/%d",
-        "%d/%m/%y",
-        "%d/%m/%Y",
-    ]
+def extraction_timestamp_formatter():
+    format = "%Y%m%d%H%M%SZ"
     # mapping converts python dates to simple dates for java
     mapping = {
         "Y": "yyyy",
         "y": "yy",
         "m": "MM",
         "d": "dd",
-        "dT": "dd'T'",
         "H": "HH",
         "M": "mm",
-        "S": "ss",
         "SZ": "ss'Z'",
     }
-    # TODO - Find more common formats from inspecting user data
-    correct_format = None
-    for format in formats:
-        try:
-            dt.strptime(input, format)
-            correct_format = format
-            break
-        except ValueError:
-            continue
-    if correct_format is None:
-        try:
-            dt.fromisoformat(input)
-            return_format = "iso"
-        except ValueError:
-            return_format = None
-            pass
-    else:
-        return_format = Template(correct_format.replace("%", "$")).substitute(**mapping)
+    return_format = Template(format.replace("%", "$")).substitute(**mapping)
     return return_format
 
 
 def date_converter(dataframe: DataFrame):
-    try:
-        sample = (
-            dataframe.select(
-                [F.first(x, ignorenulls=True).alias(x) for x in dataframe.columns]
-            )
-            .first()
-            .asDict()
-        )
-    except Exception:
-        print(f"dataframe of {path} appears to have no rows!")
-        return dataframe
-
-    date_columns = {}
-    for column in sample:
-        # Only bother checking if it's already not a non-string type
-        if type(sample[column]) == str:
-            date_format = date_finder(sample[column])
-            if date_format is not None:
-                date_columns[column] = date_format
-
-    for column in date_columns:
-        dataframe = time_column_converter(
-            dataframe=dataframe, column=column, format=date_columns[column]
-        )
+    dataframe = time_column_converter(
+        dataframe=dataframe,
+        column="extraction_timestamp",
+        format=extraction_timestamp_formatter(),
+    )
     return dataframe
 
 
 def key_splitter(key: str):
     """
     Takes standard AWS Key, as output by boto3.client.list_objects_v2(),
     and splits the key into the databasename, filename + extension, and the file path.
 
     Arguments:
     key: str
         A key of the format path/to/file/filename.ext
     """
     key_list = key.split("/")
     filename = key_list.pop()
-    key_list.pop()  # Drop extraction timestamp
     database_key = [s for s in key_list if "database_name=" in s]
     table_key = [s for s in key_list if "table_name=" in s]
+    extraction_key = [s for s in key_list if "extraction_timestamp=" in s]
     filetype = filename.split(".")[-1]
+    # drop extraction timestamp before conjoining
+    key_list.pop()
     filepath = "/".join(key_list) + "/"
     database_name = database_key[0].split("=")[-1]
+    extraction_timestamp = extraction_key[0].split("=")[-1]
     table_name = table_key[0].split("=")[-1]
     if filetype not in ["csv", "json", "jsonl"]:
         raise InvalidFileType(
             f"The filetype, {filetype} is not supported by this operation"
         )
-    return filepath, database_name, table_name, filetype
+    return filepath, database_name, table_name, filetype, filename, extraction_timestamp
 
 
 def replace_space_in_string(name: str) -> str:
     """
-    If a string contains space inbetween, then replace by underscore.
-    If it contains brackets then remove them.
+    If a string contains space inbetween, then replace by underscore
     """
-    replaced_name = name.strip().replace(" ", "_").replace("(", "").replace(")", "")
+    replaced_name = name.strip().replace(" ", "_")
     return replaced_name
 
 
-def destination_cleaner(bucket: str, path: str, role_arn: str = None):
-    """
-    Takes a path, locates all keys it conains,
-    and cleans any files matching the supplied path in the bucket.
-
-    Arguments:
-    path: str
-        A path to a file, or files. Used as a prefix to locate keys within.
-    bucket: str
-        An AWS Bucket name
-    role_arn:
-        An optional ARN, if the bucket being cleared requires an assumed role.
-    """
-    if role_arn is not None:
-        sts_client = boto3.client("sts")
-        assumed_role_object = sts_client.assume_role(
-            RoleArn=role_arn, RoleSessionName="AssumedRoleSession1"
-        )
-        assume_creds = assumed_role_object["Credentials"]
-        access_key_id = assume_creds["AccessKeyId"]
-        secret_access_key = assume_creds["SecretAccessKey"]
-        session_token = assume_creds["SessionToken"]
-        s3 = boto3.client(
-            "s3",
-            aws_access_key_id=access_key_id,
-            aws_secret_access_key=secret_access_key,
-            aws_session_token=session_token,
-        )
-    else:
-        s3 = boto3.client("s3")
-    paginator = s3.get_paginator("list_objects_v2")
-    page_iterator = paginator.paginate(
-        Bucket=bucket,
-        Prefix=path,
-    )
-    response_list = []
-
-    for page in page_iterator:
-        response_list.append(page)
-
-    key_count = 0
-    if response_list[0]["KeyCount"]:
-        print(f"files already exist at destination {path}, flushing...")
-        for response in response_list:
-            for item in response["Contents"]:
-                key = item["Key"]
-                s3.delete_object(Bucket=bucket, Key=key)
-            key_count += response["KeyCount"]
-        print(f"No. of keys deleted: {key_count}")
-    else:
-        print(path + " does not exist in destination!")
-
-
 def dynamic_frame_to_glue_catalog(
     path: str,
     table_name: str,
     database_name: str,
     dynamic_frame: DynamicFrame,
     glue_context: GlueContext,
 ):
@@ -222,215 +113,214 @@
         The name of the database which the table is to appear in.
     dynamic_frame: DynamicFrame
         A Glue DynamicFrame, including partitioning info, to be written out.
     glue_context:
         An AWS GlueContext
     """
     print("Attempting to register to Glue Catalogue")
+    # recommended to use write_dynamic_frame.from_options() rather than getSink
     try:
         sink = glue_context.getSink(
-            connection_type="s3",
             path=path,
-            enableUpdateCatalog=True,
+            connection_type="s3",
             updateBehavior="UPDATE_IN_DATABASE",
             partitionKeys=["extraction_timestamp"],
+            compression="snappy",
+            enableUpdateCatalog=True,
+            transformation_ctx="sink",
         )
-
-        sink.setFormat("glueparquet")
+        sink.setFormat("glueparquet", useGlueParquetWriter=True)
         sink.setCatalogInfo(catalogDatabase=database_name, catalogTableName=table_name)
+
         sink.writeFrame(dynamic_frame)
         print("Write out of file succeeded!")
     except Exception as e:
         print(f"Could not convert {path} to glue table, due to an error!")
         print(e)
 
 
-def send_alert_to_slack(
-    title, desc, event_source, source_id, msg, user, icon, args: dict
-):
-    """Sends an alert to Slack
-    Parameters
-    ----------
-    title : str
-        Event title
-    desc : str
-        Event description
-    event_source : str
-        Event source
-    source_id : str
-        Event source ID
-    msg : str
-        Message
-    user : str
-        Name of AWS service raising alerts
-    icon : str
-        Slack icon representing the service
-    args : dict
-        args fed into script
-    """
-    try:
-        http = PoolManager()
-        url = args["webhook_url"]
-        now = datetime.datetime.now(datetime.timezone.utc).isoformat()
-        now = now.replace("+00:00", "Z")
-        payload = {
-            "channel": args["channel"],
-            "text": title,
-            "username": user,
-            "icon_emoji": icon,
-            "blocks": [
-                {
-                    "type": "header",
-                    "text": {
-                        "type": "plain_text",
-                        "text": f"{title} – {desc}",
-                        "emoji": True,
-                    },
-                },
-                {
-                    "type": "section",
-                    "text": {
-                        "type": "mrkdwn",
-                        "text": (
-                            f"*Event Source:* {event_source}\n"
-                            f"*Event Time:* {now}\n"
-                            f"*Source ID:* {source_id}\n"
-                            f"*Message:* {msg}"
-                        ),
-                    },
-                },
-            ],
-        }
-        encoded_payload = json.dumps(payload).encode("utf-8")
-        response = http.request(method="POST", url=url, body=encoded_payload)
-        root_logger.info(
-            {
-                "message": payload,
-                "status_code": response.status,
-                "response": response.data,
-            }
-        )
-    except Exception as e:
-        root_logger.error(f"Failed to send an alert to Slack: {e}")
+def add_extraction_timestamp(df):
+    df["extraction_timestamp"] = extraction_timestamp
+    return df
+
+
+def clean_dynamic_frame_fields(df):
+    """
+    Collects the field names from a Glue DynamicFrame, converts to lowercase
+    and replaces any special characters (not [a-z0-9_]) with underscore; checks
+    once for duplicate field names and adds a suffix to any found.
+
+    For example, "AN.T" and "an@T" both become "an_t" then the second occurence
+    is renamed "an_t_2". Hopefully this is sufficent to ensure no duplicates!
+
+    Input:
+    df: Glue DynamicFrame
+
+    Output:
+    df: Glue DynamicFrame
+        With field names comprising only [a-z0-9_] characters.
+    """
+    # get list of fields from dynamic frame
+    fields = list(df.schema().field_map.keys())
+    # create backticked version to enable replacement of awkward special chars: .{}[]()
+    fields_backticked = ["`" + field + "`" for field in fields]
+    # create new names allowing only [a-z0-9_], replace special chars with "_"
+    fields_clean = [re.sub("[^a-z0-9_]", "_", f.lower()) for f in fields]
+    # strip underscores from start of field name
+    fields_clean = [f.lstrip("_") for f in fields_clean]
+    # check fields_clean for duplicate names; if any add suffix
+    if len(set(fields_clean)) != len(fields_clean):
+        counts = {}
+        for i, field in enumerate(fields_clean):
+            if field in counts:
+                counts[field] += 1
+                # add suffix if duplicate found
+                fields_clean[i] = f"{field}_{counts[field]}"
+            else:
+                counts[field] = 1
+    # rename every field if at least one field needs cleaning
+    if fields != fields_clean:
+        for old_name, clean_name in zip(fields_backticked, fields_clean):
+            df = df.rename_field(old_name, clean_name)
 
+    return df
 
-def files_to_dynamic_frame(
+
+def new_files_to_dynamic_frame(
     path: str,
     filetype: str,
+    filename: str,
     source_bucket: str,
+    destination_bucket: str,
     table_name: str,
     allow_data_conversion: str,
+    extraction_timestamp: str,
     spark: SparkSession,
     glue_context: GlueContext,
-    args: dict,
 ):
     """
-    Reads in files at a filepath, and transforms them into
+    Reads in a files at a filepath, and transforms them into
     a partitioned DynamicFrame using Spark and Glue.
+    (Usually there is only one file under the extraction_timestamp subfolder)
 
     Arguments:
     path: str
         A S3 path of the format path/to/file/, not including any "s3://" prefixes
     filetype: str
         A filetype, currently only of the format "csv" or "json/jsonl"
     source_bucket: str
         The name of AWS bucket in which the files are contained.
     table_name: str
         The name of the table to be constructed.
+    extraction_timestamp: str
+        The timestamp of the extract
     spark: SparkSession
         A SparkSession to be used to construct a Dataframe,
         containing the partitioned data.
     glue_context:
         An AWS GlueContext
-    args: dict
-        Dict of args fed to the script
+
+    Output:
+    dynamic_frame: Glue Dynamic Frame
+        A dynamic frame of the files read; can be null, with zero rows.
     """
     try:
-        file_location = "s3://" + source_bucket + "/" + path
+        file_location = (
+            "s3://" + source_bucket + "/" + path
+            + "extraction_timestamp=" + extraction_timestamp
+        )
+
+        print("file location: ", file_location)
         if filetype == "csv":
-            datasource = spark.read.load(
-                path=file_location,
+            print("using csv")
+            dynamic_frame = glue_context.create_dynamic_frame.from_options(
+                format_options={"multiline": False, "withHeader": True},
+                connection_type="s3",
                 format="csv",
-                header="true",
-                multiLine=True,
-                escape='"',
+                connection_options={
+                    "paths": [file_location],
+                    "recurse": False,
+                    "optimizePerformance": True
+                },
+                transformation_ctx="df_" + table_name + "_" + extraction_timestamp,
             )
         else:
-            datasource = spark.read.load(
-                path=file_location,
+            print("using json")
+            dynamic_frame = glue_context.create_dynamic_frame.from_options(
+                format_options={"multiline": True},
+                connection_type="s3",
                 format="json",
+                connection_options={
+                    "paths": [file_location],
+                    "recurse": False,
+                },
+                transformation_ctx="df_" + table_name + "_" + extraction_timestamp,
             )
-        print(f"Successfully read files at {path} to Spark")
 
-        # If the columnname contains space and add an underscore
-        exprs = [
-            F.col(column).alias(replace_space_in_string(column))
-            for column in datasource.columns
-        ]
-        renamed_datasource = datasource.select(*exprs)
-        print(f"Converting dates for {path}")
-        if allow_data_conversion == "True":
-            finalised_datasource = date_converter(renamed_datasource)
-        else:
-            finalised_datasource = renamed_datasource
-
-        dynamic_frame = DynamicFrame.fromDF(
-            finalised_datasource, glue_context, table_name
-        )
+        # bookmarking is noted at the point of create_dynamic_frame above
+        print(f"Successfully read files at {file_location} to Glue Dynamic Frame")
+        # print("Dynamic Frame row count: ", dynamic_frame.count())
+
+        # logic to apply further processing/printouts iff DynF rows not 0
+        if dynamic_frame.count() > 0:
+            # print("First 2 rows of Dynamic Frame:")
+            # dynamic_frame.show(2)
+
+            # add extraction_timestamp column, no bookmarking required
+            dynamic_frame = dynamic_frame.map(
+                f=add_extraction_timestamp,
+            )
+            # clean dynamic frame field names
+            print("fields: ", list(dynamic_frame.schema().field_map.keys()))
+            dynamic_frame = clean_dynamic_frame_fields(dynamic_frame)
+            # check new fields
+            print("clean fields: ", list(dynamic_frame.schema().field_map.keys()))
+
+            # df = dynamic_frame.toDF()
+            # print("First 2 rows of cleaned Dynamic Frame as Spark DF:")
+            # df.show(2)
 
         return dynamic_frame
 
     except Exception as e:
         print(f"Could not convert {file_location} to dynamic_frame, due to an error!")
-        send_alert_to_slack(
-            title="Glue validation error",
-            desc="Dynamic frame conversion error",
-            event_source=f"Bucket {file_location}",
-            source_id=f"Source table {table_name}",
-            msg=e,
-            user="AWS Lambda",
-            icon=":lambda:",
-            args=args,
-        )
         print(e)
 
 
 def setup_glue(inputs: dict):
     """
     Setup glue environment and create a spark session
 
-    Returns a spark session and glue context
+    Returns a spark session, glue context and job
     """
     sc = SparkContext()
     glueContext = GlueContext(sc)
     job = Job(glueContext)
     job.init(inputs["JOB_NAME"], inputs)
     glueContext._jsc.hadoopConfiguration().set(
         "fs.s3.enableServerSideEncryption", "true"
     )
     glueContext._jsc.hadoopConfiguration().set(
         "fs.s3.canned.acl", "BucketOwnerFullControl"
     )
     spark = glueContext.spark_session
 
-    return spark, glueContext
+    return spark, glueContext, job
 
 
 def job_inputs():
     return getResolvedOptions(
         sys.argv,
         [
             "JOB_NAME",
             "source_bucket",
             "destination_bucket",
             "stack_name",
             "multiple_db_in_bucket",
             "allow_data_conversion",
-            "webhook_url",
-            "channel",
         ],
     )
 
 
 def list_of_data_objects_to_process(bucket):
     """
     List all objects under the data/ path for a given bucket.
@@ -462,28 +352,38 @@
     per path to table.
 
     A dictionary is returned with a key for each path found.
     """
     paths = {}
     for item in list_of_objects:
         key = item["Key"]
-
         try:
-            input_path, database_name, table_name, filetype = key_splitter(key=key)
+            (
+                input_path,
+                database_name,
+                table_name,
+                filetype,
+                filename,
+                extraction_timestamp,
+            ) = key_splitter(key=key)
             if input_path not in paths:
                 paths[input_path] = {}
-
             paths[input_path]["filetype"] = filetype
+            paths[input_path]["filename"] = filename
             paths[input_path]["table_name"] = table_name
             paths[input_path]["database_name"] = database_name
-
+            if "extraction_timestamps" not in paths[input_path].keys():
+                paths[input_path]["extraction_timestamps"] = []
+            if extraction_timestamp not in paths[input_path]["extraction_timestamps"]:
+                paths[input_path]["extraction_timestamps"].append(extraction_timestamp)
+            else:
+                continue
         except Exception as e:
             print(e)
             print(f"This is due to the file at {item['Key']}")
-
     return paths
 
 
 def does_database_exist(client, database_name):
     """Determine if this database exists in the Data Catalog
     The Glue client will raise an exception if it does not exist.
     """
@@ -498,71 +398,84 @@
     print(
         f"Job name: {args['JOB_NAME']},",
         f"source_bucket: {args['source_bucket']},",
         f"destination_bucket: {args['destination_bucket']},",
         f"stack_name: {args['stack_name']},",
         f"multiple_db_in_bucket: {args['multiple_db_in_bucket']},",
         f"allow_data_conversion: {args['allow_data_conversion']},",
-        f"webhook url: {args['webhook_url']}",
-        f"channel: {args['channel']}",
     )
 
 
 if __name__ == "__main__":
     args = job_inputs()
-    spark, glueContext = setup_glue(inputs=args)
-    print_inputs(inputs=args)
+    print("args: ", args)
+    # set up spark, glueContext and initialise job
+    spark, glueContext, job = setup_glue(inputs=args)
 
+    stack_name = args["stack_name"]
     response = list_of_data_objects_to_process(bucket=args["source_bucket"])
+    print("Objects in source bucket: ", len(response))
 
     if len(response) > 0:
+
         paths = paths_to_tables(list_of_objects=response)
+        print("paths: ", paths)
 
         for path in paths:
-            destination_cleaner(bucket=args["destination_bucket"], path=path)
-            desired_path = "s3://" + args["destination_bucket"] + "/" + path
+            for extraction_timestamp in paths[path]["extraction_timestamps"]:
 
-            dynamic_frame = files_to_dynamic_frame(
-                path=path,
-                filetype=paths[path]["filetype"],
-                source_bucket=args["source_bucket"],
-                table_name=paths[path]["table_name"],
-                allow_data_conversion=args["allow_data_conversion"],
-                glue_context=glueContext,
-                spark=spark,
-                args=args,
-            )
-
-            # if multiple_db_in_bucket then use
-            # databasename from 'database_name=xxx' else
-            # bucketname as databasename
-            # CREATE  GLUE CATALOG USING BOTO
-            if args["multiple_db_in_bucket"] == "True":
-                db_name = args["stack_name"] + "_" + paths[path]["database_name"]
-            else:
-                db_name = args["stack_name"]
-
-            db_name = db_name.replace("-", "_")
-            print("database", db_name)
+                desired_path = "s3://" + args["destination_bucket"] + "/" + path
 
-            client = boto3.client("glue")
-
-            if (
-                not does_database_exist(client, db_name)
-                and args["multiple_db_in_bucket"] == "True"
-            ):
-                print("create database")
-                response = client.create_database(
-                    DatabaseInput={
-                        "Name": db_name,
-                        "Description": "A Glue Database for tables from "
-                        + args["stack_name"],
-                    }
+                dynamic_frame = new_files_to_dynamic_frame(
+                    path=path,
+                    filetype=paths[path]["filetype"],
+                    filename=paths[path]["filename"],
+                    source_bucket=args["source_bucket"],
+                    destination_bucket=args["destination_bucket"],
+                    table_name=paths[path]["table_name"],
+                    allow_data_conversion=args["allow_data_conversion"],
+                    extraction_timestamp=extraction_timestamp,
+                    glue_context=glueContext,
+                    spark=spark,
                 )
 
-            dynamic_frame_to_glue_catalog(
-                path=desired_path,
-                table_name=paths[path]["table_name"],
-                database_name=db_name,
-                dynamic_frame=dynamic_frame,
-                glue_context=glueContext,
-            )
+                if dynamic_frame.count() == 0:
+                    print("No files to process; continuing to next iteration.\n")
+                    continue
+                else:
+                    # if multiple_db_in_bucket then use
+                    # databasename from 'database_name=xxx' else
+                    # bucketname as databasename
+                    # CREATE GLUE CATALOG USING BOTO
+                    if args["multiple_db_in_bucket"] == "True":
+                        db_name = (
+                            args["stack_name"] + "_" + paths[path]["database_name"]
+                        )
+                    else:
+                        db_name = args["stack_name"]
+
+                    db_name = db_name.replace("-", "_")
+                    print("database: ", db_name)
+
+                    client = boto3.client("glue")
+
+                    if (
+                        not does_database_exist(client, db_name)
+                        and args["multiple_db_in_bucket"] == "True"
+                    ):
+                        print("create database")
+                        response = client.create_database(
+                            DatabaseInput={
+                                "Name": db_name,
+                                "Description": "A Glue Database for tables from "
+                                + args["stack_name"],
+                            }
+                        )
+                    dynamic_frame_to_glue_catalog(
+                        path=desired_path,
+                        table_name=paths[path]["table_name"],
+                        database_name=db_name,
+                        dynamic_frame=dynamic_frame,
+                        glue_context=glueContext,
+                    )
+
+    job.commit()
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/copy_object_function_new.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/move_object_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import json
 from pathlib import Path
 from typing import Optional, Union
 
 from data_engineering_pulumi_components.aws.buckets.bucket import Bucket
-from data_engineering_pulumi_components.aws.lambdas.lambda_handlers.copy import copy_
+from data_engineering_pulumi_components.aws.lambdas.lambda_handlers.move import move
 from data_engineering_pulumi_components.utils import Tagger, BucketDetails
 from pulumi import AssetArchive, ComponentResource, FileArchive, Output, ResourceOptions
 from pulumi_aws.iam import Role, RolePolicy, RolePolicyAttachment
 from pulumi_aws.lambda_ import Function, FunctionEnvironmentArgs, Permission
-from pulumi_aws.cloudwatch import EventRule, EventTarget
+from pulumi_aws.s3 import BucketNotification, BucketNotificationLambdaFunctionArgs
 
 
-class CopyObjectFunction(ComponentResource):
+class MoveObjectFunction(ComponentResource):
     def __init__(
         self,
         destination_bucket: Union[Bucket, str],
         name: str,
         source_bucket: Bucket,
         tagger: Tagger,
         prefix: str = None,
         opts: Optional[ResourceOptions] = None,
         create_notification: bool = True,
     ) -> None:
         """
         Provides a Lambda function that copies objects from a source bucket to a
-        destination bucket.
+        destination bucket and then deletes the original object.
 
         Parameters
         ----------
         destination_bucket : Bucket, str
-            The bucket to copy data to, if created in this stack. Or if the bucket
+            The bucket to move data to, if created in this stack. Or if the bucket
             already exists, its name as a string.
         name : str
             The name of the resource.
         source_bucket : Bucket
-            The bucket to copy data from.
+            The bucket to move data from.
         tagger : Tagger
             A tagger resource.
         prefix : str, optional
-            If included, only copy files from this 'folder'.
+            If included, only move files from this 'folder'.
             Don't include the trailing slash: 'project-name', not 'project-name/'
         opts : Optional[ResourceOptions]
             Options for the resource. By default, None.
         create_notification : bool
             If True, create a BucketNotification to run the Lambda when an object is
             created in the source bucket. If False, don't create a BucketNotification.
             If you have separate Lambdas for different prefixes in the same bucket,
             you'll need to set this to False and create a combined BucketNotification
             separately.
         """
         super().__init__(
-            t="data-engineering-pulumi-components:aws:CopyObjectFunction",
+            t="data-engineering-pulumi-components:aws:MoveObjectFunction",
             name=name,
             props=None,
             opts=opts,
         )
 
         # If destination bucket already exists, create a BucketDetails from its name
         if isinstance(destination_bucket, str):
@@ -70,37 +70,39 @@
                             "Effect": "Allow",
                             "Principal": {"Service": "lambda.amazonaws.com"},
                             "Action": "sts:AssumeRole",
                         }
                     ],
                 }
             ),
-            name=f"{name}-copy",
+            name=f"{name}-move",
             path="/service-role/",
-            tags=tagger.create_tags(f"{name}-copy"),
+            tags=tagger.create_tags(f"{name}-move"),
             opts=ResourceOptions(parent=self),
         )
         self._rolePolicy = RolePolicy(
             resource_name=f"{name}-role-policy",
             name="s3-access",
             policy=Output.all(source_bucket.arn, destination_bucket.arn, prefix).apply(
                 lambda args: json.dumps(
                     {
                         "Version": "2012-10-17",
                         "Statement": [
                             {
-                                "Sid": "GetSourceBucket",
+                                "Sid": "GetDeleteSourceBucket",
                                 "Effect": "Allow",
-                                "Resource": [f"{args[0]}/raw_history/{args[2]}/data/*"],
-                                "Action": ["s3:GetObject*"],
+                                "Resource": [f"{args[0]}/{args[2]}/*"]
+                                if args[2]
+                                else [f"{args[0]}/*"],
+                                "Action": ["s3:GetObject*", "s3:DeleteObject*"],
                             },
                             {
                                 "Sid": "PutDestinationBucket",
                                 "Effect": "Allow",
-                                "Resource": [f"{args[1]}/{args[2]}/data/*"],
+                                "Resource": [f"{args[1]}/*"],
                                 "Action": ["s3:PutObject*"],
                             },
                         ],
                     }
                 )
             ),
             role=self._role.id,
@@ -111,76 +113,50 @@
             policy_arn=(
                 "arn:aws:iam::aws:policy/service-role/AWSLambdaBasicExecutionRole"
             ),
             role=self._role.name,
             opts=ResourceOptions(parent=self._role),
         )
         self._function = Function(
-            resource_name=f"{name}-copy-function",
+            resource_name=f"{name}-function",
             code=AssetArchive(
                 assets={
-                    ".": FileArchive(path=str(Path(copy_.__file__).absolute().parent))
+                    ".": FileArchive(path=str(Path(move.__file__).absolute().parent))
                 }
             ),
             description=Output.all(source_bucket.name, destination_bucket.name).apply(
-                lambda args: f"Copies data from {args[0]} to {args[1]}"
+                lambda args: f"Moves data from {args[0]} to {args[1]}"
             ),
             environment=Output.all(destination_bucket.name).apply(
                 lambda args: FunctionEnvironmentArgs(
                     variables={"DESTINATION_BUCKET": args[0]}
                 )
             ),
-            handler="copy_.handler",
-            name=f"{name}-copy",
+            handler="move.handler",
+            name=f"{name}-move",
             role=self._role.arn,
             runtime="python3.8",
-            tags=tagger.create_tags(f"{name}-copy"),
+            tags=tagger.create_tags(f"{name}-move"),
             timeout=300,
             opts=ResourceOptions(parent=self),
         )
         self._permission = Permission(
-            resource_name=f"{name}-copy-permission",
+            resource_name=f"{name}-permission",
             action="lambda:InvokeFunction",
             function=self._function.arn,
             principal="s3.amazonaws.com",
             source_arn=source_bucket.arn,
             opts=ResourceOptions(parent=self._function),
         )
         if create_notification:
-            self._eventRule = EventRule(
-                resource_name=f"{prefix}-copy",
-                opts=ResourceOptions(parent=self),
-                name=f"{prefix}-copy",
-                description=f"Triggers the {name} lambda function to re-run "
-                f"validation and move files from raw history to curated for {prefix}",
-                event_pattern=Output.all(source_bucket.id, prefix).apply(
-                    lambda args: json.dumps(
-                        {
-                            "source": ["aws.s3"],
-                            "detail-type": ["Object Created"],
-                            "detail": {
-                                "bucket": {"name": [args[0]]},
-                                "object": {
-                                    "key": [{"prefix": f"raw_history/{prefix}/data"}]
-                                },
-                            },
-                        }
+            self._bucketNotification = BucketNotification(
+                resource_name=f"{name}-bucket-notification",
+                bucket=source_bucket.id,
+                lambda_functions=[
+                    BucketNotificationLambdaFunctionArgs(
+                        events=["s3:ObjectCreated:*"],
+                        lambda_function_arn=self._function.arn,
+                        filter_prefix=f"{prefix}/" if prefix else None,
                     )
-                ),
-                tags=tagger.create_tags(f"{prefix}"),
-            )
-
-            self._eventPermission = Permission(
-                resource_name=f"{name}-copy-event-permission",
-                action="lambda:InvokeFunction",
-                function=self._function.arn,
-                principal="events.amazonaws.com",
-                source_arn=self._eventRule.arn,
-                opts=ResourceOptions(parent=self._function),
-            )
-            self._eventTarget = EventTarget(
-                resource_name=f"{name}-copy",
-                opts=ResourceOptions(parent=self._eventRule),
-                arn=self._function.arn,
-                rule=self._eventRule.name,
-                input_path="$.detail",
+                ],
+                opts=ResourceOptions(parent=self._permission),
             )
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,96 +3,91 @@
 
 from data_engineering_pulumi_components.utils import Tagger
 
 from pulumi import AssetArchive, ComponentResource, FileArchive, ResourceOptions
 import pulumi_aws as aws
 from pulumi_aws.lambda_ import Function, FunctionEnvironmentArgs, Permission
 
-from data_engineering_pulumi_components.aws import get_databases
+from data_engineering_pulumi_components.aws import get_tables
 
 
-class GetDatabasesFunction(ComponentResource):
+class GetTablesFunction(ComponentResource):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
         bucket_name: str,
-        bucket_prefix: str,
         account_id: str,
         region: str,
         api: aws.apigateway,
         resource_path: str,
         lambda_role_arn: str,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         """
-        Provide a Lambda function that gets a list of all the databases in a bucket.
+        Provide a Lambda function that gets a list of all the tables in a database.
         Parameters
         ----------
         name : str
             The name of the resource.
         tagger : Tagger
             A tagger resource.
         bucket_name : str, Bucket
             The bucket to read data from.
-        bucket_prefix : str,
-            Sub folder the to read from.
         account_id : str,
             The account number for creation of resources.
         region : str,
             Region the resources to be created.
         api : aws.apigateway,
-            The API which uses the lambda to read the list of databases.
+            The API which uses the lambda to read the list of tables.
         resource_path : str,
             API resource path.
         lambda_role_arn : str
             Lambda role arn for the function to use. Should have ListBucket permission.
         opts : Optional[ResourceOptions]
             Options for the resource. By default, None.
         """
         super().__init__(
-            t="data-engineering-pulumi-components:aws:GetDatabasesFunction",
+            t="data-engineering-pulumi-components:aws:GetTablesFunction",
             name=name,
             props=None,
             opts=opts,
         )
 
         self._bucketname = bucket_name
-        self._bucket_prefix = bucket_prefix
         self._region = region
         self._account_id = account_id
         self._resource_path = resource_path
         self._lambda_role_arn = lambda_role_arn
 
         self.function = Function(
             resource_name=f"{name}-function",
             code=AssetArchive(
                 assets={
                     ".": FileArchive(
-                        path=str(Path(get_databases.__file__).absolute().parent)
+                        path=str(Path(get_tables.__file__).absolute().parent)
                     )
                 }
             ),
-            description="Create list of databases in a bucket.",
+            description="Create list of tables in a database.",
             role=self._lambda_role_arn,
-            handler="get_databases.handler",
+            handler="get_tables.handler",
             environment=FunctionEnvironmentArgs(
                 variables={
-                    "bucket_name": f"{self._bucketname}",
-                    "prefix": f"{self._bucket_prefix}",
+                    "bucket_name": f"{bucket_name}",
                 }
             ),
             runtime="python3.8",
-            tags=tagger.create_tags(f"{name}-get-databases"),
+            tags=tagger.create_tags(f"{name}-get-tables"),
             timeout=300,
             opts=ResourceOptions(parent=self),
         )
 
         self._permission = Permission(
-            resource_name=f"{name}-get-databases-permission",
+            resource_name=f"{name}-get-tables-permission",
             principal="apigateway.amazonaws.com",
             action="lambda:InvokeFunction",
             function=self.function.arn,
             source_arn=api.id.apply(
                 lambda api_id: f"arn:aws:execute-api:{self._region}:"
                 + f"{self._account_id}:{api_id}/*/GET/{self._resource_path}"
             ),
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/get_fields.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,95 @@
 from pathlib import Path
 from typing import Optional
+from data_engineering_pulumi_components.aws.lambdas.lambda_handlers.upload_ import (
+    upload_,
+)
 
 from data_engineering_pulumi_components.utils import Tagger
+
 from pulumi import AssetArchive, ComponentResource, FileArchive, ResourceOptions
 import pulumi_aws as aws
 from pulumi_aws.lambda_ import Function, FunctionEnvironmentArgs, Permission
-from data_engineering_pulumi_components.aws import get_fields
 
 
-class GetFieldsLambda(ComponentResource):
+class UploadObjectFunction(ComponentResource):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
-        glue_prefix: str,
-        account_id: str,
+        bucket_name: str,
+        accountid: str,
         region: str,
         api: aws.apigateway,
         resource_path: str,
         lambda_role_arn: str,
-        data_stack_provider,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         """
-        Provide a Lambda function that gets a list of all the fields in a table.
+        Provides a Lambda function that allows file upload
+        using presigned url
         Parameters
         ----------
         name : str
             The name of the resource.
         tagger : Tagger
             A tagger resource.
-        glue_prefix : str
-            Prefix to find the right db on glue
-        account_id : str,
-            The account number for creation of resources.
-        region : str,
-            Region the resources to be created.
-        api : aws.apigateway,
-            The API which uses the lambda to read the list of fields.
-        resource_path : str,
-            API resource path.
-        lambda_role_arn : str
-            Lambda role arn for the function to use.
+        bucket_name: str, : Bucket
+            The bucket to upload data to.
+        api :aws.apigateway,
+                The Api which use the lambda to upload
+        accountid: str,
+            The account number for creation of resource
+        region: str,
+            Region the resources to be created
+        resource_path: str,
+            Api Resource path
+        lambda_role_arn:str
+            Upload Lambda role arn
         opts : Optional[ResourceOptions]
             Options for the resource. By default, None.
         """
         super().__init__(
-            t="data-engineering-pulumi-components:aws:GetFieldsFunction",
+            t="data-engineering-pulumi-components:aws:UploadObjectFunction",
             name=name,
             props=None,
             opts=opts,
         )
 
-        self._glue_prefix = glue_prefix
+        self._bucketname = bucket_name
         self._region = region
-        self._account_id = account_id
+        self._accountid = accountid
         self._resource_path = resource_path
         self._lambda_role_arn = lambda_role_arn
 
         self.function = Function(
             resource_name=f"{name}-function",
             code=AssetArchive(
                 assets={
-                    ".": FileArchive(
-                        path=str(Path(get_fields.__file__).absolute().parent)
-                    )
+                    ".": FileArchive(path=str(Path(upload_.__file__).absolute().parent))
                 }
             ),
-            description="Return list of fields in a table.",
+            description="Generates presigned url and allows object upload to bucket ",
             role=self._lambda_role_arn,
-            handler="get_fields.handler",
+            handler="upload_.handler",
             environment=FunctionEnvironmentArgs(
-                variables={"glue_prefix": self._glue_prefix}
+                variables={
+                    "bucketname": f"{bucket_name}",
+                }
             ),
             runtime="python3.8",
-            tags=tagger.create_tags(f"{name}-get-fields"),
+            tags=tagger.create_tags(f"{name}-upload"),
             timeout=300,
-            opts=ResourceOptions(parent=self, provider=data_stack_provider),
+            opts=ResourceOptions(parent=self),
         )
 
         self._permission = Permission(
-            resource_name=f"{name}-get-fields-permission",
+            resource_name=f"{name}-permission",
             principal="apigateway.amazonaws.com",
             action="lambda:InvokeFunction",
             function=self.function.arn,
             source_arn=api.id.apply(
                 lambda api_id: f"arn:aws:execute-api:{self._region}:"
-                + f"{self._account_id}:{api_id}/*/GET/{self._resource_path}"
+                + f"{self._accountid}:{api_id}/*/GET/{self._resource_path}"
             ),
-            opts=ResourceOptions(parent=self.function, provider=data_stack_provider),
+            opts=ResourceOptions(parent=self.function),
         )
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,96 +3,91 @@
 
 from data_engineering_pulumi_components.utils import Tagger
 
 from pulumi import AssetArchive, ComponentResource, FileArchive, ResourceOptions
 import pulumi_aws as aws
 from pulumi_aws.lambda_ import Function, FunctionEnvironmentArgs, Permission
 
-from data_engineering_pulumi_components.aws import get_tables
+from data_engineering_pulumi_components.aws import get_databases
 
 
-class GetTablesFunction(ComponentResource):
+class GetDatabasesFunction(ComponentResource):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
         bucket_name: str,
-        bucket_prefix: str,
         account_id: str,
         region: str,
         api: aws.apigateway,
         resource_path: str,
         lambda_role_arn: str,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         """
-        Provide a Lambda function that gets a list of all the tables in a database.
+        Provide a Lambda function that gets a list of all the databases in a bucket.
         Parameters
         ----------
         name : str
             The name of the resource.
         tagger : Tagger
             A tagger resource.
         bucket_name : str, Bucket
             The bucket to read data from.
-        bucket_prefix : str,
-             Sub folder the to read from.
         account_id : str,
             The account number for creation of resources.
         region : str,
             Region the resources to be created.
         api : aws.apigateway,
-            The API which uses the lambda to read the list of tables.
+            The API which uses the lambda to read the list of databases.
         resource_path : str,
             API resource path.
         lambda_role_arn : str
             Lambda role arn for the function to use. Should have ListBucket permission.
         opts : Optional[ResourceOptions]
             Options for the resource. By default, None.
         """
         super().__init__(
-            t="data-engineering-pulumi-components:aws:GetTablesFunction",
+            t="data-engineering-pulumi-components:aws:GetDatabasesFunction",
             name=name,
             props=None,
             opts=opts,
         )
 
         self._bucketname = bucket_name
-        self._bucket_prefix = bucket_prefix
         self._region = region
         self._account_id = account_id
         self._resource_path = resource_path
         self._lambda_role_arn = lambda_role_arn
 
         self.function = Function(
             resource_name=f"{name}-function",
             code=AssetArchive(
                 assets={
                     ".": FileArchive(
-                        path=str(Path(get_tables.__file__).absolute().parent)
+                        path=str(Path(get_databases.__file__).absolute().parent)
                     )
                 }
             ),
-            description="Create list of tables in a database.",
+            description="Create list of databases in a bucket.",
             role=self._lambda_role_arn,
-            handler="get_tables.handler",
+            handler="get_databases.handler",
             environment=FunctionEnvironmentArgs(
                 variables={
-                    "bucket_name": f"{self._bucketname}",
-                    "prefix": f"{self._bucket_prefix}",
+                    "bucket_name": f"{bucket_name}",
                 }
             ),
             runtime="python3.8",
-            tags=tagger.create_tags(f"{name}-get-tables"),
+            tags=tagger.create_tags(f"{name}-get-databases"),
             timeout=300,
             opts=ResourceOptions(parent=self),
         )
 
         self._permission = Permission(
-            resource_name=f"{name}-get-tables-permission",
+            resource_name=f"{name}-get-databases-permission",
             principal="apigateway.amazonaws.com",
             action="lambda:InvokeFunction",
             function=self.function.arn,
             source_arn=api.id.apply(
                 lambda api_id: f"arn:aws:execute-api:{self._region}:"
                 + f"{self._account_id}:{api_id}/*/GET/{self._resource_path}"
             ),
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 
 
 def handler(event, context):
+
     # 1 - Log the event
     print("*********** The event is: ***************")
 
     authorizationToken = json.dumps(event["multiValueHeaders"]["authorisationToken"])
 
     characters_to_remove = '"[]"'
     for character in characters_to_remove:
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,43 +10,22 @@
         "s3", endpoint_url=f"http://{os.getenv('LOCALSTACK_HOSTNAME')}:4566"
     )
 else:
     client = boto3.client("s3")
 
 
 def handler(event, context):
-    if "moj-reg" not in os.environ["DESTINATION_BUCKET"]:
-        for record in event["Records"]:
-            source_bucket = record["s3"]["bucket"]["name"]
-            source_key = unquote_plus(record["s3"]["object"]["key"])
-            destination_bucket = os.environ["DESTINATION_BUCKET"]
-            destination_key = (
-                source_key.replace("raw_history/", "")
-                if "raw_history/" in source_key
-                else source_key
-            )
-
-            client.copy_object(
-                Bucket=destination_bucket,
-                CopySource={"Bucket": source_bucket, "Key": source_key},
-                Key=destination_key,
-                ServerSideEncryption="AES256",
-                ACL="bucket-owner-full-control",
-            )
-
-    if "moj-reg" in os.environ["DESTINATION_BUCKET"]:
-        source_bucket = event["bucket"]["name"]
-        source_key = unquote_plus(event["object"]["key"])
+    for record in event["Records"]:
+        source_bucket = record["s3"]["bucket"]["name"]
+        source_key = unquote_plus(record["s3"]["object"]["key"])
         destination_bucket = os.environ["DESTINATION_BUCKET"]
-        destination_key = (
-            source_key.replace("raw_history/", "")
-            if "raw_history/" in source_key
-            else source_key
-        )
+        destination_key = source_key
 
         client.copy_object(
             Bucket=destination_bucket,
             CopySource={"Bucket": source_bucket, "Key": source_key},
             Key=destination_key,
             ServerSideEncryption="AES256",
             ACL="bucket-owner-full-control",
         )
+
+        client.delete_object(Bucket=source_bucket, Key=source_key)
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 from typing import List
 
 import boto3
 from botocore.client import BaseClient
 from botocore.exceptions import ClientError, NoCredentialsError
 
 
-def get_s3_objects(client: BaseClient, bucket: str, prefix: str) -> List[str]:
-    """Get list of all objects in an S3 bucket (get keys).
+def get_s3_objects(client: BaseClient, bucket: str) -> List[str]:
+    """Get list of all objects in an S3 bucket.
     Parameters
     ----------
     client : S3
         Boto3 s3 client initialised with boto3.client("s3")
     bucket : str
         Name of the bucket to get objects from.
-    prefix : str
-        subfolder of the bucket to get objects from.
-
     Returns
     -------
     List
         List of S3 objects.
     """
     bucket_objects = []
     try:
-        response = client.list_objects_v2(Bucket=bucket, Prefix=prefix)
+        response = client.list_objects_v2(Bucket=bucket)
         if response.get("Contents"):
             for item in response["Contents"]:
                 bucket_objects.append(item["Key"])
         else:
             print("Bucket empty")
     except (ClientError, NoCredentialsError) as e:
         print(e)
@@ -52,39 +49,30 @@
     databases = set()
     for bucket_object in s3_objects:
         # Get database name from each file and add it to a set
         # NB hive partitioning used for defining directory hierarchy
         # hence split at "="
         try:
             components = bucket_object.split("/")
-            database_name = [
-                item.split("=")[1] for item in components if item.startswith("database")
-            ][0]
+            database_name = components[1].split("=")[1]
             databases.add(database_name)
         except IndexError:
             print(f"Could not split database name from {bucket_object}")
             continue
     return sorted(list(databases))
 
 
 def handler(event, context):
-    # The endpoint_url is only needed for when we run integration tests using localstack
-    endpoint_url = (
-        f"http://{os.getenv('LOCALSTACK_HOSTNAME')}:{os.getenv('EDGE_PORT')}"
-        if os.getenv("LOCALSTACK_HOSTNAME")
-        else None
-    )
-    s3 = boto3.client("s3", endpoint_url=endpoint_url)
+    s3 = boto3.client("s3")
 
     # Fetch bucket_name and file_name using proxy integration method from API Gateway
     bucket = os.environ["bucket_name"]
-    prefix = os.environ["prefix"]
 
     # Get list of objects from bucket and work out database names from them
-    s3_objects = get_s3_objects(s3, bucket, prefix)
+    s3_objects = get_s3_objects(s3, bucket)
     database_names = get_database_names(s3_objects)
 
     # Return API response json
     return {
         "statusCode": 200,
         "headers": {"Content-Type": "application/json"},
         "body": json.dumps({"databases": database_names}),
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,89 +3,77 @@
 from typing import List
 
 import boto3
 from botocore.client import BaseClient
 from botocore.exceptions import ClientError, NoCredentialsError
 
 
-def get_s3_objects(client: BaseClient, bucket: str, prefix: str) -> List[str]:
+def get_s3_objects(client: BaseClient, bucket: str) -> List[str]:
     """Get list of all objects in an S3 bucket.
     Parameters
     ----------
     client : S3
         Boto3 s3 client initialised with boto3.client("s3")
     bucket : str
         Name of the bucket to get objects from.
-    prefix : str
-        subfolder of the bucket to get objects from.
     Returns
     -------
     List
         List of S3 objects.
     """
     bucket_objects = []
     try:
-        response = client.list_objects_v2(Bucket=bucket, Prefix=prefix)
+        response = client.list_objects_v2(Bucket=bucket)
         if response.get("Contents"):
             for item in response["Contents"]:
                 bucket_objects.append(item["Key"])
         else:
             print("Bucket empty")
     except (ClientError, NoCredentialsError) as e:
         print(e)
         raise
 
     return bucket_objects
 
 
-def get_table_names(s3_objects: List[str], database_name: str) -> List[str]:
+def get_table_names(s3_objects: List[str], database: str) -> List[str]:
     """Get table names for a specific database in the S3 object list
     Parameters
     ----------
     s3_objects : list
         List of keys of objects in the bucket.
-    database_name : str
+    database : str
         Name of the database to list tables from.
     Returns
     -------
     List
         Sorted list of table names.
     """
     # Get all the bucket objects
     tables = set()
     for bucket_object in s3_objects:
         # Get table name for all objects with matching database name
         try:
-            if (
-                f"database={database_name}" in bucket_object
-                or f"database_name={database_name}" in bucket_object
-            ):
-                components = bucket_object.split("/")
-                table_name = [
-                    item.split("=")[1]
-                    for item in components
-                    if item.startswith("table")
-                ][0]
-                print(table_name)
-                tables.add(table_name)
+            components = bucket_object.split("/")
+            if components[1].split("=")[1] == database:
+                tables.add(components[2].split("=")[1])
         except IndexError:
             print(f"Could not split database and table name from {bucket_object}")
             continue
     return sorted(list(tables))
 
 
 def handler(event, context):
     s3 = boto3.client("s3")
 
     # Fetch bucket_name and file_name using proxy integration method from API Gateway
     bucket = os.environ["bucket_name"]
-    prefix = os.environ["prefix"]
 
     # Get list of objects from bucket
-    s3_objects = get_s3_objects(s3, bucket, prefix)
+    s3_objects = get_s3_objects(s3, bucket)
 
     # Try to get database name from the API request
     try:
         database_name = event["queryStringParameters"]["databasename"]
     except TypeError:  # will try None["databasename"] if no databasename provided
         return {
             "statusCode": 404,
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,9 +23,7 @@
         client.copy_object(
             Bucket=destination_bucket,
             CopySource={"Bucket": source_bucket, "Key": source_key},
             Key=destination_key,
             ServerSideEncryption="AES256",
             ACL="bucket-owner-full-control",
         )
-
-        client.delete_object(Bucket=source_bucket, Key=source_key)
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,18 @@
-import datetime
-import fnmatch
-import json
-import logging
 import os
 from urllib.parse import unquote_plus
-import functools
-from typing import Callable
-
-import boto3
 from urllib3 import PoolManager
+import boto3
+import s3fs
+import fnmatch
+import json
+import datetime
 
 client = boto3.client("s3")
-
-logging.basicConfig(level=logging.INFO, force=True)
-root_logger = logging.getLogger()
-
-
-def validate_object(func: Callable) -> Callable:
-    """
-    This simple function will just check to see if the key in the bucket exists,
-    before executing the func
-    """
-
-    @functools.wraps(func)
-    def wrapper_decorator(*args, **kwargs):
-        source_bucket = kwargs["source_bucket"]
-        source_key = kwargs["source_key"]
-
-        s3 = boto3.client("s3")
-        response = s3.list_objects_v2(Bucket=source_bucket)
-        try:
-            response["Contents"]
-        except KeyError:
-            root_logger.info(f"Bucket {source_bucket} is empty")
-            raise
-
-        keys = [key_info["Key"] for key_info in response["Contents"]]
-        if source_key not in keys:
-            root_logger.info(
-                f"The file {source_key} does not exist in bucket {source_bucket}"
-            )
-        return func(*args, **kwargs)
-
-    return wrapper_decorator
+fs = s3fs.S3FileSystem()
 
 
 def validate_folder_structure(key: str):
     """The function will validate the folder structure (prefix) of S3 objects in the
     landing bucket to ensure they conform to the structure required by downstream
     processes.
     Parameters
@@ -60,16 +26,15 @@
         "metadata/database_name=*/table_name=db_and_table_list/extraction_timestamp=*",
     ]
     for prefix in valid_prefixes:
         if fnmatch.fnmatch(key, prefix):
             return True
 
 
-@validate_object
-def move_object(source_bucket: str, source_key: str, destination_bucket: str):
+def move_object(destination_bucket: str, source_bucket: str, source_key: str):
     """The function will copy the object in S3 to the "destination_bucket" bucket,
     while adding a timestamp to the filename. It will then
     delete the original object from "source_bucket".
     Parameters
     ----------
     destination_bucket : str
         The bucket where the S3 object will be copied to.
@@ -140,23 +105,23 @@
                         ),
                     },
                 },
             ],
         }
         encoded_payload = json.dumps(payload).encode("utf-8")
         response = http.request(method="POST", url=url, body=encoded_payload)
-        root_logger.info(
+        print(
             {
                 "message": payload,
                 "status_code": response.status,
                 "response": response.data,
             }
         )
     except Exception as e:
-        root_logger.error(f"Failed to send an alert to Slack: {e}")
+        print(f"Failed to send an alert to Slack: {e}")
 
 
 class EmptyFileError(Exception):
     """Raised when the file opened has no contents"""
 
     pass
 
@@ -227,15 +192,15 @@
         size : int
             The size of the file being validated.
         """
         if validate_folder_structure(self.key) is not True:
             self._add_error(error=f"'{self.key}' Folder structure is invalid")
         elif self.size < 1:
             self._add_error(error=f"'{self.key}' File has no content")
-            root_logger.error(self.key, self.size)
+            print(self.key, self.size)
 
     def execute(self):
         self._validate_file(self.key, self.size)
         if len(self.errors) > 0:
             error = ", ".join(map(str, self.errors))
             move_object(
                 destination_bucket=self.fail_bucket,
@@ -250,66 +215,59 @@
                 msg=f"File {self.key} failed validation, Error - {error}",
                 user="AWS Lambda",
                 icon=":lambda:",
             )
             return {"validation_outcome": "Fail"}
         else:
             move_object(
+                destination_bucket=self.pass_bucket,
                 source_bucket=self.source_bucket,
                 source_key=self.key,
-                destination_bucket=self.pass_bucket,
             )
             return {"validation_outcome": "Pass"}
 
 
 def handler(event, context):
-    def log_status(
-        validator_dict: dict, source_bucket: str, key: str, size: str
-    ) -> None:
-        root_logger.info(f"s3 source: {source_bucket}")
-        root_logger.info(f"s3 key: {key}")
-        root_logger.info(f"file size: {size}")
-        root_logger.info(f"validation status: {validator_dict['validation_outcome']}")
 
     if event.get("scheduled_event"):
         source_bucket = os.environ["SOURCE_BUCKET"]
         bucket_objects = client.list_objects_v2(Bucket=source_bucket)
         if bucket_objects["KeyCount"] > 0:
             paginator = client.get_paginator("list_objects_v2")
             pages = paginator.paginate(Bucket=source_bucket)
             for page in pages:
                 for obj in page["Contents"]:
                     pass_bucket = os.environ["PASS_BUCKET"]
                     fail_bucket = os.environ["FAIL_BUCKET"]
                     key = obj["Key"]
                     size = obj["Size"]
+
                     fileValidator = FileValidator(
                         key=key,
                         size=size,
                         pass_bucket=pass_bucket,
                         fail_bucket=fail_bucket,
                         source_bucket=source_bucket,
                     )
-                    root_logger.info(f"s3 key: {key}")
-                    val_dict = fileValidator.execute()
-                    log_status(val_dict, source_bucket, key, size)
+
+                    fileValidator.execute()
 
     elif event.get("Records"):
         for record in event["Records"]:
             source_bucket = record["s3"]["bucket"]["name"]
             pass_bucket = os.environ["PASS_BUCKET"]
             fail_bucket = os.environ["FAIL_BUCKET"]
             key = unquote_plus(record["s3"]["object"]["key"])
             size = record["s3"]["object"]["size"]
+
             fileValidator = FileValidator(
                 key=key,
                 size=size,
                 pass_bucket=pass_bucket,
                 fail_bucket=fail_bucket,
                 source_bucket=source_bucket,
             )
-            root_logger.info(f"s3 key: {key}")
-            val_dict = fileValidator.execute()
-            log_status(val_dict, source_bucket, key, size)
+
+            fileValidator.execute()
 
     else:
         raise KeyError
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/lambdas/validate_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/validate_function.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         )
         self._function = Function(
             resource_name=f"{name}-function",
             code=AssetArchive(
                 assets={
                     ".": FileArchive(
                         str(Path(__file__).parent.absolute())
-                        + "/lambda_handlers/validate/dependencies.zip"
+                        + "/lambda_handlers/validate/dependencies.tar.gz"
                     ),
                     "validate.py": FileAsset(
                         str(Path(__file__).parent.absolute())
                         + "/lambda_handlers/validate/validate.py"
                     ),
                 }
             ),
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/rest_apigateway.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/rest_apigateway.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
+
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ComponentResource, ResourceOptions
 import pulumi_aws as aws
-import hashlib
 
 
 class RestApigatewayService(ComponentResource):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
@@ -115,25 +115,13 @@
         # List all components to be created before the deployment
         # Resources and methods not needed, as their integrations already depend on them
         # But not all integrations need a response200, so list both here
         dependencies = list(self._integrations.values()) + list(
             self._response200.values()
         )
 
-        # Redeployment is triggered when there's a change in method or resource
-        redeployment_trigger = hashlib.sha1(
-            str(list(self._methods.keys()) + list(self._resources.keys())).encode()
-        ).hexdigest()
-
         self._deployment = aws.apigateway.Deployment(
             f"{self._name}-deployment",
-            rest_api=self._api.id,
-            triggers={"redeployment": redeployment_trigger},
-            opts=ResourceOptions(depends_on=dependencies),
-        )
-
-        self._stage = aws.apigateway.Stage(
-            f"{self._name}-stage",
-            deployment=self._deployment.id,
-            rest_api=self._api.id,
+            rest_api=self._api,
             stage_name=stage_name,
+            opts=ResourceOptions(depends_on=dependencies),
         )
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,47 +9,37 @@
 
 class CreateListBucketRole(ComponentResource):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
         bucket_name: str,
-        prefix: str,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         """
         Role to allow lambda to list databases and tables in an s3 bucket.
 
         name : str
             The name of the resource.
         tagger : Tagger
             A tagger resource.
         bucket_name: str,
-            Name of the bucket to enble list permission
-        prefix: str,
-             prefix of the bucket to enble list permission
+            Name of the bucket to enble upload permission
         opts : Optional[ResourceOptions]
             Options for the resource. By default, None.
         """
 
         super().__init__(
             t="data-engineering-pulumi-components:aws:CreateListRole",
             name=name,
             props=None,
             opts=opts,
         )
 
         self._bucketname = bucket_name
-        self._prefix = prefix
-        self._resourcelist = [f"arn:aws:s3:::{self._bucketname}"]
-        if self._prefix != "":
-            self._resourcelist.append(f"arn:aws:s3:::{self._bucketname}/{self._prefix}")
-            self._resourcelist.append(
-                f"arn:aws:s3:::{self._bucketname}/{self._prefix}/*"
-            )
         self.lambdarole = Role(
             resource_name=f"{name}-lambda-role",
             assume_role_policy=json.dumps(
                 {
                     "Version": "2012-10-17",
                     "Statement": [
                         {
@@ -72,18 +62,16 @@
             policy=json.dumps(
                 {
                     "Version": "2012-10-17",
                     "Statement": [
                         {
                             "Action": [
                                 "s3:ListBucket",
-                                "s3:GetObjectAcl",
-                                "s3:GetObject",
                             ],
-                            "Resource": self._resourcelist,
+                            "Resource": f"arn:aws:s3:::{self._bucketname}",
                             "Effect": "Allow",
                         }
                     ],
                 }
             ),
             role=self.lambdarole.id,
             opts=ResourceOptions(parent=self.lambdarole),
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/aws/roles/create_upload_role.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_upload_role.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     def __init__(
         self,
         name: str,
         aws_arn_for_put_permission: str,
         tagger: Tagger,
         slack_channel: str,
         slack_webhook_url: str,
-        lifecycle_rules_expiration_days: dict = {},
         move_on_object_create: bool = True,
         move_on_schedule: bool = True,
         schedule: str = None,
         cors_allowed_headers: list = None,
         cors_allowed_origins: list = None,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
@@ -36,24 +35,22 @@
             opts=opts,
         )
 
         self._landing_bucket = LandingBucket(
             name=name,
             aws_arn_for_put_permission=aws_arn_for_put_permission,
             tagger=tagger,
-            lifecycle_rules_expiration_days=lifecycle_rules_expiration_days,
             cors_allowed_headers=cors_allowed_headers,
             cors_allowed_origins=cors_allowed_origins,
             opts=ResourceOptions(parent=self),
         )
 
         self._raw_history_bucket = RawHistoryBucket(
             name=name,
             tagger=tagger,
-            lifecycle_rules_expiration_days=lifecycle_rules_expiration_days,
             opts=ResourceOptions(parent=self),
         )
 
         self._fail_bucket = FailBucket(
             name=name,
             tagger=tagger,
             opts=ResourceOptions(parent=self),
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,42 +19,38 @@
 
 class RawHistoryToCuratedPipeline(ComponentResource):
     def __init__(
         self,
         name: str,
         raw_history_bucket: RawHistoryBucket,
         tagger: Tagger,
-        lifecycle_rules_expiration_days: dict = {},
         add_tables_to_db: bool = False,
         default_provider: Optional[Provider] = None,
         stack_provider: Optional[Provider] = None,
         opts: Optional[ResourceOptions] = None,
         db_refresh_schedule: bool = True,
         db_refresh_on_create: bool = False,
         block_access: bool = True,
         high_memory_worker: bool = False,
         number_of_workers: int = 2,
         allow_data_conversion: str = "True",
         multiple_db_in_bucket: str = "False",
-        webhook_url: str = "",
-        slack_channel: str = "",
     ) -> None:
         super().__init__(
             t=(
                 "data-engineering-pulumi-components:pipelines:"
                 "RawHistoryToCuratedPipeline"
             ),
             name=name,
             props=None,
             opts=opts,
         )
         self._curatedBucket = CuratedBucket(
             name=name,
             tagger=tagger,
-            lifecycle_rules_expiration_days=lifecycle_rules_expiration_days,
             provider=stack_provider,
             opts=ResourceOptions(parent=self, provider=stack_provider),
         )
         if add_tables_to_db is False:
             self._copyObjectFunction = CopyObjectFunction(
                 destination_bucket=self._curatedBucket,
                 name=name,
@@ -66,15 +62,14 @@
             bpb = BucketPolicyBuilder(
                 Bucket=self._curatedBucket,
                 put_permissions=[
                     BucketPutPermissionsArgs(
                         principal=self._copyObjectFunction._role.arn
                     )
                 ],
-                provider=stack_provider,
             )
             if block_access is True:
                 self._curatedBucket._bucketPolicy = (
                     bpb.add_basic_access_permissions.add_access_block.build()
                 )
             if block_access is False:
                 self._curatedBucket._bucketPolicy = (
@@ -86,36 +81,36 @@
 
             if multiple_db_in_bucket == "False":
                 db_name = name.replace("-", "_")
                 self._database = CatalogDatabase(
                     resource_name=f"{name}-database",
                     description=f"A Glue Database for tables from {name}",
                     name=f"{db_name}",
-                    opts=ResourceOptions(provider=default_provider, retain_on_delete=True),
+                    opts=ResourceOptions(provider=default_provider),
                 )
 
             self._glueMoveJob = GlueComponent(
                 destination_bucket=self._curatedBucket,
                 name=name,
                 source_bucket=raw_history_bucket,
                 tagger=tagger,
                 glue_script=(
                     os.path.join(
                         Path(__file__).parents[1],
                         "aws/glue/glue_move_script.py",
                     )
                 ),
                 glue_inputs={
+                    "--job-bookmark-option": "job-bookmark-enable",
+                    "--enable-metrics": "",
                     "--source_bucket": raw_history_bucket._name,
                     "--destination_bucket": self._curatedBucket._name,
                     "--stack_name": name,
                     "--multiple_db_in_bucket": multiple_db_in_bucket,
                     "--allow_data_conversion": allow_data_conversion,
-                    "--webhook_url": webhook_url,
-                    "--channel": slack_channel,
                 },
                 default_provider=default_provider,
                 stack_provider=stack_provider,
                 opts=ResourceOptions(
                     parent=self,
                     depends_on=[self._curatedBucket],
                 ),
@@ -133,14 +128,8 @@
             ).add_glue_permissions.build()
 
             self._curatedBucket._bucketPolicy = BucketPolicyBuilder(
                 Bucket=self._curatedBucket,
                 put_permissions=[
                     BucketPutPermissionsArgs(principal=self._glueMoveJob._role.arn)
                 ],
-                provider=stack_provider,
             ).add_glue_permissions.build()
-
-        if add_tables_to_db is False:
-            raw_history_bucket._bucketPolicy = BucketPolicyBuilder(
-                Bucket=raw_history_bucket
-            ).build()
```

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/data_engineering_pulumi_components/utils.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/utils.py`

 * *Files identical despite different names*

### Comparing `data_engineering_pulumi_components-0.4.1.dev66/PKG-INFO` & `data-engineering-pulumi-components-0.4.1.dev7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: data-engineering-pulumi-components
-Version: 0.4.1.dev66
+Version: 0.4.1.dev7
 Summary: Reusable components for use in Pulumi Python projects
 License: MIT
 Author: MoJ Data Engineering Team
 Author-email: data-engineering@digital.justice.gov.uk
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.26.42,<2.0.0)
+Requires-Dist: boto3 (>=1.17.00,<2.0.0)
 Requires-Dist: protobuf (>=4.21.5,<5.0.0)
-Requires-Dist: pulumi (==3.40.0)
-Requires-Dist: pulumi-auth0 (>=2.14.0,<3.0.0)
-Requires-Dist: pulumi-aws (>=5.25.0,<6.0.0)
+Requires-Dist: pulumi (>=3.38.0,<4.0.0)
+Requires-Dist: pulumi-auth0 (>=2.13.0,<3.0.0)
+Requires-Dist: pulumi-aws (>=5.0.0,<6.0.0)
```

