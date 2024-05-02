# Comparing `tmp/elements-sdk-3.6.0.tar.gz` & `tmp/elements-sdk-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-sdk-3.6.0.tar", last modified: Fri Dec  2 15:41:08 2022, max compression
+gzip compressed data, was "elements-sdk-3.6.1.tar", last modified: Mon Jan 23 14:30:42 2023, max compression
```

## Comparing `elements-sdk-3.6.0.tar` & `elements-sdk-3.6.1.tar`

### file list

```diff
@@ -1,938 +1,938 @@
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.867518 elements-sdk-3.6.0/
--rw-r--r--   0 eugene     (501) staff       (20)     1065 2021-01-28 11:22:09.000000 elements-sdk-3.6.0/LICENSE
--rw-r--r--   0 eugene     (501) staff       (20)      387 2022-12-02 15:41:08.867596 elements-sdk-3.6.0/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)    97694 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/README.md
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.646061 elements-sdk-3.6.0/elements_sdk/
--rw-r--r--   0 eugene     (501) staff       (20)      751 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/__init__.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.658613 elements-sdk-3.6.0/elements_sdk/api/
--rw-r--r--   0 eugene     (501) staff       (20)      211 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)   226652 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/ai_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   161652 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/auth_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   218625 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/automation_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    41799 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/aws_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    65079 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/click_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   106050 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/integrations_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   635911 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/main_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   939194 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/media_library_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    67975 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/private_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    39335 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/satellite_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    20596 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/sharedstorage_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    30350 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/status_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   380791 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/storage_api.py
--rw-r--r--   0 eugene     (501) staff       (20)   171030 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api/tape_archive_api.py
--rw-r--r--   0 eugene     (501) staff       (20)    37713 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/api_client.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.659665 elements-sdk-3.6.0/elements_sdk/apis/
--rw-r--r--   0 eugene     (501) staff       (20)     1147 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/apis/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)    17110 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/configuration.py
--rw-r--r--   0 eugene     (501) staff       (20)     5089 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/exceptions.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.775553 elements-sdk-3.6.0/elements_sdk/model/
--rw-r--r--   0 eugene     (501) staff       (20)      348 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/model/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)    11151 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/add_assets_to_click_gallery.py
--rw-r--r--   0 eugene     (501) staff       (20)    12386 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/address.py
--rw-r--r--   0 eugene     (501) staff       (20)    14281 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_annotation.py
--rw-r--r--   0 eugene     (501) staff       (20)    12777 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_annotation_create_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    13080 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_annotation_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13419 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_annotation_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12310 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_category.py
--rw-r--r--   0 eugene     (501) staff       (20)    12612 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_category_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)    11668 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_category_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11719 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_category_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11401 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_category_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11350 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)    11909 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset.py
--rw-r--r--   0 eugene     (501) staff       (20)    12911 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_detail_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11181 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_export_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11293 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_export_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11972 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    13767 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_with_preview.py
--rw-r--r--   0 eugene     (501) staff       (20)    11723 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_with_preview_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11792 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_dataset_with_preview_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12960 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_image.py
--rw-r--r--   0 eugene     (501) staff       (20)    13120 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_image_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    12764 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)    14455 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model.py
--rw-r--r--   0 eugene     (501) staff       (20)    11175 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_export_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11287 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_export_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    12369 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_inference_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11242 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_inference_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    13041 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11408 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_progress.py
--rw-r--r--   0 eugene     (501) staff       (20)    12223 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_training_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    13140 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_model_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11880 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/ai_processing_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    13647 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/alert.py
--rw-r--r--   0 eugene     (501) staff       (20)    11887 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/alert_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11986 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/alert_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11183 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/all_media_files_for_bundles_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11339 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/api_token.py
--rw-r--r--   0 eugene     (501) staff       (20)    11168 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/api_token_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11189 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/api_token_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11614 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/api_token_with_secret.py
--rw-r--r--   0 eugene     (501) staff       (20)    11464 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/api_token_with_secret_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12700 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/archive_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11574 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/argument_type.py
--rw-r--r--   0 eugene     (501) staff       (20)    18513 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset.py
--rw-r--r--   0 eugene     (501) staff       (20)    12326 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_backup.py
--rw-r--r--   0 eugene     (501) staff       (20)    12356 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_cloud_link.py
--rw-r--r--   0 eugene     (501) staff       (20)    13232 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    13420 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11561 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12042 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_project_link.py
--rw-r--r--   0 eugene     (501) staff       (20)    12235 2022-12-02 15:38:53.000000 elements-sdk-3.6.0/elements_sdk/model/asset_rating.py
--rw-r--r--   0 eugene     (501) staff       (20)    11871 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/asset_rating_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11910 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/asset_rating_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12384 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/asset_subtitle_link.py
--rw-r--r--   0 eugene     (501) staff       (20)    12119 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/asset_subtitle_link_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12206 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/asset_subtitle_link_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11648 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/asset_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12060 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/auth_login_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12135 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/auth_login_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11625 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/backend.py
--rw-r--r--   0 eugene     (501) staff       (20)    14846 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/backend_properties.py
--rw-r--r--   0 eugene     (501) staff       (20)    12418 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/basic_file.py
--rw-r--r--   0 eugene     (501) staff       (20)    12001 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/bee_gfs_node.py
--rw-r--r--   0 eugene     (501) staff       (20)    13433 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/bee_gfs_target.py
--rw-r--r--   0 eugene     (501) staff       (20)    20604 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/bootstrap_data.py
--rw-r--r--   0 eugene     (501) staff       (20)    13329 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/certificate.py
--rw-r--r--   0 eugene     (501) staff       (20)    11423 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/certificate_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11944 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/change_own_password_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11226 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/change_password_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11407 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/check_connectivity_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11859 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/click_background_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11849 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/click_gallery.py
--rw-r--r--   0 eugene     (501) staff       (20)    13173 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/click_gallery_link.py
--rw-r--r--   0 eugene     (501) staff       (20)    11415 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/click_gallery_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12072 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/click_link_user.py
--rw-r--r--   0 eugene     (501) staff       (20)    11431 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/click_start_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12613 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/client_session.py
--rw-r--r--   0 eugene     (501) staff       (20)    11642 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/client_side_path_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11337 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/client_side_path_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    12117 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/clients_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    13371 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_account.py
--rw-r--r--   0 eugene     (501) staff       (20)    11722 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_account_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    11551 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_account_mini_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11572 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_account_mini_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13200 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_account_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13221 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_account_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11827 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_bucket_costs.py
--rw-r--r--   0 eugene     (501) staff       (20)    11913 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)    12996 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_mount_authorization.py
--rw-r--r--   0 eugene     (501) staff       (20)    11634 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cloud_storage_costs.py
--rw-r--r--   0 eugene     (501) staff       (20)    14796 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/comment.py
--rw-r--r--   0 eugene     (501) staff       (20)    13963 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/comment_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13990 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/comment_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11393 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cost.py
--rw-r--r--   0 eugene     (501) staff       (20)    12226 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/cpu_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)    11936 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/create_download_archive.py
--rw-r--r--   0 eugene     (501) staff       (20)    11154 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/create_home_workspace_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11166 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/create_path_quota_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11735 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/create_template_folder_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    16278 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/custom_field.py
--rw-r--r--   0 eugene     (501) staff       (20)    16013 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/custom_field_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    16827 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/custom_field_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    16100 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/custom_field_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11414 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/deleted_workspace.py
--rw-r--r--   0 eugene     (501) staff       (20)    12216 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/download.py
--rw-r--r--   0 eugene     (501) staff       (20)    13615 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/download_archive.py
--rw-r--r--   0 eugene     (501) staff       (20)    12346 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/download_archive_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12421 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/download_archive_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12445 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/editor_project.py
--rw-r--r--   0 eugene     (501) staff       (20)    12424 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/editor_project_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12463 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/editor_project_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12165 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/editor_subtitle.py
--rw-r--r--   0 eugene     (501) staff       (20)    12138 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/editor_subtitle_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12183 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/editor_subtitle_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    14650 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_group.py
--rw-r--r--   0 eugene     (501) staff       (20)    14974 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_group_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)    13216 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_group_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13237 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_group_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    14922 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_group_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    21245 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user.py
--rw-r--r--   0 eugene     (501) staff       (20)    21491 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)    18409 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    18532 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12861 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    13082 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    14860 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_profile.py
--rw-r--r--   0 eugene     (501) staff       (20)    12418 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_profile_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12397 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_profile_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    22210 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_user_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    12423 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/elements_version.py
--rw-r--r--   0 eugene     (501) staff       (20)    11123 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/email_preview.py
--rw-r--r--   0 eugene     (501) staff       (20)    11393 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/enable_totp_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12594 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/event.py
--rw-r--r--   0 eugene     (501) staff       (20)    12325 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/external_transcoder.py
--rw-r--r--   0 eugene     (501) staff       (20)    12058 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/external_transcoder_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12175 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/external_transcoder_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11453 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/extract_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12551 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_copy_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11327 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_delete_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12060 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_move_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    16177 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11492 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_size_distribution.py
--rw-r--r--   0 eugene     (501) staff       (20)    12142 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_size_distribution_item.py
--rw-r--r--   0 eugene     (501) staff       (20)    11192 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_size_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11390 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_unzip_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    16222 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11639 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/file_zip_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    17763 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/filesystem_file.py
--rw-r--r--   0 eugene     (501) staff       (20)    12007 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/filesystem_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)    11836 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/filesystem_permission_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11857 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/filesystem_permission_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11188 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/filesystem_trace_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12095 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/filesystem_trace_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11184 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/finish_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12297 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/format_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)    14478 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/fs_properties.py
--rw-r--r--   0 eugene     (501) staff       (20)    11259 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/generate_password_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    12081 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/generate_proxies_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11736 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/get_cloud_account_costs_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11219 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/get_cloud_account_volume_sizes_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11297 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/get_multiple_bundles_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11140 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/elements_sdk/model/get_multiple_files_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11148 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/global_alert.py
--rw-r--r--   0 eugene     (501) staff       (20)    11175 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/help_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11205 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/image_upload_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11138 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/impersonation_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11947 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/import_ai_dataset_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11350 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/import_ai_dataset_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11175 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/import_ai_model_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11308 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/import_ai_model_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11709 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/import_job_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11245 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/import_job_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    12014 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/inline_response200.py
--rw-r--r--   0 eugene     (501) staff       (20)    11549 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/install_license_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11700 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/instantiate_file_template_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    13243 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/interface.py
--rw-r--r--   0 eugene     (501) staff       (20)    11525 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/io_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)    11677 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ipmi.py
--rw-r--r--   0 eugene     (501) staff       (20)    17329 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/job.py
--rw-r--r--   0 eugene     (501) staff       (20)    16502 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/job_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    17973 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/job_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    16523 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/job_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12220 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/kapacitor_alert.py
--rw-r--r--   0 eugene     (501) staff       (20)    11842 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ldap_server.py
--rw-r--r--   0 eugene     (501) staff       (20)    11807 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ldap_server_group.py
--rw-r--r--   0 eugene     (501) staff       (20)    11350 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ldap_server_groups.py
--rw-r--r--   0 eugene     (501) staff       (20)    11952 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ldap_server_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11934 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ldap_server_user.py
--rw-r--r--   0 eugene     (501) staff       (20)    11329 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ldap_server_users.py
--rw-r--r--   0 eugene     (501) staff       (20)    15113 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/license.py
--rw-r--r--   0 eugene     (501) staff       (20)    11112 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/list_topics.py
--rw-r--r--   0 eugene     (501) staff       (20)    14119 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/lizard_fs_disk.py
--rw-r--r--   0 eugene     (501) staff       (20)    13616 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/lizard_fs_node.py
--rw-r--r--   0 eugene     (501) staff       (20)    11213 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/locale_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11319 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/locate_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11155 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/locate_proxies_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11867 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/locate_proxies_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11806 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/locate_result.py
--rw-r--r--   0 eugene     (501) staff       (20)    12822 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/marker.py
--rw-r--r--   0 eugene     (501) staff       (20)    11808 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/marker_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11865 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/marker_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    18716 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file.py
--rw-r--r--   0 eugene     (501) staff       (20)    13517 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_bundle.py
--rw-r--r--   0 eugene     (501) staff       (20)    12246 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_bundle_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    12266 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_bundle_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11835 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_contents.py
--rw-r--r--   0 eugene     (501) staff       (20)    14014 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    12247 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    19647 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11796 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_template.py
--rw-r--r--   0 eugene     (501) staff       (20)    11613 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_template_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11646 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_template_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12226 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_file_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11196 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_files_lookup_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12240 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_library_delete_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    13429 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_library_share_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    20305 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root.py
--rw-r--r--   0 eugene     (501) staff       (20)    20832 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)    19657 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    19702 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12965 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    13133 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    17355 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)    15555 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_permission_access_options.py
--rw-r--r--   0 eugene     (501) staff       (20)    16979 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_permission_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    17000 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_permission_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    19456 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_root_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    14529 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/media_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11675 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/member_preview.py
--rw-r--r--   0 eugene     (501) staff       (20)    11756 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/metadata_item.py
--rw-r--r--   0 eugene     (501) staff       (20)    11559 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/move_workspace_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11145 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/multiple_assets_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11953 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/net_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)    11689 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/nfs_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)    11665 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ntp_server.py
--rw-r--r--   0 eugene     (501) staff       (20)    11476 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ntp_server_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11515 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ntp_server_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    16297 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/one_time_access_token.py
--rw-r--r--   0 eugene     (501) staff       (20)    11744 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/one_time_access_token_activity.py
--rw-r--r--   0 eugene     (501) staff       (20)    11373 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/one_time_access_token_shared_object.py
--rw-r--r--   0 eugene     (501) staff       (20)    19557 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/parameters.py
--rw-r--r--   0 eugene     (501) staff       (20)    19575 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/parameters_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11184 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/parse_samlidp_metadata_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12117 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/parsed_samlidp_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)    11510 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/password_reset_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11127 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/path.py
--rw-r--r--   0 eugene     (501) staff       (20)    11098 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/path_input.py
--rw-r--r--   0 eugene     (501) staff       (20)    13536 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/production.py
--rw-r--r--   0 eugene     (501) staff       (20)    11690 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/production_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    12626 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/production_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13877 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/production_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    12647 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/production_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    14118 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy.py
--rw-r--r--   0 eugene     (501) staff       (20)    11095 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_count.py
--rw-r--r--   0 eugene     (501) staff       (20)    11168 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_fs_size_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11923 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_generator.py
--rw-r--r--   0 eugene     (501) staff       (20)    13506 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_generator_properties.py
--rw-r--r--   0 eugene     (501) staff       (20)    19556 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_profile.py
--rw-r--r--   0 eugene     (501) staff       (20)    11362 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_profile_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    19385 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_profile_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    19406 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/proxy_profile_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11680 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/python_environment.py
--rw-r--r--   0 eugene     (501) staff       (20)    12651 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/queue.py
--rw-r--r--   0 eugene     (501) staff       (20)    11547 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/quota.py
--rw-r--r--   0 eugene     (501) staff       (20)    12030 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/ram_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)    13093 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/rdc_activation.py
--rw-r--r--   0 eugene     (501) staff       (20)    11947 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/rdc_host.py
--rw-r--r--   0 eugene     (501) staff       (20)    12165 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/rdc_session.py
--rw-r--r--   0 eugene     (501) staff       (20)    11561 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/rdc_session_create.py
--rw-r--r--   0 eugene     (501) staff       (20)    11513 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/register_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11380 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/register_upload_metadata_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11486 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/release_notes_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11187 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/rename_custom_field_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12201 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/render_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11238 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/render_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12826 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/restore_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    15247 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saml_provider.py
--rw-r--r--   0 eugene     (501) staff       (20)    11767 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saml_provider_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    14078 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saml_provider_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    14213 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saml_provider_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12765 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saved_search.py
--rw-r--r--   0 eugene     (501) staff       (20)    11938 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saved_search_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11977 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/saved_search_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11444 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/scanner_discover_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11910 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/scanner_scan_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    14614 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/schedule.py
--rw-r--r--   0 eugene     (501) staff       (20)    14242 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/schedule_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    15115 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/schedule_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    14257 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/schedule_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12295 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/search_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11814 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/search_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11635 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/send_link_email_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11922 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/sensor.py
--rw-r--r--   0 eugene     (501) staff       (20)    11269 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/sensors.py
--rw-r--r--   0 eugene     (501) staff       (20)    11129 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/service_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    14790 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/share.py
--rw-r--r--   0 eugene     (501) staff       (20)    14595 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/share_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11798 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/share_to_home_workspace_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    14640 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/share_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11701 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_channel.py
--rw-r--r--   0 eugene     (501) staff       (20)    11833 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)    11188 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_connection_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11839 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_connection_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    11209 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_connection_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11384 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_emoji.py
--rw-r--r--   0 eugene     (501) staff       (20)    12036 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_message.py
--rw-r--r--   0 eugene     (501) staff       (20)    11369 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/slack_user.py
--rw-r--r--   0 eugene     (501) staff       (20)    12500 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/smtp_configuration.py
--rw-r--r--   0 eugene     (501) staff       (20)    12518 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/smtp_configuration_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11977 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/snapshot.py
--rw-r--r--   0 eugene     (501) staff       (20)    11341 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/snapshot_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11392 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/snapshot_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12343 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/snfs_stripe_group.py
--rw-r--r--   0 eugene     (501) staff       (20)    11322 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/solr_reindex_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11467 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/start_job_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11836 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/start_task_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12091 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stats.py
--rw-r--r--   0 eugene     (501) staff       (20)    12203 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stor_next_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)    12174 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stor_next_connections.py
--rw-r--r--   0 eugene     (501) staff       (20)    12443 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stor_next_license_check_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11806 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stor_next_license_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    14424 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_node.py
--rw-r--r--   0 eugene     (501) staff       (20)    11980 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_node_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    12929 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_node_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12278 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_node_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    12908 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_node_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11418 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11143 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11423 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/storage_root.py
--rw-r--r--   0 eugene     (501) staff       (20)    11196 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stornext_license.py
--rw-r--r--   0 eugene     (501) staff       (20)    12185 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/stornext_manager_attributes.py
--rw-r--r--   0 eugene     (501) staff       (20)    13372 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subclip.py
--rw-r--r--   0 eugene     (501) staff       (20)    12033 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subclip_clipboard_entry.py
--rw-r--r--   0 eugene     (501) staff       (20)    11709 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subclip_clipboard_entry_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12855 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subclip_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13583 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subclip_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    12882 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subclip_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11378 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subscription.py
--rw-r--r--   0 eugene     (501) staff       (20)    15988 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtask.py
--rw-r--r--   0 eugene     (501) staff       (20)    15245 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtask_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    16282 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtask_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    15302 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtask_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11713 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtitle.py
--rw-r--r--   0 eugene     (501) staff       (20)    12106 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtitle_clipboard_entry.py
--rw-r--r--   0 eugene     (501) staff       (20)    11782 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtitle_clipboard_entry_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    13276 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/subtitle_event.py
--rw-r--r--   0 eugene     (501) staff       (20)    11089 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/elements_sdk/model/sync_totp.py
--rw-r--r--   0 eugene     (501) staff       (20)    11148 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/sync_totp_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    14165 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/system_info_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11297 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tag_media_directory_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12117 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tag_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    15314 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape.py
--rw-r--r--   0 eugene     (501) staff       (20)    14086 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_file.py
--rw-r--r--   0 eugene     (501) staff       (20)    11753 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_group.py
--rw-r--r--   0 eugene     (501) staff       (20)    11564 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_group_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11603 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_group_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    16563 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_job.py
--rw-r--r--   0 eugene     (501) staff       (20)    11730 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_job_source.py
--rw-r--r--   0 eugene     (501) staff       (20)    11891 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11247 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_format_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11241 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_fsck_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11241 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_load_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11431 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_move_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11250 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_reindex_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12045 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_slot.py
--rw-r--r--   0 eugene     (501) staff       (20)    11247 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_library_unload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    14908 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    15846 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    14929 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tape_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    17037 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/task_info.py
--rw-r--r--   0 eugene     (501) staff       (20)    11124 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/task_log.py
--rw-r--r--   0 eugene     (501) staff       (20)    11801 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/task_progress.py
--rw-r--r--   0 eugene     (501) staff       (20)    16286 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/task_type.py
--rw-r--r--   0 eugene     (501) staff       (20)    11920 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/tasks_summary.py
--rw-r--r--   0 eugene     (501) staff       (20)    11833 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/teams_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)    11188 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/teams_connection_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11349 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/teams_connection_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    11209 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/teams_connection_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11462 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/teams_message.py
--rw-r--r--   0 eugene     (501) staff       (20)    11496 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/teams_recipient.py
--rw-r--r--   0 eugene     (501) staff       (20)    11705 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_aws_credentials_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11860 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_aws_credentials_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    13269 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_cloud_account_credentials_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11461 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_cloud_account_credentials_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11519 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_external_transcoder_connection_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11155 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_external_transcoder_connection_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11151 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/test_smtp.py
--rw-r--r--   0 eugene     (501) staff       (20)    11157 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/ticket.py
--rw-r--r--   0 eugene     (501) staff       (20)    11520 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/time_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11789 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/time_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11208 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/time_sync_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11211 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/time_sync_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11886 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/timeline_export_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11315 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/timezone.py
--rw-r--r--   0 eugene     (501) staff       (20)    11939 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/trace_node.py
--rw-r--r--   0 eugene     (501) staff       (20)    13205 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/transcoder_profile.py
--rw-r--r--   0 eugene     (501) staff       (20)    11405 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/type_documentation.py
--rw-r--r--   0 eugene     (501) staff       (20)    12026 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/unfiltered_tag.py
--rw-r--r--   0 eugene     (501) staff       (20)    11837 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/unfiltered_tag_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11876 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/unfiltered_tag_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11310 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/update_quota_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11612 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/updated_file.py
--rw-r--r--   0 eugene     (501) staff       (20)    11445 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/upload_ai_image_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11617 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/upload_chunk_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11444 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/upload_image_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11217 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/user_preview_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11495 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/user_preview_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    11387 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/vantage_workflow.py
--rw-r--r--   0 eugene     (501) staff       (20)    11382 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/vantage_workflows.py
--rw-r--r--   0 eugene     (501) staff       (20)    11368 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/veritone_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)    11207 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/veritone_engine_list.py
--rw-r--r--   0 eugene     (501) staff       (20)    11366 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/veritone_job_list.py
--rw-r--r--   0 eugene     (501) staff       (20)    14232 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/veritone_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)    11549 2022-05-29 13:31:50.000000 elements-sdk-3.6.0/elements_sdk/model/veritone_upload_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    15767 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume.py
--rw-r--r--   0 eugene     (501) staff       (20)    11674 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_bee_gfs_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    12040 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_lizard_fs_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    12803 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    12964 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    14195 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    16183 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    11427 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_snfs_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    11531 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)    11288 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_stats.py
--rw-r--r--   0 eugene     (501) staff       (20)    13154 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    14222 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/volume_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11989 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workflow_transition_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    11319 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workflow_transition_response.py
--rw-r--r--   0 eugene     (501) staff       (20)    27533 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace.py
--rw-r--r--   0 eugene     (501) staff       (20)    11776 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_check_in.py
--rw-r--r--   0 eugene     (501) staff       (20)    27878 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)    22859 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    22916 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12882 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_endpoint.py
--rw-r--r--   0 eugene     (501) staff       (20)    11186 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_move_to_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    12243 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)    12042 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_permission_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    12093 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_permission_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    11990 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workspace_resolved_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)    14806 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workstation.py
--rw-r--r--   0 eugene     (501) staff       (20)    11795 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workstation_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)    14223 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workstation_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    14268 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/elements_sdk/model/workstation_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    82101 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/model_utils.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.775771 elements-sdk-3.6.0/elements_sdk/models/
--rw-r--r--   0 eugene     (501) staff       (20)    31551 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/models/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)    14211 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/elements_sdk/rest.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.646913 elements-sdk-3.6.0/elements_sdk.egg-info/
--rw-r--r--   0 eugene     (501) staff       (20)      387 2022-12-02 15:41:08.000000 elements-sdk-3.6.0/elements_sdk.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)    35622 2022-12-02 15:41:08.000000 elements-sdk-3.6.0/elements_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2022-12-02 15:41:08.000000 elements-sdk-3.6.0/elements_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) staff       (20)       32 2022-12-02 15:41:08.000000 elements-sdk-3.6.0/elements_sdk.egg-info/requires.txt
--rw-r--r--   0 eugene     (501) staff       (20)       13 2022-12-02 15:41:08.000000 elements-sdk-3.6.0/elements_sdk.egg-info/top_level.txt
--rw-r--r--   0 eugene     (501) staff       (20)       69 2022-12-02 15:41:08.867927 elements-sdk-3.6.0/setup.cfg
--rwxr-xr-x   0 eugene     (501) staff       (20)     1089 2022-12-02 15:38:58.000000 elements-sdk-3.6.0/setup.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2022-12-02 15:41:08.867330 elements-sdk-3.6.0/test/
--rw-r--r--   0 eugene     (501) staff       (20)     1496 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_add_assets_to_click_gallery.py
--rw-r--r--   0 eugene     (501) staff       (20)     1427 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_address.py
--rw-r--r--   0 eugene     (501) staff       (20)     1024 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_annotation.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_annotation_create_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1117 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_annotation_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1067 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_annotation_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      749 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_category.py
--rw-r--r--   0 eugene     (501) staff       (20)      941 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_category_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)     1034 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_category_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      984 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_category_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      842 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_category_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)      742 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset.py
--rw-r--r--   0 eugene     (501) staff       (20)      928 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_detail_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_export_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      925 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_export_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      999 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_with_preview.py
--rw-r--r--   0 eugene     (501) staff       (20)      914 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_with_preview_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      864 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_dataset_with_preview_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      728 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_image.py
--rw-r--r--   0 eugene     (501) staff       (20)      792 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_image_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      915 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)      964 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model.py
--rw-r--r--   0 eugene     (501) staff       (20)      821 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_export_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      911 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_export_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      842 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_inference_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      849 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_inference_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      945 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_progress.py
--rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_training_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      895 2022-02-22 16:14:43.000000 elements-sdk-3.6.0/test/test_ai_model_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      813 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_ai_processing_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1869 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_alert.py
--rw-r--r--   0 eugene     (501) staff       (20)     1519 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_alert_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      756 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_alert_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1575 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_all_media_files_for_bundles_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      735 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_api_token.py
--rw-r--r--   0 eugene     (501) staff       (20)      828 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_api_token_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      778 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_api_token_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      807 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_api_token_with_secret.py
--rw-r--r--   0 eugene     (501) staff       (20)      850 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_api_token_with_secret_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2343 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_archive_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1467 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_argument_type.py
--rw-r--r--   0 eugene     (501) staff       (20)     8284 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset.py
--rw-r--r--   0 eugene     (501) staff       (20)    10101 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_backup.py
--rw-r--r--   0 eugene     (501) staff       (20)     1708 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_cloud_link.py
--rw-r--r--   0 eugene     (501) staff       (20)     2099 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     2200 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1477 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     8948 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_project_link.py
--rw-r--r--   0 eugene     (501) staff       (20)     2224 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_rating.py
--rw-r--r--   0 eugene     (501) staff       (20)     1820 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_asset_rating_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      952 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_asset_rating_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      923 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_asset_subtitle_link.py
--rw-r--r--   0 eugene     (501) staff       (20)     1016 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_asset_subtitle_link_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      966 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_asset_subtitle_link_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      756 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_asset_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1551 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_auth_login_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     5034 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_auth_login_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1523 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_aws_account.py
--rw-r--r--   0 eugene     (501) staff       (20)     1538 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_aws_account_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1799 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_backend.py
--rw-r--r--   0 eugene     (501) staff       (20)     2181 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_backend_properties.py
--rw-r--r--   0 eugene     (501) staff       (20)     1490 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_basic_file.py
--rw-r--r--   0 eugene     (501) staff       (20)     1770 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_bee_gfs_node.py
--rw-r--r--   0 eugene     (501) staff       (20)     2092 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_bee_gfs_target.py
--rw-r--r--   0 eugene     (501) staff       (20)     2097 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_bootstrap_data.py
--rw-r--r--   0 eugene     (501) staff       (20)     1622 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_certificate.py
--rw-r--r--   0 eugene     (501) staff       (20)      798 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_certificate_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1538 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_change_own_password_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1386 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_change_password_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1669 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_check_connectivity_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1803 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_click_background_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1408 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_click_gallery.py
--rw-r--r--   0 eugene     (501) staff       (20)     1872 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_click_gallery_link.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_click_gallery_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1483 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_click_link_user.py
--rw-r--r--   0 eugene     (501) staff       (20)     1649 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_click_start_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2659 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_client_session.py
--rw-r--r--   0 eugene     (501) staff       (20)      885 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_client_side_path_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      892 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_client_side_path_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1601 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_clients_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_cloud_account.py
--rw-r--r--   0 eugene     (501) staff       (20)      792 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_cloud_account_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)      885 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_cloud_account_mini_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_cloud_account_mini_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_cloud_account_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_cloud_account_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      858 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/test/test_cloud_bucket_costs.py
--rw-r--r--   0 eugene     (501) staff       (20)     1435 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_cloud_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)      841 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/test/test_cloud_mount_authorization.py
--rw-r--r--   0 eugene     (501) staff       (20)      915 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/test/test_cloud_storage_costs.py
--rw-r--r--   0 eugene     (501) staff       (20)    10448 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_comment.py
--rw-r--r--   0 eugene     (501) staff       (20)     2880 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_comment_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      869 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_comment_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      706 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/test/test_cost.py
--rw-r--r--   0 eugene     (501) staff       (20)     1561 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_cpu_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)     1685 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_create_download_archive.py
--rw-r--r--   0 eugene     (501) staff       (20)     1437 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_create_home_workspace_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1381 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_create_path_quota_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1630 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_create_template_folder_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2117 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_custom_field.py
--rw-r--r--   0 eugene     (501) staff       (20)     2032 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_custom_field_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2087 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_custom_field_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      799 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_custom_field_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1378 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_deleted_workspace.py
--rw-r--r--   0 eugene     (501) staff       (20)     1380 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_download.py
--rw-r--r--   0 eugene     (501) staff       (20)    21348 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_download_archive.py
--rw-r--r--   0 eugene     (501) staff       (20)    11353 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_download_archive_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      910 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_download_archive_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1458 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_editor_project.py
--rw-r--r--   0 eugene     (501) staff       (20)     1573 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_editor_project_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      813 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_editor_project_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      859 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_editor_subtitle.py
--rw-r--r--   0 eugene     (501) staff       (20)      952 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_editor_subtitle_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      902 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_editor_subtitle_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2099 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_elements_group.py
--rw-r--r--   0 eugene     (501) staff       (20)     5813 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_elements_group_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)     5574 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_elements_group_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      992 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_elements_group_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2098 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_elements_group_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     4234 2022-02-22 16:08:41.000000 elements-sdk-3.6.0/test/test_elements_user.py
--rw-r--r--   0 eugene     (501) staff       (20)     4657 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)     3011 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      849 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_elements_user_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1560 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     1629 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1987 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_profile.py
--rw-r--r--   0 eugene     (501) staff       (20)     1663 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_profile_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_elements_user_profile_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     4224 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_user_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1529 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_elements_version.py
--rw-r--r--   0 eugene     (501) staff       (20)     1304 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_email_preview.py
--rw-r--r--   0 eugene     (501) staff       (20)     1387 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_enable_totp_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1548 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_event.py
--rw-r--r--   0 eugene     (501) staff       (20)     1552 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_external_transcoder.py
--rw-r--r--   0 eugene     (501) staff       (20)     1532 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_external_transcoder_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      848 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_external_transcoder_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_extract_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1627 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_copy_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1544 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_delete_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1593 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_move_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2491 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2057 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_size_distribution.py
--rw-r--r--   0 eugene     (501) staff       (20)     1698 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_size_distribution_item.py
--rw-r--r--   0 eugene     (501) staff       (20)     1423 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_size_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1447 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_unzip_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      836 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_file_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1595 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_file_zip_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2972 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_filesystem_file.py
--rw-r--r--   0 eugene     (501) staff       (20)      819 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_filesystem_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)      912 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_filesystem_permission_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      862 2022-02-22 16:14:44.000000 elements-sdk-3.6.0/test/test_filesystem_permission_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1485 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_filesystem_trace_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2315 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_filesystem_trace_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1423 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_finish_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_format_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)     2030 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_fs_properties.py
--rw-r--r--   0 eugene     (501) staff       (20)     1509 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_generate_password_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1722 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_generate_proxies_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      998 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/test/test_get_cloud_account_costs_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      921 2022-12-02 15:38:54.000000 elements-sdk-3.6.0/test/test_get_cloud_account_volume_sizes_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1515 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_get_multiple_bundles_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1490 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_get_multiple_files_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1266 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_global_alert.py
--rw-r--r--   0 eugene     (501) staff       (20)      820 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_help_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/test/test_image_upload_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1453 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_impersonation_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_import_ai_dataset_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      929 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_import_ai_dataset_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      821 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_import_ai_model_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      907 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_import_ai_model_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1425 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_import_job_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    18420 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_import_job_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1969 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_inline_response200.py
--rw-r--r--   0 eugene     (501) staff       (20)     2926 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_inline_response2001.py
--rw-r--r--   0 eugene     (501) staff       (20)     2242 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_inline_response2002.py
--rw-r--r--   0 eugene     (501) staff       (20)     3212 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_inline_response2003.py
--rw-r--r--   0 eugene     (501) staff       (20)     4728 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_inline_response2004.py
--rw-r--r--   0 eugene     (501) staff       (20)      884 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_install_license_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1627 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_instantiate_file_template_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1828 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_interface.py
--rw-r--r--   0 eugene     (501) staff       (20)     1347 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_io_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)     1309 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ipmi.py
--rw-r--r--   0 eugene     (501) staff       (20)     8582 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_job.py
--rw-r--r--   0 eugene     (501) staff       (20)     8604 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_job_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     8655 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_job_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1252 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_job_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1641 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_kapacitor_alert.py
--rw-r--r--   0 eugene     (501) staff       (20)     1329 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ldap_server.py
--rw-r--r--   0 eugene     (501) staff       (20)     1912 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ldap_server_group.py
--rw-r--r--   0 eugene     (501) staff       (20)     2323 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ldap_server_groups.py
--rw-r--r--   0 eugene     (501) staff       (20)     1430 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ldap_server_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1476 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ldap_server_user.py
--rw-r--r--   0 eugene     (501) staff       (20)     1802 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ldap_server_users.py
--rw-r--r--   0 eugene     (501) staff       (20)     2592 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_license.py
--rw-r--r--   0 eugene     (501) staff       (20)     1360 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_list_buckets.py
--rw-r--r--   0 eugene     (501) staff       (20)     1347 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_list_topics.py
--rw-r--r--   0 eugene     (501) staff       (20)     2162 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_lizard_fs_disk.py
--rw-r--r--   0 eugene     (501) staff       (20)     2014 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_lizard_fs_node.py
--rw-r--r--   0 eugene     (501) staff       (20)      834 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_locale_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_locate_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      877 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_locate_proxies_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      971 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_locate_proxies_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1358 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_locate_result.py
--rw-r--r--   0 eugene     (501) staff       (20)     1784 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_marker.py
--rw-r--r--   0 eugene     (501) staff       (20)     1450 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_marker_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_marker_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     7471 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file.py
--rw-r--r--   0 eugene     (501) staff       (20)    10295 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_bundle.py
--rw-r--r--   0 eugene     (501) staff       (20)     2483 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_bundle_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     2497 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_bundle_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    19243 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_contents.py
--rw-r--r--   0 eugene     (501) staff       (20)     2035 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     1668 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     7572 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    15285 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_template.py
--rw-r--r--   0 eugene     (501) staff       (20)     8416 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_file_template_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      966 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_file_template_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_file_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      842 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_files_lookup_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_library_delete_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     3719 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_library_share_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    24428 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root.py
--rw-r--r--   0 eugene     (501) staff       (20)     1334 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_root_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)     1237 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_root_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1187 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_root_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     3138 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     3211 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)    12766 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     3564 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)     2171 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root_permission_access_options.py
--rw-r--r--   0 eugene     (501) staff       (20)     3624 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_root_permission_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_media_root_permission_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1045 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/test/test_media_root_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    22199 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_media_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1343 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_member_preview.py
--rw-r--r--   0 eugene     (501) staff       (20)     1721 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_metadata_item.py
--rw-r--r--   0 eugene     (501) staff       (20)     1408 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_move_workspace_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1468 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_multiple_assets_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1486 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_net_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)      770 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_nfs_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)     1308 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ntp_server.py
--rw-r--r--   0 eugene     (501) staff       (20)     1398 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ntp_server_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_ntp_server_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     3982 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_one_time_access_token.py
--rw-r--r--   0 eugene     (501) staff       (20)     1618 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_one_time_access_token_activity.py
--rw-r--r--   0 eugene     (501) staff       (20)     1534 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_one_time_access_token_shared_object.py
--rw-r--r--   0 eugene     (501) staff       (20)     2496 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_parameters.py
--rw-r--r--   0 eugene     (501) staff       (20)      791 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_parameters_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      870 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_parse_samlidp_metadata_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_parsed_samlidp_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)     1524 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_password_reset_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1187 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_path.py
--rw-r--r--   0 eugene     (501) staff       (20)     1334 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_path_input.py
--rw-r--r--   0 eugene     (501) staff       (20)     1601 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_production.py
--rw-r--r--   0 eugene     (501) staff       (20)     1434 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_production_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1588 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_production_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1674 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_production_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      791 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_production_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1703 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy.py
--rw-r--r--   0 eugene     (501) staff       (20)     1255 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy_count.py
--rw-r--r--   0 eugene     (501) staff       (20)      871 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_proxy_fs_size_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     2557 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy_generator.py
--rw-r--r--   0 eugene     (501) staff       (20)     1812 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy_generator_properties.py
--rw-r--r--   0 eugene     (501) staff       (20)     2378 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy_profile.py
--rw-r--r--   0 eugene     (501) staff       (20)     1349 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy_profile_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     2471 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_proxy_profile_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_proxy_profile_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1448 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_python_environment.py
--rw-r--r--   0 eugene     (501) staff       (20)     1839 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_queue.py
--rw-r--r--   0 eugene     (501) staff       (20)     1312 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_quota.py
--rw-r--r--   0 eugene     (501) staff       (20)     1500 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_ram_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)    28707 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_rdc_activation.py
--rw-r--r--   0 eugene     (501) staff       (20)    14582 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_rdc_host.py
--rw-r--r--   0 eugene     (501) staff       (20)     2171 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_rdc_session.py
--rw-r--r--   0 eugene     (501) staff       (20)     2083 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_rdc_session_create.py
--rw-r--r--   0 eugene     (501) staff       (20)     1535 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_register_upload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2386 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_register_upload_metadata_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1520 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_release_notes_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1413 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_rename_custom_field_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1720 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_render_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1302 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_render_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2459 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_restore_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_saml_provider.py
--rw-r--r--   0 eugene     (501) staff       (20)     1355 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_saml_provider_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_saml_provider_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_saml_provider_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      909 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_saved_search.py
--rw-r--r--   0 eugene     (501) staff       (20)      849 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_saved_search_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      799 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_saved_search_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1514 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_scanner_discover_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1540 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_scanner_scan_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1897 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_schedule.py
--rw-r--r--   0 eugene     (501) staff       (20)     1886 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_schedule_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1972 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_schedule_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_schedule_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1573 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_search_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     5827 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_search_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1403 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_send_link_email_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1386 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_sensor.py
--rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_sensors.py
--rw-r--r--   0 eugene     (501) staff       (20)     1296 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_service_status.py
--rw-r--r--   0 eugene     (501) staff       (20)    14161 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_share.py
--rw-r--r--   0 eugene     (501) staff       (20)     8044 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_share_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1742 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_share_to_home_workspace_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      970 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_share_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1399 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_channel.py
--rw-r--r--   0 eugene     (501) staff       (20)     1561 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)     1429 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_connection_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1545 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_connection_status.py
--rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_slack_connection_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1310 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_emoji.py
--rw-r--r--   0 eugene     (501) staff       (20)     1407 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_message.py
--rw-r--r--   0 eugene     (501) staff       (20)     1297 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_slack_user.py
--rw-r--r--   0 eugene     (501) staff       (20)     1649 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_smtp_configuration.py
--rw-r--r--   0 eugene     (501) staff       (20)      841 2022-02-22 16:14:45.000000 elements-sdk-3.6.0/test/test_smtp_configuration_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1436 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_snapshot.py
--rw-r--r--   0 eugene     (501) staff       (20)     1383 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_snapshot_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_snapshot_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1604 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_snfs_stripe_group.py
--rw-r--r--   0 eugene     (501) staff       (20)    22532 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_solr_reindex_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1372 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_start_job_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1536 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_start_task_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     3715 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stats.py
--rw-r--r--   0 eugene     (501) staff       (20)     1500 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stor_next_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)     2445 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stor_next_connections.py
--rw-r--r--   0 eugene     (501) staff       (20)     1840 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stor_next_license_check_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1622 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stor_next_license_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     3388 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_storage_node.py
--rw-r--r--   0 eugene     (501) staff       (20)     1369 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_storage_node_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)      849 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/test/test_storage_node_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1790 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_storage_node_status.py
--rw-r--r--   0 eugene     (501) staff       (20)      799 2022-12-02 15:38:55.000000 elements-sdk-3.6.0/test/test_storage_node_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_storage_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      784 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_storage_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      756 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_storage_root.py
--rw-r--r--   0 eugene     (501) staff       (20)     1316 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stornext_license.py
--rw-r--r--   0 eugene     (501) staff       (20)     1653 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_stornext_manager_attributes.py
--rw-r--r--   0 eugene     (501) staff       (20)     8425 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subclip.py
--rw-r--r--   0 eugene     (501) staff       (20)    10694 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subclip_clipboard_entry.py
--rw-r--r--   0 eugene     (501) staff       (20)      985 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subclip_clipboard_entry_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     7260 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subclip_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     8465 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subclip_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1035 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subclip_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      762 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subscription.py
--rw-r--r--   0 eugene     (501) staff       (20)     2011 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subtask.py
--rw-r--r--   0 eugene     (501) staff       (20)     1980 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subtask_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2001 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_subtask_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      770 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subtask_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      837 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subtitle.py
--rw-r--r--   0 eugene     (501) staff       (20)      958 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subtitle_clipboard_entry.py
--rw-r--r--   0 eugene     (501) staff       (20)     1001 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subtitle_clipboard_entry_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      770 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_subtitle_event.py
--rw-r--r--   0 eugene     (501) staff       (20)     1233 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_sync_totp.py
--rw-r--r--   0 eugene     (501) staff       (20)     1310 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_sync_totp_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     4521 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_system_info_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1466 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tag_media_directory_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1410 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tag_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1738 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape.py
--rw-r--r--   0 eugene     (501) staff       (20)     2340 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_file.py
--rw-r--r--   0 eugene     (501) staff       (20)     2927 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_group.py
--rw-r--r--   0 eugene     (501) staff       (20)     2192 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_group_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      888 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_tape_group_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     2963 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_job.py
--rw-r--r--   0 eugene     (501) staff       (20)     1406 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_job_source.py
--rw-r--r--   0 eugene     (501) staff       (20)     3318 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1509 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_format_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1487 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_fsck_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1487 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_load_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1542 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_move_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1520 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_reindex_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1410 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_slot.py
--rw-r--r--   0 eugene     (501) staff       (20)     1509 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_library_unload_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1797 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1811 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tape_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)      749 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_tape_update.py
--rw-r--r--   0 eugene     (501) staff       (20)    10289 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_task_info.py
--rw-r--r--   0 eugene     (501) staff       (20)     1220 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_task_log.py
--rw-r--r--   0 eugene     (501) staff       (20)     1310 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_task_progress.py
--rw-r--r--   0 eugene     (501) staff       (20)     3340 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_task_type.py
--rw-r--r--   0 eugene     (501) staff       (20)    43603 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_tasks_summary.py
--rw-r--r--   0 eugene     (501) staff       (20)     1496 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_teams_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)     1429 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_teams_connection_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1433 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_teams_connection_status.py
--rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_teams_connection_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1344 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_teams_message.py
--rw-r--r--   0 eugene     (501) staff       (20)     1330 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_teams_recipient.py
--rw-r--r--   0 eugene     (501) staff       (20)     1525 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_test_aws_credentials_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1525 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_test_aws_credentials_response.py
--rw-r--r--   0 eugene     (501) staff       (20)      920 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_test_cloud_account_credentials_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1025 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_test_cloud_account_credentials_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1643 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_test_external_transcoder_connection_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1589 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_test_external_transcoder_connection_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1235 2022-02-22 16:08:42.000000 elements-sdk-3.6.0/test/test_test_smtp.py
--rw-r--r--   0 eugene     (501) staff       (20)     1213 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_ticket.py
--rw-r--r--   0 eugene     (501) staff       (20)     1631 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_time_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     2019 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_time_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1406 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_time_sync_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1417 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_time_sync_endpoint_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1512 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_timeline_export_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1262 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_timezone.py
--rw-r--r--   0 eugene     (501) staff       (20)     1583 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_trace_node.py
--rw-r--r--   0 eugene     (501) staff       (20)     1616 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_transcoder_profile.py
--rw-r--r--   0 eugene     (501) staff       (20)     1387 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_type_documentation.py
--rw-r--r--   0 eugene     (501) staff       (20)     1521 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_unfiltered_tag.py
--rw-r--r--   0 eugene     (501) staff       (20)     1542 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_unfiltered_tag_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      813 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_unfiltered_tag_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1344 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_update_quota_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      946 2022-12-02 15:38:56.000000 elements-sdk-3.6.0/test/test_updated_file.py
--rw-r--r--   0 eugene     (501) staff       (20)      821 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_upload_ai_image_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1484 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_upload_chunk_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)      863 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_upload_image_endpoint_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1353 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_user_preview_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     1425 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_user_preview_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     1363 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_vantage_workflow.py
--rw-r--r--   0 eugene     (501) staff       (20)     1665 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_vantage_workflows.py
--rw-r--r--   0 eugene     (501) staff       (20)      805 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_veritone_connection.py
--rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_veritone_engine_list.py
--rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_veritone_job_list.py
--rw-r--r--   0 eugene     (501) staff       (20)      791 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_veritone_metadata.py
--rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_veritone_upload_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     6897 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume.py
--rw-r--r--   0 eugene     (501) staff       (20)     4086 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_bee_gfs_status.py
--rw-r--r--   0 eugene     (501) staff       (20)     4869 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_lizard_fs_status.py
--rw-r--r--   0 eugene     (501) staff       (20)     1389 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     1490 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_mini_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     1740 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     6926 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_reference.py
--rw-r--r--   0 eugene     (501) staff       (20)     2145 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_snfs_status.py
--rw-r--r--   0 eugene     (501) staff       (20)     1385 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_stat.py
--rw-r--r--   0 eugene     (501) staff       (20)     1676 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_stats.py
--rw-r--r--   0 eugene     (501) staff       (20)     5170 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_volume_status.py
--rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_volume_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1713 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workflow_transition_request.py
--rw-r--r--   0 eugene     (501) staff       (20)    22519 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workflow_transition_response.py
--rw-r--r--   0 eugene     (501) staff       (20)     4907 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace.py
--rw-r--r--   0 eugene     (501) staff       (20)     1366 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_check_in.py
--rw-r--r--   0 eugene     (501) staff       (20)    11539 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_detail.py
--rw-r--r--   0 eugene     (501) staff       (20)     9713 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_detail_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1057 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_workspace_detail_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1718 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_endpoint.py
--rw-r--r--   0 eugene     (501) staff       (20)     1401 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_move_to_request.py
--rw-r--r--   0 eugene     (501) staff       (20)     5645 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)     5734 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_permission_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)      855 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_workspace_permission_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1570 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workspace_resolved_permission.py
--rw-r--r--   0 eugene     (501) staff       (20)     7541 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workstation.py
--rw-r--r--   0 eugene     (501) staff       (20)     1408 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workstation_mini.py
--rw-r--r--   0 eugene     (501) staff       (20)     6469 2022-02-22 16:08:43.000000 elements-sdk-3.6.0/test/test_workstation_partial_update.py
--rw-r--r--   0 eugene     (501) staff       (20)     1074 2022-02-22 16:14:46.000000 elements-sdk-3.6.0/test/test_workstation_update.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.952268 elements-sdk-3.6.1/
+-rw-r--r--   0 eugene     (501) staff       (20)     1065 2021-01-28 11:22:09.000000 elements-sdk-3.6.1/LICENSE
+-rw-r--r--   0 eugene     (501) staff       (20)      387 2023-01-23 14:30:42.952345 elements-sdk-3.6.1/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)    97694 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/README.md
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.823242 elements-sdk-3.6.1/elements_sdk/
+-rw-r--r--   0 eugene     (501) staff       (20)      751 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/__init__.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.827596 elements-sdk-3.6.1/elements_sdk/api/
+-rw-r--r--   0 eugene     (501) staff       (20)      211 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)   226652 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/ai_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   161652 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/auth_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   218625 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/automation_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    41799 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/aws_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    65079 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/click_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   106050 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/integrations_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   635911 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/main_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   939194 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/media_library_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    67975 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/private_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    39335 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/satellite_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    20596 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/sharedstorage_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    30350 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/status_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   381831 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/storage_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)   171030 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api/tape_archive_api.py
+-rw-r--r--   0 eugene     (501) staff       (20)    37713 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/api_client.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.827801 elements-sdk-3.6.1/elements_sdk/apis/
+-rw-r--r--   0 eugene     (501) staff       (20)     1147 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/apis/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17110 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/configuration.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5089 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/exceptions.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.887750 elements-sdk-3.6.1/elements_sdk/model/
+-rw-r--r--   0 eugene     (501) staff       (20)      348 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/model/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11151 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/add_assets_to_click_gallery.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12386 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/address.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14281 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_annotation.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12777 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_annotation_create_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13080 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_annotation_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13419 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_annotation_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12310 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_category.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12612 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_category_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11668 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_category_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11719 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_category_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11401 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_category_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11350 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11909 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12911 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_detail_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11181 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_export_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11293 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_export_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11972 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13767 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_with_preview.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11723 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_with_preview_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11792 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_dataset_with_preview_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12960 2023-01-23 14:30:14.000000 elements-sdk-3.6.1/elements_sdk/model/ai_image.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13120 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_image_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12764 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14455 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11175 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_export_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11287 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_export_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12369 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_inference_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11242 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_inference_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13041 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11408 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_progress.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12223 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_training_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13140 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_model_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11880 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/ai_processing_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13647 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/alert.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11887 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/alert_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11986 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/alert_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11183 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/all_media_files_for_bundles_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11339 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/api_token.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11168 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/api_token_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11189 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/api_token_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11614 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/api_token_with_secret.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11464 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/api_token_with_secret_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12700 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/archive_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11574 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/argument_type.py
+-rw-r--r--   0 eugene     (501) staff       (20)    18513 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12326 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_backup.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12356 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_cloud_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13232 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13420 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11561 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12042 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_project_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12235 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_rating.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11871 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_rating_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11910 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_rating_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12384 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_subtitle_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12119 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_subtitle_link_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12206 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_subtitle_link_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11648 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/asset_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12060 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/auth_login_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12135 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/auth_login_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11625 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/backend.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14846 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/backend_properties.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12418 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/basic_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12001 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/bee_gfs_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13433 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/bee_gfs_target.py
+-rw-r--r--   0 eugene     (501) staff       (20)    20604 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/bootstrap_data.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13329 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/certificate.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11423 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/certificate_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11944 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/change_own_password_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11226 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/change_password_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11407 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/check_connectivity_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11859 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/click_background_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11849 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/click_gallery.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13173 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/click_gallery_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11415 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/click_gallery_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12072 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/click_link_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11431 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/click_start_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12613 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/client_session.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11642 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/client_side_path_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11337 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/client_side_path_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12117 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/clients_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13371 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_account.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11722 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_account_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11551 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_account_mini_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11572 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_account_mini_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13200 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_account_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13221 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_account_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11827 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_bucket_costs.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11913 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13217 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_mount_authorization.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11634 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/cloud_storage_costs.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14796 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/comment.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13963 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/comment_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13990 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/comment_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11393 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/cost.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12226 2023-01-23 14:30:15.000000 elements-sdk-3.6.1/elements_sdk/model/cpu_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11936 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/create_download_archive.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11154 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/create_home_workspace_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11166 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/create_path_quota_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11735 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/create_template_folder_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16278 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/custom_field.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16013 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/custom_field_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16827 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/custom_field_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16100 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/custom_field_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11414 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/deleted_workspace.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12216 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/download.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13615 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/download_archive.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12346 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/download_archive_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12421 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/download_archive_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12445 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/editor_project.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12424 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/editor_project_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12463 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/editor_project_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12165 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/editor_subtitle.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12138 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/editor_subtitle_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12183 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/editor_subtitle_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13778 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14102 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_group_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13216 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_group_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13237 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_group_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14050 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_group_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    20373 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)    20619 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)    18409 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    18532 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12861 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13082 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14860 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_profile.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12418 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_profile_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12397 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_profile_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    21338 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_user_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12423 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/elements_version.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11123 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/email_preview.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11393 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/enable_totp_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12594 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/event.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12325 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/external_transcoder.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12058 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/external_transcoder_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12175 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/external_transcoder_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11453 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/extract_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12551 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_copy_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11327 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_delete_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12060 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_move_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16177 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11492 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_size_distribution.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12142 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_size_distribution_item.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11192 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_size_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11390 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_unzip_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16222 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11639 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/file_zip_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17763 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/filesystem_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12007 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/filesystem_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11836 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/filesystem_permission_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11857 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/filesystem_permission_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11188 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/filesystem_trace_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12095 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/filesystem_trace_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11184 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/finish_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12297 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/format_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14478 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/fs_properties.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11259 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/generate_password_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12081 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/generate_proxies_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11736 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/get_cloud_account_costs_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11219 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/get_cloud_account_volume_sizes_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11297 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/get_multiple_bundles_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11140 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/get_multiple_files_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11148 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/global_alert.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11175 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/help_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11205 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/image_upload_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11138 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/impersonation_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11947 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/import_ai_dataset_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11350 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/import_ai_dataset_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11175 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/import_ai_model_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11308 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/import_ai_model_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11709 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/import_job_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11245 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/import_job_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12014 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/inline_response200.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11549 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/install_license_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11700 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/instantiate_file_template_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13243 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/interface.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11525 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/io_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11677 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ipmi.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17329 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/job.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16502 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/job_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17973 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/job_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16523 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/job_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12220 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/kapacitor_alert.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11842 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ldap_server.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11807 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ldap_server_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11350 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ldap_server_groups.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11952 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ldap_server_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11934 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ldap_server_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11329 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ldap_server_users.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15113 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/license.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11112 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/list_topics.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14119 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/lizard_fs_disk.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13616 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/lizard_fs_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11213 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/locale_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11319 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/locate_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11155 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/locate_proxies_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11867 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/locate_proxies_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11806 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/locate_result.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12822 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/marker.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11808 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/marker_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11865 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/marker_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    18716 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13517 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_bundle.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12246 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_bundle_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12266 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_bundle_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11835 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_contents.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14014 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12247 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19647 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11796 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_template.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11613 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_template_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11646 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_template_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12226 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_file_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11196 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_files_lookup_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12240 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_library_delete_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13429 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_library_share_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    20305 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root.py
+-rw-r--r--   0 eugene     (501) staff       (20)    20832 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19657 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19702 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12965 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13133 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17355 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15555 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_permission_access_options.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16979 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_permission_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17000 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_permission_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19456 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_root_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14529 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/media_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11675 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/member_preview.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11756 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/metadata_item.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11559 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/move_workspace_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11145 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/multiple_assets_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11953 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/net_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11689 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/nfs_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11665 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ntp_server.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11476 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ntp_server_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11515 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/ntp_server_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16297 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/one_time_access_token.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11744 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/one_time_access_token_activity.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11373 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/one_time_access_token_shared_object.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19557 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/parameters.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19575 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/parameters_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11184 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/parse_samlidp_metadata_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12117 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/parsed_samlidp_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11510 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/password_reset_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11127 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/path.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11098 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/path_input.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13536 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/production.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11690 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/production_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12626 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/production_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13877 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/production_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12647 2023-01-23 14:30:16.000000 elements-sdk-3.6.1/elements_sdk/model/production_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14118 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11095 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_count.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11168 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_fs_size_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11923 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_generator.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13506 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_generator_properties.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19556 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_profile.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11362 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_profile_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19385 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_profile_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19406 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/proxy_profile_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11680 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/python_environment.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12651 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/queue.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11547 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/quota.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12030 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/ram_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13093 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/rdc_activation.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11947 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/rdc_host.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12165 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/rdc_session.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11561 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/rdc_session_create.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11513 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/register_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11380 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/register_upload_metadata_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11486 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/release_notes_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11187 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/rename_custom_field_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12201 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/render_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11238 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/render_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12826 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/restore_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15247 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saml_provider.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11767 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saml_provider_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14078 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saml_provider_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14213 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saml_provider_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12765 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saved_search.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11938 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saved_search_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11977 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/saved_search_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11444 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/scanner_discover_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11910 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/scanner_scan_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14614 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/schedule.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14242 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/schedule_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15115 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/schedule_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14257 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/schedule_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12295 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/search_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11814 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/search_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11635 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/send_link_email_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11922 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/sensor.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11269 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/sensors.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11129 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/service_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14790 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/share.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14595 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/share_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11798 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/share_to_home_workspace_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14640 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/share_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11701 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_channel.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11833 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11188 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_connection_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11839 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_connection_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11209 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_connection_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11384 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_emoji.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12036 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_message.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11369 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/slack_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12500 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/smtp_configuration.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12518 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/smtp_configuration_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11977 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/snapshot.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11341 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/snapshot_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11392 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/snapshot_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12343 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/snfs_stripe_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11322 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/solr_reindex_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11467 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/start_job_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11836 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/start_task_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12091 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stats.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12203 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stor_next_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12174 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stor_next_connections.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12443 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stor_next_license_check_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11806 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stor_next_license_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14424 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11980 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_node_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12929 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_node_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12278 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_node_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12908 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_node_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11418 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11143 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11423 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/storage_root.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11196 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stornext_license.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12185 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/stornext_manager_attributes.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13372 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subclip.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12033 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subclip_clipboard_entry.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11709 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subclip_clipboard_entry_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12855 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subclip_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13583 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subclip_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12882 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subclip_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11378 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subscription.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15988 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtask.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15245 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtask_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16282 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtask_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15302 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtask_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11713 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtitle.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12106 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtitle_clipboard_entry.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11782 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtitle_clipboard_entry_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13276 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/subtitle_event.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11089 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/sync_totp.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11148 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/sync_totp_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14165 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/system_info_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11297 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tag_media_directory_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12117 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tag_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15314 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14086 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11753 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11564 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_group_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11603 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_group_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16563 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_job.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11730 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_job_source.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11891 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11247 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_format_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11241 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_fsck_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11241 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_load_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11431 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_move_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11250 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_reindex_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12045 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_slot.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11247 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_library_unload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14908 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15846 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14929 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tape_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    17037 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/task_info.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11124 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/task_log.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11801 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/task_progress.py
+-rw-r--r--   0 eugene     (501) staff       (20)    16286 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/task_type.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11920 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/tasks_summary.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11833 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/teams_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11188 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/teams_connection_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11349 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/teams_connection_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11209 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/teams_connection_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11462 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/teams_message.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11496 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/teams_recipient.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11705 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_aws_credentials_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11860 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_aws_credentials_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13269 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_cloud_account_credentials_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11461 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_cloud_account_credentials_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11519 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_external_transcoder_connection_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11155 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_external_transcoder_connection_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11151 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/test_smtp.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11157 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/ticket.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11520 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/time_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11789 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/time_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11208 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/time_sync_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11211 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/time_sync_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11886 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/timeline_export_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11315 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/timezone.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11939 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/trace_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13205 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/transcoder_profile.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11405 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/type_documentation.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12026 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/unfiltered_tag.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11837 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/unfiltered_tag_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11876 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/unfiltered_tag_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11310 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/update_quota_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11612 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/updated_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11445 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/upload_ai_image_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11617 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/upload_chunk_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11444 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/upload_image_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11217 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/user_preview_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11495 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/user_preview_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11387 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/vantage_workflow.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11382 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/vantage_workflows.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11368 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/veritone_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11207 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/veritone_engine_list.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11366 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/veritone_job_list.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14232 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/veritone_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11549 2022-05-29 13:31:50.000000 elements-sdk-3.6.1/elements_sdk/model/veritone_upload_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15436 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11674 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_bee_gfs_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12040 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_lizard_fs_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12472 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12633 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14195 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15852 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11427 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_snfs_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11531 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11288 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_stats.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13154 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14222 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/volume_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11989 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workflow_transition_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11319 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workflow_transition_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)    27533 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11776 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_check_in.py
+-rw-r--r--   0 eugene     (501) staff       (20)    27878 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)    22859 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    22916 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12882 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_endpoint.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11186 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_move_to_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12243 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12042 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_permission_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12093 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_permission_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11990 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workspace_resolved_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14806 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workstation.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11795 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workstation_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14223 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workstation_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14268 2023-01-23 14:30:17.000000 elements-sdk-3.6.1/elements_sdk/model/workstation_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    82101 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/model_utils.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.887893 elements-sdk-3.6.1/elements_sdk/models/
+-rw-r--r--   0 eugene     (501) staff       (20)    31551 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/models/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14211 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/elements_sdk/rest.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.823816 elements-sdk-3.6.1/elements_sdk.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)      387 2023-01-23 14:30:42.000000 elements-sdk-3.6.1/elements_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)    35622 2023-01-23 14:30:42.000000 elements-sdk-3.6.1/elements_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-01-23 14:30:42.000000 elements-sdk-3.6.1/elements_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       32 2023-01-23 14:30:42.000000 elements-sdk-3.6.1/elements_sdk.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       13 2023-01-23 14:30:42.000000 elements-sdk-3.6.1/elements_sdk.egg-info/top_level.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       69 2023-01-23 14:30:42.952595 elements-sdk-3.6.1/setup.cfg
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1089 2023-01-23 14:30:19.000000 elements-sdk-3.6.1/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-01-23 14:30:42.952151 elements-sdk-3.6.1/test/
+-rw-r--r--   0 eugene     (501) staff       (20)     1496 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_add_assets_to_click_gallery.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1427 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_address.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1024 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_annotation.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_annotation_create_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1117 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_annotation_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1067 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_annotation_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      749 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_category.py
+-rw-r--r--   0 eugene     (501) staff       (20)      941 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_category_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1034 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_category_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      984 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_category_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      842 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_category_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)      742 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset.py
+-rw-r--r--   0 eugene     (501) staff       (20)      928 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_detail_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_export_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      925 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_export_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      999 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_with_preview.py
+-rw-r--r--   0 eugene     (501) staff       (20)      914 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_with_preview_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      864 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_dataset_with_preview_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      728 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_image.py
+-rw-r--r--   0 eugene     (501) staff       (20)      792 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_image_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      915 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)      964 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model.py
+-rw-r--r--   0 eugene     (501) staff       (20)      821 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_export_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      911 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_export_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      842 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_inference_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      849 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_inference_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      945 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_progress.py
+-rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_training_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      895 2022-02-22 16:14:43.000000 elements-sdk-3.6.1/test/test_ai_model_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      813 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_ai_processing_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1869 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_alert.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1519 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_alert_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      756 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_alert_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1575 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_all_media_files_for_bundles_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      735 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_api_token.py
+-rw-r--r--   0 eugene     (501) staff       (20)      828 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_api_token_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      778 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_api_token_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      807 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_api_token_with_secret.py
+-rw-r--r--   0 eugene     (501) staff       (20)      850 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_api_token_with_secret_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2343 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_archive_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1467 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_argument_type.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8284 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10101 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_backup.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1708 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_cloud_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2099 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2200 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1477 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8948 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_project_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2224 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_rating.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1820 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_asset_rating_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      952 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_asset_rating_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      923 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_asset_subtitle_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1016 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_asset_subtitle_link_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      966 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_asset_subtitle_link_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      756 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_asset_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1551 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_auth_login_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5034 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_auth_login_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1523 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_aws_account.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1538 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_aws_account_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1799 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_backend.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2181 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_backend_properties.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1490 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_basic_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1770 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_bee_gfs_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2092 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_bee_gfs_target.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2097 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_bootstrap_data.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1622 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_certificate.py
+-rw-r--r--   0 eugene     (501) staff       (20)      798 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_certificate_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1538 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_change_own_password_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1386 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_change_password_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1669 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_check_connectivity_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1803 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_click_background_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1408 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_click_gallery.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1872 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_click_gallery_link.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_click_gallery_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1483 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_click_link_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1649 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_click_start_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2659 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_client_session.py
+-rw-r--r--   0 eugene     (501) staff       (20)      885 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_client_side_path_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      892 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_client_side_path_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1601 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_clients_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_cloud_account.py
+-rw-r--r--   0 eugene     (501) staff       (20)      792 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_cloud_account_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)      885 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_cloud_account_mini_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_cloud_account_mini_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_cloud_account_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_cloud_account_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      858 2022-12-02 15:38:54.000000 elements-sdk-3.6.1/test/test_cloud_bucket_costs.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1435 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_cloud_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)      841 2022-12-02 15:38:54.000000 elements-sdk-3.6.1/test/test_cloud_mount_authorization.py
+-rw-r--r--   0 eugene     (501) staff       (20)      915 2022-12-02 15:38:54.000000 elements-sdk-3.6.1/test/test_cloud_storage_costs.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10448 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_comment.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2880 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_comment_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      869 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_comment_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      706 2022-12-02 15:38:54.000000 elements-sdk-3.6.1/test/test_cost.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1561 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_cpu_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1685 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_create_download_archive.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1437 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_create_home_workspace_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1381 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_create_path_quota_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1630 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_create_template_folder_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2117 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_custom_field.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2032 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_custom_field_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2087 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_custom_field_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      799 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_custom_field_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1378 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_deleted_workspace.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1380 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_download.py
+-rw-r--r--   0 eugene     (501) staff       (20)    21348 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_download_archive.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11353 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_download_archive_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      910 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_download_archive_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1458 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_editor_project.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1573 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_editor_project_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      813 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_editor_project_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      859 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_editor_subtitle.py
+-rw-r--r--   0 eugene     (501) staff       (20)      952 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_editor_subtitle_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      902 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_editor_subtitle_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2099 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_elements_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5813 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_elements_group_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5574 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_elements_group_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      992 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_elements_group_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2098 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_elements_group_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4234 2022-02-22 16:08:41.000000 elements-sdk-3.6.1/test/test_elements_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4657 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3011 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      849 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_elements_user_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1560 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1629 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1987 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_profile.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1663 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_profile_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_elements_user_profile_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4224 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_user_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1529 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_elements_version.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1304 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_email_preview.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1387 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_enable_totp_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1548 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_event.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1552 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_external_transcoder.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1532 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_external_transcoder_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      848 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_external_transcoder_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_extract_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1627 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_copy_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1544 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_delete_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1593 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_move_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2491 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2057 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_size_distribution.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1698 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_size_distribution_item.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1423 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_size_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1447 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_unzip_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      836 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_file_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1595 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_file_zip_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2972 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_filesystem_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)      819 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_filesystem_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)      912 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_filesystem_permission_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      862 2022-02-22 16:14:44.000000 elements-sdk-3.6.1/test/test_filesystem_permission_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1485 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_filesystem_trace_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2315 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_filesystem_trace_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1423 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_finish_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_format_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2030 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_fs_properties.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1509 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_generate_password_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1722 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_generate_proxies_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      998 2022-12-02 15:38:54.000000 elements-sdk-3.6.1/test/test_get_cloud_account_costs_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      921 2022-12-02 15:38:54.000000 elements-sdk-3.6.1/test/test_get_cloud_account_volume_sizes_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1515 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_get_multiple_bundles_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1490 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_get_multiple_files_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1266 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_global_alert.py
+-rw-r--r--   0 eugene     (501) staff       (20)      820 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_help_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-12-02 15:38:55.000000 elements-sdk-3.6.1/test/test_image_upload_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1453 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_impersonation_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      835 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_import_ai_dataset_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      929 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_import_ai_dataset_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      821 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_import_ai_model_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      907 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_import_ai_model_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1425 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_import_job_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    18420 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_import_job_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1969 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_inline_response200.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2926 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_inline_response2001.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2242 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_inline_response2002.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3212 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_inline_response2003.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4728 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_inline_response2004.py
+-rw-r--r--   0 eugene     (501) staff       (20)      884 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_install_license_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1627 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_instantiate_file_template_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1828 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_interface.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1347 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_io_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1309 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ipmi.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8582 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_job.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8604 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_job_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8655 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_job_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1252 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_job_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1641 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_kapacitor_alert.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1329 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ldap_server.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1912 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ldap_server_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2323 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ldap_server_groups.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1430 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ldap_server_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1476 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ldap_server_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1802 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ldap_server_users.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2592 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_license.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1360 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_list_buckets.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1347 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_list_topics.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2162 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_lizard_fs_disk.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2014 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_lizard_fs_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)      834 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_locale_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_locate_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      877 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_locate_proxies_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      971 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_locate_proxies_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1358 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_locate_result.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1784 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_marker.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1450 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_marker_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_marker_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7471 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10295 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_bundle.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2483 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_bundle_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2497 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_bundle_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    19243 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_contents.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2035 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1668 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7572 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    15285 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_template.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8416 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_file_template_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      966 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_file_template_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_file_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      842 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_files_lookup_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_library_delete_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3719 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_library_share_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    24428 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1334 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_root_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1237 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_root_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1187 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_root_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3138 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3211 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12766 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3564 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2171 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root_permission_access_options.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3624 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_root_permission_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_media_root_permission_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1045 2022-12-02 15:38:55.000000 elements-sdk-3.6.1/test/test_media_root_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    22199 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_media_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1343 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_member_preview.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1721 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_metadata_item.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1408 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_move_workspace_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1468 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_multiple_assets_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1486 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_net_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)      770 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_nfs_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1308 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ntp_server.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1398 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ntp_server_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_ntp_server_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3982 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_one_time_access_token.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1618 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_one_time_access_token_activity.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1534 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_one_time_access_token_shared_object.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2496 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_parameters.py
+-rw-r--r--   0 eugene     (501) staff       (20)      791 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_parameters_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      870 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_parse_samlidp_metadata_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_parsed_samlidp_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1524 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_password_reset_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1187 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_path.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1334 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_path_input.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1601 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_production.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1434 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_production_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1588 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_production_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1674 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_production_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      791 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_production_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1703 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1255 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy_count.py
+-rw-r--r--   0 eugene     (501) staff       (20)      871 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_proxy_fs_size_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2557 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy_generator.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1812 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy_generator_properties.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2378 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy_profile.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1349 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy_profile_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2471 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_proxy_profile_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_proxy_profile_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1448 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_python_environment.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1839 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_queue.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1312 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_quota.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1500 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_ram_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    28707 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_rdc_activation.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14582 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_rdc_host.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2171 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_rdc_session.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2083 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_rdc_session_create.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1535 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_register_upload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2386 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_register_upload_metadata_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1520 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_release_notes_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1413 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_rename_custom_field_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1720 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_render_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1302 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_render_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2459 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_restore_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_saml_provider.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1355 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_saml_provider_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_saml_provider_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_saml_provider_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      909 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_saved_search.py
+-rw-r--r--   0 eugene     (501) staff       (20)      849 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_saved_search_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      799 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_saved_search_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1514 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_scanner_discover_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1540 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_scanner_scan_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1897 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_schedule.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1886 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_schedule_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1972 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_schedule_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_schedule_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1573 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_search_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5827 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_search_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1403 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_send_link_email_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1386 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_sensor.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_sensors.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1296 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_service_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)    14161 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_share.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8044 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_share_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1742 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_share_to_home_workspace_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      970 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_share_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1399 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_channel.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1561 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1429 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_connection_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1545 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_connection_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_slack_connection_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1310 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_emoji.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1407 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_message.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1297 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_slack_user.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1649 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_smtp_configuration.py
+-rw-r--r--   0 eugene     (501) staff       (20)      841 2022-02-22 16:14:45.000000 elements-sdk-3.6.1/test/test_smtp_configuration_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1436 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_snapshot.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1383 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_snapshot_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_snapshot_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1604 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_snfs_stripe_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)    22532 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_solr_reindex_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1372 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_start_job_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1536 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_start_task_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3715 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stats.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1500 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stor_next_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2445 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stor_next_connections.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1840 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stor_next_license_check_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1622 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stor_next_license_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3388 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_storage_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1369 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_storage_node_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)      849 2022-12-02 15:38:55.000000 elements-sdk-3.6.1/test/test_storage_node_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1790 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_storage_node_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)      799 2022-12-02 15:38:55.000000 elements-sdk-3.6.1/test/test_storage_node_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      777 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_storage_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      784 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_storage_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      756 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_storage_root.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1316 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stornext_license.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1653 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_stornext_manager_attributes.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8425 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subclip.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10694 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subclip_clipboard_entry.py
+-rw-r--r--   0 eugene     (501) staff       (20)      985 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subclip_clipboard_entry_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7260 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subclip_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8465 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subclip_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1035 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subclip_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      762 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subscription.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2011 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subtask.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1980 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subtask_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2001 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_subtask_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      770 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subtask_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      837 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subtitle.py
+-rw-r--r--   0 eugene     (501) staff       (20)      958 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subtitle_clipboard_entry.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1001 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subtitle_clipboard_entry_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      770 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_subtitle_event.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1233 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_sync_totp.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1310 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_sync_totp_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4521 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_system_info_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1466 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tag_media_directory_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1410 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tag_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1738 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2340 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2927 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_group.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2192 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_group_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      888 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_tape_group_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2963 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_job.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1406 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_job_source.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3318 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1509 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_format_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1487 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_fsck_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1487 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_load_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1542 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_move_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1520 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_reindex_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1410 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_slot.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1509 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_library_unload_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1797 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1811 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tape_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)      749 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_tape_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10289 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_task_info.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1220 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_task_log.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1310 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_task_progress.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3340 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_task_type.py
+-rw-r--r--   0 eugene     (501) staff       (20)    43603 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_tasks_summary.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1496 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_teams_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1429 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_teams_connection_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1433 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_teams_connection_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_teams_connection_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1344 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_teams_message.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1330 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_teams_recipient.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1525 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_test_aws_credentials_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1525 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_test_aws_credentials_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)      920 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_test_cloud_account_credentials_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1025 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_test_cloud_account_credentials_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1643 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_test_external_transcoder_connection_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1589 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_test_external_transcoder_connection_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1235 2022-02-22 16:08:42.000000 elements-sdk-3.6.1/test/test_test_smtp.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1213 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_ticket.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1631 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_time_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2019 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_time_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1406 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_time_sync_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1417 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_time_sync_endpoint_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1512 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_timeline_export_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1262 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_timezone.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1583 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_trace_node.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1616 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_transcoder_profile.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1387 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_type_documentation.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1521 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_unfiltered_tag.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1542 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_unfiltered_tag_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      813 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_unfiltered_tag_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1344 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_update_quota_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      946 2022-12-02 15:38:56.000000 elements-sdk-3.6.1/test/test_updated_file.py
+-rw-r--r--   0 eugene     (501) staff       (20)      821 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_upload_ai_image_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1484 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_upload_chunk_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)      863 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_upload_image_endpoint_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1353 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_user_preview_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1425 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_user_preview_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1363 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_vantage_workflow.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1665 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_vantage_workflows.py
+-rw-r--r--   0 eugene     (501) staff       (20)      805 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_veritone_connection.py
+-rw-r--r--   0 eugene     (501) staff       (20)      806 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_veritone_engine_list.py
+-rw-r--r--   0 eugene     (501) staff       (20)      785 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_veritone_job_list.py
+-rw-r--r--   0 eugene     (501) staff       (20)      791 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_veritone_metadata.py
+-rw-r--r--   0 eugene     (501) staff       (20)      827 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_veritone_upload_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     6897 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4086 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_bee_gfs_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4869 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_lizard_fs_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1389 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1490 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_mini_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1740 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     6926 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_reference.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2145 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_snfs_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1385 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_stat.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1676 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_stats.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5170 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_volume_status.py
+-rw-r--r--   0 eugene     (501) staff       (20)      763 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_volume_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1713 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workflow_transition_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)    22519 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workflow_transition_response.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4907 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1366 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_check_in.py
+-rw-r--r--   0 eugene     (501) staff       (20)    11539 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_detail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     9713 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_detail_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1057 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_workspace_detail_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1718 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_endpoint.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1401 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_move_to_request.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5645 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)     5734 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_permission_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)      855 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_workspace_permission_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1570 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workspace_resolved_permission.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7541 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workstation.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1408 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workstation_mini.py
+-rw-r--r--   0 eugene     (501) staff       (20)     6469 2022-02-22 16:08:43.000000 elements-sdk-3.6.1/test/test_workstation_partial_update.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1074 2022-02-22 16:14:46.000000 elements-sdk-3.6.1/test/test_workstation_update.py
```

### Comparing `elements-sdk-3.6.0/LICENSE` & `elements-sdk-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/README.md` & `elements-sdk-3.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # ELEMENTS Python SDK
 
 - API version: 2
 - Python 2.7 and 3.4+
-- Latest build: 3.6.0
+- Latest build: 3.6.1
 
 ## Installation & Usage
 
 ```sh
 pip install elements-sdk
 ```
```

### Comparing `elements-sdk-3.6.0/elements_sdk/__init__.py` & `elements-sdk-3.6.1/elements_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 2
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "3.6.0"
+__version__ = "3.6.1"
 
 # import ApiClient
 from elements_sdk.api_client import ApiClient
 
 # import Configuration
 from elements_sdk.configuration import Configuration
```

### Comparing `elements-sdk-3.6.0/elements_sdk/api/ai_api.py` & `elements-sdk-3.6.1/elements_sdk/api/ai_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/auth_api.py` & `elements-sdk-3.6.1/elements_sdk/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/automation_api.py` & `elements-sdk-3.6.1/elements_sdk/api/automation_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/aws_api.py` & `elements-sdk-3.6.1/elements_sdk/api/aws_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/click_api.py` & `elements-sdk-3.6.1/elements_sdk/api/click_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/integrations_api.py` & `elements-sdk-3.6.1/elements_sdk/api/integrations_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/main_api.py` & `elements-sdk-3.6.1/elements_sdk/api/main_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/media_library_api.py` & `elements-sdk-3.6.1/elements_sdk/api/media_library_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/private_api.py` & `elements-sdk-3.6.1/elements_sdk/api/private_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/satellite_api.py` & `elements-sdk-3.6.1/elements_sdk/api/satellite_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/sharedstorage_api.py` & `elements-sdk-3.6.1/elements_sdk/api/sharedstorage_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/status_api.py` & `elements-sdk-3.6.1/elements_sdk/api/status_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api/storage_api.py` & `elements-sdk-3.6.1/elements_sdk/api/storage_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -2131,14 +2131,18 @@
                     'production__active',
                     'name',
                     'is_external',
                     'active',
                     'ordering',
                     'limit',
                     'offset',
+                    'full_path',
+                    'resolve_access_for',
+                    'include_endpoints',
+                    'include_quotas',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -2172,14 +2176,22 @@
                         (str,),
                     'ordering':
                         (str,),
                     'limit':
                         (int,),
                     'offset':
                         (int,),
+                    'full_path':
+                        (str,),
+                    'resolve_access_for':
+                        (int,),
+                    'include_endpoints':
+                        (bool,),
+                    'include_quotas':
+                        (bool,),
                 },
                 'attribute_map': {
                     'is_template': 'is_template',
                     'production': 'production',
                     'volume': 'volume',
                     'home_for': 'home_for',
                     'volume__type': 'volume__type',
@@ -2187,14 +2199,18 @@
                     'production__active': 'production__active',
                     'name': 'name',
                     'is_external': 'is_external',
                     'active': 'active',
                     'ordering': 'ordering',
                     'limit': 'limit',
                     'offset': 'offset',
+                    'full_path': 'full_path',
+                    'resolve_access_for': 'resolve_access_for',
+                    'include_endpoints': 'include_endpoints',
+                    'include_quotas': 'include_quotas',
                 },
                 'location_map': {
                     'is_template': 'query',
                     'production': 'query',
                     'volume': 'query',
                     'home_for': 'query',
                     'volume__type': 'query',
@@ -2202,14 +2218,18 @@
                     'production__active': 'query',
                     'name': 'query',
                     'is_external': 'query',
                     'active': 'query',
                     'ordering': 'query',
                     'limit': 'query',
                     'offset': 'query',
+                    'full_path': 'query',
+                    'resolve_access_for': 'query',
+                    'include_endpoints': 'query',
+                    'include_quotas': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
@@ -7061,14 +7081,18 @@
             production__active (str): Filter the returned list by `production__active`.. [optional]
             name (str): Filter the returned list by `name`.. [optional]
             is_external (str): Filter the returned list by `is_external`.. [optional]
             active (str): Filter the returned list by `active`.. [optional]
             ordering (str): Which field to use when ordering the results.. [optional]
             limit (int): Number of results to return per page.. [optional]
             offset (int): The initial index from which to return the results.. [optional]
+            full_path (str): [optional]
+            resolve_access_for (int): [optional]
+            include_endpoints (bool): [optional]
+            include_quotas (bool): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `elements-sdk-3.6.0/elements_sdk/api/tape_archive_api.py` & `elements-sdk-3.6.1/elements_sdk/api/tape_archive_api.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/api_client.py` & `elements-sdk-3.6.1/elements_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/3.6.0/python'
+        self.user_agent = 'OpenAPI-Generator/3.6.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `elements-sdk-3.6.0/elements_sdk/apis/__init__.py` & `elements-sdk-3.6.1/elements_sdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/configuration.py` & `elements-sdk-3.6.1/elements_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2\n"\
-               "SDK Package Version: 3.6.0".\
+               "SDK Package Version: 3.6.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `elements-sdk-3.6.0/elements_sdk/exceptions.py` & `elements-sdk-3.6.1/elements_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/add_assets_to_click_gallery.py` & `elements-sdk-3.6.1/elements_sdk/model/add_assets_to_click_gallery.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/address.py` & `elements-sdk-3.6.1/elements_sdk/model/address.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_annotation.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_annotation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_annotation_create_request.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_annotation_create_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_annotation_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_annotation_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_annotation_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_annotation_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_category.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_category.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_category_detail.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_category_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_category_detail_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_category_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_category_detail_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_category_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_category_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_category_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_connection.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_detail_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_detail_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_export_request.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_export_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_export_response.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_export_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_with_preview.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_with_preview.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_with_preview_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_with_preview_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_dataset_with_preview_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_dataset_with_preview_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_image.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_image.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_image_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_image_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_metadata.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_export_request.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_export_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_export_response.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_export_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_inference_request.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_inference_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_inference_response.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_inference_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_progress.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_progress.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_training_request.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_training_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_model_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_model_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ai_processing_request.py` & `elements-sdk-3.6.1/elements_sdk/model/ai_processing_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/alert.py` & `elements-sdk-3.6.1/elements_sdk/model/alert.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/alert_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/alert_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/alert_update.py` & `elements-sdk-3.6.1/elements_sdk/model/alert_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/all_media_files_for_bundles_request.py` & `elements-sdk-3.6.1/elements_sdk/model/all_media_files_for_bundles_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/api_token.py` & `elements-sdk-3.6.1/elements_sdk/model/api_token.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/api_token_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/api_token_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/api_token_update.py` & `elements-sdk-3.6.1/elements_sdk/model/api_token_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/api_token_with_secret.py` & `elements-sdk-3.6.1/elements_sdk/model/api_token_with_secret.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/api_token_with_secret_update.py` & `elements-sdk-3.6.1/elements_sdk/model/api_token_with_secret_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/archive_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/archive_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/argument_type.py` & `elements-sdk-3.6.1/elements_sdk/model/argument_type.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset.py` & `elements-sdk-3.6.1/elements_sdk/model/asset.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_backup.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_backup.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_cloud_link.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_cloud_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_project_link.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_project_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_rating.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_rating.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_rating_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_rating_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_rating_update.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_rating_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_subtitle_link.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_subtitle_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_subtitle_link_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_subtitle_link_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_subtitle_link_update.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_subtitle_link_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/asset_update.py` & `elements-sdk-3.6.1/elements_sdk/model/asset_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/auth_login_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/auth_login_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/auth_login_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/auth_login_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/backend.py` & `elements-sdk-3.6.1/elements_sdk/model/backend.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/backend_properties.py` & `elements-sdk-3.6.1/elements_sdk/model/backend_properties.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/basic_file.py` & `elements-sdk-3.6.1/elements_sdk/model/basic_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/bee_gfs_node.py` & `elements-sdk-3.6.1/elements_sdk/model/bee_gfs_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/bee_gfs_target.py` & `elements-sdk-3.6.1/elements_sdk/model/bee_gfs_target.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/bootstrap_data.py` & `elements-sdk-3.6.1/elements_sdk/model/bootstrap_data.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/certificate.py` & `elements-sdk-3.6.1/elements_sdk/model/certificate.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/certificate_update.py` & `elements-sdk-3.6.1/elements_sdk/model/certificate_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/change_own_password_request.py` & `elements-sdk-3.6.1/elements_sdk/model/change_own_password_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/change_password_request.py` & `elements-sdk-3.6.1/elements_sdk/model/change_password_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/check_connectivity_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/check_connectivity_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/click_background_upload_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/click_background_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/click_gallery.py` & `elements-sdk-3.6.1/elements_sdk/model/click_gallery.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/click_gallery_link.py` & `elements-sdk-3.6.1/elements_sdk/model/click_gallery_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/click_gallery_update.py` & `elements-sdk-3.6.1/elements_sdk/model/click_gallery_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/click_link_user.py` & `elements-sdk-3.6.1/elements_sdk/model/click_link_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/click_start_upload_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/click_start_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/client_session.py` & `elements-sdk-3.6.1/elements_sdk/model/client_session.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/client_side_path_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/client_side_path_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/client_side_path_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/client_side_path_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/clients_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/clients_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_account.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_account.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_account_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_account_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_account_mini_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_account_mini_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_account_mini_update.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_account_mini_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_account_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_account_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_account_update.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_account_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_bucket_costs.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_bucket_costs.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_connection.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_mount_authorization.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_mount_authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
             'secret': (str,),  # noqa: E501
             'access_id': (str, none_type,),  # noqa: E501
             'project_id': (str, none_type,),  # noqa: E501
             'endpoint': (str, none_type,),  # noqa: E501
             'token': (str, none_type,),  # noqa: E501
             'tenant': (str, none_type,),  # noqa: E501
             'subscription': (str, none_type,),  # noqa: E501
+            'expiry': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -120,14 +121,15 @@
         'secret': 'secret',  # noqa: E501
         'access_id': 'access_id',  # noqa: E501
         'project_id': 'project_id',  # noqa: E501
         'endpoint': 'endpoint',  # noqa: E501
         'token': 'token',  # noqa: E501
         'tenant': 'tenant',  # noqa: E501
         'subscription': 'subscription',  # noqa: E501
+        'expiry': 'expiry',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -172,14 +174,15 @@
                                 _visited_composed_classes = (Animal,)
             access_id (str, none_type): [optional]  # noqa: E501
             project_id (str, none_type): [optional]  # noqa: E501
             endpoint (str, none_type): [optional]  # noqa: E501
             token (str, none_type): [optional]  # noqa: E501
             tenant (str, none_type): [optional]  # noqa: E501
             subscription (str, none_type): [optional]  # noqa: E501
+            expiry (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
@@ -265,14 +268,15 @@
                                 _visited_composed_classes = (Animal,)
             access_id (str, none_type): [optional]  # noqa: E501
             project_id (str, none_type): [optional]  # noqa: E501
             endpoint (str, none_type): [optional]  # noqa: E501
             token (str, none_type): [optional]  # noqa: E501
             tenant (str, none_type): [optional]  # noqa: E501
             subscription (str, none_type): [optional]  # noqa: E501
+            expiry (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cloud_storage_costs.py` & `elements-sdk-3.6.1/elements_sdk/model/cloud_storage_costs.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/comment.py` & `elements-sdk-3.6.1/elements_sdk/model/comment.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/comment_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/comment_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/comment_update.py` & `elements-sdk-3.6.1/elements_sdk/model/comment_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cost.py` & `elements-sdk-3.6.1/elements_sdk/model/cost.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/cpu_stat.py` & `elements-sdk-3.6.1/elements_sdk/model/cpu_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/create_download_archive.py` & `elements-sdk-3.6.1/elements_sdk/model/create_download_archive.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/create_home_workspace_request.py` & `elements-sdk-3.6.1/elements_sdk/model/create_home_workspace_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/create_path_quota_request.py` & `elements-sdk-3.6.1/elements_sdk/model/create_path_quota_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/create_template_folder_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/create_template_folder_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/custom_field.py` & `elements-sdk-3.6.1/elements_sdk/model/custom_field.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/custom_field_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/custom_field_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/custom_field_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/custom_field_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/custom_field_update.py` & `elements-sdk-3.6.1/elements_sdk/model/custom_field_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/deleted_workspace.py` & `elements-sdk-3.6.1/elements_sdk/model/deleted_workspace.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/download.py` & `elements-sdk-3.6.1/elements_sdk/model/download.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/download_archive.py` & `elements-sdk-3.6.1/elements_sdk/model/download_archive.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/download_archive_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/download_archive_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/download_archive_update.py` & `elements-sdk-3.6.1/elements_sdk/model/download_archive_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/editor_project.py` & `elements-sdk-3.6.1/elements_sdk/model/editor_project.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/editor_project_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/editor_project_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/editor_project_update.py` & `elements-sdk-3.6.1/elements_sdk/model/editor_project_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/editor_subtitle.py` & `elements-sdk-3.6.1/elements_sdk/model/editor_subtitle.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/editor_subtitle_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/editor_subtitle_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/editor_subtitle_update.py` & `elements-sdk-3.6.1/elements_sdk/model/editor_subtitle_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_group.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,22 +62,14 @@
     }
 
     validations = {
         ('name',): {
             'max_length': 255,
             'min_length': 1,
         },
-        ('ancillary_path',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
-        ('ancillary_path_read_only',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
         ('ldap_dn',): {
             'max_length': 255,
         },
         ('unix_groupname',): {
             'max_length': 255,
         },
         ('gid',): {
@@ -111,16 +103,14 @@
         return {
             'id': (int,),  # noqa: E501
             'members_preview': ([MemberPreview],),  # noqa: E501
             'effective_permissions': ([str, none_type],),  # noqa: E501
             'name': (str,),  # noqa: E501
             'members': ([int],),  # noqa: E501
             'permissions': ([str, none_type],),  # noqa: E501
-            'ancillary_path': (str, none_type,),  # noqa: E501
-            'ancillary_path_read_only': (str, none_type,),  # noqa: E501
             'ldap_dn': (str, none_type,),  # noqa: E501
             'unix_groupname': (str, none_type,),  # noqa: E501
             'gid': (int, none_type,),  # noqa: E501
             'ldap': (int, none_type,),  # noqa: E501
         }
 
     @cached_property
@@ -131,27 +121,23 @@
     attribute_map = {
         'id': 'id',  # noqa: E501
         'members_preview': 'members_preview',  # noqa: E501
         'effective_permissions': 'effective_permissions',  # noqa: E501
         'name': 'name',  # noqa: E501
         'members': 'members',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
-        'ancillary_path': 'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only': 'ancillary_path_read_only',  # noqa: E501
         'ldap_dn': 'ldap_dn',  # noqa: E501
         'unix_groupname': 'unix_groupname',  # noqa: E501
         'gid': 'gid',  # noqa: E501
         'ldap': 'ldap',  # noqa: E501
     }
 
     read_only_vars = {
         'members_preview',  # noqa: E501
         'effective_permissions',  # noqa: E501
-        'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, members_preview, effective_permissions, name, members, *args, **xkwargs):  # noqa: E501
@@ -192,16 +178,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             permissions ([str, none_type]): [optional]  # noqa: E501
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             ldap_dn (str, none_type): [optional]  # noqa: E501
             unix_groupname (str, none_type): [optional]  # noqa: E501
             gid (int, none_type): [optional]  # noqa: E501
             ldap (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
@@ -292,16 +276,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             permissions ([str, none_type]): [optional]  # noqa: E501
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             ldap_dn (str, none_type): [optional]  # noqa: E501
             unix_groupname (str, none_type): [optional]  # noqa: E501
             gid (int, none_type): [optional]  # noqa: E501
             ldap (int, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_group_detail.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_group_detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,22 +64,14 @@
     }
 
     validations = {
         ('name',): {
             'max_length': 255,
             'min_length': 1,
         },
-        ('ancillary_path',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
-        ('ancillary_path_read_only',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
         ('ldap_dn',): {
             'max_length': 255,
         },
         ('unix_groupname',): {
             'max_length': 255,
         },
         ('gid',): {
@@ -112,16 +104,14 @@
         lazy_import()
         return {
             'id': (int,),  # noqa: E501
             'members_preview': ([MemberPreview],),  # noqa: E501
             'effective_permissions': ([str, none_type],),  # noqa: E501
             'name': (str,),  # noqa: E501
             'permissions': ([str, none_type],),  # noqa: E501
-            'ancillary_path': (str, none_type,),  # noqa: E501
-            'ancillary_path_read_only': (str, none_type,),  # noqa: E501
             'members': ([ElementsUserReference],),  # noqa: E501
             'ldap': (bool, date, datetime, dict, float, int, list, str, none_type,),  # noqa: E501
             'ldap_dn': (str, none_type,),  # noqa: E501
             'unix_groupname': (str, none_type,),  # noqa: E501
             'gid': (int, none_type,),  # noqa: E501
         }
 
@@ -132,28 +122,24 @@
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'members_preview': 'members_preview',  # noqa: E501
         'effective_permissions': 'effective_permissions',  # noqa: E501
         'name': 'name',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
-        'ancillary_path': 'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only': 'ancillary_path_read_only',  # noqa: E501
         'members': 'members',  # noqa: E501
         'ldap': 'ldap',  # noqa: E501
         'ldap_dn': 'ldap_dn',  # noqa: E501
         'unix_groupname': 'unix_groupname',  # noqa: E501
         'gid': 'gid',  # noqa: E501
     }
 
     read_only_vars = {
         'members_preview',  # noqa: E501
         'effective_permissions',  # noqa: E501
-        'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, members_preview, effective_permissions, name, *args, **xkwargs):  # noqa: E501
@@ -193,16 +179,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             permissions ([str, none_type]): [optional]  # noqa: E501
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             members ([ElementsUserReference]): [optional]  # noqa: E501
             ldap (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             ldap_dn (str, none_type): [optional]  # noqa: E501
             unix_groupname (str, none_type): [optional]  # noqa: E501
             gid (int, none_type): [optional]  # noqa: E501
         """
 
@@ -292,16 +276,14 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             permissions ([str, none_type]): [optional]  # noqa: E501
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             members ([ElementsUserReference]): [optional]  # noqa: E501
             ldap (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             ldap_dn (str, none_type): [optional]  # noqa: E501
             unix_groupname (str, none_type): [optional]  # noqa: E501
             gid (int, none_type): [optional]  # noqa: E501
         """
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_group_detail_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_group_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_group_detail_update.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_group_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_group_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_group_reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,22 +58,14 @@
           as additional properties values.
     """
 
     allowed_values = {
     }
 
     validations = {
-        ('ancillary_path',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
-        ('ancillary_path_read_only',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
         ('name',): {
             'max_length': 255,
             'min_length': 1,
         },
         ('ldap_dn',): {
             'max_length': 255,
         },
@@ -109,16 +101,14 @@
         """
         lazy_import()
         return {
             'id': (int,),  # noqa: E501
             'permissions': ([str, none_type],),  # noqa: E501
             'members_preview': ([MemberPreview],),  # noqa: E501
             'effective_permissions': ([str, none_type],),  # noqa: E501
-            'ancillary_path': (str, none_type,),  # noqa: E501
-            'ancillary_path_read_only': (str, none_type,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'ldap_dn': (str, none_type,),  # noqa: E501
             'unix_groupname': (str, none_type,),  # noqa: E501
             'gid': (int, none_type,),  # noqa: E501
             'ldap': (int, none_type,),  # noqa: E501
             'members': ([int],),  # noqa: E501
         }
@@ -129,30 +119,26 @@
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
         'members_preview': 'members_preview',  # noqa: E501
         'effective_permissions': 'effective_permissions',  # noqa: E501
-        'ancillary_path': 'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only': 'ancillary_path_read_only',  # noqa: E501
         'name': 'name',  # noqa: E501
         'ldap_dn': 'ldap_dn',  # noqa: E501
         'unix_groupname': 'unix_groupname',  # noqa: E501
         'gid': 'gid',  # noqa: E501
         'ldap': 'ldap',  # noqa: E501
         'members': 'members',  # noqa: E501
     }
 
     read_only_vars = {
         'permissions',  # noqa: E501
         'members_preview',  # noqa: E501
         'effective_permissions',  # noqa: E501
-        'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only',  # noqa: E501
         'name',  # noqa: E501
         'ldap_dn',  # noqa: E501
         'unix_groupname',  # noqa: E501
         'gid',  # noqa: E501
         'ldap',  # noqa: E501
         'members',  # noqa: E501
     }
@@ -197,16 +183,14 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             permissions ([str, none_type]): [optional]  # noqa: E501
             members_preview ([MemberPreview]): [optional]  # noqa: E501
             effective_permissions ([str, none_type]): [optional]  # noqa: E501
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
             ldap_dn (str, none_type): [optional]  # noqa: E501
             unix_groupname (str, none_type): [optional]  # noqa: E501
             gid (int, none_type): [optional]  # noqa: E501
             ldap (int, none_type): [optional]  # noqa: E501
             members ([int]): [optional]  # noqa: E501
         """
@@ -295,16 +279,14 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             permissions ([str, none_type]): [optional]  # noqa: E501
             members_preview ([MemberPreview]): [optional]  # noqa: E501
             effective_permissions ([str, none_type]): [optional]  # noqa: E501
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             name (str): [optional]  # noqa: E501
             ldap_dn (str, none_type): [optional]  # noqa: E501
             unix_groupname (str, none_type): [optional]  # noqa: E501
             gid (int, none_type): [optional]  # noqa: E501
             ldap (int, none_type): [optional]  # noqa: E501
             members ([int]): [optional]  # noqa: E501
         """
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,22 +65,14 @@
     }
 
     validations = {
         ('username',): {
             'max_length': 255,
             'min_length': 1,
         },
-        ('ancillary_path',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
-        ('ancillary_path_read_only',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
         ('default_page',): {
             'max_length': 63,
             'min_length': 1,
         },
         ('email',): {
             'max_length': 255,
         },
@@ -140,16 +132,14 @@
             'group_permissions': ([str, none_type],),  # noqa: E501
             'has_password': (bool,),  # noqa: E501
             'is_cloud_default': (bool,),  # noqa: E501
             'permissions': ([str, none_type],),  # noqa: E501
             'sync_id': (str,),  # noqa: E501
             'totp_enabled': (bool,),  # noqa: E501
             'username': (str,),  # noqa: E501
-            'ancillary_path': (str, none_type,),  # noqa: E501
-            'ancillary_path_read_only': (str, none_type,),  # noqa: E501
             'allow_changing_password': (bool,),  # noqa: E501
             'allow_wan_login': (bool,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'default_page': (str,),  # noqa: E501
             'email': (str, none_type,),  # noqa: E501
             'expiry': (datetime, none_type,),  # noqa: E501
             'fm_bookmarks': ([str, none_type],),  # noqa: E501
@@ -184,16 +174,14 @@
         'group_permissions': 'group_permissions',  # noqa: E501
         'has_password': 'has_password',  # noqa: E501
         'is_cloud_default': 'is_cloud_default',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
         'sync_id': 'sync_id',  # noqa: E501
         'totp_enabled': 'totp_enabled',  # noqa: E501
         'username': 'username',  # noqa: E501
-        'ancillary_path': 'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only': 'ancillary_path_read_only',  # noqa: E501
         'allow_changing_password': 'allow_changing_password',  # noqa: E501
         'allow_wan_login': 'allow_wan_login',  # noqa: E501
         'avatar': 'avatar',  # noqa: E501
         'default_page': 'default_page',  # noqa: E501
         'email': 'email',  # noqa: E501
         'expiry': 'expiry',  # noqa: E501
         'fm_bookmarks': 'fm_bookmarks',  # noqa: E501
@@ -220,16 +208,14 @@
         'display_name',  # noqa: E501
         'effective_permissions',  # noqa: E501
         'group_permissions',  # noqa: E501
         'has_password',  # noqa: E501
         'is_cloud_default',  # noqa: E501
         'sync_id',  # noqa: E501
         'totp_enabled',  # noqa: E501
-        'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only',  # noqa: E501
         'last_seen',  # noqa: E501
         'ldap',  # noqa: E501
         'ldap_dn',  # noqa: E501
     }
 
     _composed_schemas = {}
 
@@ -279,16 +265,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             allow_changing_password (bool): [optional]  # noqa: E501
             allow_wan_login (bool): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             default_page (str): [optional]  # noqa: E501
             email (str, none_type): [optional]  # noqa: E501
             expiry (datetime, none_type): [optional]  # noqa: E501
             fm_bookmarks ([str, none_type]): [optional]  # noqa: E501
@@ -403,16 +387,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             allow_changing_password (bool): [optional]  # noqa: E501
             allow_wan_login (bool): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             default_page (str): [optional]  # noqa: E501
             email (str, none_type): [optional]  # noqa: E501
             expiry (datetime, none_type): [optional]  # noqa: E501
             fm_bookmarks ([str, none_type]): [optional]  # noqa: E501
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_detail.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_detail.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,22 +65,14 @@
     }
 
     validations = {
         ('username',): {
             'max_length': 255,
             'min_length': 1,
         },
-        ('ancillary_path',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
-        ('ancillary_path_read_only',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
         ('default_page',): {
             'max_length': 63,
             'min_length': 1,
         },
         ('email',): {
             'max_length': 255,
         },
@@ -139,16 +131,14 @@
             'effective_permissions': ([str, none_type],),  # noqa: E501
             'group_permissions': ([str, none_type],),  # noqa: E501
             'has_password': (bool,),  # noqa: E501
             'permissions': ([str, none_type],),  # noqa: E501
             'sync_id': (str,),  # noqa: E501
             'username': (str,),  # noqa: E501
             'groups': ([int],),  # noqa: E501
-            'ancillary_path': (str, none_type,),  # noqa: E501
-            'ancillary_path_read_only': (str, none_type,),  # noqa: E501
             'allow_changing_password': (bool,),  # noqa: E501
             'allow_wan_login': (bool,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'default_page': (str,),  # noqa: E501
             'email': (str, none_type,),  # noqa: E501
             'expiry': (datetime, none_type,),  # noqa: E501
             'fm_bookmarks': ([str, none_type],),  # noqa: E501
@@ -184,16 +174,14 @@
         'effective_permissions': 'effective_permissions',  # noqa: E501
         'group_permissions': 'group_permissions',  # noqa: E501
         'has_password': 'has_password',  # noqa: E501
         'permissions': 'permissions',  # noqa: E501
         'sync_id': 'sync_id',  # noqa: E501
         'username': 'username',  # noqa: E501
         'groups': 'groups',  # noqa: E501
-        'ancillary_path': 'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only': 'ancillary_path_read_only',  # noqa: E501
         'allow_changing_password': 'allow_changing_password',  # noqa: E501
         'allow_wan_login': 'allow_wan_login',  # noqa: E501
         'avatar': 'avatar',  # noqa: E501
         'default_page': 'default_page',  # noqa: E501
         'email': 'email',  # noqa: E501
         'expiry': 'expiry',  # noqa: E501
         'fm_bookmarks': 'fm_bookmarks',  # noqa: E501
@@ -220,16 +208,14 @@
         'allowed_fs_paths',  # noqa: E501
         'allowed_fs_write_paths',  # noqa: E501
         'display_name',  # noqa: E501
         'effective_permissions',  # noqa: E501
         'group_permissions',  # noqa: E501
         'has_password',  # noqa: E501
         'sync_id',  # noqa: E501
-        'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, allowed_fs_paths, allowed_fs_write_paths, display_name, effective_permissions, group_permissions, has_password, permissions, sync_id, username, groups, *args, **xkwargs):  # noqa: E501
@@ -275,16 +261,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             allow_changing_password (bool): [optional]  # noqa: E501
             allow_wan_login (bool): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             default_page (str): [optional]  # noqa: E501
             email (str, none_type): [optional]  # noqa: E501
             expiry (datetime, none_type): [optional]  # noqa: E501
             fm_bookmarks ([str, none_type]): [optional]  # noqa: E501
@@ -401,16 +385,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             allow_changing_password (bool): [optional]  # noqa: E501
             allow_wan_login (bool): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             default_page (str): [optional]  # noqa: E501
             email (str, none_type): [optional]  # noqa: E501
             expiry (datetime, none_type): [optional]  # noqa: E501
             fm_bookmarks ([str, none_type]): [optional]  # noqa: E501
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_detail_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_detail_update.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_profile.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_profile.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_profile_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_profile_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_profile_update.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_profile_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_user_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_user_reference.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,22 +61,14 @@
             'FR': "fr",
             'DE': "de",
             'RU': "ru",
         },
     }
 
     validations = {
-        ('ancillary_path',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
-        ('ancillary_path_read_only',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
         ('default_page',): {
             'max_length': 63,
             'min_length': 1,
         },
         ('email',): {
             'max_length': 255,
         },
@@ -129,16 +121,14 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'id': (int,),  # noqa: E501
-            'ancillary_path': (str, none_type,),  # noqa: E501
-            'ancillary_path_read_only': (str, none_type,),  # noqa: E501
             'allow_changing_password': (bool,),  # noqa: E501
             'allow_wan_login': (bool,),  # noqa: E501
             'allowed_fs_paths': ([str, none_type], none_type,),  # noqa: E501
             'allowed_fs_write_paths': ([str, none_type], none_type,),  # noqa: E501
             'avatar': (str, none_type,),  # noqa: E501
             'default_page': (str,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
@@ -173,16 +163,14 @@
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
-        'ancillary_path': 'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only': 'ancillary_path_read_only',  # noqa: E501
         'allow_changing_password': 'allow_changing_password',  # noqa: E501
         'allow_wan_login': 'allow_wan_login',  # noqa: E501
         'allowed_fs_paths': 'allowed_fs_paths',  # noqa: E501
         'allowed_fs_write_paths': 'allowed_fs_write_paths',  # noqa: E501
         'avatar': 'avatar',  # noqa: E501
         'default_page': 'default_page',  # noqa: E501
         'display_name': 'display_name',  # noqa: E501
@@ -211,16 +199,14 @@
         'totp_enabled': 'totp_enabled',  # noqa: E501
         'uid': 'uid',  # noqa: E501
         'unix_username': 'unix_username',  # noqa: E501
         'username': 'username',  # noqa: E501
     }
 
     read_only_vars = {
-        'ancillary_path',  # noqa: E501
-        'ancillary_path_read_only',  # noqa: E501
         'allow_changing_password',  # noqa: E501
         'allow_wan_login',  # noqa: E501
         'allowed_fs_paths',  # noqa: E501
         'allowed_fs_write_paths',  # noqa: E501
         'avatar',  # noqa: E501
         'default_page',  # noqa: E501
         'display_name',  # noqa: E501
@@ -289,16 +275,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             allow_changing_password (bool): [optional]  # noqa: E501
             allow_wan_login (bool): [optional]  # noqa: E501
             allowed_fs_paths ([str, none_type], none_type): [optional]  # noqa: E501
             allowed_fs_write_paths ([str, none_type], none_type): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             default_page (str): [optional]  # noqa: E501
             display_name (str): [optional]  # noqa: E501
@@ -411,16 +395,14 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            ancillary_path (str, none_type): [optional]  # noqa: E501
-            ancillary_path_read_only (str, none_type): [optional]  # noqa: E501
             allow_changing_password (bool): [optional]  # noqa: E501
             allow_wan_login (bool): [optional]  # noqa: E501
             allowed_fs_paths ([str, none_type], none_type): [optional]  # noqa: E501
             allowed_fs_write_paths ([str, none_type], none_type): [optional]  # noqa: E501
             avatar (str, none_type): [optional]  # noqa: E501
             default_page (str): [optional]  # noqa: E501
             display_name (str): [optional]  # noqa: E501
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/elements_version.py` & `elements-sdk-3.6.1/elements_sdk/model/elements_version.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/email_preview.py` & `elements-sdk-3.6.1/elements_sdk/model/email_preview.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/enable_totp_request.py` & `elements-sdk-3.6.1/elements_sdk/model/enable_totp_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/event.py` & `elements-sdk-3.6.1/elements_sdk/model/event.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/external_transcoder.py` & `elements-sdk-3.6.1/elements_sdk/model/external_transcoder.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/external_transcoder_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/external_transcoder_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/external_transcoder_update.py` & `elements-sdk-3.6.1/elements_sdk/model/external_transcoder_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/extract_request.py` & `elements-sdk-3.6.1/elements_sdk/model/extract_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_copy_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/file_copy_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_delete_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/file_delete_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_move_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/file_move_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/file_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_size_distribution.py` & `elements-sdk-3.6.1/elements_sdk/model/file_size_distribution.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_size_distribution_item.py` & `elements-sdk-3.6.1/elements_sdk/model/file_size_distribution_item.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_size_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/file_size_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_unzip_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/file_unzip_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_update.py` & `elements-sdk-3.6.1/elements_sdk/model/file_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/file_zip_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/file_zip_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/filesystem_file.py` & `elements-sdk-3.6.1/elements_sdk/model/filesystem_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/filesystem_permission.py` & `elements-sdk-3.6.1/elements_sdk/model/filesystem_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/filesystem_permission_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/filesystem_permission_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/filesystem_permission_update.py` & `elements-sdk-3.6.1/elements_sdk/model/filesystem_permission_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/filesystem_trace_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/filesystem_trace_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/filesystem_trace_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/filesystem_trace_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/finish_upload_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/finish_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/format_metadata.py` & `elements-sdk-3.6.1/elements_sdk/model/format_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/fs_properties.py` & `elements-sdk-3.6.1/elements_sdk/model/fs_properties.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/generate_password_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/generate_password_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/generate_proxies_request.py` & `elements-sdk-3.6.1/elements_sdk/model/generate_proxies_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/get_cloud_account_costs_response.py` & `elements-sdk-3.6.1/elements_sdk/model/get_cloud_account_costs_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/get_cloud_account_volume_sizes_response.py` & `elements-sdk-3.6.1/elements_sdk/model/get_cloud_account_volume_sizes_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/get_multiple_bundles_request.py` & `elements-sdk-3.6.1/elements_sdk/model/get_multiple_bundles_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/get_multiple_files_request.py` & `elements-sdk-3.6.1/elements_sdk/model/get_multiple_files_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/global_alert.py` & `elements-sdk-3.6.1/elements_sdk/model/global_alert.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/help_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/help_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/image_upload_request.py` & `elements-sdk-3.6.1/elements_sdk/model/image_upload_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/impersonation_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/impersonation_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/import_ai_dataset_request.py` & `elements-sdk-3.6.1/elements_sdk/model/import_ai_dataset_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/import_ai_dataset_response.py` & `elements-sdk-3.6.1/elements_sdk/model/import_ai_dataset_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/import_ai_model_request.py` & `elements-sdk-3.6.1/elements_sdk/model/import_ai_model_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/import_ai_model_response.py` & `elements-sdk-3.6.1/elements_sdk/model/import_ai_model_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/import_job_request.py` & `elements-sdk-3.6.1/elements_sdk/model/import_job_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/import_job_response.py` & `elements-sdk-3.6.1/elements_sdk/model/import_job_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/inline_response200.py` & `elements-sdk-3.6.1/elements_sdk/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/install_license_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/install_license_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/instantiate_file_template_request.py` & `elements-sdk-3.6.1/elements_sdk/model/instantiate_file_template_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/interface.py` & `elements-sdk-3.6.1/elements_sdk/model/interface.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/io_stat.py` & `elements-sdk-3.6.1/elements_sdk/model/io_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ipmi.py` & `elements-sdk-3.6.1/elements_sdk/model/ipmi.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/job.py` & `elements-sdk-3.6.1/elements_sdk/model/job.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/job_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/job_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/job_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/job_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/job_update.py` & `elements-sdk-3.6.1/elements_sdk/model/job_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/kapacitor_alert.py` & `elements-sdk-3.6.1/elements_sdk/model/kapacitor_alert.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ldap_server.py` & `elements-sdk-3.6.1/elements_sdk/model/ldap_server.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ldap_server_group.py` & `elements-sdk-3.6.1/elements_sdk/model/ldap_server_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ldap_server_groups.py` & `elements-sdk-3.6.1/elements_sdk/model/ldap_server_groups.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ldap_server_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/ldap_server_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ldap_server_user.py` & `elements-sdk-3.6.1/elements_sdk/model/ldap_server_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ldap_server_users.py` & `elements-sdk-3.6.1/elements_sdk/model/ldap_server_users.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/license.py` & `elements-sdk-3.6.1/elements_sdk/model/license.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/list_topics.py` & `elements-sdk-3.6.1/elements_sdk/model/list_topics.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/lizard_fs_disk.py` & `elements-sdk-3.6.1/elements_sdk/model/lizard_fs_disk.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/lizard_fs_node.py` & `elements-sdk-3.6.1/elements_sdk/model/lizard_fs_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/locale_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/locale_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/locate_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/locate_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/locate_proxies_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/locate_proxies_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/locate_proxies_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/locate_proxies_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/locate_result.py` & `elements-sdk-3.6.1/elements_sdk/model/locate_result.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/marker.py` & `elements-sdk-3.6.1/elements_sdk/model/marker.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/marker_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/marker_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/marker_update.py` & `elements-sdk-3.6.1/elements_sdk/model/marker_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_bundle.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_bundle.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_bundle_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_bundle_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_bundle_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_bundle_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_contents.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_contents.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_template.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_template.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_template_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_template_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_template_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_template_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_file_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_file_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_files_lookup_request.py` & `elements-sdk-3.6.1/elements_sdk/model/media_files_lookup_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_library_delete_request.py` & `elements-sdk-3.6.1/elements_sdk/model/media_library_delete_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_library_share_request.py` & `elements-sdk-3.6.1/elements_sdk/model/media_library_share_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_detail.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_detail_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_detail_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_permission.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_permission_access_options.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_permission_access_options.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_permission_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_permission_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_permission_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_permission_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_root_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_root_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/media_update.py` & `elements-sdk-3.6.1/elements_sdk/model/media_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/member_preview.py` & `elements-sdk-3.6.1/elements_sdk/model/member_preview.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/metadata_item.py` & `elements-sdk-3.6.1/elements_sdk/model/metadata_item.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/move_workspace_request.py` & `elements-sdk-3.6.1/elements_sdk/model/move_workspace_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/multiple_assets_request.py` & `elements-sdk-3.6.1/elements_sdk/model/multiple_assets_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/net_stat.py` & `elements-sdk-3.6.1/elements_sdk/model/net_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/nfs_permission.py` & `elements-sdk-3.6.1/elements_sdk/model/nfs_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ntp_server.py` & `elements-sdk-3.6.1/elements_sdk/model/ntp_server.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ntp_server_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ntp_server_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ntp_server_update.py` & `elements-sdk-3.6.1/elements_sdk/model/ntp_server_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/one_time_access_token.py` & `elements-sdk-3.6.1/elements_sdk/model/one_time_access_token.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/one_time_access_token_activity.py` & `elements-sdk-3.6.1/elements_sdk/model/one_time_access_token_activity.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/one_time_access_token_shared_object.py` & `elements-sdk-3.6.1/elements_sdk/model/one_time_access_token_shared_object.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/parameters.py` & `elements-sdk-3.6.1/elements_sdk/model/parameters.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/parameters_update.py` & `elements-sdk-3.6.1/elements_sdk/model/parameters_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/parse_samlidp_metadata_request.py` & `elements-sdk-3.6.1/elements_sdk/model/parse_samlidp_metadata_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/parsed_samlidp_metadata.py` & `elements-sdk-3.6.1/elements_sdk/model/parsed_samlidp_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/password_reset_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/password_reset_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/path.py` & `elements-sdk-3.6.1/elements_sdk/model/path.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/path_input.py` & `elements-sdk-3.6.1/elements_sdk/model/path_input.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/production.py` & `elements-sdk-3.6.1/elements_sdk/model/production.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/production_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/production_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/production_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/production_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/production_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/production_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/production_update.py` & `elements-sdk-3.6.1/elements_sdk/model/production_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_count.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_count.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_fs_size_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_fs_size_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_generator.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_generator.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_generator_properties.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_generator_properties.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_profile.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_profile.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_profile_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_profile_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_profile_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_profile_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/proxy_profile_update.py` & `elements-sdk-3.6.1/elements_sdk/model/proxy_profile_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/python_environment.py` & `elements-sdk-3.6.1/elements_sdk/model/python_environment.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/queue.py` & `elements-sdk-3.6.1/elements_sdk/model/queue.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/quota.py` & `elements-sdk-3.6.1/elements_sdk/model/quota.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ram_stat.py` & `elements-sdk-3.6.1/elements_sdk/model/ram_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/rdc_activation.py` & `elements-sdk-3.6.1/elements_sdk/model/rdc_activation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/rdc_host.py` & `elements-sdk-3.6.1/elements_sdk/model/rdc_host.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/rdc_session.py` & `elements-sdk-3.6.1/elements_sdk/model/rdc_session.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/rdc_session_create.py` & `elements-sdk-3.6.1/elements_sdk/model/rdc_session_create.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/register_upload_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/register_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/register_upload_metadata_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/register_upload_metadata_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/release_notes_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/release_notes_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/rename_custom_field_request.py` & `elements-sdk-3.6.1/elements_sdk/model/rename_custom_field_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/render_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/render_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/render_request.py` & `elements-sdk-3.6.1/elements_sdk/model/render_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/restore_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/restore_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saml_provider.py` & `elements-sdk-3.6.1/elements_sdk/model/saml_provider.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saml_provider_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/saml_provider_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saml_provider_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/saml_provider_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saml_provider_update.py` & `elements-sdk-3.6.1/elements_sdk/model/saml_provider_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saved_search.py` & `elements-sdk-3.6.1/elements_sdk/model/saved_search.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saved_search_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/saved_search_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/saved_search_update.py` & `elements-sdk-3.6.1/elements_sdk/model/saved_search_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/scanner_discover_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/scanner_discover_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/scanner_scan_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/scanner_scan_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/schedule.py` & `elements-sdk-3.6.1/elements_sdk/model/schedule.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/schedule_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/schedule_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/schedule_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/schedule_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/schedule_update.py` & `elements-sdk-3.6.1/elements_sdk/model/schedule_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/search_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/search_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/search_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/search_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/send_link_email_request.py` & `elements-sdk-3.6.1/elements_sdk/model/send_link_email_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/sensor.py` & `elements-sdk-3.6.1/elements_sdk/model/sensor.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/sensors.py` & `elements-sdk-3.6.1/elements_sdk/model/sensors.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/service_status.py` & `elements-sdk-3.6.1/elements_sdk/model/service_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/share.py` & `elements-sdk-3.6.1/elements_sdk/model/share.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/share_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/share_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/share_to_home_workspace_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/share_to_home_workspace_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/share_update.py` & `elements-sdk-3.6.1/elements_sdk/model/share_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_channel.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_channel.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_connection.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_connection_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_connection_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_connection_status.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_connection_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_connection_update.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_connection_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_emoji.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_emoji.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_message.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_message.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/slack_user.py` & `elements-sdk-3.6.1/elements_sdk/model/slack_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/smtp_configuration.py` & `elements-sdk-3.6.1/elements_sdk/model/smtp_configuration.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/smtp_configuration_update.py` & `elements-sdk-3.6.1/elements_sdk/model/smtp_configuration_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/snapshot.py` & `elements-sdk-3.6.1/elements_sdk/model/snapshot.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/snapshot_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/snapshot_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/snapshot_update.py` & `elements-sdk-3.6.1/elements_sdk/model/snapshot_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/snfs_stripe_group.py` & `elements-sdk-3.6.1/elements_sdk/model/snfs_stripe_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/solr_reindex_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/solr_reindex_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/start_job_request.py` & `elements-sdk-3.6.1/elements_sdk/model/start_job_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/start_task_request.py` & `elements-sdk-3.6.1/elements_sdk/model/start_task_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stats.py` & `elements-sdk-3.6.1/elements_sdk/model/stats.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stor_next_connection.py` & `elements-sdk-3.6.1/elements_sdk/model/stor_next_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stor_next_connections.py` & `elements-sdk-3.6.1/elements_sdk/model/stor_next_connections.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stor_next_license_check_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/stor_next_license_check_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stor_next_license_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/stor_next_license_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_node.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_node_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_node_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_node_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_node_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_node_status.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_node_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_node_update.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_node_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_request.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_response.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/storage_root.py` & `elements-sdk-3.6.1/elements_sdk/model/storage_root.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stornext_license.py` & `elements-sdk-3.6.1/elements_sdk/model/stornext_license.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/stornext_manager_attributes.py` & `elements-sdk-3.6.1/elements_sdk/model/stornext_manager_attributes.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subclip.py` & `elements-sdk-3.6.1/elements_sdk/model/subclip.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subclip_clipboard_entry.py` & `elements-sdk-3.6.1/elements_sdk/model/subclip_clipboard_entry.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subclip_clipboard_entry_update.py` & `elements-sdk-3.6.1/elements_sdk/model/subclip_clipboard_entry_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subclip_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/subclip_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subclip_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/subclip_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subclip_update.py` & `elements-sdk-3.6.1/elements_sdk/model/subclip_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subscription.py` & `elements-sdk-3.6.1/elements_sdk/model/subscription.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtask.py` & `elements-sdk-3.6.1/elements_sdk/model/subtask.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtask_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/subtask_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtask_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/subtask_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtask_update.py` & `elements-sdk-3.6.1/elements_sdk/model/subtask_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtitle.py` & `elements-sdk-3.6.1/elements_sdk/model/subtitle.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtitle_clipboard_entry.py` & `elements-sdk-3.6.1/elements_sdk/model/subtitle_clipboard_entry.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtitle_clipboard_entry_update.py` & `elements-sdk-3.6.1/elements_sdk/model/subtitle_clipboard_entry_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/subtitle_event.py` & `elements-sdk-3.6.1/elements_sdk/model/subtitle_event.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/sync_totp.py` & `elements-sdk-3.6.1/elements_sdk/model/sync_totp.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/sync_totp_request.py` & `elements-sdk-3.6.1/elements_sdk/model/sync_totp_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/system_info_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/system_info_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tag_media_directory_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tag_media_directory_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tag_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/tag_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape.py` & `elements-sdk-3.6.1/elements_sdk/model/tape.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_file.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_group.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_group_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_group_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_group_update.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_group_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_job.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_job.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_job_source.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_job_source.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_format_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_format_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_fsck_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_fsck_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_load_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_load_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_move_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_move_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_reindex_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_reindex_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_slot.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_slot.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_library_unload_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_library_unload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tape_update.py` & `elements-sdk-3.6.1/elements_sdk/model/tape_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/task_info.py` & `elements-sdk-3.6.1/elements_sdk/model/task_info.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/task_log.py` & `elements-sdk-3.6.1/elements_sdk/model/task_log.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/task_progress.py` & `elements-sdk-3.6.1/elements_sdk/model/task_progress.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/task_type.py` & `elements-sdk-3.6.1/elements_sdk/model/task_type.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/tasks_summary.py` & `elements-sdk-3.6.1/elements_sdk/model/tasks_summary.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/teams_connection.py` & `elements-sdk-3.6.1/elements_sdk/model/teams_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/teams_connection_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/teams_connection_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/teams_connection_status.py` & `elements-sdk-3.6.1/elements_sdk/model/teams_connection_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/teams_connection_update.py` & `elements-sdk-3.6.1/elements_sdk/model/teams_connection_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/teams_message.py` & `elements-sdk-3.6.1/elements_sdk/model/teams_message.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/teams_recipient.py` & `elements-sdk-3.6.1/elements_sdk/model/teams_recipient.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_aws_credentials_request.py` & `elements-sdk-3.6.1/elements_sdk/model/test_aws_credentials_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_aws_credentials_response.py` & `elements-sdk-3.6.1/elements_sdk/model/test_aws_credentials_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_cloud_account_credentials_request.py` & `elements-sdk-3.6.1/elements_sdk/model/test_cloud_account_credentials_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_cloud_account_credentials_response.py` & `elements-sdk-3.6.1/elements_sdk/model/test_cloud_account_credentials_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_external_transcoder_connection_request.py` & `elements-sdk-3.6.1/elements_sdk/model/test_external_transcoder_connection_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_external_transcoder_connection_response.py` & `elements-sdk-3.6.1/elements_sdk/model/test_external_transcoder_connection_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/test_smtp.py` & `elements-sdk-3.6.1/elements_sdk/model/test_smtp.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/ticket.py` & `elements-sdk-3.6.1/elements_sdk/model/ticket.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/time_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/time_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/time_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/time_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/time_sync_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/time_sync_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/time_sync_endpoint_response.py` & `elements-sdk-3.6.1/elements_sdk/model/time_sync_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/timeline_export_request.py` & `elements-sdk-3.6.1/elements_sdk/model/timeline_export_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/timezone.py` & `elements-sdk-3.6.1/elements_sdk/model/timezone.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/trace_node.py` & `elements-sdk-3.6.1/elements_sdk/model/trace_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/transcoder_profile.py` & `elements-sdk-3.6.1/elements_sdk/model/transcoder_profile.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/type_documentation.py` & `elements-sdk-3.6.1/elements_sdk/model/type_documentation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/unfiltered_tag.py` & `elements-sdk-3.6.1/elements_sdk/model/unfiltered_tag.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/unfiltered_tag_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/unfiltered_tag_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/unfiltered_tag_update.py` & `elements-sdk-3.6.1/elements_sdk/model/unfiltered_tag_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/update_quota_request.py` & `elements-sdk-3.6.1/elements_sdk/model/update_quota_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/updated_file.py` & `elements-sdk-3.6.1/elements_sdk/model/updated_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/upload_ai_image_request.py` & `elements-sdk-3.6.1/elements_sdk/model/upload_ai_image_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/upload_chunk_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/upload_chunk_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/upload_image_endpoint_request.py` & `elements-sdk-3.6.1/elements_sdk/model/upload_image_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/user_preview_request.py` & `elements-sdk-3.6.1/elements_sdk/model/user_preview_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/user_preview_response.py` & `elements-sdk-3.6.1/elements_sdk/model/user_preview_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/vantage_workflow.py` & `elements-sdk-3.6.1/elements_sdk/model/vantage_workflow.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/vantage_workflows.py` & `elements-sdk-3.6.1/elements_sdk/model/vantage_workflows.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/veritone_connection.py` & `elements-sdk-3.6.1/elements_sdk/model/veritone_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/veritone_engine_list.py` & `elements-sdk-3.6.1/elements_sdk/model/veritone_engine_list.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/veritone_job_list.py` & `elements-sdk-3.6.1/elements_sdk/model/veritone_job_list.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/veritone_metadata.py` & `elements-sdk-3.6.1/elements_sdk/model/veritone_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/veritone_upload_request.py` & `elements-sdk-3.6.1/elements_sdk/model/veritone_upload_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume.py` & `elements-sdk-3.6.1/elements_sdk/model/volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,18 +87,14 @@
         },
         ('visual_tag',): {
             'max_length': 255,
         },
         ('snfs_name',): {
             'max_length': 255,
         },
-        ('name',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -132,15 +128,14 @@
             'type': (str,),  # noqa: E501
             'snm_enabled': (bool,),  # noqa: E501
             'snfs_name': (str, none_type,),  # noqa: E501
             'simulated_quotas': (bool,),  # noqa: E501
             'fs_properties': (FSProperties,),  # noqa: E501
             'status': (VolumeStatus,),  # noqa: E501
             'cloud_account': (int, none_type,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -157,19 +152,17 @@
         'type': 'type',  # noqa: E501
         'snm_enabled': 'snm_enabled',  # noqa: E501
         'snfs_name': 'snfs_name',  # noqa: E501
         'simulated_quotas': 'simulated_quotas',  # noqa: E501
         'fs_properties': 'fs_properties',  # noqa: E501
         'status': 'status',  # noqa: E501
         'cloud_account': 'cloud_account',  # noqa: E501
-        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
-        'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, nodes, backend, *args, **xkwargs):  # noqa: E501
@@ -220,15 +213,14 @@
             type (str): [optional]  # noqa: E501
             snm_enabled (bool): [optional]  # noqa: E501
             snfs_name (str, none_type): [optional]  # noqa: E501
             simulated_quotas (bool): [optional]  # noqa: E501
             fs_properties (FSProperties): [optional]  # noqa: E501
             status (VolumeStatus): [optional]  # noqa: E501
             cloud_account (int, none_type): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
@@ -325,15 +317,14 @@
             type (str): [optional]  # noqa: E501
             snm_enabled (bool): [optional]  # noqa: E501
             snfs_name (str, none_type): [optional]  # noqa: E501
             simulated_quotas (bool): [optional]  # noqa: E501
             fs_properties (FSProperties): [optional]  # noqa: E501
             status (VolumeStatus): [optional]  # noqa: E501
             cloud_account (int, none_type): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_bee_gfs_status.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_bee_gfs_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_lizard_fs_status.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_lizard_fs_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_mini_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from elements_sdk.exceptions import ApiAttributeError
 
 
 
-class VolumeMini(ModelNormal):
+class VolumeMiniReference(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,18 +76,14 @@
         ('display_name',): {
             'max_length': 255,
             'min_length': 1,
         },
         ('visual_tag',): {
             'max_length': 255,
         },
-        ('name',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -108,41 +104,42 @@
         """
         return {
             'id': (int,),  # noqa: E501
             'path': (str,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'visual_tag': (str, none_type,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'path': 'path',  # noqa: E501
         'display_name': 'display_name',  # noqa: E501
         'visual_tag': 'visual_tag',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
-        'name',  # noqa: E501
+        'path',  # noqa: E501
+        'display_name',  # noqa: E501
+        'visual_tag',  # noqa: E501
+        'type',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, *args, **xkwargs):  # noqa: E501
-        """VolumeMini - a model defined in OpenAPI
+        """VolumeMiniReference - a model defined in OpenAPI
 
         Args:
             id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -174,15 +171,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             path (str): [optional]  # noqa: E501
             display_name (str): [optional]  # noqa: E501
             visual_tag (str, none_type): [optional]  # noqa: E501
             type (str): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
@@ -226,15 +222,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, *args, **xkwargs):  # noqa: E501
-        """VolumeMini - a model defined in OpenAPI
+        """VolumeMiniReference - a model defined in OpenAPI
 
         Args:
             id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -266,15 +262,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             path (str): [optional]  # noqa: E501
             display_name (str): [optional]  # noqa: E501
             visual_tag (str, none_type): [optional]  # noqa: E501
             type (str): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_mini_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_mini.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from elements_sdk.exceptions import ApiAttributeError
 
 
 
-class VolumeMiniReference(ModelNormal):
+class VolumeMini(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -76,18 +76,14 @@
         ('display_name',): {
             'max_length': 255,
             'min_length': 1,
         },
         ('visual_tag',): {
             'max_length': 255,
         },
-        ('name',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -108,45 +104,38 @@
         """
         return {
             'id': (int,),  # noqa: E501
             'path': (str,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'visual_tag': (str, none_type,),  # noqa: E501
             'type': (str,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'path': 'path',  # noqa: E501
         'display_name': 'display_name',  # noqa: E501
         'visual_tag': 'visual_tag',  # noqa: E501
         'type': 'type',  # noqa: E501
-        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
-        'path',  # noqa: E501
-        'display_name',  # noqa: E501
-        'visual_tag',  # noqa: E501
-        'type',  # noqa: E501
-        'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, *args, **xkwargs):  # noqa: E501
-        """VolumeMiniReference - a model defined in OpenAPI
+        """VolumeMini - a model defined in OpenAPI
 
         Args:
             id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -178,15 +167,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             path (str): [optional]  # noqa: E501
             display_name (str): [optional]  # noqa: E501
             visual_tag (str, none_type): [optional]  # noqa: E501
             type (str): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
@@ -230,15 +218,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, id, *args, **xkwargs):  # noqa: E501
-        """VolumeMiniReference - a model defined in OpenAPI
+        """VolumeMini - a model defined in OpenAPI
 
         Args:
             id (int):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -270,15 +258,14 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             path (str): [optional]  # noqa: E501
             display_name (str): [optional]  # noqa: E501
             visual_tag (str, none_type): [optional]  # noqa: E501
             type (str): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_reference.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,18 +87,14 @@
         },
         ('visual_tag',): {
             'max_length': 255,
         },
         ('snfs_name',): {
             'max_length': 255,
         },
-        ('name',): {
-            'max_length': 1,
-            'min_length': 1,
-        },
     }
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
@@ -132,15 +128,14 @@
             'snm_enabled': (bool,),  # noqa: E501
             'snfs_name': (str, none_type,),  # noqa: E501
             'simulated_quotas': (bool,),  # noqa: E501
             'fs_properties': (FSProperties,),  # noqa: E501
             'backend': (Backend,),  # noqa: E501
             'status': (VolumeStatus,),  # noqa: E501
             'cloud_account': (int, none_type,),  # noqa: E501
-            'name': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -157,15 +152,14 @@
         'snm_enabled': 'snm_enabled',  # noqa: E501
         'snfs_name': 'snfs_name',  # noqa: E501
         'simulated_quotas': 'simulated_quotas',  # noqa: E501
         'fs_properties': 'fs_properties',  # noqa: E501
         'backend': 'backend',  # noqa: E501
         'status': 'status',  # noqa: E501
         'cloud_account': 'cloud_account',  # noqa: E501
-        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
         'path',  # noqa: E501
         'nodes',  # noqa: E501
         'display_name',  # noqa: E501
         'visual_tag',  # noqa: E501
@@ -173,15 +167,14 @@
         'use_for_homes',  # noqa: E501
         'use_for_workspaces',  # noqa: E501
         'type',  # noqa: E501
         'snm_enabled',  # noqa: E501
         'snfs_name',  # noqa: E501
         'simulated_quotas',  # noqa: E501
         'cloud_account',  # noqa: E501
-        'name',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, id, *args, **xkwargs):  # noqa: E501
@@ -232,15 +225,14 @@
             snm_enabled (bool): [optional]  # noqa: E501
             snfs_name (str, none_type): [optional]  # noqa: E501
             simulated_quotas (bool): [optional]  # noqa: E501
             fs_properties (FSProperties): [optional]  # noqa: E501
             backend (Backend): [optional]  # noqa: E501
             status (VolumeStatus): [optional]  # noqa: E501
             cloud_account (int, none_type): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
@@ -335,15 +327,14 @@
             snm_enabled (bool): [optional]  # noqa: E501
             snfs_name (str, none_type): [optional]  # noqa: E501
             simulated_quotas (bool): [optional]  # noqa: E501
             fs_properties (FSProperties): [optional]  # noqa: E501
             backend (Backend): [optional]  # noqa: E501
             status (VolumeStatus): [optional]  # noqa: E501
             cloud_account (int, none_type): [optional]  # noqa: E501
-            name (str, none_type): [optional]  # noqa: E501
         """
 
         _check_type = xkwargs.pop('_check_type', True)
         _spec_property_naming = xkwargs.pop('_spec_property_naming', False)
         _path_to_item = xkwargs.pop('_path_to_item', ())
         _configuration = xkwargs.pop('_configuration', None)
         _visited_composed_classes = xkwargs.pop('_visited_composed_classes', ())
```

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_snfs_status.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_snfs_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_stat.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_stats.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_stats.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_status.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/volume_update.py` & `elements-sdk-3.6.1/elements_sdk/model/volume_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workflow_transition_request.py` & `elements-sdk-3.6.1/elements_sdk/model/workflow_transition_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workflow_transition_response.py` & `elements-sdk-3.6.1/elements_sdk/model/workflow_transition_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_check_in.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_check_in.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_detail.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_detail_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_detail_update.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_endpoint.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_endpoint.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_move_to_request.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_move_to_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_permission.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_permission_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_permission_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_permission_update.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_permission_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workspace_resolved_permission.py` & `elements-sdk-3.6.1/elements_sdk/model/workspace_resolved_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workstation.py` & `elements-sdk-3.6.1/elements_sdk/model/workstation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workstation_mini.py` & `elements-sdk-3.6.1/elements_sdk/model/workstation_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workstation_partial_update.py` & `elements-sdk-3.6.1/elements_sdk/model/workstation_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model/workstation_update.py` & `elements-sdk-3.6.1/elements_sdk/model/workstation_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/model_utils.py` & `elements-sdk-3.6.1/elements_sdk/model_utils.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/models/__init__.py` & `elements-sdk-3.6.1/elements_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk/rest.py` & `elements-sdk-3.6.1/elements_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/elements_sdk.egg-info/SOURCES.txt` & `elements-sdk-3.6.1/elements_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/setup.py` & `elements-sdk-3.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "elements-sdk"
-VERSION = "3.6.0"
+VERSION = "3.6.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `elements-sdk-3.6.0/test/test_add_assets_to_click_gallery.py` & `elements-sdk-3.6.1/test/test_add_assets_to_click_gallery.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_address.py` & `elements-sdk-3.6.1/test/test_address.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_annotation.py` & `elements-sdk-3.6.1/test/test_ai_annotation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_annotation_create_request.py` & `elements-sdk-3.6.1/test/test_ai_annotation_create_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_annotation_partial_update.py` & `elements-sdk-3.6.1/test/test_ai_annotation_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_annotation_update.py` & `elements-sdk-3.6.1/test/test_ai_annotation_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_category.py` & `elements-sdk-3.6.1/test/test_ai_category.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_category_detail.py` & `elements-sdk-3.6.1/test/test_ai_category_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_category_detail_partial_update.py` & `elements-sdk-3.6.1/test/test_ai_category_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_category_detail_update.py` & `elements-sdk-3.6.1/test/test_ai_category_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_category_mini_reference.py` & `elements-sdk-3.6.1/test/test_ai_category_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_connection.py` & `elements-sdk-3.6.1/test/test_ai_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset.py` & `elements-sdk-3.6.1/test/test_ai_dataset.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_detail_reference.py` & `elements-sdk-3.6.1/test/test_ai_dataset_detail_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_export_request.py` & `elements-sdk-3.6.1/test/test_ai_dataset_export_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_export_response.py` & `elements-sdk-3.6.1/test/test_ai_dataset_export_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_reference.py` & `elements-sdk-3.6.1/test/test_ai_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_with_preview.py` & `elements-sdk-3.6.1/test/test_ai_dataset_with_preview.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_with_preview_partial_update.py` & `elements-sdk-3.6.1/test/test_ai_dataset_with_preview_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_dataset_with_preview_update.py` & `elements-sdk-3.6.1/test/test_ai_dataset_with_preview_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_image.py` & `elements-sdk-3.6.1/test/test_ai_image.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_image_reference.py` & `elements-sdk-3.6.1/test/test_ai_image_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_metadata.py` & `elements-sdk-3.6.1/test/test_ai_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model.py` & `elements-sdk-3.6.1/test/test_ai_model.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_export_request.py` & `elements-sdk-3.6.1/test/test_ai_model_export_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_export_response.py` & `elements-sdk-3.6.1/test/test_ai_model_export_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_inference_request.py` & `elements-sdk-3.6.1/test/test_ai_model_inference_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_inference_response.py` & `elements-sdk-3.6.1/test/test_ai_model_inference_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_partial_update.py` & `elements-sdk-3.6.1/test/test_ai_model_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_progress.py` & `elements-sdk-3.6.1/test/test_ai_model_progress.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_training_request.py` & `elements-sdk-3.6.1/test/test_ai_model_training_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_model_update.py` & `elements-sdk-3.6.1/test/test_ai_model_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ai_processing_request.py` & `elements-sdk-3.6.1/test/test_ai_processing_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_alert.py` & `elements-sdk-3.6.1/test/test_alert.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_alert_partial_update.py` & `elements-sdk-3.6.1/test/test_alert_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_alert_update.py` & `elements-sdk-3.6.1/test/test_alert_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_all_media_files_for_bundles_request.py` & `elements-sdk-3.6.1/test/test_all_media_files_for_bundles_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_api_token.py` & `elements-sdk-3.6.1/test/test_api_token.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_api_token_partial_update.py` & `elements-sdk-3.6.1/test/test_api_token_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_api_token_update.py` & `elements-sdk-3.6.1/test/test_api_token_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_api_token_with_secret.py` & `elements-sdk-3.6.1/test/test_api_token_with_secret.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_api_token_with_secret_update.py` & `elements-sdk-3.6.1/test/test_api_token_with_secret_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_archive_endpoint_request.py` & `elements-sdk-3.6.1/test/test_archive_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_argument_type.py` & `elements-sdk-3.6.1/test/test_argument_type.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset.py` & `elements-sdk-3.6.1/test/test_asset.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_backup.py` & `elements-sdk-3.6.1/test/test_asset_backup.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_cloud_link.py` & `elements-sdk-3.6.1/test/test_asset_cloud_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_mini.py` & `elements-sdk-3.6.1/test/test_asset_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_mini_reference.py` & `elements-sdk-3.6.1/test/test_asset_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_partial_update.py` & `elements-sdk-3.6.1/test/test_asset_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_project_link.py` & `elements-sdk-3.6.1/test/test_asset_project_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_rating.py` & `elements-sdk-3.6.1/test/test_asset_rating.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_rating_partial_update.py` & `elements-sdk-3.6.1/test/test_asset_rating_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_rating_update.py` & `elements-sdk-3.6.1/test/test_asset_rating_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_subtitle_link.py` & `elements-sdk-3.6.1/test/test_asset_subtitle_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_subtitle_link_partial_update.py` & `elements-sdk-3.6.1/test/test_asset_subtitle_link_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_subtitle_link_update.py` & `elements-sdk-3.6.1/test/test_asset_subtitle_link_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_asset_update.py` & `elements-sdk-3.6.1/test/test_asset_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_auth_login_endpoint_request.py` & `elements-sdk-3.6.1/test/test_auth_login_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_auth_login_endpoint_response.py` & `elements-sdk-3.6.1/test/test_auth_login_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_aws_account.py` & `elements-sdk-3.6.1/test/test_aws_account.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_aws_account_partial_update.py` & `elements-sdk-3.6.1/test/test_aws_account_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_backend.py` & `elements-sdk-3.6.1/test/test_backend.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_backend_properties.py` & `elements-sdk-3.6.1/test/test_backend_properties.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_basic_file.py` & `elements-sdk-3.6.1/test/test_basic_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_bee_gfs_node.py` & `elements-sdk-3.6.1/test/test_bee_gfs_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_bee_gfs_target.py` & `elements-sdk-3.6.1/test/test_bee_gfs_target.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_bootstrap_data.py` & `elements-sdk-3.6.1/test/test_bootstrap_data.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_certificate.py` & `elements-sdk-3.6.1/test/test_certificate.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_certificate_update.py` & `elements-sdk-3.6.1/test/test_certificate_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_change_own_password_request.py` & `elements-sdk-3.6.1/test/test_change_own_password_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_change_password_request.py` & `elements-sdk-3.6.1/test/test_change_password_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_check_connectivity_endpoint_response.py` & `elements-sdk-3.6.1/test/test_check_connectivity_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_click_background_upload_endpoint_request.py` & `elements-sdk-3.6.1/test/test_click_background_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_click_gallery.py` & `elements-sdk-3.6.1/test/test_click_gallery.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_click_gallery_link.py` & `elements-sdk-3.6.1/test/test_click_gallery_link.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_click_gallery_update.py` & `elements-sdk-3.6.1/test/test_click_gallery_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_click_link_user.py` & `elements-sdk-3.6.1/test/test_click_link_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_click_start_upload_endpoint_request.py` & `elements-sdk-3.6.1/test/test_click_start_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_client_session.py` & `elements-sdk-3.6.1/test/test_client_session.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_client_side_path_endpoint_request.py` & `elements-sdk-3.6.1/test/test_client_side_path_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_client_side_path_endpoint_response.py` & `elements-sdk-3.6.1/test/test_client_side_path_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_clients_endpoint_response.py` & `elements-sdk-3.6.1/test/test_clients_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_account.py` & `elements-sdk-3.6.1/test/test_cloud_account.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_account_mini.py` & `elements-sdk-3.6.1/test/test_cloud_account_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_account_mini_partial_update.py` & `elements-sdk-3.6.1/test/test_cloud_account_mini_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_account_mini_update.py` & `elements-sdk-3.6.1/test/test_cloud_account_mini_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_account_partial_update.py` & `elements-sdk-3.6.1/test/test_cloud_account_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_account_update.py` & `elements-sdk-3.6.1/test/test_cloud_account_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_bucket_costs.py` & `elements-sdk-3.6.1/test/test_cloud_bucket_costs.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_connection.py` & `elements-sdk-3.6.1/test/test_cloud_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_mount_authorization.py` & `elements-sdk-3.6.1/test/test_cloud_mount_authorization.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cloud_storage_costs.py` & `elements-sdk-3.6.1/test/test_cloud_storage_costs.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_comment.py` & `elements-sdk-3.6.1/test/test_comment.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_comment_partial_update.py` & `elements-sdk-3.6.1/test/test_comment_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_comment_update.py` & `elements-sdk-3.6.1/test/test_comment_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cost.py` & `elements-sdk-3.6.1/test/test_cost.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_cpu_stat.py` & `elements-sdk-3.6.1/test/test_cpu_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_create_download_archive.py` & `elements-sdk-3.6.1/test/test_create_download_archive.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_create_home_workspace_request.py` & `elements-sdk-3.6.1/test/test_create_home_workspace_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_create_path_quota_request.py` & `elements-sdk-3.6.1/test/test_create_path_quota_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_create_template_folder_endpoint_request.py` & `elements-sdk-3.6.1/test/test_create_template_folder_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_custom_field.py` & `elements-sdk-3.6.1/test/test_custom_field.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_custom_field_partial_update.py` & `elements-sdk-3.6.1/test/test_custom_field_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_custom_field_reference.py` & `elements-sdk-3.6.1/test/test_custom_field_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_custom_field_update.py` & `elements-sdk-3.6.1/test/test_custom_field_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_deleted_workspace.py` & `elements-sdk-3.6.1/test/test_deleted_workspace.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_download.py` & `elements-sdk-3.6.1/test/test_download.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_download_archive.py` & `elements-sdk-3.6.1/test/test_download_archive.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_download_archive_partial_update.py` & `elements-sdk-3.6.1/test/test_download_archive_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_download_archive_update.py` & `elements-sdk-3.6.1/test/test_download_archive_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_editor_project.py` & `elements-sdk-3.6.1/test/test_editor_project.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_editor_project_partial_update.py` & `elements-sdk-3.6.1/test/test_editor_project_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_editor_project_update.py` & `elements-sdk-3.6.1/test/test_editor_project_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_editor_subtitle.py` & `elements-sdk-3.6.1/test/test_editor_subtitle.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_editor_subtitle_partial_update.py` & `elements-sdk-3.6.1/test/test_editor_subtitle_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_editor_subtitle_update.py` & `elements-sdk-3.6.1/test/test_editor_subtitle_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_group.py` & `elements-sdk-3.6.1/test/test_elements_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_group_detail.py` & `elements-sdk-3.6.1/test/test_elements_group_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_group_detail_partial_update.py` & `elements-sdk-3.6.1/test/test_elements_group_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_group_detail_update.py` & `elements-sdk-3.6.1/test/test_elements_group_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_group_reference.py` & `elements-sdk-3.6.1/test/test_elements_group_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user.py` & `elements-sdk-3.6.1/test/test_elements_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_detail.py` & `elements-sdk-3.6.1/test/test_elements_user_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_detail_partial_update.py` & `elements-sdk-3.6.1/test/test_elements_user_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_detail_update.py` & `elements-sdk-3.6.1/test/test_elements_user_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_mini.py` & `elements-sdk-3.6.1/test/test_elements_user_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_mini_reference.py` & `elements-sdk-3.6.1/test/test_elements_user_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_profile.py` & `elements-sdk-3.6.1/test/test_elements_user_profile.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_profile_partial_update.py` & `elements-sdk-3.6.1/test/test_elements_user_profile_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_profile_update.py` & `elements-sdk-3.6.1/test/test_elements_user_profile_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_user_reference.py` & `elements-sdk-3.6.1/test/test_elements_user_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_elements_version.py` & `elements-sdk-3.6.1/test/test_elements_version.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_email_preview.py` & `elements-sdk-3.6.1/test/test_email_preview.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_enable_totp_request.py` & `elements-sdk-3.6.1/test/test_enable_totp_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_event.py` & `elements-sdk-3.6.1/test/test_event.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_external_transcoder.py` & `elements-sdk-3.6.1/test/test_external_transcoder.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_external_transcoder_partial_update.py` & `elements-sdk-3.6.1/test/test_external_transcoder_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_external_transcoder_update.py` & `elements-sdk-3.6.1/test/test_external_transcoder_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_extract_request.py` & `elements-sdk-3.6.1/test/test_extract_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_copy_endpoint_request.py` & `elements-sdk-3.6.1/test/test_file_copy_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_delete_endpoint_request.py` & `elements-sdk-3.6.1/test/test_file_delete_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_move_endpoint_request.py` & `elements-sdk-3.6.1/test/test_file_move_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_partial_update.py` & `elements-sdk-3.6.1/test/test_file_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_size_distribution.py` & `elements-sdk-3.6.1/test/test_file_size_distribution.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_size_distribution_item.py` & `elements-sdk-3.6.1/test/test_file_size_distribution_item.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_size_endpoint_response.py` & `elements-sdk-3.6.1/test/test_file_size_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_unzip_endpoint_request.py` & `elements-sdk-3.6.1/test/test_file_unzip_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_update.py` & `elements-sdk-3.6.1/test/test_file_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_file_zip_endpoint_request.py` & `elements-sdk-3.6.1/test/test_file_zip_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_filesystem_file.py` & `elements-sdk-3.6.1/test/test_filesystem_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_filesystem_permission.py` & `elements-sdk-3.6.1/test/test_filesystem_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_filesystem_permission_partial_update.py` & `elements-sdk-3.6.1/test/test_filesystem_permission_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_filesystem_permission_update.py` & `elements-sdk-3.6.1/test/test_filesystem_permission_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_filesystem_trace_endpoint_request.py` & `elements-sdk-3.6.1/test/test_filesystem_trace_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_filesystem_trace_endpoint_response.py` & `elements-sdk-3.6.1/test/test_filesystem_trace_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_finish_upload_endpoint_request.py` & `elements-sdk-3.6.1/test/test_finish_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_format_metadata.py` & `elements-sdk-3.6.1/test/test_format_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_fs_properties.py` & `elements-sdk-3.6.1/test/test_fs_properties.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_generate_password_endpoint_response.py` & `elements-sdk-3.6.1/test/test_generate_password_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_generate_proxies_request.py` & `elements-sdk-3.6.1/test/test_generate_proxies_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_get_cloud_account_costs_response.py` & `elements-sdk-3.6.1/test/test_get_cloud_account_costs_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_get_cloud_account_volume_sizes_response.py` & `elements-sdk-3.6.1/test/test_get_cloud_account_volume_sizes_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_get_multiple_bundles_request.py` & `elements-sdk-3.6.1/test/test_get_multiple_bundles_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_get_multiple_files_request.py` & `elements-sdk-3.6.1/test/test_get_multiple_files_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_global_alert.py` & `elements-sdk-3.6.1/test/test_global_alert.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_help_endpoint_response.py` & `elements-sdk-3.6.1/test/test_help_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_image_upload_request.py` & `elements-sdk-3.6.1/test/test_image_upload_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_impersonation_endpoint_request.py` & `elements-sdk-3.6.1/test/test_impersonation_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_import_ai_dataset_request.py` & `elements-sdk-3.6.1/test/test_import_ai_dataset_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_import_ai_dataset_response.py` & `elements-sdk-3.6.1/test/test_import_ai_dataset_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_import_ai_model_request.py` & `elements-sdk-3.6.1/test/test_import_ai_model_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_import_ai_model_response.py` & `elements-sdk-3.6.1/test/test_import_ai_model_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_import_job_request.py` & `elements-sdk-3.6.1/test/test_import_job_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_import_job_response.py` & `elements-sdk-3.6.1/test/test_import_job_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_inline_response200.py` & `elements-sdk-3.6.1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_inline_response2001.py` & `elements-sdk-3.6.1/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_inline_response2002.py` & `elements-sdk-3.6.1/test/test_inline_response2002.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_inline_response2003.py` & `elements-sdk-3.6.1/test/test_inline_response2003.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_inline_response2004.py` & `elements-sdk-3.6.1/test/test_inline_response2004.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_install_license_endpoint_request.py` & `elements-sdk-3.6.1/test/test_install_license_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_instantiate_file_template_request.py` & `elements-sdk-3.6.1/test/test_instantiate_file_template_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_interface.py` & `elements-sdk-3.6.1/test/test_interface.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_io_stat.py` & `elements-sdk-3.6.1/test/test_io_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ipmi.py` & `elements-sdk-3.6.1/test/test_ipmi.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_job.py` & `elements-sdk-3.6.1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_job_partial_update.py` & `elements-sdk-3.6.1/test/test_job_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_job_reference.py` & `elements-sdk-3.6.1/test/test_job_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_job_update.py` & `elements-sdk-3.6.1/test/test_job_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_kapacitor_alert.py` & `elements-sdk-3.6.1/test/test_kapacitor_alert.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ldap_server.py` & `elements-sdk-3.6.1/test/test_ldap_server.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ldap_server_group.py` & `elements-sdk-3.6.1/test/test_ldap_server_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ldap_server_groups.py` & `elements-sdk-3.6.1/test/test_ldap_server_groups.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ldap_server_reference.py` & `elements-sdk-3.6.1/test/test_ldap_server_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ldap_server_user.py` & `elements-sdk-3.6.1/test/test_ldap_server_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ldap_server_users.py` & `elements-sdk-3.6.1/test/test_ldap_server_users.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_license.py` & `elements-sdk-3.6.1/test/test_license.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_list_buckets.py` & `elements-sdk-3.6.1/test/test_list_buckets.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_list_topics.py` & `elements-sdk-3.6.1/test/test_list_topics.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_lizard_fs_disk.py` & `elements-sdk-3.6.1/test/test_lizard_fs_disk.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_lizard_fs_node.py` & `elements-sdk-3.6.1/test/test_lizard_fs_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_locale_endpoint_response.py` & `elements-sdk-3.6.1/test/test_locale_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_locate_endpoint_request.py` & `elements-sdk-3.6.1/test/test_locate_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_locate_proxies_endpoint_request.py` & `elements-sdk-3.6.1/test/test_locate_proxies_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_locate_proxies_endpoint_response.py` & `elements-sdk-3.6.1/test/test_locate_proxies_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_locate_result.py` & `elements-sdk-3.6.1/test/test_locate_result.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_marker.py` & `elements-sdk-3.6.1/test/test_marker.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_marker_partial_update.py` & `elements-sdk-3.6.1/test/test_marker_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_marker_update.py` & `elements-sdk-3.6.1/test/test_marker_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file.py` & `elements-sdk-3.6.1/test/test_media_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_bundle.py` & `elements-sdk-3.6.1/test/test_media_file_bundle.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_bundle_mini.py` & `elements-sdk-3.6.1/test/test_media_file_bundle_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_bundle_mini_reference.py` & `elements-sdk-3.6.1/test/test_media_file_bundle_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_contents.py` & `elements-sdk-3.6.1/test/test_media_file_contents.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_mini.py` & `elements-sdk-3.6.1/test/test_media_file_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_partial_update.py` & `elements-sdk-3.6.1/test/test_media_file_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_reference.py` & `elements-sdk-3.6.1/test/test_media_file_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_template.py` & `elements-sdk-3.6.1/test/test_media_file_template.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_template_partial_update.py` & `elements-sdk-3.6.1/test/test_media_file_template_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_template_update.py` & `elements-sdk-3.6.1/test/test_media_file_template_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_file_update.py` & `elements-sdk-3.6.1/test/test_media_file_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_files_lookup_request.py` & `elements-sdk-3.6.1/test/test_media_files_lookup_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_library_delete_request.py` & `elements-sdk-3.6.1/test/test_media_library_delete_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_library_share_request.py` & `elements-sdk-3.6.1/test/test_media_library_share_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root.py` & `elements-sdk-3.6.1/test/test_media_root.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_detail.py` & `elements-sdk-3.6.1/test/test_media_root_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_detail_partial_update.py` & `elements-sdk-3.6.1/test/test_media_root_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_detail_update.py` & `elements-sdk-3.6.1/test/test_media_root_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_mini.py` & `elements-sdk-3.6.1/test/test_media_root_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_mini_reference.py` & `elements-sdk-3.6.1/test/test_media_root_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_partial_update.py` & `elements-sdk-3.6.1/test/test_media_root_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_permission.py` & `elements-sdk-3.6.1/test/test_media_root_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_permission_access_options.py` & `elements-sdk-3.6.1/test/test_media_root_permission_access_options.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_permission_partial_update.py` & `elements-sdk-3.6.1/test/test_media_root_permission_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_permission_update.py` & `elements-sdk-3.6.1/test/test_media_root_permission_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_root_update.py` & `elements-sdk-3.6.1/test/test_media_root_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_media_update.py` & `elements-sdk-3.6.1/test/test_media_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_member_preview.py` & `elements-sdk-3.6.1/test/test_member_preview.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_metadata_item.py` & `elements-sdk-3.6.1/test/test_metadata_item.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_move_workspace_request.py` & `elements-sdk-3.6.1/test/test_move_workspace_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_multiple_assets_request.py` & `elements-sdk-3.6.1/test/test_multiple_assets_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_net_stat.py` & `elements-sdk-3.6.1/test/test_net_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_nfs_permission.py` & `elements-sdk-3.6.1/test/test_nfs_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ntp_server.py` & `elements-sdk-3.6.1/test/test_ntp_server.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ntp_server_partial_update.py` & `elements-sdk-3.6.1/test/test_ntp_server_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ntp_server_update.py` & `elements-sdk-3.6.1/test/test_ntp_server_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_one_time_access_token.py` & `elements-sdk-3.6.1/test/test_one_time_access_token.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_one_time_access_token_activity.py` & `elements-sdk-3.6.1/test/test_one_time_access_token_activity.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_one_time_access_token_shared_object.py` & `elements-sdk-3.6.1/test/test_one_time_access_token_shared_object.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_parameters.py` & `elements-sdk-3.6.1/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_parameters_update.py` & `elements-sdk-3.6.1/test/test_parameters_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_parse_samlidp_metadata_request.py` & `elements-sdk-3.6.1/test/test_parse_samlidp_metadata_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_parsed_samlidp_metadata.py` & `elements-sdk-3.6.1/test/test_parsed_samlidp_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_password_reset_endpoint_request.py` & `elements-sdk-3.6.1/test/test_password_reset_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_path.py` & `elements-sdk-3.6.1/test/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_path_input.py` & `elements-sdk-3.6.1/test/test_path_input.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_production.py` & `elements-sdk-3.6.1/test/test_production.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_production_mini_reference.py` & `elements-sdk-3.6.1/test/test_production_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_production_partial_update.py` & `elements-sdk-3.6.1/test/test_production_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_production_reference.py` & `elements-sdk-3.6.1/test/test_production_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_production_update.py` & `elements-sdk-3.6.1/test/test_production_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy.py` & `elements-sdk-3.6.1/test/test_proxy.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_count.py` & `elements-sdk-3.6.1/test/test_proxy_count.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_fs_size_endpoint_response.py` & `elements-sdk-3.6.1/test/test_proxy_fs_size_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_generator.py` & `elements-sdk-3.6.1/test/test_proxy_generator.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_generator_properties.py` & `elements-sdk-3.6.1/test/test_proxy_generator_properties.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_profile.py` & `elements-sdk-3.6.1/test/test_proxy_profile.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_profile_mini.py` & `elements-sdk-3.6.1/test/test_proxy_profile_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_profile_partial_update.py` & `elements-sdk-3.6.1/test/test_proxy_profile_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_proxy_profile_update.py` & `elements-sdk-3.6.1/test/test_proxy_profile_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_python_environment.py` & `elements-sdk-3.6.1/test/test_python_environment.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_queue.py` & `elements-sdk-3.6.1/test/test_queue.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_quota.py` & `elements-sdk-3.6.1/test/test_quota.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ram_stat.py` & `elements-sdk-3.6.1/test/test_ram_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_rdc_activation.py` & `elements-sdk-3.6.1/test/test_rdc_activation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_rdc_host.py` & `elements-sdk-3.6.1/test/test_rdc_host.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_rdc_session.py` & `elements-sdk-3.6.1/test/test_rdc_session.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_rdc_session_create.py` & `elements-sdk-3.6.1/test/test_rdc_session_create.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_register_upload_endpoint_request.py` & `elements-sdk-3.6.1/test/test_register_upload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_register_upload_metadata_endpoint_request.py` & `elements-sdk-3.6.1/test/test_register_upload_metadata_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_release_notes_endpoint_response.py` & `elements-sdk-3.6.1/test/test_release_notes_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_rename_custom_field_request.py` & `elements-sdk-3.6.1/test/test_rename_custom_field_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_render_endpoint_request.py` & `elements-sdk-3.6.1/test/test_render_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_render_request.py` & `elements-sdk-3.6.1/test/test_render_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_restore_endpoint_request.py` & `elements-sdk-3.6.1/test/test_restore_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saml_provider.py` & `elements-sdk-3.6.1/test/test_saml_provider.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saml_provider_mini.py` & `elements-sdk-3.6.1/test/test_saml_provider_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saml_provider_partial_update.py` & `elements-sdk-3.6.1/test/test_saml_provider_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saml_provider_update.py` & `elements-sdk-3.6.1/test/test_saml_provider_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saved_search.py` & `elements-sdk-3.6.1/test/test_saved_search.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saved_search_partial_update.py` & `elements-sdk-3.6.1/test/test_saved_search_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_saved_search_update.py` & `elements-sdk-3.6.1/test/test_saved_search_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_scanner_discover_endpoint_request.py` & `elements-sdk-3.6.1/test/test_scanner_discover_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_scanner_scan_endpoint_request.py` & `elements-sdk-3.6.1/test/test_scanner_scan_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_schedule.py` & `elements-sdk-3.6.1/test/test_schedule.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_schedule_partial_update.py` & `elements-sdk-3.6.1/test/test_schedule_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_schedule_reference.py` & `elements-sdk-3.6.1/test/test_schedule_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_schedule_update.py` & `elements-sdk-3.6.1/test/test_schedule_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_search_endpoint_request.py` & `elements-sdk-3.6.1/test/test_search_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_search_endpoint_response.py` & `elements-sdk-3.6.1/test/test_search_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_send_link_email_request.py` & `elements-sdk-3.6.1/test/test_send_link_email_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_sensor.py` & `elements-sdk-3.6.1/test/test_sensor.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_sensors.py` & `elements-sdk-3.6.1/test/test_sensors.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_service_status.py` & `elements-sdk-3.6.1/test/test_service_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_share.py` & `elements-sdk-3.6.1/test/test_share.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_share_partial_update.py` & `elements-sdk-3.6.1/test/test_share_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_share_to_home_workspace_endpoint_request.py` & `elements-sdk-3.6.1/test/test_share_to_home_workspace_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_share_update.py` & `elements-sdk-3.6.1/test/test_share_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_channel.py` & `elements-sdk-3.6.1/test/test_slack_channel.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_connection.py` & `elements-sdk-3.6.1/test/test_slack_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_connection_partial_update.py` & `elements-sdk-3.6.1/test/test_slack_connection_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_connection_status.py` & `elements-sdk-3.6.1/test/test_slack_connection_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_connection_update.py` & `elements-sdk-3.6.1/test/test_slack_connection_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_emoji.py` & `elements-sdk-3.6.1/test/test_slack_emoji.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_message.py` & `elements-sdk-3.6.1/test/test_slack_message.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_slack_user.py` & `elements-sdk-3.6.1/test/test_slack_user.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_smtp_configuration.py` & `elements-sdk-3.6.1/test/test_smtp_configuration.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_smtp_configuration_update.py` & `elements-sdk-3.6.1/test/test_smtp_configuration_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_snapshot.py` & `elements-sdk-3.6.1/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_snapshot_partial_update.py` & `elements-sdk-3.6.1/test/test_snapshot_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_snapshot_update.py` & `elements-sdk-3.6.1/test/test_snapshot_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_snfs_stripe_group.py` & `elements-sdk-3.6.1/test/test_snfs_stripe_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_solr_reindex_endpoint_response.py` & `elements-sdk-3.6.1/test/test_solr_reindex_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_start_job_request.py` & `elements-sdk-3.6.1/test/test_start_job_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_start_task_request.py` & `elements-sdk-3.6.1/test/test_start_task_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stats.py` & `elements-sdk-3.6.1/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stor_next_connection.py` & `elements-sdk-3.6.1/test/test_stor_next_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stor_next_connections.py` & `elements-sdk-3.6.1/test/test_stor_next_connections.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stor_next_license_check_endpoint_response.py` & `elements-sdk-3.6.1/test/test_stor_next_license_check_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stor_next_license_endpoint_response.py` & `elements-sdk-3.6.1/test/test_stor_next_license_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_node.py` & `elements-sdk-3.6.1/test/test_storage_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_node_mini.py` & `elements-sdk-3.6.1/test/test_storage_node_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_node_partial_update.py` & `elements-sdk-3.6.1/test/test_storage_node_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_node_status.py` & `elements-sdk-3.6.1/test/test_storage_node_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_node_update.py` & `elements-sdk-3.6.1/test/test_storage_node_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_request.py` & `elements-sdk-3.6.1/test/test_storage_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_response.py` & `elements-sdk-3.6.1/test/test_storage_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_storage_root.py` & `elements-sdk-3.6.1/test/test_storage_root.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stornext_license.py` & `elements-sdk-3.6.1/test/test_stornext_license.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_stornext_manager_attributes.py` & `elements-sdk-3.6.1/test/test_stornext_manager_attributes.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subclip.py` & `elements-sdk-3.6.1/test/test_subclip.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subclip_clipboard_entry.py` & `elements-sdk-3.6.1/test/test_subclip_clipboard_entry.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subclip_clipboard_entry_update.py` & `elements-sdk-3.6.1/test/test_subclip_clipboard_entry_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subclip_partial_update.py` & `elements-sdk-3.6.1/test/test_subclip_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subclip_reference.py` & `elements-sdk-3.6.1/test/test_subclip_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subclip_update.py` & `elements-sdk-3.6.1/test/test_subclip_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subscription.py` & `elements-sdk-3.6.1/test/test_subscription.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtask.py` & `elements-sdk-3.6.1/test/test_subtask.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtask_partial_update.py` & `elements-sdk-3.6.1/test/test_subtask_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtask_reference.py` & `elements-sdk-3.6.1/test/test_subtask_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtask_update.py` & `elements-sdk-3.6.1/test/test_subtask_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtitle.py` & `elements-sdk-3.6.1/test/test_subtitle.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtitle_clipboard_entry.py` & `elements-sdk-3.6.1/test/test_subtitle_clipboard_entry.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtitle_clipboard_entry_update.py` & `elements-sdk-3.6.1/test/test_subtitle_clipboard_entry_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_subtitle_event.py` & `elements-sdk-3.6.1/test/test_subtitle_event.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_sync_totp.py` & `elements-sdk-3.6.1/test/test_sync_totp.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_sync_totp_request.py` & `elements-sdk-3.6.1/test/test_sync_totp_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_system_info_endpoint_response.py` & `elements-sdk-3.6.1/test/test_system_info_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tag_media_directory_request.py` & `elements-sdk-3.6.1/test/test_tag_media_directory_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tag_reference.py` & `elements-sdk-3.6.1/test/test_tag_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape.py` & `elements-sdk-3.6.1/test/test_tape.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_file.py` & `elements-sdk-3.6.1/test/test_tape_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_group.py` & `elements-sdk-3.6.1/test/test_tape_group.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_group_partial_update.py` & `elements-sdk-3.6.1/test/test_tape_group_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_group_update.py` & `elements-sdk-3.6.1/test/test_tape_group_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_job.py` & `elements-sdk-3.6.1/test/test_tape_job.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_job_source.py` & `elements-sdk-3.6.1/test/test_tape_job_source.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_endpoint_response.py` & `elements-sdk-3.6.1/test/test_tape_library_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_format_endpoint_request.py` & `elements-sdk-3.6.1/test/test_tape_library_format_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_fsck_endpoint_request.py` & `elements-sdk-3.6.1/test/test_tape_library_fsck_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_load_endpoint_request.py` & `elements-sdk-3.6.1/test/test_tape_library_load_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_move_endpoint_request.py` & `elements-sdk-3.6.1/test/test_tape_library_move_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_reindex_endpoint_request.py` & `elements-sdk-3.6.1/test/test_tape_library_reindex_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_slot.py` & `elements-sdk-3.6.1/test/test_tape_library_slot.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_library_unload_endpoint_request.py` & `elements-sdk-3.6.1/test/test_tape_library_unload_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_partial_update.py` & `elements-sdk-3.6.1/test/test_tape_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_reference.py` & `elements-sdk-3.6.1/test/test_tape_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tape_update.py` & `elements-sdk-3.6.1/test/test_tape_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_task_info.py` & `elements-sdk-3.6.1/test/test_task_info.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_task_log.py` & `elements-sdk-3.6.1/test/test_task_log.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_task_progress.py` & `elements-sdk-3.6.1/test/test_task_progress.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_task_type.py` & `elements-sdk-3.6.1/test/test_task_type.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_tasks_summary.py` & `elements-sdk-3.6.1/test/test_tasks_summary.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_teams_connection.py` & `elements-sdk-3.6.1/test/test_teams_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_teams_connection_partial_update.py` & `elements-sdk-3.6.1/test/test_teams_connection_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_teams_connection_status.py` & `elements-sdk-3.6.1/test/test_teams_connection_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_teams_connection_update.py` & `elements-sdk-3.6.1/test/test_teams_connection_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_teams_message.py` & `elements-sdk-3.6.1/test/test_teams_message.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_teams_recipient.py` & `elements-sdk-3.6.1/test/test_teams_recipient.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_aws_credentials_request.py` & `elements-sdk-3.6.1/test/test_test_aws_credentials_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_aws_credentials_response.py` & `elements-sdk-3.6.1/test/test_test_aws_credentials_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_cloud_account_credentials_request.py` & `elements-sdk-3.6.1/test/test_test_cloud_account_credentials_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_cloud_account_credentials_response.py` & `elements-sdk-3.6.1/test/test_test_cloud_account_credentials_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_external_transcoder_connection_request.py` & `elements-sdk-3.6.1/test/test_test_external_transcoder_connection_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_external_transcoder_connection_response.py` & `elements-sdk-3.6.1/test/test_test_external_transcoder_connection_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_test_smtp.py` & `elements-sdk-3.6.1/test/test_test_smtp.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_ticket.py` & `elements-sdk-3.6.1/test/test_ticket.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_time_endpoint_request.py` & `elements-sdk-3.6.1/test/test_time_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_time_endpoint_response.py` & `elements-sdk-3.6.1/test/test_time_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_time_sync_endpoint_request.py` & `elements-sdk-3.6.1/test/test_time_sync_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_time_sync_endpoint_response.py` & `elements-sdk-3.6.1/test/test_time_sync_endpoint_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_timeline_export_request.py` & `elements-sdk-3.6.1/test/test_timeline_export_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_timezone.py` & `elements-sdk-3.6.1/test/test_timezone.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_trace_node.py` & `elements-sdk-3.6.1/test/test_trace_node.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_transcoder_profile.py` & `elements-sdk-3.6.1/test/test_transcoder_profile.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_type_documentation.py` & `elements-sdk-3.6.1/test/test_type_documentation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_unfiltered_tag.py` & `elements-sdk-3.6.1/test/test_unfiltered_tag.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_unfiltered_tag_partial_update.py` & `elements-sdk-3.6.1/test/test_unfiltered_tag_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_unfiltered_tag_update.py` & `elements-sdk-3.6.1/test/test_unfiltered_tag_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_update_quota_request.py` & `elements-sdk-3.6.1/test/test_update_quota_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_updated_file.py` & `elements-sdk-3.6.1/test/test_updated_file.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_upload_ai_image_request.py` & `elements-sdk-3.6.1/test/test_upload_ai_image_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_upload_chunk_endpoint_request.py` & `elements-sdk-3.6.1/test/test_upload_chunk_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_upload_image_endpoint_request.py` & `elements-sdk-3.6.1/test/test_upload_image_endpoint_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_user_preview_request.py` & `elements-sdk-3.6.1/test/test_user_preview_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_user_preview_response.py` & `elements-sdk-3.6.1/test/test_user_preview_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_vantage_workflow.py` & `elements-sdk-3.6.1/test/test_vantage_workflow.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_vantage_workflows.py` & `elements-sdk-3.6.1/test/test_vantage_workflows.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_veritone_connection.py` & `elements-sdk-3.6.1/test/test_veritone_connection.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_veritone_engine_list.py` & `elements-sdk-3.6.1/test/test_veritone_engine_list.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_veritone_job_list.py` & `elements-sdk-3.6.1/test/test_veritone_job_list.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_veritone_metadata.py` & `elements-sdk-3.6.1/test/test_veritone_metadata.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_veritone_upload_request.py` & `elements-sdk-3.6.1/test/test_veritone_upload_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume.py` & `elements-sdk-3.6.1/test/test_volume.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_bee_gfs_status.py` & `elements-sdk-3.6.1/test/test_volume_bee_gfs_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_lizard_fs_status.py` & `elements-sdk-3.6.1/test/test_volume_lizard_fs_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_mini.py` & `elements-sdk-3.6.1/test/test_volume_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_mini_reference.py` & `elements-sdk-3.6.1/test/test_volume_mini_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_partial_update.py` & `elements-sdk-3.6.1/test/test_volume_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_reference.py` & `elements-sdk-3.6.1/test/test_volume_reference.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_snfs_status.py` & `elements-sdk-3.6.1/test/test_volume_snfs_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_stat.py` & `elements-sdk-3.6.1/test/test_volume_stat.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_stats.py` & `elements-sdk-3.6.1/test/test_volume_stats.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_status.py` & `elements-sdk-3.6.1/test/test_volume_status.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_volume_update.py` & `elements-sdk-3.6.1/test/test_volume_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workflow_transition_request.py` & `elements-sdk-3.6.1/test/test_workflow_transition_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workflow_transition_response.py` & `elements-sdk-3.6.1/test/test_workflow_transition_response.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace.py` & `elements-sdk-3.6.1/test/test_workspace.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_check_in.py` & `elements-sdk-3.6.1/test/test_workspace_check_in.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_detail.py` & `elements-sdk-3.6.1/test/test_workspace_detail.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_detail_partial_update.py` & `elements-sdk-3.6.1/test/test_workspace_detail_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_detail_update.py` & `elements-sdk-3.6.1/test/test_workspace_detail_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_endpoint.py` & `elements-sdk-3.6.1/test/test_workspace_endpoint.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_move_to_request.py` & `elements-sdk-3.6.1/test/test_workspace_move_to_request.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_permission.py` & `elements-sdk-3.6.1/test/test_workspace_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_permission_partial_update.py` & `elements-sdk-3.6.1/test/test_workspace_permission_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_permission_update.py` & `elements-sdk-3.6.1/test/test_workspace_permission_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workspace_resolved_permission.py` & `elements-sdk-3.6.1/test/test_workspace_resolved_permission.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workstation.py` & `elements-sdk-3.6.1/test/test_workstation.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workstation_mini.py` & `elements-sdk-3.6.1/test/test_workstation_mini.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workstation_partial_update.py` & `elements-sdk-3.6.1/test/test_workstation_partial_update.py`

 * *Files identical despite different names*

### Comparing `elements-sdk-3.6.0/test/test_workstation_update.py` & `elements-sdk-3.6.1/test/test_workstation_update.py`

 * *Files identical despite different names*

