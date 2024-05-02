# Comparing `tmp/carbon_python_sdk-0.1.8.tar.gz` & `tmp/carbon_python_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carbon_python_sdk-0.1.8.tar", max compression
+gzip compressed data, was "carbon_python_sdk-0.1.9.tar", max compression
```

## Comparing `carbon_python_sdk-0.1.8.tar` & `carbon_python_sdk-0.1.9.tar`

### file list

```diff
@@ -1,771 +1,831 @@
--rw-r--r--   0        0        0     1081 2024-03-12 19:34:27.406162 carbon_python_sdk-0.1.8/LICENSE
--rw-r--r--   0        0        0    92506 2024-03-12 19:34:27.715855 carbon_python_sdk-0.1.8/README.md
--rw-r--r--   0        0        0      675 2024-03-12 19:34:27.186957 carbon_python_sdk-0.1.8/carbon/__init__.py
--rw-r--r--   0        0        0    76911 2024-03-12 19:34:27.187165 carbon_python_sdk-0.1.8/carbon/api_client.py
--rw-r--r--   0        0        0      663 2024-03-12 19:34:27.187348 carbon_python_sdk-0.1.8/carbon/api_response.py
--rw-r--r--   0        0        0      214 2024-03-12 19:34:27.187489 carbon_python_sdk-0.1.8/carbon/apis/__init__.py
--rw-r--r--   0        0        0     9538 2024-03-12 19:34:27.187619 carbon_python_sdk-0.1.8/carbon/apis/path_to_api.py
--rw-r--r--   0        0        0      233 2024-03-12 19:34:27.187981 carbon_python_sdk-0.1.8/carbon/apis/paths/__init__.py
--rw-r--r--   0        0        0      101 2024-03-12 19:34:27.188111 carbon_python_sdk-0.1.8/carbon/apis/paths/add_webhook.py
--rw-r--r--   0        0        0      114 2024-03-12 19:34:27.188243 carbon_python_sdk-0.1.8/carbon/apis/paths/auth_v1_access_token.py
--rw-r--r--   0        0        0      118 2024-03-12 19:34:27.188489 carbon_python_sdk-0.1.8/carbon/apis/paths/auth_v1_white_labeling.py
--rw-r--r--   0        0        0      119 2024-03-12 19:34:27.188946 carbon_python_sdk-0.1.8/carbon/apis/paths/create_user_file_tags.py
--rw-r--r--   0        0        0      103 2024-03-12 19:34:27.189144 carbon_python_sdk-0.1.8/carbon/apis/paths/delete_files.py
--rw-r--r--   0        0        0      119 2024-03-12 19:34:27.189309 carbon_python_sdk-0.1.8/carbon/apis/paths/delete_user_file_tags.py
--rw-r--r--   0        0        0      103 2024-03-12 19:34:27.189548 carbon_python_sdk-0.1.8/carbon/apis/paths/delete_users.py
--rw-r--r--   0        0        0      133 2024-03-12 19:34:27.189742 carbon_python_sdk-0.1.8/carbon/apis/paths/delete_webhook_webhook_id.py
--rw-r--r--   0        0        0      120 2024-03-12 19:34:27.189944 carbon_python_sdk-0.1.8/carbon/apis/paths/deletefile_file_id.py
--rw-r--r--   0        0        0      100 2024-03-12 19:34:27.190131 carbon_python_sdk-0.1.8/carbon/apis/paths/embeddings.py
--rw-r--r--   0        0        0       96 2024-03-12 19:34:27.190395 carbon_python_sdk-0.1.8/carbon/apis/paths/fetch_urls.py
--rw-r--r--   0        0        0      123 2024-03-12 19:34:27.190509 carbon_python_sdk-0.1.8/carbon/apis/paths/fetch_youtube_transcript.py
--rw-r--r--   0        0        0       89 2024-03-12 19:34:27.190627 carbon_python_sdk-0.1.8/carbon/apis/paths/health.py
--rw-r--r--   0        0        0      134 2024-03-12 19:34:27.190794 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_confluence_list.py
--rw-r--r--   0        0        0      134 2024-03-12 19:34:27.190988 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_confluence_sync.py
--rw-r--r--   0        0        0      124 2024-03-12 19:34:27.191112 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_files_sync.py
--rw-r--r--   0        0        0      123 2024-03-12 19:34:27.191223 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_freshdesk.py
--rw-r--r--   0        0        0      119 2024-03-12 19:34:27.191348 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_gitbook.py
--rw-r--r--   0        0        0      129 2024-03-12 19:34:27.191471 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_gitbook_spaces.py
--rw-r--r--   0        0        0      128 2024-03-12 19:34:27.191590 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_gitbook_sync.py
--rw-r--r--   0        0        0      124 2024-03-12 19:34:27.191702 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_gmail_sync.py
--rw-r--r--   0        0        0      134 2024-03-12 19:34:27.191819 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_gmail_user_labels.py
--rw-r--r--   0        0        0      124 2024-03-12 19:34:27.191948 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_items_list.py
--rw-r--r--   0        0        0      124 2024-03-12 19:34:27.192078 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_items_sync.py
--rw-r--r--   0        0        0      122 2024-03-12 19:34:27.192222 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_oauth_url.py
--rw-r--r--   0        0        0      128 2024-03-12 19:34:27.192363 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_outlook_sync.py
--rw-r--r--   0        0        0      146 2024-03-12 19:34:27.192491 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_outlook_user_categories.py
--rw-r--r--   0        0        0      140 2024-03-12 19:34:27.192613 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_outlook_user_folders.py
--rw-r--r--   0        0        0      120 2024-03-12 19:34:27.192739 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_rss_feed.py
--rw-r--r--   0        0        0      109 2024-03-12 19:34:27.192859 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_s3.py
--rw-r--r--   0        0        0      120 2024-03-12 19:34:27.192994 carbon_python_sdk-0.1.8/carbon/apis/paths/integrations_s3_files.py
--rw-r--r--   0        0        0      128 2024-03-12 19:34:27.193122 carbon_python_sdk-0.1.8/carbon/apis/paths/modify_user_configuration.py
--rw-r--r--   0        0        0      101 2024-03-12 19:34:27.193245 carbon_python_sdk-0.1.8/carbon/apis/paths/organization.py
--rw-r--r--   0        0        0      112 2024-03-12 19:34:27.193370 carbon_python_sdk-0.1.8/carbon/apis/paths/parsed_file_file_id.py
--rw-r--r--   0        0        0      106 2024-03-12 19:34:27.193496 carbon_python_sdk-0.1.8/carbon/apis/paths/process_sitemap.py
--rw-r--r--   0        0        0      106 2024-03-12 19:34:27.193633 carbon_python_sdk-0.1.8/carbon/apis/paths/raw_file_file_id.py
--rw-r--r--   0        0        0      101 2024-03-12 19:34:27.193752 carbon_python_sdk-0.1.8/carbon/apis/paths/resync_file.py
--rw-r--r--   0        0        0      116 2024-03-12 19:34:27.193874 carbon_python_sdk-0.1.8/carbon/apis/paths/revoke_access_token.py
--rw-r--r--   0        0        0      107 2024-03-12 19:34:27.194176 carbon_python_sdk-0.1.8/carbon/apis/paths/scrape_sitemap.py
--rw-r--r--   0        0        0       98 2024-03-12 19:34:27.194755 carbon_python_sdk-0.1.8/carbon/apis/paths/search_urls.py
--rw-r--r--   0        0        0      101 2024-03-12 19:34:27.195144 carbon_python_sdk-0.1.8/carbon/apis/paths/text_chunks.py
--rw-r--r--   0        0        0      133 2024-03-12 19:34:27.195270 carbon_python_sdk-0.1.8/carbon/apis/paths/upload_chunks_and_embeddings.py
--rw-r--r--   0        0        0      117 2024-03-12 19:34:27.195379 carbon_python_sdk-0.1.8/carbon/apis/paths/upload_file_from_url.py
--rw-r--r--   0        0        0      101 2024-03-12 19:34:27.195479 carbon_python_sdk-0.1.8/carbon/apis/paths/upload_text.py
--rw-r--r--   0        0        0      100 2024-03-12 19:34:27.195680 carbon_python_sdk-0.1.8/carbon/apis/paths/uploadfile.py
--rw-r--r--   0        0        0       88 2024-03-12 19:34:27.196549 carbon_python_sdk-0.1.8/carbon/apis/paths/user.py
--rw-r--r--   0        0        0      112 2024-03-12 19:34:27.197548 carbon_python_sdk-0.1.8/carbon/apis/paths/user_data_sources.py
--rw-r--r--   0        0        0       99 2024-03-12 19:34:27.197764 carbon_python_sdk-0.1.8/carbon/apis/paths/user_files.py
--rw-r--r--   0        0        0      104 2024-03-12 19:34:27.198091 carbon_python_sdk-0.1.8/carbon/apis/paths/user_files_v2.py
--rw-r--r--   0        0        0       99 2024-03-12 19:34:27.198254 carbon_python_sdk-0.1.8/carbon/apis/paths/web_scrape.py
--rw-r--r--   0        0        0       96 2024-03-12 19:34:27.198376 carbon_python_sdk-0.1.8/carbon/apis/paths/webhooks.py
--rw-r--r--   0        0        0     2044 2024-03-12 19:34:27.198509 carbon_python_sdk-0.1.8/carbon/apis/tag_to_api.py
--rw-r--r--   0        0        0      655 2024-03-12 19:34:27.198650 carbon_python_sdk-0.1.8/carbon/apis/tags/__init__.py
--rw-r--r--   0        0        0      663 2024-03-12 19:34:27.198787 carbon_python_sdk-0.1.8/carbon/apis/tags/auth_api.py
--rw-r--r--   0        0        0      493 2024-03-12 19:34:27.198912 carbon_python_sdk-0.1.8/carbon/apis/tags/auth_api_raw.py
--rw-r--r--   0        0        0      709 2024-03-12 19:34:27.199038 carbon_python_sdk-0.1.8/carbon/apis/tags/data_sources_api.py
--rw-r--r--   0        0        0      510 2024-03-12 19:34:27.199146 carbon_python_sdk-0.1.8/carbon/apis/tags/data_sources_api_raw.py
--rw-r--r--   0        0        0      798 2024-03-12 19:34:27.199273 carbon_python_sdk-0.1.8/carbon/apis/tags/embeddings_api.py
--rw-r--r--   0        0        0      610 2024-03-12 19:34:27.199382 carbon_python_sdk-0.1.8/carbon/apis/tags/embeddings_api_raw.py
--rw-r--r--   0        0        0     1418 2024-03-12 19:34:27.199505 carbon_python_sdk-0.1.8/carbon/apis/tags/files_api.py
--rw-r--r--   0        0        0     1304 2024-03-12 19:34:27.199620 carbon_python_sdk-0.1.8/carbon/apis/tags/files_api_raw.py
--rw-r--r--   0        0        0      550 2024-03-12 19:34:27.199741 carbon_python_sdk-0.1.8/carbon/apis/tags/health_api.py
--rw-r--r--   0        0        0      366 2024-03-12 19:34:27.200330 carbon_python_sdk-0.1.8/carbon/apis/tags/health_api_raw.py
--rw-r--r--   0        0        0     2150 2024-03-12 19:34:27.200588 carbon_python_sdk-0.1.8/carbon/apis/tags/integrations_api.py
--rw-r--r--   0        0        0     2044 2024-03-12 19:34:27.200716 carbon_python_sdk-0.1.8/carbon/apis/tags/integrations_api_raw.py
--rw-r--r--   0        0        0      587 2024-03-12 19:34:27.200833 carbon_python_sdk-0.1.8/carbon/apis/tags/organizations_api.py
--rw-r--r--   0        0        0      375 2024-03-12 19:34:27.200949 carbon_python_sdk-0.1.8/carbon/apis/tags/organizations_api_raw.py
--rw-r--r--   0        0        0      701 2024-03-12 19:34:27.201070 carbon_python_sdk-0.1.8/carbon/apis/tags/users_api.py
--rw-r--r--   0        0        0      533 2024-03-12 19:34:27.201188 carbon_python_sdk-0.1.8/carbon/apis/tags/users_api_raw.py
--rw-r--r--   0        0        0      976 2024-03-12 19:34:27.201300 carbon_python_sdk-0.1.8/carbon/apis/tags/utilities_api.py
--rw-r--r--   0        0        0      810 2024-03-12 19:34:27.201406 carbon_python_sdk-0.1.8/carbon/apis/tags/utilities_api_raw.py
--rw-r--r--   0        0        0      705 2024-03-12 19:34:27.201521 carbon_python_sdk-0.1.8/carbon/apis/tags/webhooks_api.py
--rw-r--r--   0        0        0      525 2024-03-12 19:34:27.202900 carbon_python_sdk-0.1.8/carbon/apis/tags/webhooks_api_raw.py
--rw-r--r--   0        0        0     1986 2024-03-12 19:34:27.203128 carbon_python_sdk-0.1.8/carbon/client.py
--rw-r--r--   0        0        0     1986 2024-03-12 19:34:27.204591 carbon_python_sdk-0.1.8/carbon/client.pyi
--rw-r--r--   0        0        0      676 2024-03-12 19:34:27.204720 carbon_python_sdk-0.1.8/carbon/client_custom.py
--rw-r--r--   0        0        0    17804 2024-03-12 19:34:27.204875 carbon_python_sdk-0.1.8/carbon/configuration.py
--rw-r--r--   0        0        0     7679 2024-03-12 19:34:27.205055 carbon_python_sdk-0.1.8/carbon/exceptions.py
--rw-r--r--   0        0        0     2274 2024-03-12 19:34:27.205156 carbon_python_sdk-0.1.8/carbon/exceptions_base.py
--rw-r--r--   0        0        0      340 2024-03-12 19:34:27.205474 carbon_python_sdk-0.1.8/carbon/model/__init__.py
--rw-r--r--   0        0        0     2282 2024-03-12 19:34:27.206204 carbon_python_sdk-0.1.8/carbon/model/add_webhook_props.py
--rw-r--r--   0        0        0     2282 2024-03-12 19:34:27.206365 carbon_python_sdk-0.1.8/carbon/model/add_webhook_props.pyi
--rw-r--r--   0        0        0     2371 2024-03-12 19:34:27.206499 carbon_python_sdk-0.1.8/carbon/model/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0     2371 2024-03-12 19:34:27.206614 carbon_python_sdk-0.1.8/carbon/model/body_create_upload_file_uploadfile_post.pyi
--rw-r--r--   0        0        0     4752 2024-03-12 19:34:27.206741 carbon_python_sdk-0.1.8/carbon/model/chunk_properties.py
--rw-r--r--   0        0        0     4752 2024-03-12 19:34:27.206894 carbon_python_sdk-0.1.8/carbon/model/chunk_properties.pyi
--rw-r--r--   0        0        0     4359 2024-03-12 19:34:27.207035 carbon_python_sdk-0.1.8/carbon/model/chunk_properties_nullable.py
--rw-r--r--   0        0        0     4359 2024-03-12 19:34:27.207176 carbon_python_sdk-0.1.8/carbon/model/chunk_properties_nullable.pyi
--rw-r--r--   0        0        0     4319 2024-03-12 19:34:27.207292 carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings.py
--rw-r--r--   0        0        0     4319 2024-03-12 19:34:27.207423 carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings.pyi
--rw-r--r--   0        0        0     1100 2024-03-12 19:34:27.207548 carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1100 2024-03-12 19:34:27.207660 carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_embedding.pyi
--rw-r--r--   0        0        0     6383 2024-03-12 19:34:27.207784 carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     6383 2024-03-12 19:34:27.207911 carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_upload_input.pyi
--rw-r--r--   0        0        0      548 2024-03-12 19:34:27.208033 carbon_python_sdk-0.1.8/carbon/model/configuration_keys.py
--rw-r--r--   0        0        0      548 2024-03-12 19:34:27.208176 carbon_python_sdk-0.1.8/carbon/model/configuration_keys.pyi
--rw-r--r--   0        0        0     1183 2024-03-12 19:34:27.208305 carbon_python_sdk-0.1.8/carbon/model/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      998 2024-03-12 19:34:27.208426 carbon_python_sdk-0.1.8/carbon/model/data_source_last_sync_actions.pyi
--rw-r--r--   0        0        0     1256 2024-03-12 19:34:27.208544 carbon_python_sdk-0.1.8/carbon/model/data_source_sync_statuses.py
--rw-r--r--   0        0        0     1033 2024-03-12 19:34:27.208663 carbon_python_sdk-0.1.8/carbon/model/data_source_sync_statuses.pyi
--rw-r--r--   0        0        0     5534 2024-03-12 19:34:27.209392 carbon_python_sdk-0.1.8/carbon/model/data_source_type.py
--rw-r--r--   0        0        0     4143 2024-03-12 19:34:27.209526 carbon_python_sdk-0.1.8/carbon/model/data_source_type.pyi
--rw-r--r--   0        0        0     5909 2024-03-12 19:34:27.209652 carbon_python_sdk-0.1.8/carbon/model/data_source_type_nullable.py
--rw-r--r--   0        0        0     5909 2024-03-12 19:34:27.209774 carbon_python_sdk-0.1.8/carbon/model/data_source_type_nullable.pyi
--rw-r--r--   0        0        0     6047 2024-03-12 19:34:27.209890 carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input.py
--rw-r--r--   0        0        0     6047 2024-03-12 19:34:27.210014 carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input.pyi
--rw-r--r--   0        0        0     1097 2024-03-12 19:34:27.210145 carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0     1097 2024-03-12 19:34:27.210274 carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input_file_ids.pyi
--rw-r--r--   0        0        0     2600 2024-03-12 19:34:27.210454 carbon_python_sdk-0.1.8/carbon/model/delete_users_input.py
--rw-r--r--   0        0        0     2600 2024-03-12 19:34:27.210916 carbon_python_sdk-0.1.8/carbon/model/delete_users_input.pyi
--rw-r--r--   0        0        0     1199 2024-03-12 19:34:27.211054 carbon_python_sdk-0.1.8/carbon/model/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0     1199 2024-03-12 19:34:27.211209 carbon_python_sdk-0.1.8/carbon/model/delete_users_input_customer_ids.pyi
--rw-r--r--   0        0        0     3902 2024-03-12 19:34:27.211333 carbon_python_sdk-0.1.8/carbon/model/directory_item.py
--rw-r--r--   0        0        0     3902 2024-03-12 19:34:27.211460 carbon_python_sdk-0.1.8/carbon/model/directory_item.pyi
--rw-r--r--   0        0        0    13554 2024-03-12 19:34:27.211963 carbon_python_sdk-0.1.8/carbon/model/document_response.py
--rw-r--r--   0        0        0    13554 2024-03-12 19:34:27.212640 carbon_python_sdk-0.1.8/carbon/model/document_response.pyi
--rw-r--r--   0        0        0     3350 2024-03-12 19:34:27.213073 carbon_python_sdk-0.1.8/carbon/model/document_response_list.py
--rw-r--r--   0        0        0     3350 2024-03-12 19:34:27.213202 carbon_python_sdk-0.1.8/carbon/model/document_response_list.pyi
--rw-r--r--   0        0        0     7489 2024-03-12 19:34:27.213340 carbon_python_sdk-0.1.8/carbon/model/document_response_tags.py
--rw-r--r--   0        0        0     7489 2024-03-12 19:34:27.213464 carbon_python_sdk-0.1.8/carbon/model/document_response_tags.pyi
--rw-r--r--   0        0        0     1088 2024-03-12 19:34:27.213595 carbon_python_sdk-0.1.8/carbon/model/document_response_vector.py
--rw-r--r--   0        0        0     1088 2024-03-12 19:34:27.213721 carbon_python_sdk-0.1.8/carbon/model/document_response_vector.pyi
--rw-r--r--   0        0        0     5044 2024-03-12 19:34:27.214057 carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk.py
--rw-r--r--   0        0        0     5044 2024-03-12 19:34:27.214323 carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk.pyi
--rw-r--r--   0        0        0     1096 2024-03-12 19:34:27.214632 carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0     1096 2024-03-12 19:34:27.214789 carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk_embedding.pyi
--rw-r--r--   0        0        0     3025 2024-03-12 19:34:27.214906 carbon_python_sdk-0.1.8/carbon/model/embedding_generators.py
--rw-r--r--   0        0        0     2166 2024-03-12 19:34:27.215039 carbon_python_sdk-0.1.8/carbon/model/embedding_generators.pyi
--rw-r--r--   0        0        0     3405 2024-03-12 19:34:27.215159 carbon_python_sdk-0.1.8/carbon/model/embedding_generators_nullable.py
--rw-r--r--   0        0        0     3405 2024-03-12 19:34:27.215281 carbon_python_sdk-0.1.8/carbon/model/embedding_generators_nullable.pyi
--rw-r--r--   0        0        0     4307 2024-03-12 19:34:27.215394 carbon_python_sdk-0.1.8/carbon/model/embedding_properties.py
--rw-r--r--   0        0        0     4307 2024-03-12 19:34:27.215530 carbon_python_sdk-0.1.8/carbon/model/embedding_properties.pyi
--rw-r--r--   0        0        0     3267 2024-03-12 19:34:27.215639 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0     3267 2024-03-12 19:34:27.215754 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_filters.pyi
--rw-r--r--   0        0        0     1141 2024-03-12 19:34:27.215875 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0      956 2024-03-12 19:34:27.216002 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_order_by_columns.pyi
--rw-r--r--   0        0        0     5194 2024-03-12 19:34:27.216114 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0     5194 2024-03-12 19:34:27.216225 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_query_input.pyi
--rw-r--r--   0        0        0     3847 2024-03-12 19:34:27.216340 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0     3847 2024-03-12 19:34:27.216453 carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_response.pyi
--rw-r--r--   0        0        0     1944 2024-03-12 19:34:27.216565 carbon_python_sdk-0.1.8/carbon/model/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1503 2024-03-12 19:34:27.216673 carbon_python_sdk-0.1.8/carbon/model/external_file_sync_statuses.pyi
--rw-r--r--   0        0        0    16741 2024-03-12 19:34:27.216792 carbon_python_sdk-0.1.8/carbon/model/external_source_item.py
--rw-r--r--   0        0        0    16741 2024-03-12 19:34:27.216976 carbon_python_sdk-0.1.8/carbon/model/external_source_item.pyi
--rw-r--r--   0        0        0     3061 2024-03-12 19:34:27.217130 carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response.py
--rw-r--r--   0        0        0     3061 2024-03-12 19:34:27.217248 carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response.pyi
--rw-r--r--   0        0        0     1187 2024-03-12 19:34:27.217357 carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response_urls.py
--rw-r--r--   0        0        0     1187 2024-03-12 19:34:27.217469 carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response_urls.pyi
--rw-r--r--   0        0        0      946 2024-03-12 19:34:27.217593 carbon_python_sdk-0.1.8/carbon/model/file_content_types.py
--rw-r--r--   0        0        0      825 2024-03-12 19:34:27.217724 carbon_python_sdk-0.1.8/carbon/model/file_content_types.pyi
--rw-r--r--   0        0        0     1706 2024-03-12 19:34:27.217837 carbon_python_sdk-0.1.8/carbon/model/file_content_types_nullable.py
--rw-r--r--   0        0        0     1706 2024-03-12 19:34:27.217954 carbon_python_sdk-0.1.8/carbon/model/file_content_types_nullable.pyi
--rw-r--r--   0        0        0     4851 2024-03-12 19:34:27.218098 carbon_python_sdk-0.1.8/carbon/model/file_formats.py
--rw-r--r--   0        0        0     3650 2024-03-12 19:34:27.218213 carbon_python_sdk-0.1.8/carbon/model/file_formats.pyi
--rw-r--r--   0        0        0     5223 2024-03-12 19:34:27.218337 carbon_python_sdk-0.1.8/carbon/model/file_formats_nullable.py
--rw-r--r--   0        0        0     5223 2024-03-12 19:34:27.218460 carbon_python_sdk-0.1.8/carbon/model/file_formats_nullable.pyi
--rw-r--r--   0        0        0     7489 2024-03-12 19:34:27.218584 carbon_python_sdk-0.1.8/carbon/model/file_statistics.py
--rw-r--r--   0        0        0     7489 2024-03-12 19:34:27.218711 carbon_python_sdk-0.1.8/carbon/model/file_statistics.pyi
--rw-r--r--   0        0        0     6952 2024-03-12 19:34:27.220154 carbon_python_sdk-0.1.8/carbon/model/file_statistics_nullable.py
--rw-r--r--   0        0        0     6952 2024-03-12 19:34:27.220698 carbon_python_sdk-0.1.8/carbon/model/file_statistics_nullable.pyi
--rw-r--r--   0        0        0     1283 2024-03-12 19:34:27.221059 carbon_python_sdk-0.1.8/carbon/model/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1283 2024-03-12 19:34:27.221277 carbon_python_sdk-0.1.8/carbon/model/files_query_user_files_deprecated_response.pyi
--rw-r--r--   0        0        0    12927 2024-03-12 19:34:27.221499 carbon_python_sdk-0.1.8/carbon/model/fresh_desk_connect_request.py
--rw-r--r--   0        0        0    12927 2024-03-12 19:34:27.221828 carbon_python_sdk-0.1.8/carbon/model/fresh_desk_connect_request.pyi
--rw-r--r--   0        0        0     2362 2024-03-12 19:34:27.222078 carbon_python_sdk-0.1.8/carbon/model/generic_success_response.py
--rw-r--r--   0        0        0     2362 2024-03-12 19:34:27.222191 carbon_python_sdk-0.1.8/carbon/model/generic_success_response.pyi
--rw-r--r--   0        0        0    15093 2024-03-12 19:34:27.222515 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body.py
--rw-r--r--   0        0        0    14942 2024-03-12 19:34:27.224255 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body.pyi
--rw-r--r--   0        0        0     1159 2024-03-12 19:34:27.224937 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0     1159 2024-03-12 19:34:27.225248 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_file_ids.pyi
--rw-r--r--   0        0        0     1264 2024-03-12 19:34:27.225493 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0     1264 2024-03-12 19:34:27.225986 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_parent_file_ids.pyi
--rw-r--r--   0        0        0     1377 2024-03-12 19:34:27.226465 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0     1377 2024-03-12 19:34:27.227204 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_query_vector.pyi
--rw-r--r--   0        0        0     6490 2024-03-12 19:34:27.228028 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0     6490 2024-03-12 19:34:27.228851 carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_tags.pyi
--rw-r--r--   0        0        0    13042 2024-03-12 19:34:27.229639 carbon_python_sdk-0.1.8/carbon/model/gitbook_connect_request.py
--rw-r--r--   0        0        0    13042 2024-03-12 19:34:27.231066 carbon_python_sdk-0.1.8/carbon/model/gitbook_connect_request.pyi
--rw-r--r--   0        0        0    11852 2024-03-12 19:34:27.231469 carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request.py
--rw-r--r--   0        0        0    11852 2024-03-12 19:34:27.232138 carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request.pyi
--rw-r--r--   0        0        0     1220 2024-03-12 19:34:27.232477 carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0     1197 2024-03-12 19:34:27.232632 carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request_space_ids.pyi
--rw-r--r--   0        0        0    12263 2024-03-12 19:34:27.232789 carbon_python_sdk-0.1.8/carbon/model/gmail_sync_input.py
--rw-r--r--   0        0        0    12263 2024-03-12 19:34:27.232983 carbon_python_sdk-0.1.8/carbon/model/gmail_sync_input.pyi
--rw-r--r--   0        0        0     3251 2024-03-12 19:34:27.233160 carbon_python_sdk-0.1.8/carbon/model/http_validation_error.py
--rw-r--r--   0        0        0     3251 2024-03-12 19:34:27.233261 carbon_python_sdk-0.1.8/carbon/model/http_validation_error.pyi
--rw-r--r--   0        0        0     2974 2024-03-12 19:34:27.233384 carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0     2974 2024-03-12 19:34:27.233502 carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params.pyi
--rw-r--r--   0        0        0     2907 2024-03-12 19:34:27.233616 carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0     2907 2024-03-12 19:34:27.233726 carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params_nullable.pyi
--rw-r--r--   0        0        0     4274 2024-03-12 19:34:27.233863 carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_request.py
--rw-r--r--   0        0        0     4274 2024-03-12 19:34:27.233982 carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_request.pyi
--rw-r--r--   0        0        0     3820 2024-03-12 19:34:27.234096 carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_response.py
--rw-r--r--   0        0        0     3820 2024-03-12 19:34:27.234207 carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_response.pyi
--rw-r--r--   0        0        0     3613 2024-03-12 19:34:27.234320 carbon_python_sdk-0.1.8/carbon/model/list_request.py
--rw-r--r--   0        0        0     3613 2024-03-12 19:34:27.234435 carbon_python_sdk-0.1.8/carbon/model/list_request.pyi
--rw-r--r--   0        0        0     3228 2024-03-12 19:34:27.234552 carbon_python_sdk-0.1.8/carbon/model/list_response.py
--rw-r--r--   0        0        0     3228 2024-03-12 19:34:27.234656 carbon_python_sdk-0.1.8/carbon/model/list_response.pyi
--rw-r--r--   0        0        0     3129 2024-03-12 19:34:27.234765 carbon_python_sdk-0.1.8/carbon/model/modify_user_configuration_input.py
--rw-r--r--   0        0        0     3129 2024-03-12 19:34:27.235854 carbon_python_sdk-0.1.8/carbon/model/modify_user_configuration_input.pyi
--rw-r--r--   0        0        0    23818 2024-03-12 19:34:27.236105 carbon_python_sdk-0.1.8/carbon/model/o_auth_url_request.py
--rw-r--r--   0        0        0    23818 2024-03-12 19:34:27.236442 carbon_python_sdk-0.1.8/carbon/model/o_auth_url_request.pyi
--rw-r--r--   0        0        0      930 2024-03-12 19:34:27.236588 carbon_python_sdk-0.1.8/carbon/model/order_dir.py
--rw-r--r--   0        0        0      813 2024-03-12 19:34:27.236710 carbon_python_sdk-0.1.8/carbon/model/order_dir.pyi
--rw-r--r--   0        0        0    14659 2024-03-12 19:34:27.236841 carbon_python_sdk-0.1.8/carbon/model/organization_response.py
--rw-r--r--   0        0        0    14659 2024-03-12 19:34:27.237119 carbon_python_sdk-0.1.8/carbon/model/organization_response.pyi
--rw-r--r--   0        0        0    12247 2024-03-12 19:34:27.237373 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_api.py
--rw-r--r--   0        0        0    12247 2024-03-12 19:34:27.237579 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_api.pyi
--rw-r--r--   0        0        0     4467 2024-03-12 19:34:27.237803 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters.py
--rw-r--r--   0        0        0     4467 2024-03-12 19:34:27.237919 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters.pyi
--rw-r--r--   0        0        0     1113 2024-03-12 19:34:27.238026 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0     1113 2024-03-12 19:34:27.239616 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters_ids.pyi
--rw-r--r--   0        0        0     1014 2024-03-12 19:34:27.239783 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0      871 2024-03-12 19:34:27.239924 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_order_by_columns.pyi
--rw-r--r--   0        0        0     4657 2024-03-12 19:34:27.240059 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0     4657 2024-03-12 19:34:27.240191 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_query_input.pyi
--rw-r--r--   0        0        0     3947 2024-03-12 19:34:27.240322 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_response.py
--rw-r--r--   0        0        0     3947 2024-03-12 19:34:27.240448 carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_response.pyi
--rw-r--r--   0        0        0     3408 2024-03-12 19:34:27.240553 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create.py
--rw-r--r--   0        0        0     3408 2024-03-12 19:34:27.240667 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create.pyi
--rw-r--r--   0        0        0     6330 2024-03-12 19:34:27.240795 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0     6330 2024-03-12 19:34:27.240931 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create_tags.pyi
--rw-r--r--   0        0        0     3418 2024-03-12 19:34:27.241263 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0     3418 2024-03-12 19:34:27.241710 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove.pyi
--rw-r--r--   0        0        0     1213 2024-03-12 19:34:27.241975 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     1213 2024-03-12 19:34:27.242199 carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove_tags.pyi
--rw-r--r--   0        0        0    16946 2024-03-12 19:34:27.242415 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0    16946 2024-03-12 19:34:27.242637 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters.pyi
--rw-r--r--   0        0        0     1139 2024-03-12 19:34:27.242849 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0     1139 2024-03-12 19:34:27.242993 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi
--rw-r--r--   0        0        0     1115 2024-03-12 19:34:27.243133 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0     1115 2024-03-12 19:34:27.243251 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_ids.pyi
--rw-r--r--   0        0        0     1165 2024-03-12 19:34:27.243359 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0     1165 2024-03-12 19:34:27.243473 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi
--rw-r--r--   0        0        0     1135 2024-03-12 19:34:27.243610 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0     1135 2024-03-12 19:34:27.243722 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi
--rw-r--r--   0        0        0     6420 2024-03-12 19:34:27.243859 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0     6420 2024-03-12 19:34:27.243985 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_tags.pyi
--rw-r--r--   0        0        0     1371 2024-03-12 19:34:27.244103 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1124 2024-03-12 19:34:27.244210 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_order_by_types.pyi
--rw-r--r--   0        0        0     8629 2024-03-12 19:34:27.244310 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0     8629 2024-03-12 19:34:27.244502 carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_query_input.pyi
--rw-r--r--   0        0        0     2378 2024-03-12 19:34:27.244709 carbon_python_sdk-0.1.8/carbon/model/outh_url_response.py
--rw-r--r--   0        0        0     2378 2024-03-12 19:34:27.244833 carbon_python_sdk-0.1.8/carbon/model/outh_url_response.pyi
--rw-r--r--   0        0        0    13371 2024-03-12 19:34:27.244945 carbon_python_sdk-0.1.8/carbon/model/outlook_sync_input.py
--rw-r--r--   0        0        0    13371 2024-03-12 19:34:27.245194 carbon_python_sdk-0.1.8/carbon/model/outlook_sync_input.pyi
--rw-r--r--   0        0        0     2807 2024-03-12 19:34:27.245423 carbon_python_sdk-0.1.8/carbon/model/pagination.py
--rw-r--r--   0        0        0     2807 2024-03-12 19:34:27.245525 carbon_python_sdk-0.1.8/carbon/model/pagination.pyi
--rw-r--r--   0        0        0     2452 2024-03-12 19:34:27.245648 carbon_python_sdk-0.1.8/carbon/model/presigned_url_response.py
--rw-r--r--   0        0        0     2452 2024-03-12 19:34:27.245747 carbon_python_sdk-0.1.8/carbon/model/presigned_url_response.pyi
--rw-r--r--   0        0        0    10068 2024-03-12 19:34:27.245854 carbon_python_sdk-0.1.8/carbon/model/raw_text_input.py
--rw-r--r--   0        0        0    10068 2024-03-12 19:34:27.246053 carbon_python_sdk-0.1.8/carbon/model/raw_text_input.pyi
--rw-r--r--   0        0        0     5578 2024-03-12 19:34:27.246242 carbon_python_sdk-0.1.8/carbon/model/resync_file_query_input.py
--rw-r--r--   0        0        0     5578 2024-03-12 19:34:27.246520 carbon_python_sdk-0.1.8/carbon/model/resync_file_query_input.pyi
--rw-r--r--   0        0        0     2489 2024-03-12 19:34:27.246753 carbon_python_sdk-0.1.8/carbon/model/revoke_access_token_input.py
--rw-r--r--   0        0        0     2489 2024-03-12 19:34:27.246884 carbon_python_sdk-0.1.8/carbon/model/revoke_access_token_input.pyi
--rw-r--r--   0        0        0    10916 2024-03-12 19:34:27.247023 carbon_python_sdk-0.1.8/carbon/model/rss_feed_input.py
--rw-r--r--   0        0        0    10916 2024-03-12 19:34:27.247230 carbon_python_sdk-0.1.8/carbon/model/rss_feed_input.pyi
--rw-r--r--   0        0        0     3074 2024-03-12 19:34:27.247424 carbon_python_sdk-0.1.8/carbon/model/s3_auth_request.py
--rw-r--r--   0        0        0     3074 2024-03-12 19:34:27.247549 carbon_python_sdk-0.1.8/carbon/model/s3_auth_request.pyi
--rw-r--r--   0        0        0    15132 2024-03-12 19:34:27.247701 carbon_python_sdk-0.1.8/carbon/model/s3_file_sync_input.py
--rw-r--r--   0        0        0    15132 2024-03-12 19:34:27.247970 carbon_python_sdk-0.1.8/carbon/model/s3_file_sync_input.pyi
--rw-r--r--   0        0        0     3936 2024-03-12 19:34:27.248268 carbon_python_sdk-0.1.8/carbon/model/s3_get_file_input.py
--rw-r--r--   0        0        0     3936 2024-03-12 19:34:27.248399 carbon_python_sdk-0.1.8/carbon/model/s3_get_file_input.pyi
--rw-r--r--   0        0        0     6587 2024-03-12 19:34:27.248590 carbon_python_sdk-0.1.8/carbon/model/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     6587 2024-03-12 19:34:27.248738 carbon_python_sdk-0.1.8/carbon/model/single_chunks_and_embeddings_upload_input.pyi
--rw-r--r--   0        0        0    15550 2024-03-12 19:34:27.248900 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request.py
--rw-r--r--   0        0        0    15550 2024-03-12 19:34:27.249184 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request.pyi
--rw-r--r--   0        0        0     1113 2024-03-12 19:34:27.249460 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0     1113 2024-03-12 19:34:27.249617 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi
--rw-r--r--   0        0        0     1117 2024-03-12 19:34:27.249765 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0     1117 2024-03-12 19:34:27.249914 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi
--rw-r--r--   0        0        0     1109 2024-03-12 19:34:27.250070 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0     1109 2024-03-12 19:34:27.250226 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi
--rw-r--r--   0        0        0     6392 2024-03-12 19:34:27.250371 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0     6392 2024-03-12 19:34:27.250523 carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_tags.pyi
--rw-r--r--   0        0        0     2485 2024-03-12 19:34:27.250692 carbon_python_sdk-0.1.8/carbon/model/sync_directory_request.py
--rw-r--r--   0        0        0     2485 2024-03-12 19:34:27.250844 carbon_python_sdk-0.1.8/carbon/model/sync_directory_request.pyi
--rw-r--r--   0        0        0     2784 2024-03-12 19:34:27.250990 carbon_python_sdk-0.1.8/carbon/model/sync_files_ids.py
--rw-r--r--   0        0        0     2784 2024-03-12 19:34:27.251235 carbon_python_sdk-0.1.8/carbon/model/sync_files_ids.pyi
--rw-r--r--   0        0        0    17722 2024-03-12 19:34:27.251406 carbon_python_sdk-0.1.8/carbon/model/sync_files_request.py
--rw-r--r--   0        0        0    17722 2024-03-12 19:34:27.251572 carbon_python_sdk-0.1.8/carbon/model/sync_files_request.pyi
--rw-r--r--   0        0        0     2029 2024-03-12 19:34:27.251820 carbon_python_sdk-0.1.8/carbon/model/text_embedding_generators.py
--rw-r--r--   0        0        0     1520 2024-03-12 19:34:27.252083 carbon_python_sdk-0.1.8/carbon/model/text_embedding_generators.pyi
--rw-r--r--   0        0        0     3042 2024-03-12 19:34:27.252213 carbon_python_sdk-0.1.8/carbon/model/token_response.py
--rw-r--r--   0        0        0     3042 2024-03-12 19:34:27.252459 carbon_python_sdk-0.1.8/carbon/model/token_response.pyi
--rw-r--r--   0        0        0    11472 2024-03-12 19:34:27.252728 carbon_python_sdk-0.1.8/carbon/model/upload_file_from_url_input.py
--rw-r--r--   0        0        0    11472 2024-03-12 19:34:27.252974 carbon_python_sdk-0.1.8/carbon/model/upload_file_from_url_input.pyi
--rw-r--r--   0        0        0    31568 2024-03-12 19:34:27.253190 carbon_python_sdk-0.1.8/carbon/model/user_file.py
--rw-r--r--   0        0        0    31568 2024-03-12 19:34:27.253391 carbon_python_sdk-0.1.8/carbon/model/user_file.pyi
--rw-r--r--   0        0        0     1650 2024-03-12 19:34:27.253540 carbon_python_sdk-0.1.8/carbon/model/user_file_embedding_properties.py
--rw-r--r--   0        0        0     1650 2024-03-12 19:34:27.253667 carbon_python_sdk-0.1.8/carbon/model/user_file_embedding_properties.pyi
--rw-r--r--   0        0        0     3751 2024-03-12 19:34:27.253784 carbon_python_sdk-0.1.8/carbon/model/user_files_v2.py
--rw-r--r--   0        0        0     3751 2024-03-12 19:34:27.253908 carbon_python_sdk-0.1.8/carbon/model/user_files_v2.pyi
--rw-r--r--   0        0        0     2416 2024-03-12 19:34:27.254038 carbon_python_sdk-0.1.8/carbon/model/user_request_content.py
--rw-r--r--   0        0        0     2416 2024-03-12 19:34:27.254153 carbon_python_sdk-0.1.8/carbon/model/user_request_content.pyi
--rw-r--r--   0        0        0    10845 2024-03-12 19:34:27.254294 carbon_python_sdk-0.1.8/carbon/model/user_response.py
--rw-r--r--   0        0        0    10845 2024-03-12 19:34:27.254521 carbon_python_sdk-0.1.8/carbon/model/user_response.pyi
--rw-r--r--   0        0        0     1246 2024-03-12 19:34:27.254832 carbon_python_sdk-0.1.8/carbon/model/user_response_unique_file_tags.py
--rw-r--r--   0        0        0     1246 2024-03-12 19:34:27.255027 carbon_python_sdk-0.1.8/carbon/model/user_response_unique_file_tags.pyi
--rw-r--r--   0        0        0     1315 2024-03-12 19:34:27.255189 carbon_python_sdk-0.1.8/carbon/model/utilities_scrape_web_request.py
--rw-r--r--   0        0        0     1315 2024-03-12 19:34:27.255324 carbon_python_sdk-0.1.8/carbon/model/utilities_scrape_web_request.pyi
--rw-r--r--   0        0        0     3352 2024-03-12 19:34:27.255456 carbon_python_sdk-0.1.8/carbon/model/validation_error.py
--rw-r--r--   0        0        0     3352 2024-03-12 19:34:27.255580 carbon_python_sdk-0.1.8/carbon/model/validation_error.pyi
--rw-r--r--   0        0        0     3149 2024-03-12 19:34:27.255717 carbon_python_sdk-0.1.8/carbon/model/validation_error_loc.py
--rw-r--r--   0        0        0     3149 2024-03-12 19:34:27.255869 carbon_python_sdk-0.1.8/carbon/model/validation_error_loc.pyi
--rw-r--r--   0        0        0     5158 2024-03-12 19:34:27.256028 carbon_python_sdk-0.1.8/carbon/model/webhook.py
--rw-r--r--   0        0        0     5158 2024-03-12 19:34:27.256166 carbon_python_sdk-0.1.8/carbon/model/webhook.pyi
--rw-r--r--   0        0        0     2396 2024-03-12 19:34:27.256290 carbon_python_sdk-0.1.8/carbon/model/webhook_filters.py
--rw-r--r--   0        0        0     2396 2024-03-12 19:34:27.256420 carbon_python_sdk-0.1.8/carbon/model/webhook_filters.pyi
--rw-r--r--   0        0        0     1075 2024-03-12 19:34:27.256583 carbon_python_sdk-0.1.8/carbon/model/webhook_filters_ids.py
--rw-r--r--   0        0        0     1075 2024-03-12 19:34:27.256733 carbon_python_sdk-0.1.8/carbon/model/webhook_filters_ids.pyi
--rw-r--r--   0        0        0     4580 2024-03-12 19:34:27.256879 carbon_python_sdk-0.1.8/carbon/model/webhook_no_key.py
--rw-r--r--   0        0        0     4580 2024-03-12 19:34:27.257025 carbon_python_sdk-0.1.8/carbon/model/webhook_no_key.pyi
--rw-r--r--   0        0        0      995 2024-03-12 19:34:27.257159 carbon_python_sdk-0.1.8/carbon/model/webhook_order_by_columns.py
--rw-r--r--   0        0        0      852 2024-03-12 19:34:27.257293 carbon_python_sdk-0.1.8/carbon/model/webhook_order_by_columns.pyi
--rw-r--r--   0        0        0     4347 2024-03-12 19:34:27.257419 carbon_python_sdk-0.1.8/carbon/model/webhook_query_input.py
--rw-r--r--   0        0        0     4347 2024-03-12 19:34:27.257557 carbon_python_sdk-0.1.8/carbon/model/webhook_query_input.pyi
--rw-r--r--   0        0        0     3798 2024-03-12 19:34:27.257696 carbon_python_sdk-0.1.8/carbon/model/webhook_query_response.py
--rw-r--r--   0        0        0     3798 2024-03-12 19:34:27.257831 carbon_python_sdk-0.1.8/carbon/model/webhook_query_response.pyi
--rw-r--r--   0        0        0    16694 2024-03-12 19:34:27.257981 carbon_python_sdk-0.1.8/carbon/model/webscrape_request.py
--rw-r--r--   0        0        0    16694 2024-03-12 19:34:27.258187 carbon_python_sdk-0.1.8/carbon/model/webscrape_request.pyi
--rw-r--r--   0        0        0     1105 2024-03-12 19:34:27.258378 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0     1105 2024-03-12 19:34:27.258520 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_classes_to_skip.pyi
--rw-r--r--   0        0        0     1109 2024-03-12 19:34:27.258650 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0     1109 2024-03-12 19:34:27.258780 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_selectors_to_skip.pyi
--rw-r--r--   0        0        0     1101 2024-03-12 19:34:27.258931 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0     1101 2024-03-12 19:34:27.259058 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_html_tags_to_skip.pyi
--rw-r--r--   0        0        0     6384 2024-03-12 19:34:27.259186 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_tags.py
--rw-r--r--   0        0        0     6384 2024-03-12 19:34:27.259303 carbon_python_sdk-0.1.8/carbon/model/webscrape_request_tags.pyi
--rw-r--r--   0        0        0     3117 2024-03-12 19:34:27.259438 carbon_python_sdk-0.1.8/carbon/model/white_labeling_response.py
--rw-r--r--   0        0        0     3117 2024-03-12 19:34:27.259572 carbon_python_sdk-0.1.8/carbon/model/white_labeling_response.pyi
--rw-r--r--   0        0        0     5401 2024-03-12 19:34:27.259713 carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response.py
--rw-r--r--   0        0        0     5401 2024-03-12 19:34:27.259860 carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response.pyi
--rw-r--r--   0        0        0     1375 2024-03-12 19:34:27.259993 carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0     1375 2024-03-12 19:34:27.260141 carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript.pyi
--rw-r--r--   0        0        0     3326 2024-03-12 19:34:27.262161 carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0     3326 2024-03-12 19:34:27.262577 carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript_item.pyi
--rw-r--r--   0        0        0    10396 2024-03-12 19:34:27.263027 carbon_python_sdk-0.1.8/carbon/models/__init__.py
--rw-r--r--   0        0        0    20457 2024-03-12 19:34:27.263288 carbon_python_sdk-0.1.8/carbon/operation_parameter_map.py
--rw-r--r--   0        0        0     2733 2024-03-12 19:34:27.263450 carbon_python_sdk-0.1.8/carbon/paths/__init__.py
--rw-r--r--   0        0        0      293 2024-03-12 19:34:27.263584 carbon_python_sdk-0.1.8/carbon/paths/add_webhook/__init__.py
--rw-r--r--   0        0        0    13953 2024-03-12 19:34:27.263700 carbon_python_sdk-0.1.8/carbon/paths/add_webhook/post.py
--rw-r--r--   0        0        0    13811 2024-03-12 19:34:27.263997 carbon_python_sdk-0.1.8/carbon/paths/add_webhook/post.pyi
--rw-r--r--   0        0        0      311 2024-03-12 19:34:27.264269 carbon_python_sdk-0.1.8/carbon/paths/auth_v1_access_token/__init__.py
--rw-r--r--   0        0        0    11830 2024-03-12 19:34:27.264396 carbon_python_sdk-0.1.8/carbon/paths/auth_v1_access_token/get.py
--rw-r--r--   0        0        0    11656 2024-03-12 19:34:27.264586 carbon_python_sdk-0.1.8/carbon/paths/auth_v1_access_token/get.pyi
--rw-r--r--   0        0        0      315 2024-03-12 19:34:27.264772 carbon_python_sdk-0.1.8/carbon/paths/auth_v1_white_labeling/__init__.py
--rw-r--r--   0        0        0    11983 2024-03-12 19:34:27.264894 carbon_python_sdk-0.1.8/carbon/paths/auth_v1_white_labeling/get.py
--rw-r--r--   0        0        0    11841 2024-03-12 19:34:27.265106 carbon_python_sdk-0.1.8/carbon/paths/auth_v1_white_labeling/get.pyi
--rw-r--r--   0        0        0      313 2024-03-12 19:34:27.265889 carbon_python_sdk-0.1.8/carbon/paths/create_user_file_tags/__init__.py
--rw-r--r--   0        0        0    15880 2024-03-12 19:34:27.266152 carbon_python_sdk-0.1.8/carbon/paths/create_user_file_tags/post.py
--rw-r--r--   0        0        0    15706 2024-03-12 19:34:27.266481 carbon_python_sdk-0.1.8/carbon/paths/create_user_file_tags/post.pyi
--rw-r--r--   0        0        0      295 2024-03-12 19:34:27.266749 carbon_python_sdk-0.1.8/carbon/paths/delete_files/__init__.py
--rw-r--r--   0        0        0    18977 2024-03-12 19:34:27.266867 carbon_python_sdk-0.1.8/carbon/paths/delete_files/post.py
--rw-r--r--   0        0        0    18803 2024-03-12 19:34:27.267048 carbon_python_sdk-0.1.8/carbon/paths/delete_files/post.pyi
--rw-r--r--   0        0        0      313 2024-03-12 19:34:27.267183 carbon_python_sdk-0.1.8/carbon/paths/delete_user_file_tags/__init__.py
--rw-r--r--   0        0        0    15814 2024-03-12 19:34:27.267307 carbon_python_sdk-0.1.8/carbon/paths/delete_user_file_tags/post.py
--rw-r--r--   0        0        0    15640 2024-03-12 19:34:27.267549 carbon_python_sdk-0.1.8/carbon/paths/delete_user_file_tags/post.pyi
--rw-r--r--   0        0        0      295 2024-03-12 19:34:27.267805 carbon_python_sdk-0.1.8/carbon/paths/delete_users/__init__.py
--rw-r--r--   0        0        0    14904 2024-03-12 19:34:27.267906 carbon_python_sdk-0.1.8/carbon/paths/delete_users/post.py
--rw-r--r--   0        0        0    14762 2024-03-12 19:34:27.269438 carbon_python_sdk-0.1.8/carbon/paths/delete_users/post.pyi
--rw-r--r--   0        0        0      321 2024-03-12 19:34:27.270414 carbon_python_sdk-0.1.8/carbon/paths/delete_webhook_webhook_id/__init__.py
--rw-r--r--   0        0        0    14364 2024-03-12 19:34:27.270947 carbon_python_sdk-0.1.8/carbon/paths/delete_webhook_webhook_id/delete.py
--rw-r--r--   0        0        0    14222 2024-03-12 19:34:27.271713 carbon_python_sdk-0.1.8/carbon/paths/delete_webhook_webhook_id/delete.pyi
--rw-r--r--   0        0        0      307 2024-03-12 19:34:27.272171 carbon_python_sdk-0.1.8/carbon/paths/deletefile_file_id/__init__.py
--rw-r--r--   0        0        0    14552 2024-03-12 19:34:27.272406 carbon_python_sdk-0.1.8/carbon/paths/deletefile_file_id/delete.py
--rw-r--r--   0        0        0    14378 2024-03-12 19:34:27.272732 carbon_python_sdk-0.1.8/carbon/paths/deletefile_file_id/delete.pyi
--rw-r--r--   0        0        0      291 2024-03-12 19:34:27.273024 carbon_python_sdk-0.1.8/carbon/paths/embeddings/__init__.py
--rw-r--r--   0        0        0    28339 2024-03-12 19:34:27.273170 carbon_python_sdk-0.1.8/carbon/paths/embeddings/post.py
--rw-r--r--   0        0        0    28165 2024-03-12 19:34:27.273354 carbon_python_sdk-0.1.8/carbon/paths/embeddings/post.pyi
--rw-r--r--   0        0        0      291 2024-03-12 19:34:27.273503 carbon_python_sdk-0.1.8/carbon/paths/fetch_urls/__init__.py
--rw-r--r--   0        0        0    14466 2024-03-12 19:34:27.273611 carbon_python_sdk-0.1.8/carbon/paths/fetch_urls/get.py
--rw-r--r--   0        0        0    14292 2024-03-12 19:34:27.273916 carbon_python_sdk-0.1.8/carbon/paths/fetch_urls/get.pyi
--rw-r--r--   0        0        0      319 2024-03-12 19:34:27.274202 carbon_python_sdk-0.1.8/carbon/paths/fetch_youtube_transcript/__init__.py
--rw-r--r--   0        0        0    15695 2024-03-12 19:34:27.274339 carbon_python_sdk-0.1.8/carbon/paths/fetch_youtube_transcript/get.py
--rw-r--r--   0        0        0    15521 2024-03-12 19:34:27.274611 carbon_python_sdk-0.1.8/carbon/paths/fetch_youtube_transcript/get.pyi
--rw-r--r--   0        0        0      283 2024-03-12 19:34:27.274877 carbon_python_sdk-0.1.8/carbon/paths/health/__init__.py
--rw-r--r--   0        0        0    10429 2024-03-12 19:34:27.275004 carbon_python_sdk-0.1.8/carbon/paths/health/get.py
--rw-r--r--   0        0        0    10348 2024-03-12 19:34:27.275206 carbon_python_sdk-0.1.8/carbon/paths/health/get.pyi
--rw-r--r--   0        0        0      327 2024-03-12 19:34:27.275386 carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_list/__init__.py
--rw-r--r--   0        0        0    15289 2024-03-12 19:34:27.275509 carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_list/post.py
--rw-r--r--   0        0        0    15115 2024-03-12 19:34:27.275770 carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_list/post.pyi
--rw-r--r--   0        0        0      327 2024-03-12 19:34:27.276324 carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_sync/__init__.py
--rw-r--r--   0        0        0    24653 2024-03-12 19:34:27.276478 carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_sync/post.py
--rw-r--r--   0        0        0    24479 2024-03-12 19:34:27.276768 carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_sync/post.pyi
--rw-r--r--   0        0        0      317 2024-03-12 19:34:27.276980 carbon_python_sdk-0.1.8/carbon/paths/integrations_files_sync/__init__.py
--rw-r--r--   0        0        0    24538 2024-03-12 19:34:27.277150 carbon_python_sdk-0.1.8/carbon/paths/integrations_files_sync/post.py
--rw-r--r--   0        0        0    24364 2024-03-12 19:34:27.277329 carbon_python_sdk-0.1.8/carbon/paths/integrations_files_sync/post.pyi
--rw-r--r--   0        0        0      315 2024-03-12 19:34:27.277533 carbon_python_sdk-0.1.8/carbon/paths/integrations_freshdesk/__init__.py
--rw-r--r--   0        0        0    23357 2024-03-12 19:34:27.277658 carbon_python_sdk-0.1.8/carbon/paths/integrations_freshdesk/post.py
--rw-r--r--   0        0        0    23183 2024-03-12 19:34:27.277814 carbon_python_sdk-0.1.8/carbon/paths/integrations_freshdesk/post.pyi
--rw-r--r--   0        0        0      311 2024-03-12 19:34:27.277943 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook/__init__.py
--rw-r--r--   0        0        0    23400 2024-03-12 19:34:27.278071 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook/post.py
--rw-r--r--   0        0        0    23226 2024-03-12 19:34:27.278204 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook/post.pyi
--rw-r--r--   0        0        0      325 2024-03-12 19:34:27.278345 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_spaces/__init__.py
--rw-r--r--   0        0        0    14816 2024-03-12 19:34:27.278483 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_spaces/get.py
--rw-r--r--   0        0        0    14642 2024-03-12 19:34:27.278766 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_spaces/get.pyi
--rw-r--r--   0        0        0      321 2024-03-12 19:34:27.279026 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_sync/__init__.py
--rw-r--r--   0        0        0    22421 2024-03-12 19:34:27.279144 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_sync/post.py
--rw-r--r--   0        0        0    22247 2024-03-12 19:34:27.279353 carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_sync/post.pyi
--rw-r--r--   0        0        0      317 2024-03-12 19:34:27.279507 carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_sync/__init__.py
--rw-r--r--   0        0        0    22959 2024-03-12 19:34:27.279857 carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_sync/post.py
--rw-r--r--   0        0        0    22785 2024-03-12 19:34:27.280094 carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_sync/post.pyi
--rw-r--r--   0        0        0      331 2024-03-12 19:34:27.280245 carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_user_labels/__init__.py
--rw-r--r--   0        0        0    15340 2024-03-12 19:34:27.280379 carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_user_labels/get.py
--rw-r--r--   0        0        0    15166 2024-03-12 19:34:27.280658 carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_user_labels/get.pyi
--rw-r--r--   0        0        0      317 2024-03-12 19:34:27.280949 carbon_python_sdk-0.1.8/carbon/paths/integrations_items_list/__init__.py
--rw-r--r--   0        0        0    16639 2024-03-12 19:34:27.281096 carbon_python_sdk-0.1.8/carbon/paths/integrations_items_list/post.py
--rw-r--r--   0        0        0    16465 2024-03-12 19:34:27.281241 carbon_python_sdk-0.1.8/carbon/paths/integrations_items_list/post.pyi
--rw-r--r--   0        0        0      317 2024-03-12 19:34:27.281389 carbon_python_sdk-0.1.8/carbon/paths/integrations_items_sync/__init__.py
--rw-r--r--   0        0        0    14992 2024-03-12 19:34:27.281504 carbon_python_sdk-0.1.8/carbon/paths/integrations_items_sync/post.py
--rw-r--r--   0        0        0    14818 2024-03-12 19:34:27.281782 carbon_python_sdk-0.1.8/carbon/paths/integrations_items_sync/post.pyi
--rw-r--r--   0        0        0      315 2024-03-12 19:34:27.282964 carbon_python_sdk-0.1.8/carbon/paths/integrations_oauth_url/__init__.py
--rw-r--r--   0        0        0    31689 2024-03-12 19:34:27.283267 carbon_python_sdk-0.1.8/carbon/paths/integrations_oauth_url/post.py
--rw-r--r--   0        0        0    31515 2024-03-12 19:34:27.283736 carbon_python_sdk-0.1.8/carbon/paths/integrations_oauth_url/post.pyi
--rw-r--r--   0        0        0      321 2024-03-12 19:34:27.284096 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_sync/__init__.py
--rw-r--r--   0        0        0    23693 2024-03-12 19:34:27.284589 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_sync/post.py
--rw-r--r--   0        0        0    23519 2024-03-12 19:34:27.285000 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_sync/post.pyi
--rw-r--r--   0        0        0      343 2024-03-12 19:34:27.285673 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_categories/__init__.py
--rw-r--r--   0        0        0    15590 2024-03-12 19:34:27.285886 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_categories/get.py
--rw-r--r--   0        0        0    15416 2024-03-12 19:34:27.286200 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_categories/get.pyi
--rw-r--r--   0        0        0      337 2024-03-12 19:34:27.286491 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_folders/__init__.py
--rw-r--r--   0        0        0    15371 2024-03-12 19:34:27.286627 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_folders/get.py
--rw-r--r--   0        0        0    15197 2024-03-12 19:34:27.287342 carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_folders/get.pyi
--rw-r--r--   0        0        0      313 2024-03-12 19:34:27.288509 carbon_python_sdk-0.1.8/carbon/paths/integrations_rss_feed/__init__.py
--rw-r--r--   0        0        0    21466 2024-03-12 19:34:27.288949 carbon_python_sdk-0.1.8/carbon/paths/integrations_rss_feed/post.py
--rw-r--r--   0        0        0    21292 2024-03-12 19:34:27.289167 carbon_python_sdk-0.1.8/carbon/paths/integrations_rss_feed/post.pyi
--rw-r--r--   0        0        0      301 2024-03-12 19:34:27.289301 carbon_python_sdk-0.1.8/carbon/paths/integrations_s3/__init__.py
--rw-r--r--   0        0        0    15336 2024-03-12 19:34:27.289408 carbon_python_sdk-0.1.8/carbon/paths/integrations_s3/post.py
--rw-r--r--   0        0        0    15162 2024-03-12 19:34:27.289709 carbon_python_sdk-0.1.8/carbon/paths/integrations_s3/post.pyi
--rw-r--r--   0        0        0      313 2024-03-12 19:34:27.289990 carbon_python_sdk-0.1.8/carbon/paths/integrations_s3_files/__init__.py
--rw-r--r--   0        0        0    24552 2024-03-12 19:34:27.290109 carbon_python_sdk-0.1.8/carbon/paths/integrations_s3_files/post.py
--rw-r--r--   0        0        0    24378 2024-03-12 19:34:27.290256 carbon_python_sdk-0.1.8/carbon/paths/integrations_s3_files/post.pyi
--rw-r--r--   0        0        0      321 2024-03-12 19:34:27.290379 carbon_python_sdk-0.1.8/carbon/paths/modify_user_configuration/__init__.py
--rw-r--r--   0        0        0    16052 2024-03-12 19:34:27.290488 carbon_python_sdk-0.1.8/carbon/paths/modify_user_configuration/post.py
--rw-r--r--   0        0        0    15878 2024-03-12 19:34:27.290788 carbon_python_sdk-0.1.8/carbon/paths/modify_user_configuration/post.pyi
--rw-r--r--   0        0        0      295 2024-03-12 19:34:27.291059 carbon_python_sdk-0.1.8/carbon/paths/organization/__init__.py
--rw-r--r--   0        0        0    11658 2024-03-12 19:34:27.291244 carbon_python_sdk-0.1.8/carbon/paths/organization/get.py
--rw-r--r--   0        0        0    11516 2024-03-12 19:34:27.291566 carbon_python_sdk-0.1.8/carbon/paths/organization/get.pyi
--rw-r--r--   0        0        0      309 2024-03-12 19:34:27.291809 carbon_python_sdk-0.1.8/carbon/paths/parsed_file_file_id/__init__.py
--rw-r--r--   0        0        0    14654 2024-03-12 19:34:27.291952 carbon_python_sdk-0.1.8/carbon/paths/parsed_file_file_id/get.py
--rw-r--r--   0        0        0    14480 2024-03-12 19:34:27.292268 carbon_python_sdk-0.1.8/carbon/paths/parsed_file_file_id/get.pyi
--rw-r--r--   0        0        0      301 2024-03-12 19:34:27.292566 carbon_python_sdk-0.1.8/carbon/paths/process_sitemap/__init__.py
--rw-r--r--   0        0        0    14363 2024-03-12 19:34:27.292676 carbon_python_sdk-0.1.8/carbon/paths/process_sitemap/get.py
--rw-r--r--   0        0        0    14189 2024-03-12 19:34:27.292983 carbon_python_sdk-0.1.8/carbon/paths/process_sitemap/get.pyi
--rw-r--r--   0        0        0      303 2024-03-12 19:34:27.293312 carbon_python_sdk-0.1.8/carbon/paths/raw_file_file_id/__init__.py
--rw-r--r--   0        0        0    14585 2024-03-12 19:34:27.293448 carbon_python_sdk-0.1.8/carbon/paths/raw_file_file_id/get.py
--rw-r--r--   0        0        0    14411 2024-03-12 19:34:27.294459 carbon_python_sdk-0.1.8/carbon/paths/raw_file_file_id/get.pyi
--rw-r--r--   0        0        0      293 2024-03-12 19:34:27.295159 carbon_python_sdk-0.1.8/carbon/paths/resync_file/__init__.py
--rw-r--r--   0        0        0    16696 2024-03-12 19:34:27.295412 carbon_python_sdk-0.1.8/carbon/paths/resync_file/post.py
--rw-r--r--   0        0        0    16522 2024-03-12 19:34:27.297044 carbon_python_sdk-0.1.8/carbon/paths/resync_file/post.pyi
--rw-r--r--   0        0        0      309 2024-03-12 19:34:27.297301 carbon_python_sdk-0.1.8/carbon/paths/revoke_access_token/__init__.py
--rw-r--r--   0        0        0    14828 2024-03-12 19:34:27.297425 carbon_python_sdk-0.1.8/carbon/paths/revoke_access_token/post.py
--rw-r--r--   0        0        0    14654 2024-03-12 19:34:27.297693 carbon_python_sdk-0.1.8/carbon/paths/revoke_access_token/post.pyi
--rw-r--r--   0        0        0      299 2024-03-12 19:34:27.298047 carbon_python_sdk-0.1.8/carbon/paths/scrape_sitemap/__init__.py
--rw-r--r--   0        0        0    27300 2024-03-12 19:34:27.298238 carbon_python_sdk-0.1.8/carbon/paths/scrape_sitemap/post.py
--rw-r--r--   0        0        0    27126 2024-03-12 19:34:27.298445 carbon_python_sdk-0.1.8/carbon/paths/scrape_sitemap/post.pyi
--rw-r--r--   0        0        0      293 2024-03-12 19:34:27.298658 carbon_python_sdk-0.1.8/carbon/paths/search_urls/__init__.py
--rw-r--r--   0        0        0    14549 2024-03-12 19:34:27.298782 carbon_python_sdk-0.1.8/carbon/paths/search_urls/get.py
--rw-r--r--   0        0        0    14375 2024-03-12 19:34:27.299095 carbon_python_sdk-0.1.8/carbon/paths/search_urls/get.pyi
--rw-r--r--   0        0        0      293 2024-03-12 19:34:27.299486 carbon_python_sdk-0.1.8/carbon/paths/text_chunks/__init__.py
--rw-r--r--   0        0        0    19073 2024-03-12 19:34:27.299811 carbon_python_sdk-0.1.8/carbon/paths/text_chunks/post.py
--rw-r--r--   0        0        0    18899 2024-03-12 19:34:27.300102 carbon_python_sdk-0.1.8/carbon/paths/text_chunks/post.pyi
--rw-r--r--   0        0        0      327 2024-03-12 19:34:27.300546 carbon_python_sdk-0.1.8/carbon/paths/upload_chunks_and_embeddings/__init__.py
--rw-r--r--   0        0        0    19841 2024-03-12 19:34:27.303063 carbon_python_sdk-0.1.8/carbon/paths/upload_chunks_and_embeddings/post.py
--rw-r--r--   0        0        0    19667 2024-03-12 19:34:27.303544 carbon_python_sdk-0.1.8/carbon/paths/upload_chunks_and_embeddings/post.pyi
--rw-r--r--   0        0        0      311 2024-03-12 19:34:27.303844 carbon_python_sdk-0.1.8/carbon/paths/upload_file_from_url/__init__.py
--rw-r--r--   0        0        0    23090 2024-03-12 19:34:27.304215 carbon_python_sdk-0.1.8/carbon/paths/upload_file_from_url/post.py
--rw-r--r--   0        0        0    22916 2024-03-12 19:34:27.304701 carbon_python_sdk-0.1.8/carbon/paths/upload_file_from_url/post.pyi
--rw-r--r--   0        0        0      293 2024-03-12 19:34:27.305421 carbon_python_sdk-0.1.8/carbon/paths/upload_text/__init__.py
--rw-r--r--   0        0        0    20504 2024-03-12 19:34:27.305766 carbon_python_sdk-0.1.8/carbon/paths/upload_text/post.py
--rw-r--r--   0        0        0    20330 2024-03-12 19:34:27.306068 carbon_python_sdk-0.1.8/carbon/paths/upload_text/post.pyi
--rw-r--r--   0        0        0      291 2024-03-12 19:34:27.306337 carbon_python_sdk-0.1.8/carbon/paths/uploadfile/__init__.py
--rw-r--r--   0        0        0    29353 2024-03-12 19:34:27.309273 carbon_python_sdk-0.1.8/carbon/paths/uploadfile/post.py
--rw-r--r--   0        0        0    29179 2024-03-12 19:34:27.309838 carbon_python_sdk-0.1.8/carbon/paths/uploadfile/post.pyi
--rw-r--r--   0        0        0      279 2024-03-12 19:34:27.311432 carbon_python_sdk-0.1.8/carbon/paths/user/__init__.py
--rw-r--r--   0        0        0    14161 2024-03-12 19:34:27.313080 carbon_python_sdk-0.1.8/carbon/paths/user/post.py
--rw-r--r--   0        0        0    14019 2024-03-12 19:34:27.313444 carbon_python_sdk-0.1.8/carbon/paths/user/post.pyi
--rw-r--r--   0        0        0      305 2024-03-12 19:34:27.313763 carbon_python_sdk-0.1.8/carbon/paths/user_data_sources/__init__.py
--rw-r--r--   0        0        0    18865 2024-03-12 19:34:27.314134 carbon_python_sdk-0.1.8/carbon/paths/user_data_sources/post.py
--rw-r--r--   0        0        0    18691 2024-03-12 19:34:27.314370 carbon_python_sdk-0.1.8/carbon/paths/user_data_sources/post.pyi
--rw-r--r--   0        0        0      291 2024-03-12 19:34:27.314571 carbon_python_sdk-0.1.8/carbon/paths/user_files/__init__.py
--rw-r--r--   0        0        0    22374 2024-03-12 19:34:27.314737 carbon_python_sdk-0.1.8/carbon/paths/user_files/post.py
--rw-r--r--   0        0        0    22200 2024-03-12 19:34:27.314926 carbon_python_sdk-0.1.8/carbon/paths/user_files/post.pyi
--rw-r--r--   0        0        0      297 2024-03-12 19:34:27.315103 carbon_python_sdk-0.1.8/carbon/paths/user_files_v2/__init__.py
--rw-r--r--   0        0        0    21370 2024-03-12 19:34:27.315251 carbon_python_sdk-0.1.8/carbon/paths/user_files_v2/post.py
--rw-r--r--   0        0        0    21196 2024-03-12 19:34:27.315598 carbon_python_sdk-0.1.8/carbon/paths/user_files_v2/post.pyi
--rw-r--r--   0        0        0      291 2024-03-12 19:34:27.315971 carbon_python_sdk-0.1.8/carbon/paths/web_scrape/__init__.py
--rw-r--r--   0        0        0    14274 2024-03-12 19:34:27.316221 carbon_python_sdk-0.1.8/carbon/paths/web_scrape/post.py
--rw-r--r--   0        0        0    14100 2024-03-12 19:34:27.316547 carbon_python_sdk-0.1.8/carbon/paths/web_scrape/post.pyi
--rw-r--r--   0        0        0      287 2024-03-12 19:34:27.317107 carbon_python_sdk-0.1.8/carbon/paths/webhooks/__init__.py
--rw-r--r--   0        0        0    17372 2024-03-12 19:34:27.319581 carbon_python_sdk-0.1.8/carbon/paths/webhooks/post.py
--rw-r--r--   0        0        0    17230 2024-03-12 19:34:27.320150 carbon_python_sdk-0.1.8/carbon/paths/webhooks/post.pyi
--rw-r--r--   0        0        0        0 2024-03-12 19:34:27.320499 carbon_python_sdk-0.1.8/carbon/pydantic/__init__.py
--rw-r--r--   0        0        0      496 2024-03-12 19:34:27.320704 carbon_python_sdk-0.1.8/carbon/pydantic/add_webhook_props.py
--rw-r--r--   0        0        0      523 2024-03-12 19:34:27.320834 carbon_python_sdk-0.1.8/carbon/pydantic/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0      697 2024-03-12 19:34:27.320939 carbon_python_sdk-0.1.8/carbon/pydantic/chunk_properties.py
--rw-r--r--   0        0        0      705 2024-03-12 19:34:27.321051 carbon_python_sdk-0.1.8/carbon/pydantic/chunk_properties_nullable.py
--rw-r--r--   0        0        0      758 2024-03-12 19:34:27.321161 carbon_python_sdk-0.1.8/carbon/pydantic/chunks_and_embeddings.py
--rw-r--r--   0        0        0      457 2024-03-12 19:34:27.321305 carbon_python_sdk-0.1.8/carbon/pydantic/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1180 2024-03-12 19:34:27.321560 carbon_python_sdk-0.1.8/carbon/pydantic/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0      406 2024-03-12 19:34:27.321969 carbon_python_sdk-0.1.8/carbon/pydantic/configuration_keys.py
--rw-r--r--   0        0        0      444 2024-03-12 19:34:27.322721 carbon_python_sdk-0.1.8/carbon/pydantic/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      460 2024-03-12 19:34:27.322863 carbon_python_sdk-0.1.8/carbon/pydantic/data_source_sync_statuses.py
--rw-r--r--   0        0        0      802 2024-03-12 19:34:27.322975 carbon_python_sdk-0.1.8/carbon/pydantic/data_source_type.py
--rw-r--r--   0        0        0      810 2024-03-12 19:34:27.323100 carbon_python_sdk-0.1.8/carbon/pydantic/data_source_type_nullable.py
--rw-r--r--   0        0        0     1124 2024-03-12 19:34:27.323211 carbon_python_sdk-0.1.8/carbon/pydantic/delete_files_query_input.py
--rw-r--r--   0        0        0      436 2024-03-12 19:34:27.323324 carbon_python_sdk-0.1.8/carbon/pydantic/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0      627 2024-03-12 19:34:27.323420 carbon_python_sdk-0.1.8/carbon/pydantic/delete_users_input.py
--rw-r--r--   0        0        0      418 2024-03-12 19:34:27.323515 carbon_python_sdk-0.1.8/carbon/pydantic/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0      631 2024-03-12 19:34:27.323632 carbon_python_sdk-0.1.8/carbon/pydantic/directory_item.py
--rw-r--r--   0        0        0     1469 2024-03-12 19:34:27.323742 carbon_python_sdk-0.1.8/carbon/pydantic/document_response.py
--rw-r--r--   0        0        0      602 2024-03-12 19:34:27.323845 carbon_python_sdk-0.1.8/carbon/pydantic/document_response_list.py
--rw-r--r--   0        0        0      399 2024-03-12 19:34:27.323958 carbon_python_sdk-0.1.8/carbon/pydantic/document_response_tags.py
--rw-r--r--   0        0        0      451 2024-03-12 19:34:27.324087 carbon_python_sdk-0.1.8/carbon/pydantic/document_response_vector.py
--rw-r--r--   0        0        0      796 2024-03-12 19:34:27.324199 carbon_python_sdk-0.1.8/carbon/pydantic/embedding_and_chunk.py
--rw-r--r--   0        0        0      455 2024-03-12 19:34:27.324347 carbon_python_sdk-0.1.8/carbon/pydantic/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0      715 2024-03-12 19:34:27.324457 carbon_python_sdk-0.1.8/carbon/pydantic/embedding_generators.py
--rw-r--r--   0        0        0      723 2024-03-12 19:34:27.324567 carbon_python_sdk-0.1.8/carbon/pydantic/embedding_generators_nullable.py
--rw-r--r--   0        0        0      603 2024-03-12 19:34:27.324678 carbon_python_sdk-0.1.8/carbon/pydantic/embedding_properties.py
--rw-r--r--   0        0        0      717 2024-03-12 19:34:27.324779 carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0      458 2024-03-12 19:34:27.324885 carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0     1159 2024-03-12 19:34:27.324999 carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0      648 2024-03-12 19:34:27.325112 carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0      541 2024-03-12 19:34:27.325225 carbon_python_sdk-0.1.8/carbon/pydantic/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1647 2024-03-12 19:34:27.325326 carbon_python_sdk-0.1.8/carbon/pydantic/external_source_item.py
--rw-r--r--   0        0        0      646 2024-03-12 19:34:27.325426 carbon_python_sdk-0.1.8/carbon/pydantic/fetch_urls_response.py
--rw-r--r--   0        0        0      412 2024-03-12 19:34:27.325538 carbon_python_sdk-0.1.8/carbon/pydantic/fetch_urls_response_urls.py
--rw-r--r--   0        0        0      415 2024-03-12 19:34:27.325671 carbon_python_sdk-0.1.8/carbon/pydantic/file_content_types.py
--rw-r--r--   0        0        0      423 2024-03-12 19:34:27.325798 carbon_python_sdk-0.1.8/carbon/pydantic/file_content_types_nullable.py
--rw-r--r--   0        0        0      740 2024-03-12 19:34:27.325916 carbon_python_sdk-0.1.8/carbon/pydantic/file_formats.py
--rw-r--r--   0        0        0      748 2024-03-12 19:34:27.326056 carbon_python_sdk-0.1.8/carbon/pydantic/file_formats_nullable.py
--rw-r--r--   0        0        0      875 2024-03-12 19:34:27.326255 carbon_python_sdk-0.1.8/carbon/pydantic/file_statistics.py
--rw-r--r--   0        0        0      883 2024-03-12 19:34:27.328275 carbon_python_sdk-0.1.8/carbon/pydantic/file_statistics_nullable.py
--rw-r--r--   0        0        0      480 2024-03-12 19:34:27.328465 carbon_python_sdk-0.1.8/carbon/pydantic/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1566 2024-03-12 19:34:27.328913 carbon_python_sdk-0.1.8/carbon/pydantic/fresh_desk_connect_request.py
--rw-r--r--   0        0        0      512 2024-03-12 19:34:27.329032 carbon_python_sdk-0.1.8/carbon/pydantic/generic_success_response.py
--rw-r--r--   0        0        0     3076 2024-03-12 19:34:27.329220 carbon_python_sdk-0.1.8/carbon/pydantic/get_embedding_documents_body.py
--rw-r--r--   0        0        0      440 2024-03-12 19:34:27.329367 carbon_python_sdk-0.1.8/carbon/pydantic/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0      446 2024-03-12 19:34:27.329496 carbon_python_sdk-0.1.8/carbon/pydantic/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0      465 2024-03-12 19:34:27.329634 carbon_python_sdk-0.1.8/carbon/pydantic/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0      408 2024-03-12 19:34:27.329776 carbon_python_sdk-0.1.8/carbon/pydantic/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0     1561 2024-03-12 19:34:27.329914 carbon_python_sdk-0.1.8/carbon/pydantic/gitbook_connect_request.py
--rw-r--r--   0        0        0     1547 2024-03-12 19:34:27.330038 carbon_python_sdk-0.1.8/carbon/pydantic/gitbook_sync_request.py
--rw-r--r--   0        0        0      417 2024-03-12 19:34:27.330168 carbon_python_sdk-0.1.8/carbon/pydantic/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0     1554 2024-03-12 19:34:27.330347 carbon_python_sdk-0.1.8/carbon/pydantic/gmail_sync_input.py
--rw-r--r--   0        0        0      615 2024-03-12 19:34:27.330733 carbon_python_sdk-0.1.8/carbon/pydantic/http_validation_error.py
--rw-r--r--   0        0        0      602 2024-03-12 19:34:27.330909 carbon_python_sdk-0.1.8/carbon/pydantic/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0      610 2024-03-12 19:34:27.331042 carbon_python_sdk-0.1.8/carbon/pydantic/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0      745 2024-03-12 19:34:27.331174 carbon_python_sdk-0.1.8/carbon/pydantic/list_data_source_items_request.py
--rw-r--r--   0        0        0      647 2024-03-12 19:34:27.331302 carbon_python_sdk-0.1.8/carbon/pydantic/list_data_source_items_response.py
--rw-r--r--   0        0        0      601 2024-03-12 19:34:27.331423 carbon_python_sdk-0.1.8/carbon/pydantic/list_request.py
--rw-r--r--   0        0        0      575 2024-03-12 19:34:27.331546 carbon_python_sdk-0.1.8/carbon/pydantic/list_response.py
--rw-r--r--   0        0        0      670 2024-03-12 19:34:27.331668 carbon_python_sdk-0.1.8/carbon/pydantic/modify_user_configuration_input.py
--rw-r--r--   0        0        0     3224 2024-03-12 19:34:27.331809 carbon_python_sdk-0.1.8/carbon/pydantic/o_auth_url_request.py
--rw-r--r--   0        0        0      405 2024-03-12 19:34:27.331944 carbon_python_sdk-0.1.8/carbon/pydantic/order_dir.py
--rw-r--r--   0        0        0     1874 2024-03-12 19:34:27.332080 carbon_python_sdk-0.1.8/carbon/pydantic/organization_response.py
--rw-r--r--   0        0        0     1584 2024-03-12 19:34:27.332206 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_api.py
--rw-r--r--   0        0        0      935 2024-03-12 19:34:27.332326 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_filters.py
--rw-r--r--   0        0        0      444 2024-03-12 19:34:27.332457 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0      450 2024-03-12 19:34:27.332587 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0     1150 2024-03-12 19:34:27.332707 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0      693 2024-03-12 19:34:27.332848 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_response.py
--rw-r--r--   0        0        0      722 2024-03-12 19:34:27.332986 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_file_tag_create.py
--rw-r--r--   0        0        0      412 2024-03-12 19:34:27.333098 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0      726 2024-03-12 19:34:27.333214 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0      425 2024-03-12 19:34:27.333331 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     2693 2024-03-12 19:34:27.333457 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0      457 2024-03-12 19:34:27.333582 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0      445 2024-03-12 19:34:27.333689 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0      470 2024-03-12 19:34:27.333828 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0      455 2024-03-12 19:34:27.333969 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0      417 2024-03-12 19:34:27.334095 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0      483 2024-03-12 19:34:27.334204 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1491 2024-03-12 19:34:27.334319 carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0      508 2024-03-12 19:34:27.334446 carbon_python_sdk-0.1.8/carbon/pydantic/outh_url_response.py
--rw-r--r--   0        0        0     1637 2024-03-12 19:34:27.334562 carbon_python_sdk-0.1.8/carbon/pydantic/outlook_sync_input.py
--rw-r--r--   0        0        0      582 2024-03-12 19:34:27.334679 carbon_python_sdk-0.1.8/carbon/pydantic/pagination.py
--rw-r--r--   0        0        0      521 2024-03-12 19:34:27.334796 carbon_python_sdk-0.1.8/carbon/pydantic/presigned_url_response.py
--rw-r--r--   0        0        0     1278 2024-03-12 19:34:27.334913 carbon_python_sdk-0.1.8/carbon/pydantic/raw_text_input.py
--rw-r--r--   0        0        0      798 2024-03-12 19:34:27.335048 carbon_python_sdk-0.1.8/carbon/pydantic/resync_file_query_input.py
--rw-r--r--   0        0        0      525 2024-03-12 19:34:27.335166 carbon_python_sdk-0.1.8/carbon/pydantic/revoke_access_token_input.py
--rw-r--r--   0        0        0     1363 2024-03-12 19:34:27.335285 carbon_python_sdk-0.1.8/carbon/pydantic/rss_feed_input.py
--rw-r--r--   0        0        0      571 2024-03-12 19:34:27.335392 carbon_python_sdk-0.1.8/carbon/pydantic/s3_auth_request.py
--rw-r--r--   0        0        0     1748 2024-03-12 19:34:27.335497 carbon_python_sdk-0.1.8/carbon/pydantic/s3_file_sync_input.py
--rw-r--r--   0        0        0      614 2024-03-12 19:34:27.335608 carbon_python_sdk-0.1.8/carbon/pydantic/s3_get_file_input.py
--rw-r--r--   0        0        0      879 2024-03-12 19:34:27.335728 carbon_python_sdk-0.1.8/carbon/pydantic/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     2274 2024-03-12 19:34:27.335830 carbon_python_sdk-0.1.8/carbon/pydantic/sitemap_scrape_request.py
--rw-r--r--   0        0        0      444 2024-03-12 19:34:27.335944 carbon_python_sdk-0.1.8/carbon/pydantic/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      446 2024-03-12 19:34:27.336074 carbon_python_sdk-0.1.8/carbon/pydantic/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      442 2024-03-12 19:34:27.336202 carbon_python_sdk-0.1.8/carbon/pydantic/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      403 2024-03-12 19:34:27.336305 carbon_python_sdk-0.1.8/carbon/pydantic/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0      523 2024-03-12 19:34:27.336408 carbon_python_sdk-0.1.8/carbon/pydantic/sync_directory_request.py
--rw-r--r--   0        0        0      534 2024-03-12 19:34:27.336507 carbon_python_sdk-0.1.8/carbon/pydantic/sync_files_ids.py
--rw-r--r--   0        0        0     1759 2024-03-12 19:34:27.336622 carbon_python_sdk-0.1.8/carbon/pydantic/sync_files_request.py
--rw-r--r--   0        0        0      580 2024-03-12 19:34:27.336730 carbon_python_sdk-0.1.8/carbon/pydantic/text_embedding_generators.py
--rw-r--r--   0        0        0      567 2024-03-12 19:34:27.336871 carbon_python_sdk-0.1.8/carbon/pydantic/token_response.py
--rw-r--r--   0        0        0     1525 2024-03-12 19:34:27.336983 carbon_python_sdk-0.1.8/carbon/pydantic/upload_file_from_url_input.py
--rw-r--r--   0        0        0     3106 2024-03-12 19:34:27.337101 carbon_python_sdk-0.1.8/carbon/pydantic/user_file.py
--rw-r--r--   0        0        0      475 2024-03-12 19:34:27.337229 carbon_python_sdk-0.1.8/carbon/pydantic/user_file_embedding_properties.py
--rw-r--r--   0        0        0      604 2024-03-12 19:34:27.337571 carbon_python_sdk-0.1.8/carbon/pydantic/user_files_v2.py
--rw-r--r--   0        0        0      515 2024-03-12 19:34:27.338455 carbon_python_sdk-0.1.8/carbon/pydantic/user_request_content.py
--rw-r--r--   0        0        0     1343 2024-03-12 19:34:27.338714 carbon_python_sdk-0.1.8/carbon/pydantic/user_response.py
--rw-r--r--   0        0        0      420 2024-03-12 19:34:27.338848 carbon_python_sdk-0.1.8/carbon/pydantic/user_response_unique_file_tags.py
--rw-r--r--   0        0        0      492 2024-03-12 19:34:27.338978 carbon_python_sdk-0.1.8/carbon/pydantic/utilities_scrape_web_request.py
--rw-r--r--   0        0        0      651 2024-03-12 19:34:27.339165 carbon_python_sdk-0.1.8/carbon/pydantic/validation_error.py
--rw-r--r--   0        0        0      454 2024-03-12 19:34:27.339550 carbon_python_sdk-0.1.8/carbon/pydantic/validation_error_loc.py
--rw-r--r--   0        0        0      739 2024-03-12 19:34:27.339965 carbon_python_sdk-0.1.8/carbon/pydantic/webhook.py
--rw-r--r--   0        0        0      598 2024-03-12 19:34:27.340242 carbon_python_sdk-0.1.8/carbon/pydantic/webhook_filters.py
--rw-r--r--   0        0        0      425 2024-03-12 19:34:27.340415 carbon_python_sdk-0.1.8/carbon/pydantic/webhook_filters_ids.py
--rw-r--r--   0        0        0      693 2024-03-12 19:34:27.340527 carbon_python_sdk-0.1.8/carbon/pydantic/webhook_no_key.py
--rw-r--r--   0        0        0      431 2024-03-12 19:34:27.340653 carbon_python_sdk-0.1.8/carbon/pydantic/webhook_order_by_columns.py
--rw-r--r--   0        0        0     1011 2024-03-12 19:34:27.340912 carbon_python_sdk-0.1.8/carbon/pydantic/webhook_query_input.py
--rw-r--r--   0        0        0      626 2024-03-12 19:34:27.341292 carbon_python_sdk-0.1.8/carbon/pydantic/webhook_query_response.py
--rw-r--r--   0        0        0     2317 2024-03-12 19:34:27.341650 carbon_python_sdk-0.1.8/carbon/pydantic/webscrape_request.py
--rw-r--r--   0        0        0      440 2024-03-12 19:34:27.341847 carbon_python_sdk-0.1.8/carbon/pydantic/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      442 2024-03-12 19:34:27.342019 carbon_python_sdk-0.1.8/carbon/pydantic/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      438 2024-03-12 19:34:27.342147 carbon_python_sdk-0.1.8/carbon/pydantic/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      399 2024-03-12 19:34:27.342259 carbon_python_sdk-0.1.8/carbon/pydantic/webscrape_request_tags.py
--rw-r--r--   0        0        0      664 2024-03-12 19:34:27.342379 carbon_python_sdk-0.1.8/carbon/pydantic/white_labeling_response.py
--rw-r--r--   0        0        0      824 2024-03-12 19:34:27.342500 carbon_python_sdk-0.1.8/carbon/pydantic/youtube_transcript_response.py
--rw-r--r--   0        0        0      604 2024-03-12 19:34:27.342623 carbon_python_sdk-0.1.8/carbon/pydantic/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0      421 2024-03-12 19:34:27.342728 carbon_python_sdk-0.1.8/carbon/pydantic/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0      654 2024-03-12 19:34:27.342853 carbon_python_sdk-0.1.8/carbon/request_after_hook.py
--rw-r--r--   0        0        0      712 2024-03-12 19:34:27.343455 carbon_python_sdk-0.1.8/carbon/request_before_hook.py
--rw-r--r--   0        0        0      677 2024-03-12 19:34:27.343616 carbon_python_sdk-0.1.8/carbon/request_before_url_hook.py
--rw-r--r--   0        0        0    10974 2024-03-12 19:34:27.343748 carbon_python_sdk-0.1.8/carbon/rest.py
--rw-r--r--   0        0        0    96042 2024-03-12 19:34:27.344112 carbon_python_sdk-0.1.8/carbon/schemas.py
--rw-r--r--   0        0        0        0 2024-03-12 19:34:27.345168 carbon_python_sdk-0.1.8/carbon/type/__init__.py
--rw-r--r--   0        0        0      525 2024-03-12 19:34:27.345332 carbon_python_sdk-0.1.8/carbon/type/add_webhook_props.py
--rw-r--r--   0        0        0      627 2024-03-12 19:34:27.345452 carbon_python_sdk-0.1.8/carbon/type/body_create_upload_file_uploadfile_post.py
--rw-r--r--   0        0        0      628 2024-03-12 19:34:27.345566 carbon_python_sdk-0.1.8/carbon/type/chunk_properties.py
--rw-r--r--   0        0        0      668 2024-03-12 19:34:27.345811 carbon_python_sdk-0.1.8/carbon/type/chunk_properties_nullable.py
--rw-r--r--   0        0        0      707 2024-03-12 19:34:27.345981 carbon_python_sdk-0.1.8/carbon/type/chunks_and_embeddings.py
--rw-r--r--   0        0        0      408 2024-03-12 19:34:27.346102 carbon_python_sdk-0.1.8/carbon/type/chunks_and_embeddings_embedding.py
--rw-r--r--   0        0        0     1030 2024-03-12 19:34:27.346213 carbon_python_sdk-0.1.8/carbon/type/chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0      322 2024-03-12 19:34:27.346325 carbon_python_sdk-0.1.8/carbon/type/configuration_keys.py
--rw-r--r--   0        0        0      395 2024-03-12 19:34:27.346436 carbon_python_sdk-0.1.8/carbon/type/data_source_last_sync_actions.py
--rw-r--r--   0        0        0      411 2024-03-12 19:34:27.346538 carbon_python_sdk-0.1.8/carbon/type/data_source_sync_statuses.py
--rw-r--r--   0        0        0      753 2024-03-12 19:34:27.346638 carbon_python_sdk-0.1.8/carbon/type/data_source_type.py
--rw-r--r--   0        0        0      761 2024-03-12 19:34:27.346737 carbon_python_sdk-0.1.8/carbon/type/data_source_type_nullable.py
--rw-r--r--   0        0        0      912 2024-03-12 19:34:27.346853 carbon_python_sdk-0.1.8/carbon/type/delete_files_query_input.py
--rw-r--r--   0        0        0      387 2024-03-12 19:34:27.346958 carbon_python_sdk-0.1.8/carbon/type/delete_files_query_input_file_ids.py
--rw-r--r--   0        0        0      647 2024-03-12 19:34:27.347056 carbon_python_sdk-0.1.8/carbon/type/delete_users_input.py
--rw-r--r--   0        0        0      369 2024-03-12 19:34:27.347159 carbon_python_sdk-0.1.8/carbon/type/delete_users_input_customer_ids.py
--rw-r--r--   0        0        0      574 2024-03-12 19:34:27.347267 carbon_python_sdk-0.1.8/carbon/type/directory_item.py
--rw-r--r--   0        0        0     1224 2024-03-12 19:34:27.347375 carbon_python_sdk-0.1.8/carbon/type/document_response.py
--rw-r--r--   0        0        0      641 2024-03-12 19:34:27.347501 carbon_python_sdk-0.1.8/carbon/type/document_response_list.py
--rw-r--r--   0        0        0      350 2024-03-12 19:34:27.347610 carbon_python_sdk-0.1.8/carbon/type/document_response_tags.py
--rw-r--r--   0        0        0      402 2024-03-12 19:34:27.347714 carbon_python_sdk-0.1.8/carbon/type/document_response_vector.py
--rw-r--r--   0        0        0      732 2024-03-12 19:34:27.347831 carbon_python_sdk-0.1.8/carbon/type/embedding_and_chunk.py
--rw-r--r--   0        0        0      406 2024-03-12 19:34:27.347945 carbon_python_sdk-0.1.8/carbon/type/embedding_and_chunk_embedding.py
--rw-r--r--   0        0        0      666 2024-03-12 19:34:27.348043 carbon_python_sdk-0.1.8/carbon/type/embedding_generators.py
--rw-r--r--   0        0        0      674 2024-03-12 19:34:27.348133 carbon_python_sdk-0.1.8/carbon/type/embedding_generators_nullable.py
--rw-r--r--   0        0        0      610 2024-03-12 19:34:27.348225 carbon_python_sdk-0.1.8/carbon/type/embedding_properties.py
--rw-r--r--   0        0        0      711 2024-03-12 19:34:27.348331 carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_filters.py
--rw-r--r--   0        0        0      409 2024-03-12 19:34:27.348431 carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_order_by_columns.py
--rw-r--r--   0        0        0     1008 2024-03-12 19:34:27.348528 carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_query_input.py
--rw-r--r--   0        0        0      694 2024-03-12 19:34:27.348618 carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_response.py
--rw-r--r--   0        0        0      492 2024-03-12 19:34:27.348709 carbon_python_sdk-0.1.8/carbon/type/external_file_sync_statuses.py
--rw-r--r--   0        0        0     1149 2024-03-12 19:34:27.348805 carbon_python_sdk-0.1.8/carbon/type/external_source_item.py
--rw-r--r--   0        0        0      648 2024-03-12 19:34:27.348896 carbon_python_sdk-0.1.8/carbon/type/fetch_urls_response.py
--rw-r--r--   0        0        0      363 2024-03-12 19:34:27.348988 carbon_python_sdk-0.1.8/carbon/type/fetch_urls_response_urls.py
--rw-r--r--   0        0        0      366 2024-03-12 19:34:27.349101 carbon_python_sdk-0.1.8/carbon/type/file_content_types.py
--rw-r--r--   0        0        0      374 2024-03-12 19:34:27.349215 carbon_python_sdk-0.1.8/carbon/type/file_content_types_nullable.py
--rw-r--r--   0        0        0      691 2024-03-12 19:34:27.349317 carbon_python_sdk-0.1.8/carbon/type/file_formats.py
--rw-r--r--   0        0        0      699 2024-03-12 19:34:27.349421 carbon_python_sdk-0.1.8/carbon/type/file_formats_nullable.py
--rw-r--r--   0        0        0      769 2024-03-12 19:34:27.349524 carbon_python_sdk-0.1.8/carbon/type/file_statistics.py
--rw-r--r--   0        0        0      809 2024-03-12 19:34:27.349626 carbon_python_sdk-0.1.8/carbon/type/file_statistics_nullable.py
--rw-r--r--   0        0        0      427 2024-03-12 19:34:27.349726 carbon_python_sdk-0.1.8/carbon/type/files_query_user_files_deprecated_response.py
--rw-r--r--   0        0        0     1117 2024-03-12 19:34:27.349830 carbon_python_sdk-0.1.8/carbon/type/fresh_desk_connect_request.py
--rw-r--r--   0        0        0      565 2024-03-12 19:34:27.349927 carbon_python_sdk-0.1.8/carbon/type/generic_success_response.py
--rw-r--r--   0        0        0     2436 2024-03-12 19:34:27.350037 carbon_python_sdk-0.1.8/carbon/type/get_embedding_documents_body.py
--rw-r--r--   0        0        0      391 2024-03-12 19:34:27.350158 carbon_python_sdk-0.1.8/carbon/type/get_embedding_documents_body_file_ids.py
--rw-r--r--   0        0        0      397 2024-03-12 19:34:27.350267 carbon_python_sdk-0.1.8/carbon/type/get_embedding_documents_body_parent_file_ids.py
--rw-r--r--   0        0        0      416 2024-03-12 19:34:27.350371 carbon_python_sdk-0.1.8/carbon/type/get_embedding_documents_body_query_vector.py
--rw-r--r--   0        0        0      359 2024-03-12 19:34:27.350466 carbon_python_sdk-0.1.8/carbon/type/get_embedding_documents_body_tags.py
--rw-r--r--   0        0        0     1093 2024-03-12 19:34:27.350576 carbon_python_sdk-0.1.8/carbon/type/gitbook_connect_request.py
--rw-r--r--   0        0        0     1129 2024-03-12 19:34:27.350673 carbon_python_sdk-0.1.8/carbon/type/gitbook_sync_request.py
--rw-r--r--   0        0        0      368 2024-03-12 19:34:27.350764 carbon_python_sdk-0.1.8/carbon/type/gitbook_sync_request_space_ids.py
--rw-r--r--   0        0        0     1103 2024-03-12 19:34:27.350862 carbon_python_sdk-0.1.8/carbon/type/gmail_sync_input.py
--rw-r--r--   0        0        0      630 2024-03-12 19:34:27.350973 carbon_python_sdk-0.1.8/carbon/type/http_validation_error.py
--rw-r--r--   0        0        0      636 2024-03-12 19:34:27.351089 carbon_python_sdk-0.1.8/carbon/type/hybrid_search_tuning_params.py
--rw-r--r--   0        0        0      676 2024-03-12 19:34:27.351215 carbon_python_sdk-0.1.8/carbon/type/hybrid_search_tuning_params_nullable.py
--rw-r--r--   0        0        0      692 2024-03-12 19:34:27.351332 carbon_python_sdk-0.1.8/carbon/type/list_data_source_items_request.py
--rw-r--r--   0        0        0      695 2024-03-12 19:34:27.351453 carbon_python_sdk-0.1.8/carbon/type/list_data_source_items_response.py
--rw-r--r--   0        0        0      543 2024-03-12 19:34:27.351577 carbon_python_sdk-0.1.8/carbon/type/list_request.py
--rw-r--r--   0        0        0      587 2024-03-12 19:34:27.351688 carbon_python_sdk-0.1.8/carbon/type/list_response.py
--rw-r--r--   0        0        0      709 2024-03-12 19:34:27.351813 carbon_python_sdk-0.1.8/carbon/type/modify_user_configuration_input.py
--rw-r--r--   0        0        0     2183 2024-03-12 19:34:27.351912 carbon_python_sdk-0.1.8/carbon/type/o_auth_url_request.py
--rw-r--r--   0        0        0      356 2024-03-12 19:34:27.352020 carbon_python_sdk-0.1.8/carbon/type/order_dir.py
--rw-r--r--   0        0        0     1494 2024-03-12 19:34:27.352122 carbon_python_sdk-0.1.8/carbon/type/organization_response.py
--rw-r--r--   0        0        0     1242 2024-03-12 19:34:27.352446 carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_api.py
--rw-r--r--   0        0        0      903 2024-03-12 19:34:27.352560 carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_filters.py
--rw-r--r--   0        0        0      395 2024-03-12 19:34:27.352665 carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_filters_ids.py
--rw-r--r--   0        0        0      401 2024-03-12 19:34:27.352778 carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_order_by_columns.py
--rw-r--r--   0        0        0     1070 2024-03-12 19:34:27.352888 carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_query_input.py
--rw-r--r--   0        0        0      767 2024-03-12 19:34:27.352995 carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_response.py
--rw-r--r--   0        0        0      759 2024-03-12 19:34:27.353103 carbon_python_sdk-0.1.8/carbon/type/organization_user_file_tag_create.py
--rw-r--r--   0        0        0      363 2024-03-12 19:34:27.353212 carbon_python_sdk-0.1.8/carbon/type/organization_user_file_tag_create_tags.py
--rw-r--r--   0        0        0      767 2024-03-12 19:34:27.353324 carbon_python_sdk-0.1.8/carbon/type/organization_user_file_tags_remove.py
--rw-r--r--   0        0        0      376 2024-03-12 19:34:27.353424 carbon_python_sdk-0.1.8/carbon/type/organization_user_file_tags_remove_tags.py
--rw-r--r--   0        0        0     2200 2024-03-12 19:34:27.353530 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters.py
--rw-r--r--   0        0        0      408 2024-03-12 19:34:27.353695 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters_external_file_ids.py
--rw-r--r--   0        0        0      396 2024-03-12 19:34:27.354029 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters_ids.py
--rw-r--r--   0        0        0      421 2024-03-12 19:34:27.354201 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters_organization_user_data_source_id.py
--rw-r--r--   0        0        0      406 2024-03-12 19:34:27.354357 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters_parent_file_ids.py
--rw-r--r--   0        0        0      368 2024-03-12 19:34:27.354529 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters_tags.py
--rw-r--r--   0        0        0      434 2024-03-12 19:34:27.356263 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_order_by_types.py
--rw-r--r--   0        0        0     1228 2024-03-12 19:34:27.356415 carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_query_input.py
--rw-r--r--   0        0        0      531 2024-03-12 19:34:27.356546 carbon_python_sdk-0.1.8/carbon/type/outh_url_response.py
--rw-r--r--   0        0        0     1147 2024-03-12 19:34:27.356673 carbon_python_sdk-0.1.8/carbon/type/outlook_sync_input.py
--rw-r--r--   0        0        0      519 2024-03-12 19:34:27.356791 carbon_python_sdk-0.1.8/carbon/type/pagination.py
--rw-r--r--   0        0        0      560 2024-03-12 19:34:27.356908 carbon_python_sdk-0.1.8/carbon/type/presigned_url_response.py
--rw-r--r--   0        0        0      882 2024-03-12 19:34:27.357024 carbon_python_sdk-0.1.8/carbon/type/raw_text_input.py
--rw-r--r--   0        0        0      661 2024-03-12 19:34:27.357148 carbon_python_sdk-0.1.8/carbon/type/resync_file_query_input.py
--rw-r--r--   0        0        0      571 2024-03-12 19:34:27.357291 carbon_python_sdk-0.1.8/carbon/type/revoke_access_token_input.py
--rw-r--r--   0        0        0      963 2024-03-12 19:34:27.357436 carbon_python_sdk-0.1.8/carbon/type/rss_feed_input.py
--rw-r--r--   0        0        0      550 2024-03-12 19:34:27.357554 carbon_python_sdk-0.1.8/carbon/type/s3_auth_request.py
--rw-r--r--   0        0        0     1180 2024-03-12 19:34:27.357689 carbon_python_sdk-0.1.8/carbon/type/s3_file_sync_input.py
--rw-r--r--   0        0        0      570 2024-03-12 19:34:27.357947 carbon_python_sdk-0.1.8/carbon/type/s3_get_file_input.py
--rw-r--r--   0        0        0      830 2024-03-12 19:34:27.358392 carbon_python_sdk-0.1.8/carbon/type/single_chunks_and_embeddings_upload_input.py
--rw-r--r--   0        0        0     1593 2024-03-12 19:34:27.358685 carbon_python_sdk-0.1.8/carbon/type/sitemap_scrape_request.py
--rw-r--r--   0        0        0      395 2024-03-12 19:34:27.358868 carbon_python_sdk-0.1.8/carbon/type/sitemap_scrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      397 2024-03-12 19:34:27.359005 carbon_python_sdk-0.1.8/carbon/type/sitemap_scrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      393 2024-03-12 19:34:27.359130 carbon_python_sdk-0.1.8/carbon/type/sitemap_scrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      354 2024-03-12 19:34:27.359272 carbon_python_sdk-0.1.8/carbon/type/sitemap_scrape_request_tags.py
--rw-r--r--   0        0        0      561 2024-03-12 19:34:27.359590 carbon_python_sdk-0.1.8/carbon/type/sync_directory_request.py
--rw-r--r--   0        0        0      527 2024-03-12 19:34:27.359753 carbon_python_sdk-0.1.8/carbon/type/sync_files_ids.py
--rw-r--r--   0        0        0     1218 2024-03-12 19:34:27.359887 carbon_python_sdk-0.1.8/carbon/type/sync_files_request.py
--rw-r--r--   0        0        0      531 2024-03-12 19:34:27.360019 carbon_python_sdk-0.1.8/carbon/type/text_embedding_generators.py
--rw-r--r--   0        0        0      548 2024-03-12 19:34:27.360140 carbon_python_sdk-0.1.8/carbon/type/token_response.py
--rw-r--r--   0        0        0      986 2024-03-12 19:34:27.360265 carbon_python_sdk-0.1.8/carbon/type/upload_file_from_url_input.py
--rw-r--r--   0        0        0     2196 2024-03-12 19:34:27.360370 carbon_python_sdk-0.1.8/carbon/type/user_file.py
--rw-r--r--   0        0        0      422 2024-03-12 19:34:27.361571 carbon_python_sdk-0.1.8/carbon/type/user_file_embedding_properties.py
--rw-r--r--   0        0        0      586 2024-03-12 19:34:27.361740 carbon_python_sdk-0.1.8/carbon/type/user_files_v2.py
--rw-r--r--   0        0        0      548 2024-03-12 19:34:27.361881 carbon_python_sdk-0.1.8/carbon/type/user_request_content.py
--rw-r--r--   0        0        0     1017 2024-03-12 19:34:27.361997 carbon_python_sdk-0.1.8/carbon/type/user_response.py
--rw-r--r--   0        0        0      371 2024-03-12 19:34:27.362126 carbon_python_sdk-0.1.8/carbon/type/user_response_unique_file_tags.py
--rw-r--r--   0        0        0      439 2024-03-12 19:34:27.362241 carbon_python_sdk-0.1.8/carbon/type/utilities_scrape_web_request.py
--rw-r--r--   0        0        0      633 2024-03-12 19:34:27.362363 carbon_python_sdk-0.1.8/carbon/type/validation_error.py
--rw-r--r--   0        0        0      405 2024-03-12 19:34:27.362493 carbon_python_sdk-0.1.8/carbon/type/validation_error_loc.py
--rw-r--r--   0        0        0      598 2024-03-12 19:34:27.362607 carbon_python_sdk-0.1.8/carbon/type/webhook.py
--rw-r--r--   0        0        0      596 2024-03-12 19:34:27.362723 carbon_python_sdk-0.1.8/carbon/type/webhook_filters.py
--rw-r--r--   0        0        0      376 2024-03-12 19:34:27.362846 carbon_python_sdk-0.1.8/carbon/type/webhook_filters_ids.py
--rw-r--r--   0        0        0      601 2024-03-12 19:34:27.362948 carbon_python_sdk-0.1.8/carbon/type/webhook_no_key.py
--rw-r--r--   0        0        0      382 2024-03-12 19:34:27.363067 carbon_python_sdk-0.1.8/carbon/type/webhook_order_by_columns.py
--rw-r--r--   0        0        0      855 2024-03-12 19:34:27.363187 carbon_python_sdk-0.1.8/carbon/type/webhook_query_input.py
--rw-r--r--   0        0        0      644 2024-03-12 19:34:27.363301 carbon_python_sdk-0.1.8/carbon/type/webhook_query_response.py
--rw-r--r--   0        0        0     1564 2024-03-12 19:34:27.363417 carbon_python_sdk-0.1.8/carbon/type/webscrape_request.py
--rw-r--r--   0        0        0      391 2024-03-12 19:34:27.363546 carbon_python_sdk-0.1.8/carbon/type/webscrape_request_css_classes_to_skip.py
--rw-r--r--   0        0        0      393 2024-03-12 19:34:27.363686 carbon_python_sdk-0.1.8/carbon/type/webscrape_request_css_selectors_to_skip.py
--rw-r--r--   0        0        0      389 2024-03-12 19:34:27.363817 carbon_python_sdk-0.1.8/carbon/type/webscrape_request_html_tags_to_skip.py
--rw-r--r--   0        0        0      350 2024-03-12 19:34:27.363932 carbon_python_sdk-0.1.8/carbon/type/webscrape_request_tags.py
--rw-r--r--   0        0        0      675 2024-03-12 19:34:27.364041 carbon_python_sdk-0.1.8/carbon/type/white_labeling_response.py
--rw-r--r--   0        0        0      809 2024-03-12 19:34:27.364166 carbon_python_sdk-0.1.8/carbon/type/youtube_transcript_response.py
--rw-r--r--   0        0        0      551 2024-03-12 19:34:27.364299 carbon_python_sdk-0.1.8/carbon/type/youtube_transcript_response_raw_transcript.py
--rw-r--r--   0        0        0      372 2024-03-12 19:34:27.364449 carbon_python_sdk-0.1.8/carbon/type/youtube_transcript_response_raw_transcript_item.py
--rw-r--r--   0        0        0      514 2024-03-12 19:34:27.364579 carbon_python_sdk-0.1.8/carbon/type_util.py
--rw-r--r--   0        0        0     3162 2024-03-12 19:34:27.364726 carbon_python_sdk-0.1.8/carbon/validation_metadata.py
--rw-r--r--   0        0        0      736 2024-03-12 19:34:27.364873 carbon_python_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0    93433 1970-01-01 00:00:00.000000 carbon_python_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-03-14 20:19:21.910625 carbon_python_sdk-0.1.9/LICENSE
+-rw-r--r--   0        0        0    94401 2024-03-14 20:21:24.395283 carbon_python_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0      675 2024-03-14 20:21:24.395510 carbon_python_sdk-0.1.9/carbon/__init__.py
+-rw-r--r--   0        0        0    76911 2024-03-14 20:21:24.395766 carbon_python_sdk-0.1.9/carbon/api_client.py
+-rw-r--r--   0        0        0      663 2024-03-14 20:19:21.700070 carbon_python_sdk-0.1.9/carbon/api_response.py
+-rw-r--r--   0        0        0      214 2024-03-14 20:19:21.700228 carbon_python_sdk-0.1.9/carbon/apis/__init__.py
+-rw-r--r--   0        0        0     9733 2024-03-14 20:21:24.396028 carbon_python_sdk-0.1.9/carbon/apis/path_to_api.py
+-rw-r--r--   0        0        0      233 2024-03-14 20:19:21.700846 carbon_python_sdk-0.1.9/carbon/apis/paths/__init__.py
+-rw-r--r--   0        0        0      101 2024-03-14 20:19:21.701075 carbon_python_sdk-0.1.9/carbon/apis/paths/add_webhook.py
+-rw-r--r--   0        0        0      114 2024-03-14 20:19:21.701225 carbon_python_sdk-0.1.9/carbon/apis/paths/auth_v1_access_token.py
+-rw-r--r--   0        0        0      118 2024-03-14 20:19:21.701365 carbon_python_sdk-0.1.9/carbon/apis/paths/auth_v1_white_labeling.py
+-rw-r--r--   0        0        0      119 2024-03-14 20:19:21.701681 carbon_python_sdk-0.1.9/carbon/apis/paths/create_user_file_tags.py
+-rw-r--r--   0        0        0      103 2024-03-14 20:19:21.701879 carbon_python_sdk-0.1.9/carbon/apis/paths/delete_files.py
+-rw-r--r--   0        0        0      119 2024-03-14 20:19:21.702237 carbon_python_sdk-0.1.9/carbon/apis/paths/delete_user_file_tags.py
+-rw-r--r--   0        0        0      103 2024-03-14 20:19:21.702554 carbon_python_sdk-0.1.9/carbon/apis/paths/delete_users.py
+-rw-r--r--   0        0        0      133 2024-03-14 20:19:21.702713 carbon_python_sdk-0.1.9/carbon/apis/paths/delete_webhook_webhook_id.py
+-rw-r--r--   0        0        0      120 2024-03-14 20:19:21.702834 carbon_python_sdk-0.1.9/carbon/apis/paths/deletefile_file_id.py
+-rw-r--r--   0        0        0      100 2024-03-14 20:19:21.702948 carbon_python_sdk-0.1.9/carbon/apis/paths/embeddings.py
+-rw-r--r--   0        0        0       96 2024-03-14 20:19:21.703105 carbon_python_sdk-0.1.9/carbon/apis/paths/fetch_urls.py
+-rw-r--r--   0        0        0      123 2024-03-14 20:19:21.703324 carbon_python_sdk-0.1.9/carbon/apis/paths/fetch_youtube_transcript.py
+-rw-r--r--   0        0        0       89 2024-03-14 20:19:21.703766 carbon_python_sdk-0.1.9/carbon/apis/paths/health.py
+-rw-r--r--   0        0        0      134 2024-03-14 20:19:21.703980 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_confluence_list.py
+-rw-r--r--   0        0        0      134 2024-03-14 20:19:21.704107 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_confluence_sync.py
+-rw-r--r--   0        0        0      119 2024-03-14 20:21:24.396111 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_connect.py
+-rw-r--r--   0        0        0      124 2024-03-14 20:19:21.704346 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_files_sync.py
+-rw-r--r--   0        0        0      123 2024-03-14 20:19:21.704501 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_freshdesk.py
+-rw-r--r--   0        0        0      119 2024-03-14 20:19:21.704617 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_gitbook.py
+-rw-r--r--   0        0        0      129 2024-03-14 20:19:21.704731 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_gitbook_spaces.py
+-rw-r--r--   0        0        0      128 2024-03-14 20:19:21.704855 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_gitbook_sync.py
+-rw-r--r--   0        0        0      124 2024-03-14 20:19:21.704975 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_gmail_sync.py
+-rw-r--r--   0        0        0      134 2024-03-14 20:19:21.705083 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_gmail_user_labels.py
+-rw-r--r--   0        0        0      124 2024-03-14 20:19:21.705308 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_items_list.py
+-rw-r--r--   0        0        0      124 2024-03-14 20:19:21.705538 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_items_sync.py
+-rw-r--r--   0        0        0      122 2024-03-14 20:19:21.705660 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_oauth_url.py
+-rw-r--r--   0        0        0      128 2024-03-14 20:19:21.705775 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_outlook_sync.py
+-rw-r--r--   0        0        0      146 2024-03-14 20:19:21.706069 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_outlook_user_categories.py
+-rw-r--r--   0        0        0      140 2024-03-14 20:19:21.706238 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_outlook_user_folders.py
+-rw-r--r--   0        0        0      120 2024-03-14 20:19:21.706389 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_rss_feed.py
+-rw-r--r--   0        0        0      109 2024-03-14 20:19:21.706519 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_s3.py
+-rw-r--r--   0        0        0      120 2024-03-14 20:19:21.706641 carbon_python_sdk-0.1.9/carbon/apis/paths/integrations_s3_files.py
+-rw-r--r--   0        0        0      128 2024-03-14 20:19:21.706785 carbon_python_sdk-0.1.9/carbon/apis/paths/modify_user_configuration.py
+-rw-r--r--   0        0        0      101 2024-03-14 20:19:21.706897 carbon_python_sdk-0.1.9/carbon/apis/paths/organization.py
+-rw-r--r--   0        0        0      112 2024-03-14 20:19:21.707007 carbon_python_sdk-0.1.9/carbon/apis/paths/parsed_file_file_id.py
+-rw-r--r--   0        0        0      106 2024-03-14 20:19:21.707114 carbon_python_sdk-0.1.9/carbon/apis/paths/process_sitemap.py
+-rw-r--r--   0        0        0      106 2024-03-14 20:19:21.707221 carbon_python_sdk-0.1.9/carbon/apis/paths/raw_file_file_id.py
+-rw-r--r--   0        0        0      101 2024-03-14 20:19:21.707323 carbon_python_sdk-0.1.9/carbon/apis/paths/resync_file.py
+-rw-r--r--   0        0        0      116 2024-03-14 20:19:21.707590 carbon_python_sdk-0.1.9/carbon/apis/paths/revoke_access_token.py
+-rw-r--r--   0        0        0      107 2024-03-14 20:19:21.707803 carbon_python_sdk-0.1.9/carbon/apis/paths/scrape_sitemap.py
+-rw-r--r--   0        0        0       98 2024-03-14 20:19:21.707948 carbon_python_sdk-0.1.9/carbon/apis/paths/search_urls.py
+-rw-r--r--   0        0        0      101 2024-03-14 20:19:21.708067 carbon_python_sdk-0.1.9/carbon/apis/paths/text_chunks.py
+-rw-r--r--   0        0        0      133 2024-03-14 20:19:21.708409 carbon_python_sdk-0.1.9/carbon/apis/paths/upload_chunks_and_embeddings.py
+-rw-r--r--   0        0        0      117 2024-03-14 20:19:21.708549 carbon_python_sdk-0.1.9/carbon/apis/paths/upload_file_from_url.py
+-rw-r--r--   0        0        0      101 2024-03-14 20:19:21.708660 carbon_python_sdk-0.1.9/carbon/apis/paths/upload_text.py
+-rw-r--r--   0        0        0      100 2024-03-14 20:19:21.708939 carbon_python_sdk-0.1.9/carbon/apis/paths/uploadfile.py
+-rw-r--r--   0        0        0       88 2024-03-14 20:19:21.709322 carbon_python_sdk-0.1.9/carbon/apis/paths/user.py
+-rw-r--r--   0        0        0      112 2024-03-14 20:19:21.709500 carbon_python_sdk-0.1.9/carbon/apis/paths/user_data_sources.py
+-rw-r--r--   0        0        0       99 2024-03-14 20:19:21.709626 carbon_python_sdk-0.1.9/carbon/apis/paths/user_files.py
+-rw-r--r--   0        0        0      104 2024-03-14 20:19:21.709732 carbon_python_sdk-0.1.9/carbon/apis/paths/user_files_v2.py
+-rw-r--r--   0        0        0       99 2024-03-14 20:19:21.709858 carbon_python_sdk-0.1.9/carbon/apis/paths/web_scrape.py
+-rw-r--r--   0        0        0       96 2024-03-14 20:19:21.710142 carbon_python_sdk-0.1.9/carbon/apis/paths/webhooks.py
+-rw-r--r--   0        0        0     2044 2024-03-14 20:19:21.710315 carbon_python_sdk-0.1.9/carbon/apis/tag_to_api.py
+-rw-r--r--   0        0        0      655 2024-03-14 20:19:21.710716 carbon_python_sdk-0.1.9/carbon/apis/tags/__init__.py
+-rw-r--r--   0        0        0      663 2024-03-14 20:19:21.710996 carbon_python_sdk-0.1.9/carbon/apis/tags/auth_api.py
+-rw-r--r--   0        0        0      493 2024-03-14 20:19:21.711189 carbon_python_sdk-0.1.9/carbon/apis/tags/auth_api_raw.py
+-rw-r--r--   0        0        0      709 2024-03-14 20:19:21.711322 carbon_python_sdk-0.1.9/carbon/apis/tags/data_sources_api.py
+-rw-r--r--   0        0        0      510 2024-03-14 20:19:21.711436 carbon_python_sdk-0.1.9/carbon/apis/tags/data_sources_api_raw.py
+-rw-r--r--   0        0        0      798 2024-03-14 20:19:21.711615 carbon_python_sdk-0.1.9/carbon/apis/tags/embeddings_api.py
+-rw-r--r--   0        0        0      610 2024-03-14 20:19:21.711932 carbon_python_sdk-0.1.9/carbon/apis/tags/embeddings_api_raw.py
+-rw-r--r--   0        0        0     1418 2024-03-14 20:19:21.712130 carbon_python_sdk-0.1.9/carbon/apis/tags/files_api.py
+-rw-r--r--   0        0        0     1304 2024-03-14 20:19:21.712455 carbon_python_sdk-0.1.9/carbon/apis/tags/files_api_raw.py
+-rw-r--r--   0        0        0      550 2024-03-14 20:19:21.712612 carbon_python_sdk-0.1.9/carbon/apis/tags/health_api.py
+-rw-r--r--   0        0        0      366 2024-03-14 20:19:21.712889 carbon_python_sdk-0.1.9/carbon/apis/tags/health_api_raw.py
+-rw-r--r--   0        0        0     2242 2024-03-14 20:21:24.396257 carbon_python_sdk-0.1.9/carbon/apis/tags/integrations_api.py
+-rw-r--r--   0        0        0     2142 2024-03-14 20:21:24.396385 carbon_python_sdk-0.1.9/carbon/apis/tags/integrations_api_raw.py
+-rw-r--r--   0        0        0      587 2024-03-14 20:19:21.714947 carbon_python_sdk-0.1.9/carbon/apis/tags/organizations_api.py
+-rw-r--r--   0        0        0      375 2024-03-14 20:19:21.715088 carbon_python_sdk-0.1.9/carbon/apis/tags/organizations_api_raw.py
+-rw-r--r--   0        0        0      701 2024-03-14 20:19:21.715198 carbon_python_sdk-0.1.9/carbon/apis/tags/users_api.py
+-rw-r--r--   0        0        0      533 2024-03-14 20:19:21.716769 carbon_python_sdk-0.1.9/carbon/apis/tags/users_api_raw.py
+-rw-r--r--   0        0        0      976 2024-03-14 20:19:21.717115 carbon_python_sdk-0.1.9/carbon/apis/tags/utilities_api.py
+-rw-r--r--   0        0        0      810 2024-03-14 20:19:21.717240 carbon_python_sdk-0.1.9/carbon/apis/tags/utilities_api_raw.py
+-rw-r--r--   0        0        0      705 2024-03-14 20:19:21.717350 carbon_python_sdk-0.1.9/carbon/apis/tags/webhooks_api.py
+-rw-r--r--   0        0        0      525 2024-03-14 20:19:21.717463 carbon_python_sdk-0.1.9/carbon/apis/tags/webhooks_api_raw.py
+-rw-r--r--   0        0        0     1986 2024-03-14 20:19:21.717570 carbon_python_sdk-0.1.9/carbon/client.py
+-rw-r--r--   0        0        0     1986 2024-03-14 20:19:21.717714 carbon_python_sdk-0.1.9/carbon/client.pyi
+-rw-r--r--   0        0        0      676 2024-03-14 20:19:21.717835 carbon_python_sdk-0.1.9/carbon/client_custom.py
+-rw-r--r--   0        0        0    17804 2024-03-14 20:21:24.396573 carbon_python_sdk-0.1.9/carbon/configuration.py
+-rw-r--r--   0        0        0     7679 2024-03-14 20:19:21.718162 carbon_python_sdk-0.1.9/carbon/exceptions.py
+-rw-r--r--   0        0        0     2274 2024-03-14 20:19:21.718267 carbon_python_sdk-0.1.9/carbon/exceptions_base.py
+-rw-r--r--   0        0        0      340 2024-03-14 20:19:21.718515 carbon_python_sdk-0.1.9/carbon/model/__init__.py
+-rw-r--r--   0        0        0     2282 2024-03-14 20:19:21.718659 carbon_python_sdk-0.1.9/carbon/model/add_webhook_props.py
+-rw-r--r--   0        0        0     2282 2024-03-14 20:19:21.718766 carbon_python_sdk-0.1.9/carbon/model/add_webhook_props.pyi
+-rw-r--r--   0        0        0     2371 2024-03-14 20:19:21.718880 carbon_python_sdk-0.1.9/carbon/model/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0     2371 2024-03-14 20:19:21.719013 carbon_python_sdk-0.1.9/carbon/model/body_create_upload_file_uploadfile_post.pyi
+-rw-r--r--   0        0        0     4752 2024-03-14 20:19:21.719221 carbon_python_sdk-0.1.9/carbon/model/chunk_properties.py
+-rw-r--r--   0        0        0     4752 2024-03-14 20:19:21.719402 carbon_python_sdk-0.1.9/carbon/model/chunk_properties.pyi
+-rw-r--r--   0        0        0     4359 2024-03-14 20:19:21.719629 carbon_python_sdk-0.1.9/carbon/model/chunk_properties_nullable.py
+-rw-r--r--   0        0        0     4359 2024-03-14 20:19:21.719901 carbon_python_sdk-0.1.9/carbon/model/chunk_properties_nullable.pyi
+-rw-r--r--   0        0        0     4319 2024-03-14 20:19:21.720151 carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings.py
+-rw-r--r--   0        0        0     4319 2024-03-14 20:19:21.720361 carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings.pyi
+-rw-r--r--   0        0        0     1100 2024-03-14 20:19:21.720493 carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1100 2024-03-14 20:19:21.720649 carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_embedding.pyi
+-rw-r--r--   0        0        0     6383 2024-03-14 20:19:21.720856 carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     6383 2024-03-14 20:19:21.721048 carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_upload_input.pyi
+-rw-r--r--   0        0        0      548 2024-03-14 20:19:21.721190 carbon_python_sdk-0.1.9/carbon/model/configuration_keys.py
+-rw-r--r--   0        0        0      548 2024-03-14 20:19:21.721341 carbon_python_sdk-0.1.9/carbon/model/configuration_keys.pyi
+-rw-r--r--   0        0        0     4861 2024-03-14 20:21:24.396788 carbon_python_sdk-0.1.9/carbon/model/confluence_authentication.py
+-rw-r--r--   0        0        0     4861 2024-03-14 20:21:24.396935 carbon_python_sdk-0.1.9/carbon/model/confluence_authentication.pyi
+-rw-r--r--   0        0        0     6151 2024-03-14 20:21:24.397087 carbon_python_sdk-0.1.9/carbon/model/connect_data_source_input.py
+-rw-r--r--   0        0        0     6151 2024-03-14 20:21:24.397235 carbon_python_sdk-0.1.9/carbon/model/connect_data_source_input.pyi
+-rw-r--r--   0        0        0     3763 2024-03-14 20:21:24.397326 carbon_python_sdk-0.1.9/carbon/model/connect_data_source_response.py
+-rw-r--r--   0        0        0     3763 2024-03-14 20:21:24.397407 carbon_python_sdk-0.1.9/carbon/model/connect_data_source_response.pyi
+-rw-r--r--   0        0        0     1183 2024-03-14 20:19:21.722462 carbon_python_sdk-0.1.9/carbon/model/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      998 2024-03-14 20:19:21.722574 carbon_python_sdk-0.1.9/carbon/model/data_source_last_sync_actions.pyi
+-rw-r--r--   0        0        0     1256 2024-03-14 20:19:21.722931 carbon_python_sdk-0.1.9/carbon/model/data_source_sync_statuses.py
+-rw-r--r--   0        0        0     1033 2024-03-14 20:19:21.723086 carbon_python_sdk-0.1.9/carbon/model/data_source_sync_statuses.pyi
+-rw-r--r--   0        0        0     5534 2024-03-14 20:19:21.723280 carbon_python_sdk-0.1.9/carbon/model/data_source_type.py
+-rw-r--r--   0        0        0     4143 2024-03-14 20:19:21.723473 carbon_python_sdk-0.1.9/carbon/model/data_source_type.pyi
+-rw-r--r--   0        0        0     5909 2024-03-14 20:19:21.723676 carbon_python_sdk-0.1.9/carbon/model/data_source_type_nullable.py
+-rw-r--r--   0        0        0     5909 2024-03-14 20:19:21.723887 carbon_python_sdk-0.1.9/carbon/model/data_source_type_nullable.pyi
+-rw-r--r--   0        0        0     6047 2024-03-14 20:19:21.724087 carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input.py
+-rw-r--r--   0        0        0     6047 2024-03-14 20:19:21.724293 carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input.pyi
+-rw-r--r--   0        0        0     1097 2024-03-14 20:19:21.724430 carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0     1097 2024-03-14 20:19:21.724742 carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input_file_ids.pyi
+-rw-r--r--   0        0        0     2600 2024-03-14 20:19:21.724972 carbon_python_sdk-0.1.9/carbon/model/delete_users_input.py
+-rw-r--r--   0        0        0     2600 2024-03-14 20:19:21.725105 carbon_python_sdk-0.1.9/carbon/model/delete_users_input.pyi
+-rw-r--r--   0        0        0     1199 2024-03-14 20:19:21.725254 carbon_python_sdk-0.1.9/carbon/model/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0     1199 2024-03-14 20:19:21.725398 carbon_python_sdk-0.1.9/carbon/model/delete_users_input_customer_ids.pyi
+-rw-r--r--   0        0        0     3902 2024-03-14 20:19:21.725522 carbon_python_sdk-0.1.9/carbon/model/directory_item.py
+-rw-r--r--   0        0        0     3902 2024-03-14 20:19:21.725699 carbon_python_sdk-0.1.9/carbon/model/directory_item.pyi
+-rw-r--r--   0        0        0    13554 2024-03-14 20:19:21.725847 carbon_python_sdk-0.1.9/carbon/model/document_response.py
+-rw-r--r--   0        0        0    13554 2024-03-14 20:19:21.726157 carbon_python_sdk-0.1.9/carbon/model/document_response.pyi
+-rw-r--r--   0        0        0     3350 2024-03-14 20:19:21.726671 carbon_python_sdk-0.1.9/carbon/model/document_response_list.py
+-rw-r--r--   0        0        0     3350 2024-03-14 20:19:21.726896 carbon_python_sdk-0.1.9/carbon/model/document_response_list.pyi
+-rw-r--r--   0        0        0     7489 2024-03-14 20:19:21.727124 carbon_python_sdk-0.1.9/carbon/model/document_response_tags.py
+-rw-r--r--   0        0        0     7489 2024-03-14 20:19:21.727347 carbon_python_sdk-0.1.9/carbon/model/document_response_tags.pyi
+-rw-r--r--   0        0        0     1088 2024-03-14 20:19:21.727504 carbon_python_sdk-0.1.9/carbon/model/document_response_vector.py
+-rw-r--r--   0        0        0     1088 2024-03-14 20:19:21.727618 carbon_python_sdk-0.1.9/carbon/model/document_response_vector.pyi
+-rw-r--r--   0        0        0     5044 2024-03-14 20:19:21.727796 carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk.py
+-rw-r--r--   0        0        0     5044 2024-03-14 20:19:21.727979 carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk.pyi
+-rw-r--r--   0        0        0     1096 2024-03-14 20:19:21.728103 carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0     1096 2024-03-14 20:19:21.728214 carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk_embedding.pyi
+-rw-r--r--   0        0        0     3025 2024-03-14 20:19:21.728317 carbon_python_sdk-0.1.9/carbon/model/embedding_generators.py
+-rw-r--r--   0        0        0     2166 2024-03-14 20:19:21.728460 carbon_python_sdk-0.1.9/carbon/model/embedding_generators.pyi
+-rw-r--r--   0        0        0     3405 2024-03-14 20:19:21.728781 carbon_python_sdk-0.1.9/carbon/model/embedding_generators_nullable.py
+-rw-r--r--   0        0        0     3405 2024-03-14 20:19:21.728978 carbon_python_sdk-0.1.9/carbon/model/embedding_generators_nullable.pyi
+-rw-r--r--   0        0        0     4307 2024-03-14 20:19:21.729172 carbon_python_sdk-0.1.9/carbon/model/embedding_properties.py
+-rw-r--r--   0        0        0     4307 2024-03-14 20:19:21.729351 carbon_python_sdk-0.1.9/carbon/model/embedding_properties.pyi
+-rw-r--r--   0        0        0     3267 2024-03-14 20:19:21.729474 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0     3267 2024-03-14 20:19:21.729773 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_filters.pyi
+-rw-r--r--   0        0        0     1141 2024-03-14 20:19:21.730158 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0      956 2024-03-14 20:19:21.730413 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_order_by_columns.pyi
+-rw-r--r--   0        0        0     5194 2024-03-14 20:19:21.730629 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0     5194 2024-03-14 20:19:21.730833 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_query_input.pyi
+-rw-r--r--   0        0        0     3847 2024-03-14 20:19:21.731194 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0     3847 2024-03-14 20:19:21.731344 carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_response.pyi
+-rw-r--r--   0        0        0     1944 2024-03-14 20:19:21.731466 carbon_python_sdk-0.1.9/carbon/model/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1503 2024-03-14 20:19:21.731784 carbon_python_sdk-0.1.9/carbon/model/external_file_sync_statuses.pyi
+-rw-r--r--   0        0        0    16741 2024-03-14 20:19:21.731945 carbon_python_sdk-0.1.9/carbon/model/external_source_item.py
+-rw-r--r--   0        0        0    16741 2024-03-14 20:19:21.732128 carbon_python_sdk-0.1.9/carbon/model/external_source_item.pyi
+-rw-r--r--   0        0        0     3061 2024-03-14 20:19:21.732301 carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response.py
+-rw-r--r--   0        0        0     3061 2024-03-14 20:19:21.732438 carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response.pyi
+-rw-r--r--   0        0        0     1187 2024-03-14 20:19:21.732549 carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0     1187 2024-03-14 20:19:21.732663 carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response_urls.pyi
+-rw-r--r--   0        0        0      946 2024-03-14 20:19:21.732782 carbon_python_sdk-0.1.9/carbon/model/file_content_types.py
+-rw-r--r--   0        0        0      825 2024-03-14 20:19:21.732888 carbon_python_sdk-0.1.9/carbon/model/file_content_types.pyi
+-rw-r--r--   0        0        0     1706 2024-03-14 20:19:21.733162 carbon_python_sdk-0.1.9/carbon/model/file_content_types_nullable.py
+-rw-r--r--   0        0        0     1706 2024-03-14 20:19:21.733321 carbon_python_sdk-0.1.9/carbon/model/file_content_types_nullable.pyi
+-rw-r--r--   0        0        0     4851 2024-03-14 20:19:21.733582 carbon_python_sdk-0.1.9/carbon/model/file_formats.py
+-rw-r--r--   0        0        0     3650 2024-03-14 20:19:21.733878 carbon_python_sdk-0.1.9/carbon/model/file_formats.pyi
+-rw-r--r--   0        0        0     5223 2024-03-14 20:19:21.734132 carbon_python_sdk-0.1.9/carbon/model/file_formats_nullable.py
+-rw-r--r--   0        0        0     5223 2024-03-14 20:19:21.734330 carbon_python_sdk-0.1.9/carbon/model/file_formats_nullable.pyi
+-rw-r--r--   0        0        0     7489 2024-03-14 20:19:21.734537 carbon_python_sdk-0.1.9/carbon/model/file_statistics.py
+-rw-r--r--   0        0        0     7489 2024-03-14 20:19:21.734721 carbon_python_sdk-0.1.9/carbon/model/file_statistics.pyi
+-rw-r--r--   0        0        0     6952 2024-03-14 20:19:21.734902 carbon_python_sdk-0.1.9/carbon/model/file_statistics_nullable.py
+-rw-r--r--   0        0        0     6952 2024-03-14 20:19:21.735087 carbon_python_sdk-0.1.9/carbon/model/file_statistics_nullable.pyi
+-rw-r--r--   0        0        0     1283 2024-03-14 20:19:21.735300 carbon_python_sdk-0.1.9/carbon/model/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1283 2024-03-14 20:19:21.735671 carbon_python_sdk-0.1.9/carbon/model/files_query_user_files_deprecated_response.pyi
+-rw-r--r--   0        0        0    12927 2024-03-14 20:19:21.735836 carbon_python_sdk-0.1.9/carbon/model/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0    12927 2024-03-14 20:19:21.736216 carbon_python_sdk-0.1.9/carbon/model/fresh_desk_connect_request.pyi
+-rw-r--r--   0        0        0     3529 2024-03-14 20:21:24.397501 carbon_python_sdk-0.1.9/carbon/model/freskdesk_authentication.py
+-rw-r--r--   0        0        0     3529 2024-03-14 20:21:24.397587 carbon_python_sdk-0.1.9/carbon/model/freskdesk_authentication.pyi
+-rw-r--r--   0        0        0     2362 2024-03-14 20:19:21.737422 carbon_python_sdk-0.1.9/carbon/model/generic_success_response.py
+-rw-r--r--   0        0        0     2362 2024-03-14 20:19:21.737621 carbon_python_sdk-0.1.9/carbon/model/generic_success_response.pyi
+-rw-r--r--   0        0        0    15093 2024-03-14 20:19:21.737746 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body.py
+-rw-r--r--   0        0        0    14942 2024-03-14 20:19:21.738016 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body.pyi
+-rw-r--r--   0        0        0     1159 2024-03-14 20:19:21.738267 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0     1159 2024-03-14 20:19:21.738410 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_file_ids.pyi
+-rw-r--r--   0        0        0     1264 2024-03-14 20:19:21.738527 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0     1264 2024-03-14 20:19:21.738646 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_parent_file_ids.pyi
+-rw-r--r--   0        0        0     1377 2024-03-14 20:19:21.738761 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0     1377 2024-03-14 20:19:21.738877 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_query_vector.pyi
+-rw-r--r--   0        0        0     6490 2024-03-14 20:19:21.739064 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0     6490 2024-03-14 20:19:21.739249 carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_tags.pyi
+-rw-r--r--   0        0        0     3779 2024-03-14 20:21:24.397661 carbon_python_sdk-0.1.9/carbon/model/gitbook_authetication.py
+-rw-r--r--   0        0        0     3779 2024-03-14 20:21:24.397734 carbon_python_sdk-0.1.9/carbon/model/gitbook_authetication.pyi
+-rw-r--r--   0        0        0    13042 2024-03-14 20:19:21.739622 carbon_python_sdk-0.1.9/carbon/model/gitbook_connect_request.py
+-rw-r--r--   0        0        0    13042 2024-03-14 20:19:21.739885 carbon_python_sdk-0.1.9/carbon/model/gitbook_connect_request.pyi
+-rw-r--r--   0        0        0    11852 2024-03-14 20:19:21.740125 carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request.py
+-rw-r--r--   0        0        0    11852 2024-03-14 20:19:21.740450 carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request.pyi
+-rw-r--r--   0        0        0     1220 2024-03-14 20:19:21.740666 carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0     1197 2024-03-14 20:19:21.740785 carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request_space_ids.pyi
+-rw-r--r--   0        0        0    12263 2024-03-14 20:19:21.740898 carbon_python_sdk-0.1.9/carbon/model/gmail_sync_input.py
+-rw-r--r--   0        0        0    12263 2024-03-14 20:19:21.741092 carbon_python_sdk-0.1.9/carbon/model/gmail_sync_input.pyi
+-rw-r--r--   0        0        0     3251 2024-03-14 20:19:21.741281 carbon_python_sdk-0.1.9/carbon/model/http_validation_error.py
+-rw-r--r--   0        0        0     3251 2024-03-14 20:19:21.741391 carbon_python_sdk-0.1.9/carbon/model/http_validation_error.pyi
+-rw-r--r--   0        0        0     2974 2024-03-14 20:19:21.741499 carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0     2974 2024-03-14 20:19:21.741607 carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params.pyi
+-rw-r--r--   0        0        0     2907 2024-03-14 20:19:21.741731 carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0     2907 2024-03-14 20:19:21.741851 carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params_nullable.pyi
+-rw-r--r--   0        0        0     4274 2024-03-14 20:19:21.742036 carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_request.py
+-rw-r--r--   0        0        0     4274 2024-03-14 20:19:21.742216 carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_request.pyi
+-rw-r--r--   0        0        0     3820 2024-03-14 20:19:21.742320 carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_response.py
+-rw-r--r--   0        0        0     3820 2024-03-14 20:19:21.742429 carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_response.pyi
+-rw-r--r--   0        0        0     3613 2024-03-14 20:19:21.742536 carbon_python_sdk-0.1.9/carbon/model/list_request.py
+-rw-r--r--   0        0        0     3613 2024-03-14 20:19:21.742640 carbon_python_sdk-0.1.9/carbon/model/list_request.pyi
+-rw-r--r--   0        0        0     3228 2024-03-14 20:19:21.742813 carbon_python_sdk-0.1.9/carbon/model/list_response.py
+-rw-r--r--   0        0        0     3228 2024-03-14 20:19:21.743097 carbon_python_sdk-0.1.9/carbon/model/list_response.pyi
+-rw-r--r--   0        0        0     3129 2024-03-14 20:19:21.743234 carbon_python_sdk-0.1.9/carbon/model/modify_user_configuration_input.py
+-rw-r--r--   0        0        0     3129 2024-03-14 20:19:21.743357 carbon_python_sdk-0.1.9/carbon/model/modify_user_configuration_input.pyi
+-rw-r--r--   0        0        0     3699 2024-03-14 20:21:24.397809 carbon_python_sdk-0.1.9/carbon/model/notion_authentication.py
+-rw-r--r--   0        0        0     3699 2024-03-14 20:21:24.397890 carbon_python_sdk-0.1.9/carbon/model/notion_authentication.pyi
+-rw-r--r--   0        0        0     4300 2024-03-14 20:21:24.398043 carbon_python_sdk-0.1.9/carbon/model/o_auth_authentication.py
+-rw-r--r--   0        0        0     4300 2024-03-14 20:21:24.398185 carbon_python_sdk-0.1.9/carbon/model/o_auth_authentication.pyi
+-rw-r--r--   0        0        0    23818 2024-03-14 20:19:21.744307 carbon_python_sdk-0.1.9/carbon/model/o_auth_url_request.py
+-rw-r--r--   0        0        0    23818 2024-03-14 20:19:21.744451 carbon_python_sdk-0.1.9/carbon/model/o_auth_url_request.pyi
+-rw-r--r--   0        0        0      930 2024-03-14 20:19:21.744576 carbon_python_sdk-0.1.9/carbon/model/order_dir.py
+-rw-r--r--   0        0        0      813 2024-03-14 20:19:21.744712 carbon_python_sdk-0.1.9/carbon/model/order_dir.pyi
+-rw-r--r--   0        0        0    14659 2024-03-14 20:19:21.744844 carbon_python_sdk-0.1.9/carbon/model/organization_response.py
+-rw-r--r--   0        0        0    14659 2024-03-14 20:19:21.745174 carbon_python_sdk-0.1.9/carbon/model/organization_response.pyi
+-rw-r--r--   0        0        0    13610 2024-03-14 20:21:24.398453 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_api.py
+-rw-r--r--   0        0        0    13610 2024-03-14 20:21:24.398875 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_api.pyi
+-rw-r--r--   0        0        0     4467 2024-03-14 20:19:21.746055 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0     4467 2024-03-14 20:19:21.746250 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters.pyi
+-rw-r--r--   0        0        0     1113 2024-03-14 20:19:21.746376 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0     1113 2024-03-14 20:19:21.746497 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters_ids.pyi
+-rw-r--r--   0        0        0     1014 2024-03-14 20:19:21.746606 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0      871 2024-03-14 20:19:21.746720 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_order_by_columns.pyi
+-rw-r--r--   0        0        0     4657 2024-03-14 20:19:21.746920 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0     4657 2024-03-14 20:19:21.747123 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_query_input.pyi
+-rw-r--r--   0        0        0     3947 2024-03-14 20:19:21.747245 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_response.py
+-rw-r--r--   0        0        0     3947 2024-03-14 20:19:21.747357 carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_response.pyi
+-rw-r--r--   0        0        0     3408 2024-03-14 20:19:21.747481 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0     3408 2024-03-14 20:19:21.747603 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create.pyi
+-rw-r--r--   0        0        0     6330 2024-03-14 20:19:21.747782 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0     6330 2024-03-14 20:19:21.747962 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create_tags.pyi
+-rw-r--r--   0        0        0     3418 2024-03-14 20:19:21.748092 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0     3418 2024-03-14 20:19:21.748217 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove.pyi
+-rw-r--r--   0        0        0     1213 2024-03-14 20:19:21.748396 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     1213 2024-03-14 20:19:21.748542 carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove_tags.pyi
+-rw-r--r--   0        0        0    16946 2024-03-14 20:19:21.748689 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0    16946 2024-03-14 20:19:21.749023 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters.pyi
+-rw-r--r--   0        0        0     1139 2024-03-14 20:19:21.749303 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0     1139 2024-03-14 20:19:21.749564 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi
+-rw-r--r--   0        0        0     1115 2024-03-14 20:19:21.749837 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0     1115 2024-03-14 20:19:21.750048 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_ids.pyi
+-rw-r--r--   0        0        0     1165 2024-03-14 20:19:21.750206 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0     1165 2024-03-14 20:19:21.750349 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi
+-rw-r--r--   0        0        0     1135 2024-03-14 20:19:21.750477 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0     1135 2024-03-14 20:19:21.750604 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi
+-rw-r--r--   0        0        0     6420 2024-03-14 20:19:21.750801 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0     6420 2024-03-14 20:19:21.751036 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_tags.pyi
+-rw-r--r--   0        0        0     1371 2024-03-14 20:19:21.751182 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1124 2024-03-14 20:19:21.751314 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_order_by_types.pyi
+-rw-r--r--   0        0        0     8629 2024-03-14 20:19:21.751443 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0     8629 2024-03-14 20:19:21.751788 carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_query_input.pyi
+-rw-r--r--   0        0        0     2378 2024-03-14 20:19:21.752074 carbon_python_sdk-0.1.9/carbon/model/outh_url_response.py
+-rw-r--r--   0        0        0     2378 2024-03-14 20:19:21.752194 carbon_python_sdk-0.1.9/carbon/model/outh_url_response.pyi
+-rw-r--r--   0        0        0    13371 2024-03-14 20:19:21.752354 carbon_python_sdk-0.1.9/carbon/model/outlook_sync_input.py
+-rw-r--r--   0        0        0    13371 2024-03-14 20:19:21.752621 carbon_python_sdk-0.1.9/carbon/model/outlook_sync_input.pyi
+-rw-r--r--   0        0        0     2807 2024-03-14 20:19:21.752867 carbon_python_sdk-0.1.9/carbon/model/pagination.py
+-rw-r--r--   0        0        0     2807 2024-03-14 20:19:21.752975 carbon_python_sdk-0.1.9/carbon/model/pagination.pyi
+-rw-r--r--   0        0        0     2452 2024-03-14 20:19:21.753085 carbon_python_sdk-0.1.9/carbon/model/presigned_url_response.py
+-rw-r--r--   0        0        0     2452 2024-03-14 20:19:21.753189 carbon_python_sdk-0.1.9/carbon/model/presigned_url_response.pyi
+-rw-r--r--   0        0        0    10068 2024-03-14 20:19:21.753404 carbon_python_sdk-0.1.9/carbon/model/raw_text_input.py
+-rw-r--r--   0        0        0    10068 2024-03-14 20:19:21.753872 carbon_python_sdk-0.1.9/carbon/model/raw_text_input.pyi
+-rw-r--r--   0        0        0     5578 2024-03-14 20:19:21.754304 carbon_python_sdk-0.1.9/carbon/model/resync_file_query_input.py
+-rw-r--r--   0        0        0     5578 2024-03-14 20:19:21.754547 carbon_python_sdk-0.1.9/carbon/model/resync_file_query_input.pyi
+-rw-r--r--   0        0        0     2489 2024-03-14 20:19:21.754678 carbon_python_sdk-0.1.9/carbon/model/revoke_access_token_input.py
+-rw-r--r--   0        0        0     2489 2024-03-14 20:19:21.754789 carbon_python_sdk-0.1.9/carbon/model/revoke_access_token_input.pyi
+-rw-r--r--   0        0        0    10916 2024-03-14 20:19:21.754904 carbon_python_sdk-0.1.9/carbon/model/rss_feed_input.py
+-rw-r--r--   0        0        0    10916 2024-03-14 20:19:21.755110 carbon_python_sdk-0.1.9/carbon/model/rss_feed_input.pyi
+-rw-r--r--   0        0        0     3074 2024-03-14 20:19:21.755306 carbon_python_sdk-0.1.9/carbon/model/s3_auth_request.py
+-rw-r--r--   0        0        0     3074 2024-03-14 20:19:21.755424 carbon_python_sdk-0.1.9/carbon/model/s3_auth_request.pyi
+-rw-r--r--   0        0        0     3739 2024-03-14 20:21:24.399000 carbon_python_sdk-0.1.9/carbon/model/s3_authentication.py
+-rw-r--r--   0        0        0     3739 2024-03-14 20:21:24.399089 carbon_python_sdk-0.1.9/carbon/model/s3_authentication.pyi
+-rw-r--r--   0        0        0    15132 2024-03-14 20:19:21.755795 carbon_python_sdk-0.1.9/carbon/model/s3_file_sync_input.py
+-rw-r--r--   0        0        0    15132 2024-03-14 20:19:21.756092 carbon_python_sdk-0.1.9/carbon/model/s3_file_sync_input.pyi
+-rw-r--r--   0        0        0     3936 2024-03-14 20:19:21.756345 carbon_python_sdk-0.1.9/carbon/model/s3_get_file_input.py
+-rw-r--r--   0        0        0     3936 2024-03-14 20:19:21.756458 carbon_python_sdk-0.1.9/carbon/model/s3_get_file_input.pyi
+-rw-r--r--   0        0        0     4813 2024-03-14 20:21:24.399249 carbon_python_sdk-0.1.9/carbon/model/salesforce_authentication.py
+-rw-r--r--   0        0        0     4813 2024-03-14 20:21:24.399398 carbon_python_sdk-0.1.9/carbon/model/salesforce_authentication.pyi
+-rw-r--r--   0        0        0     5449 2024-03-14 20:21:24.399559 carbon_python_sdk-0.1.9/carbon/model/sharepoint_authentication.py
+-rw-r--r--   0        0        0     5449 2024-03-14 20:21:24.399710 carbon_python_sdk-0.1.9/carbon/model/sharepoint_authentication.pyi
+-rw-r--r--   0        0        0     1566 2024-03-14 20:21:24.399796 carbon_python_sdk-0.1.9/carbon/model/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0     1263 2024-03-14 20:21:24.399879 carbon_python_sdk-0.1.9/carbon/model/simple_o_auth_data_sources.pyi
+-rw-r--r--   0        0        0     6587 2024-03-14 20:19:21.757590 carbon_python_sdk-0.1.9/carbon/model/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     6587 2024-03-14 20:19:21.757776 carbon_python_sdk-0.1.9/carbon/model/single_chunks_and_embeddings_upload_input.pyi
+-rw-r--r--   0        0        0    15650 2024-03-14 20:21:24.400135 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request.py
+-rw-r--r--   0        0        0    15608 2024-03-14 20:21:24.400418 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request.pyi
+-rw-r--r--   0        0        0     1113 2024-03-14 20:19:21.758376 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0     1113 2024-03-14 20:19:21.758484 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi
+-rw-r--r--   0        0        0     1117 2024-03-14 20:19:21.758601 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0     1117 2024-03-14 20:19:21.758718 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi
+-rw-r--r--   0        0        0     1109 2024-03-14 20:19:21.758828 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0     1109 2024-03-14 20:19:21.758938 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi
+-rw-r--r--   0        0        0     6392 2024-03-14 20:19:21.759118 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0     6392 2024-03-14 20:19:21.759296 carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_tags.pyi
+-rw-r--r--   0        0        0     2485 2024-03-14 20:19:21.759403 carbon_python_sdk-0.1.9/carbon/model/sync_directory_request.py
+-rw-r--r--   0        0        0     2485 2024-03-14 20:19:21.759508 carbon_python_sdk-0.1.9/carbon/model/sync_directory_request.pyi
+-rw-r--r--   0        0        0     2784 2024-03-14 20:19:21.759615 carbon_python_sdk-0.1.9/carbon/model/sync_files_ids.py
+-rw-r--r--   0        0        0     2784 2024-03-14 20:19:21.759719 carbon_python_sdk-0.1.9/carbon/model/sync_files_ids.pyi
+-rw-r--r--   0        0        0    17722 2024-03-14 20:19:21.759869 carbon_python_sdk-0.1.9/carbon/model/sync_files_request.py
+-rw-r--r--   0        0        0    17722 2024-03-14 20:19:21.760015 carbon_python_sdk-0.1.9/carbon/model/sync_files_request.pyi
+-rw-r--r--   0        0        0    13129 2024-03-14 20:21:24.400650 carbon_python_sdk-0.1.9/carbon/model/sync_options.py
+-rw-r--r--   0        0        0    13129 2024-03-14 20:21:24.400872 carbon_python_sdk-0.1.9/carbon/model/sync_options.pyi
+-rw-r--r--   0        0        0     2029 2024-03-14 20:19:21.760642 carbon_python_sdk-0.1.9/carbon/model/text_embedding_generators.py
+-rw-r--r--   0        0        0     1520 2024-03-14 20:19:21.760756 carbon_python_sdk-0.1.9/carbon/model/text_embedding_generators.pyi
+-rw-r--r--   0        0        0     3042 2024-03-14 20:19:21.760863 carbon_python_sdk-0.1.9/carbon/model/token_response.py
+-rw-r--r--   0        0        0     3042 2024-03-14 20:19:21.760971 carbon_python_sdk-0.1.9/carbon/model/token_response.pyi
+-rw-r--r--   0        0        0    11472 2024-03-14 20:19:21.761087 carbon_python_sdk-0.1.9/carbon/model/upload_file_from_url_input.py
+-rw-r--r--   0        0        0    11472 2024-03-14 20:19:21.761296 carbon_python_sdk-0.1.9/carbon/model/upload_file_from_url_input.pyi
+-rw-r--r--   0        0        0    31568 2024-03-14 20:19:21.761508 carbon_python_sdk-0.1.9/carbon/model/user_file.py
+-rw-r--r--   0        0        0    31568 2024-03-14 20:19:21.761644 carbon_python_sdk-0.1.9/carbon/model/user_file.pyi
+-rw-r--r--   0        0        0     1650 2024-03-14 20:19:21.761767 carbon_python_sdk-0.1.9/carbon/model/user_file_embedding_properties.py
+-rw-r--r--   0        0        0     1650 2024-03-14 20:19:21.761875 carbon_python_sdk-0.1.9/carbon/model/user_file_embedding_properties.pyi
+-rw-r--r--   0        0        0     3751 2024-03-14 20:19:21.761995 carbon_python_sdk-0.1.9/carbon/model/user_files_v2.py
+-rw-r--r--   0        0        0     3751 2024-03-14 20:19:21.762100 carbon_python_sdk-0.1.9/carbon/model/user_files_v2.pyi
+-rw-r--r--   0        0        0     2416 2024-03-14 20:19:21.762210 carbon_python_sdk-0.1.9/carbon/model/user_request_content.py
+-rw-r--r--   0        0        0     2416 2024-03-14 20:19:21.762320 carbon_python_sdk-0.1.9/carbon/model/user_request_content.pyi
+-rw-r--r--   0        0        0    10845 2024-03-14 20:19:21.762433 carbon_python_sdk-0.1.9/carbon/model/user_response.py
+-rw-r--r--   0        0        0    10845 2024-03-14 20:19:21.762632 carbon_python_sdk-0.1.9/carbon/model/user_response.pyi
+-rw-r--r--   0        0        0     1246 2024-03-14 20:19:21.762859 carbon_python_sdk-0.1.9/carbon/model/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0     1246 2024-03-14 20:19:21.762981 carbon_python_sdk-0.1.9/carbon/model/user_response_unique_file_tags.pyi
+-rw-r--r--   0        0        0     1315 2024-03-14 20:19:21.763091 carbon_python_sdk-0.1.9/carbon/model/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0     1315 2024-03-14 20:19:21.763202 carbon_python_sdk-0.1.9/carbon/model/utilities_scrape_web_request.pyi
+-rw-r--r--   0        0        0     3352 2024-03-14 20:19:21.763305 carbon_python_sdk-0.1.9/carbon/model/validation_error.py
+-rw-r--r--   0        0        0     3352 2024-03-14 20:19:21.763412 carbon_python_sdk-0.1.9/carbon/model/validation_error.pyi
+-rw-r--r--   0        0        0     3149 2024-03-14 20:19:21.763519 carbon_python_sdk-0.1.9/carbon/model/validation_error_loc.py
+-rw-r--r--   0        0        0     3149 2024-03-14 20:19:21.763630 carbon_python_sdk-0.1.9/carbon/model/validation_error_loc.pyi
+-rw-r--r--   0        0        0     5158 2024-03-14 20:19:21.763809 carbon_python_sdk-0.1.9/carbon/model/webhook.py
+-rw-r--r--   0        0        0     5158 2024-03-14 20:19:21.763998 carbon_python_sdk-0.1.9/carbon/model/webhook.pyi
+-rw-r--r--   0        0        0     2396 2024-03-14 20:19:21.764120 carbon_python_sdk-0.1.9/carbon/model/webhook_filters.py
+-rw-r--r--   0        0        0     2396 2024-03-14 20:19:21.764235 carbon_python_sdk-0.1.9/carbon/model/webhook_filters.pyi
+-rw-r--r--   0        0        0     1075 2024-03-14 20:19:21.764395 carbon_python_sdk-0.1.9/carbon/model/webhook_filters_ids.py
+-rw-r--r--   0        0        0     1075 2024-03-14 20:19:21.764518 carbon_python_sdk-0.1.9/carbon/model/webhook_filters_ids.pyi
+-rw-r--r--   0        0        0     4580 2024-03-14 20:19:21.764706 carbon_python_sdk-0.1.9/carbon/model/webhook_no_key.py
+-rw-r--r--   0        0        0     4580 2024-03-14 20:19:21.764928 carbon_python_sdk-0.1.9/carbon/model/webhook_no_key.pyi
+-rw-r--r--   0        0        0      995 2024-03-14 20:19:21.765075 carbon_python_sdk-0.1.9/carbon/model/webhook_order_by_columns.py
+-rw-r--r--   0        0        0      852 2024-03-14 20:19:21.765220 carbon_python_sdk-0.1.9/carbon/model/webhook_order_by_columns.pyi
+-rw-r--r--   0        0        0     4347 2024-03-14 20:19:21.765415 carbon_python_sdk-0.1.9/carbon/model/webhook_query_input.py
+-rw-r--r--   0        0        0     4347 2024-03-14 20:19:21.765614 carbon_python_sdk-0.1.9/carbon/model/webhook_query_input.pyi
+-rw-r--r--   0        0        0     3798 2024-03-14 20:19:21.765778 carbon_python_sdk-0.1.9/carbon/model/webhook_query_response.py
+-rw-r--r--   0        0        0     3798 2024-03-14 20:19:21.765900 carbon_python_sdk-0.1.9/carbon/model/webhook_query_response.pyi
+-rw-r--r--   0        0        0    16894 2024-03-14 20:21:24.401013 carbon_python_sdk-0.1.9/carbon/model/webscrape_request.py
+-rw-r--r--   0        0        0    16810 2024-03-14 20:21:24.401165 carbon_python_sdk-0.1.9/carbon/model/webscrape_request.pyi
+-rw-r--r--   0        0        0     1105 2024-03-14 20:19:21.766551 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0     1105 2024-03-14 20:19:21.766679 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_classes_to_skip.pyi
+-rw-r--r--   0        0        0     1109 2024-03-14 20:19:21.766826 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0     1109 2024-03-14 20:19:21.766949 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_selectors_to_skip.pyi
+-rw-r--r--   0        0        0     1101 2024-03-14 20:19:21.767069 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0     1101 2024-03-14 20:19:21.767204 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_html_tags_to_skip.pyi
+-rw-r--r--   0        0        0     6384 2024-03-14 20:19:21.767422 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_tags.py
+-rw-r--r--   0        0        0     6384 2024-03-14 20:19:21.767648 carbon_python_sdk-0.1.9/carbon/model/webscrape_request_tags.pyi
+-rw-r--r--   0        0        0     3117 2024-03-14 20:19:21.767881 carbon_python_sdk-0.1.9/carbon/model/white_labeling_response.py
+-rw-r--r--   0        0        0     3117 2024-03-14 20:19:21.768084 carbon_python_sdk-0.1.9/carbon/model/white_labeling_response.pyi
+-rw-r--r--   0        0        0     5401 2024-03-14 20:19:21.768365 carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response.py
+-rw-r--r--   0        0        0     5401 2024-03-14 20:19:21.768629 carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response.pyi
+-rw-r--r--   0        0        0     1375 2024-03-14 20:19:21.768813 carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0     1375 2024-03-14 20:19:21.769014 carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript.pyi
+-rw-r--r--   0        0        0     3326 2024-03-14 20:19:21.769176 carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0     3326 2024-03-14 20:19:21.769430 carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript_item.pyi
+-rw-r--r--   0        0        0     3653 2024-03-14 20:21:24.401362 carbon_python_sdk-0.1.9/carbon/model/zendesk_authentication.py
+-rw-r--r--   0        0        0     3653 2024-03-14 20:21:24.401483 carbon_python_sdk-0.1.9/carbon/model/zendesk_authentication.pyi
+-rw-r--r--   0        0        0     4907 2024-03-14 20:21:24.401650 carbon_python_sdk-0.1.9/carbon/model/zotero_authentication.py
+-rw-r--r--   0        0        0     4907 2024-03-14 20:21:24.401808 carbon_python_sdk-0.1.9/carbon/model/zotero_authentication.pyi
+-rw-r--r--   0        0        0    11378 2024-03-14 20:21:24.402114 carbon_python_sdk-0.1.9/carbon/models/__init__.py
+-rw-r--r--   0        0        0    20672 2024-03-14 20:21:24.402300 carbon_python_sdk-0.1.9/carbon/operation_parameter_map.py
+-rw-r--r--   0        0        0     2784 2024-03-14 20:21:24.402483 carbon_python_sdk-0.1.9/carbon/paths/__init__.py
+-rw-r--r--   0        0        0      293 2024-03-14 20:19:21.771374 carbon_python_sdk-0.1.9/carbon/paths/add_webhook/__init__.py
+-rw-r--r--   0        0        0    13953 2024-03-14 20:19:21.771498 carbon_python_sdk-0.1.9/carbon/paths/add_webhook/post.py
+-rw-r--r--   0        0        0    13811 2024-03-14 20:19:21.771847 carbon_python_sdk-0.1.9/carbon/paths/add_webhook/post.pyi
+-rw-r--r--   0        0        0      311 2024-03-14 20:19:21.772205 carbon_python_sdk-0.1.9/carbon/paths/auth_v1_access_token/__init__.py
+-rw-r--r--   0        0        0    11830 2024-03-14 20:19:21.772319 carbon_python_sdk-0.1.9/carbon/paths/auth_v1_access_token/get.py
+-rw-r--r--   0        0        0    11656 2024-03-14 20:19:21.772525 carbon_python_sdk-0.1.9/carbon/paths/auth_v1_access_token/get.pyi
+-rw-r--r--   0        0        0      315 2024-03-14 20:19:21.772767 carbon_python_sdk-0.1.9/carbon/paths/auth_v1_white_labeling/__init__.py
+-rw-r--r--   0        0        0    11983 2024-03-14 20:19:21.772887 carbon_python_sdk-0.1.9/carbon/paths/auth_v1_white_labeling/get.py
+-rw-r--r--   0        0        0    11841 2024-03-14 20:19:21.773104 carbon_python_sdk-0.1.9/carbon/paths/auth_v1_white_labeling/get.pyi
+-rw-r--r--   0        0        0      313 2024-03-14 20:19:21.773304 carbon_python_sdk-0.1.9/carbon/paths/create_user_file_tags/__init__.py
+-rw-r--r--   0        0        0    15880 2024-03-14 20:19:21.773411 carbon_python_sdk-0.1.9/carbon/paths/create_user_file_tags/post.py
+-rw-r--r--   0        0        0    15706 2024-03-14 20:19:21.773671 carbon_python_sdk-0.1.9/carbon/paths/create_user_file_tags/post.pyi
+-rw-r--r--   0        0        0      295 2024-03-14 20:19:21.773922 carbon_python_sdk-0.1.9/carbon/paths/delete_files/__init__.py
+-rw-r--r--   0        0        0    18977 2024-03-14 20:19:21.774055 carbon_python_sdk-0.1.9/carbon/paths/delete_files/post.py
+-rw-r--r--   0        0        0    18803 2024-03-14 20:19:21.774201 carbon_python_sdk-0.1.9/carbon/paths/delete_files/post.pyi
+-rw-r--r--   0        0        0      313 2024-03-14 20:19:21.774332 carbon_python_sdk-0.1.9/carbon/paths/delete_user_file_tags/__init__.py
+-rw-r--r--   0        0        0    15814 2024-03-14 20:19:21.774478 carbon_python_sdk-0.1.9/carbon/paths/delete_user_file_tags/post.py
+-rw-r--r--   0        0        0    15640 2024-03-14 20:19:21.774788 carbon_python_sdk-0.1.9/carbon/paths/delete_user_file_tags/post.pyi
+-rw-r--r--   0        0        0      295 2024-03-14 20:19:21.775083 carbon_python_sdk-0.1.9/carbon/paths/delete_users/__init__.py
+-rw-r--r--   0        0        0    14904 2024-03-14 20:19:21.775203 carbon_python_sdk-0.1.9/carbon/paths/delete_users/post.py
+-rw-r--r--   0        0        0    14762 2024-03-14 20:19:21.775495 carbon_python_sdk-0.1.9/carbon/paths/delete_users/post.pyi
+-rw-r--r--   0        0        0      321 2024-03-14 20:19:21.775767 carbon_python_sdk-0.1.9/carbon/paths/delete_webhook_webhook_id/__init__.py
+-rw-r--r--   0        0        0    14364 2024-03-14 20:19:21.775886 carbon_python_sdk-0.1.9/carbon/paths/delete_webhook_webhook_id/delete.py
+-rw-r--r--   0        0        0    14222 2024-03-14 20:19:21.776144 carbon_python_sdk-0.1.9/carbon/paths/delete_webhook_webhook_id/delete.pyi
+-rw-r--r--   0        0        0      307 2024-03-14 20:19:21.776397 carbon_python_sdk-0.1.9/carbon/paths/deletefile_file_id/__init__.py
+-rw-r--r--   0        0        0    14552 2024-03-14 20:19:21.776521 carbon_python_sdk-0.1.9/carbon/paths/deletefile_file_id/delete.py
+-rw-r--r--   0        0        0    14378 2024-03-14 20:19:21.776772 carbon_python_sdk-0.1.9/carbon/paths/deletefile_file_id/delete.pyi
+-rw-r--r--   0        0        0      291 2024-03-14 20:19:21.777027 carbon_python_sdk-0.1.9/carbon/paths/embeddings/__init__.py
+-rw-r--r--   0        0        0    28339 2024-03-14 20:19:21.777158 carbon_python_sdk-0.1.9/carbon/paths/embeddings/post.py
+-rw-r--r--   0        0        0    28165 2024-03-14 20:19:21.777313 carbon_python_sdk-0.1.9/carbon/paths/embeddings/post.pyi
+-rw-r--r--   0        0        0      291 2024-03-14 20:19:21.777440 carbon_python_sdk-0.1.9/carbon/paths/fetch_urls/__init__.py
+-rw-r--r--   0        0        0    14466 2024-03-14 20:19:21.777558 carbon_python_sdk-0.1.9/carbon/paths/fetch_urls/get.py
+-rw-r--r--   0        0        0    14292 2024-03-14 20:19:21.777835 carbon_python_sdk-0.1.9/carbon/paths/fetch_urls/get.pyi
+-rw-r--r--   0        0        0      319 2024-03-14 20:19:21.778084 carbon_python_sdk-0.1.9/carbon/paths/fetch_youtube_transcript/__init__.py
+-rw-r--r--   0        0        0    15695 2024-03-14 20:19:21.778198 carbon_python_sdk-0.1.9/carbon/paths/fetch_youtube_transcript/get.py
+-rw-r--r--   0        0        0    15521 2024-03-14 20:19:21.778627 carbon_python_sdk-0.1.9/carbon/paths/fetch_youtube_transcript/get.pyi
+-rw-r--r--   0        0        0      283 2024-03-14 20:19:21.778895 carbon_python_sdk-0.1.9/carbon/paths/health/__init__.py
+-rw-r--r--   0        0        0    10429 2024-03-14 20:19:21.779020 carbon_python_sdk-0.1.9/carbon/paths/health/get.py
+-rw-r--r--   0        0        0    10348 2024-03-14 20:19:21.779234 carbon_python_sdk-0.1.9/carbon/paths/health/get.pyi
+-rw-r--r--   0        0        0      327 2024-03-14 20:19:21.779444 carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_list/__init__.py
+-rw-r--r--   0        0        0    15289 2024-03-14 20:19:21.779552 carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_list/post.py
+-rw-r--r--   0        0        0    15115 2024-03-14 20:19:21.779797 carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_list/post.pyi
+-rw-r--r--   0        0        0      327 2024-03-14 20:19:21.780051 carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_sync/__init__.py
+-rw-r--r--   0        0        0    24653 2024-03-14 20:19:21.780177 carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_sync/post.py
+-rw-r--r--   0        0        0    24479 2024-03-14 20:19:21.780320 carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_sync/post.pyi
+-rw-r--r--   0        0        0      311 2024-03-14 20:21:24.402578 carbon_python_sdk-0.1.9/carbon/paths/integrations_connect/__init__.py
+-rw-r--r--   0        0        0    20264 2024-03-14 20:21:24.402676 carbon_python_sdk-0.1.9/carbon/paths/integrations_connect/post.py
+-rw-r--r--   0        0        0    20090 2024-03-14 20:21:24.402793 carbon_python_sdk-0.1.9/carbon/paths/integrations_connect/post.pyi
+-rw-r--r--   0        0        0      317 2024-03-14 20:19:21.780878 carbon_python_sdk-0.1.9/carbon/paths/integrations_files_sync/__init__.py
+-rw-r--r--   0        0        0    24538 2024-03-14 20:19:21.780999 carbon_python_sdk-0.1.9/carbon/paths/integrations_files_sync/post.py
+-rw-r--r--   0        0        0    24364 2024-03-14 20:19:21.781143 carbon_python_sdk-0.1.9/carbon/paths/integrations_files_sync/post.pyi
+-rw-r--r--   0        0        0      315 2024-03-14 20:19:21.781273 carbon_python_sdk-0.1.9/carbon/paths/integrations_freshdesk/__init__.py
+-rw-r--r--   0        0        0    23357 2024-03-14 20:19:21.781397 carbon_python_sdk-0.1.9/carbon/paths/integrations_freshdesk/post.py
+-rw-r--r--   0        0        0    23183 2024-03-14 20:19:21.781533 carbon_python_sdk-0.1.9/carbon/paths/integrations_freshdesk/post.pyi
+-rw-r--r--   0        0        0      311 2024-03-14 20:19:21.781655 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook/__init__.py
+-rw-r--r--   0        0        0    23400 2024-03-14 20:19:21.781782 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook/post.py
+-rw-r--r--   0        0        0    23226 2024-03-14 20:19:21.781924 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook/post.pyi
+-rw-r--r--   0        0        0      325 2024-03-14 20:19:21.782051 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_spaces/__init__.py
+-rw-r--r--   0        0        0    14816 2024-03-14 20:19:21.782169 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_spaces/get.py
+-rw-r--r--   0        0        0    14642 2024-03-14 20:19:21.782421 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_spaces/get.pyi
+-rw-r--r--   0        0        0      321 2024-03-14 20:19:21.782671 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_sync/__init__.py
+-rw-r--r--   0        0        0    22421 2024-03-14 20:19:21.782796 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_sync/post.py
+-rw-r--r--   0        0        0    22247 2024-03-14 20:19:21.782930 carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_sync/post.pyi
+-rw-r--r--   0        0        0      317 2024-03-14 20:19:21.783056 carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_sync/__init__.py
+-rw-r--r--   0        0        0    22959 2024-03-14 20:19:21.783180 carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_sync/post.py
+-rw-r--r--   0        0        0    22785 2024-03-14 20:19:21.783333 carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_sync/post.pyi
+-rw-r--r--   0        0        0      331 2024-03-14 20:19:21.783456 carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_user_labels/__init__.py
+-rw-r--r--   0        0        0    15340 2024-03-14 20:19:21.783566 carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_user_labels/get.py
+-rw-r--r--   0        0        0    15166 2024-03-14 20:19:21.783817 carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_user_labels/get.pyi
+-rw-r--r--   0        0        0      317 2024-03-14 20:19:21.784060 carbon_python_sdk-0.1.9/carbon/paths/integrations_items_list/__init__.py
+-rw-r--r--   0        0        0    16639 2024-03-14 20:19:21.784176 carbon_python_sdk-0.1.9/carbon/paths/integrations_items_list/post.py
+-rw-r--r--   0        0        0    16465 2024-03-14 20:19:21.784317 carbon_python_sdk-0.1.9/carbon/paths/integrations_items_list/post.pyi
+-rw-r--r--   0        0        0      317 2024-03-14 20:19:21.784451 carbon_python_sdk-0.1.9/carbon/paths/integrations_items_sync/__init__.py
+-rw-r--r--   0        0        0    14992 2024-03-14 20:19:21.784566 carbon_python_sdk-0.1.9/carbon/paths/integrations_items_sync/post.py
+-rw-r--r--   0        0        0    14818 2024-03-14 20:19:21.784825 carbon_python_sdk-0.1.9/carbon/paths/integrations_items_sync/post.pyi
+-rw-r--r--   0        0        0      315 2024-03-14 20:19:21.785081 carbon_python_sdk-0.1.9/carbon/paths/integrations_oauth_url/__init__.py
+-rw-r--r--   0        0        0    31689 2024-03-14 20:19:21.785209 carbon_python_sdk-0.1.9/carbon/paths/integrations_oauth_url/post.py
+-rw-r--r--   0        0        0    31515 2024-03-14 20:19:21.785363 carbon_python_sdk-0.1.9/carbon/paths/integrations_oauth_url/post.pyi
+-rw-r--r--   0        0        0      321 2024-03-14 20:19:21.785509 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_sync/__init__.py
+-rw-r--r--   0        0        0    23693 2024-03-14 20:19:21.785635 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_sync/post.py
+-rw-r--r--   0        0        0    23519 2024-03-14 20:19:21.785766 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_sync/post.pyi
+-rw-r--r--   0        0        0      343 2024-03-14 20:19:21.785984 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_categories/__init__.py
+-rw-r--r--   0        0        0    15590 2024-03-14 20:19:21.786094 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_categories/get.py
+-rw-r--r--   0        0        0    15416 2024-03-14 20:19:21.786351 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_categories/get.pyi
+-rw-r--r--   0        0        0      337 2024-03-14 20:19:21.786631 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_folders/__init__.py
+-rw-r--r--   0        0        0    15371 2024-03-14 20:19:21.786936 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_folders/get.py
+-rw-r--r--   0        0        0    15197 2024-03-14 20:19:21.787214 carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_folders/get.pyi
+-rw-r--r--   0        0        0      313 2024-03-14 20:19:21.789328 carbon_python_sdk-0.1.9/carbon/paths/integrations_rss_feed/__init__.py
+-rw-r--r--   0        0        0    21466 2024-03-14 20:19:21.789610 carbon_python_sdk-0.1.9/carbon/paths/integrations_rss_feed/post.py
+-rw-r--r--   0        0        0    21292 2024-03-14 20:19:21.789829 carbon_python_sdk-0.1.9/carbon/paths/integrations_rss_feed/post.pyi
+-rw-r--r--   0        0        0      301 2024-03-14 20:19:21.790045 carbon_python_sdk-0.1.9/carbon/paths/integrations_s3/__init__.py
+-rw-r--r--   0        0        0    15336 2024-03-14 20:19:21.790238 carbon_python_sdk-0.1.9/carbon/paths/integrations_s3/post.py
+-rw-r--r--   0        0        0    15162 2024-03-14 20:19:21.790720 carbon_python_sdk-0.1.9/carbon/paths/integrations_s3/post.pyi
+-rw-r--r--   0        0        0      313 2024-03-14 20:19:21.791079 carbon_python_sdk-0.1.9/carbon/paths/integrations_s3_files/__init__.py
+-rw-r--r--   0        0        0    24552 2024-03-14 20:19:21.791338 carbon_python_sdk-0.1.9/carbon/paths/integrations_s3_files/post.py
+-rw-r--r--   0        0        0    24378 2024-03-14 20:19:21.791542 carbon_python_sdk-0.1.9/carbon/paths/integrations_s3_files/post.pyi
+-rw-r--r--   0        0        0      321 2024-03-14 20:19:21.791783 carbon_python_sdk-0.1.9/carbon/paths/modify_user_configuration/__init__.py
+-rw-r--r--   0        0        0    16052 2024-03-14 20:19:21.791964 carbon_python_sdk-0.1.9/carbon/paths/modify_user_configuration/post.py
+-rw-r--r--   0        0        0    15878 2024-03-14 20:19:21.792261 carbon_python_sdk-0.1.9/carbon/paths/modify_user_configuration/post.pyi
+-rw-r--r--   0        0        0      295 2024-03-14 20:19:21.792642 carbon_python_sdk-0.1.9/carbon/paths/organization/__init__.py
+-rw-r--r--   0        0        0    11658 2024-03-14 20:19:21.792888 carbon_python_sdk-0.1.9/carbon/paths/organization/get.py
+-rw-r--r--   0        0        0    11516 2024-03-14 20:19:21.793144 carbon_python_sdk-0.1.9/carbon/paths/organization/get.pyi
+-rw-r--r--   0        0        0      309 2024-03-14 20:19:21.793397 carbon_python_sdk-0.1.9/carbon/paths/parsed_file_file_id/__init__.py
+-rw-r--r--   0        0        0    14654 2024-03-14 20:19:21.793589 carbon_python_sdk-0.1.9/carbon/paths/parsed_file_file_id/get.py
+-rw-r--r--   0        0        0    14480 2024-03-14 20:19:21.793911 carbon_python_sdk-0.1.9/carbon/paths/parsed_file_file_id/get.pyi
+-rw-r--r--   0        0        0      301 2024-03-14 20:19:21.794322 carbon_python_sdk-0.1.9/carbon/paths/process_sitemap/__init__.py
+-rw-r--r--   0        0        0    14363 2024-03-14 20:19:21.794851 carbon_python_sdk-0.1.9/carbon/paths/process_sitemap/get.py
+-rw-r--r--   0        0        0    14189 2024-03-14 20:19:21.795238 carbon_python_sdk-0.1.9/carbon/paths/process_sitemap/get.pyi
+-rw-r--r--   0        0        0      303 2024-03-14 20:19:21.795661 carbon_python_sdk-0.1.9/carbon/paths/raw_file_file_id/__init__.py
+-rw-r--r--   0        0        0    14585 2024-03-14 20:19:21.795951 carbon_python_sdk-0.1.9/carbon/paths/raw_file_file_id/get.py
+-rw-r--r--   0        0        0    14411 2024-03-14 20:19:21.796430 carbon_python_sdk-0.1.9/carbon/paths/raw_file_file_id/get.pyi
+-rw-r--r--   0        0        0      293 2024-03-14 20:19:21.796791 carbon_python_sdk-0.1.9/carbon/paths/resync_file/__init__.py
+-rw-r--r--   0        0        0    16696 2024-03-14 20:19:21.797003 carbon_python_sdk-0.1.9/carbon/paths/resync_file/post.py
+-rw-r--r--   0        0        0    16522 2024-03-14 20:19:21.799209 carbon_python_sdk-0.1.9/carbon/paths/resync_file/post.pyi
+-rw-r--r--   0        0        0      309 2024-03-14 20:19:21.799489 carbon_python_sdk-0.1.9/carbon/paths/revoke_access_token/__init__.py
+-rw-r--r--   0        0        0    14828 2024-03-14 20:19:21.799856 carbon_python_sdk-0.1.9/carbon/paths/revoke_access_token/post.py
+-rw-r--r--   0        0        0    14654 2024-03-14 20:19:21.800227 carbon_python_sdk-0.1.9/carbon/paths/revoke_access_token/post.pyi
+-rw-r--r--   0        0        0      299 2024-03-14 20:19:21.800634 carbon_python_sdk-0.1.9/carbon/paths/scrape_sitemap/__init__.py
+-rw-r--r--   0        0        0    27300 2024-03-14 20:19:21.800889 carbon_python_sdk-0.1.9/carbon/paths/scrape_sitemap/post.py
+-rw-r--r--   0        0        0    27126 2024-03-14 20:19:21.801226 carbon_python_sdk-0.1.9/carbon/paths/scrape_sitemap/post.pyi
+-rw-r--r--   0        0        0      293 2024-03-14 20:19:21.801484 carbon_python_sdk-0.1.9/carbon/paths/search_urls/__init__.py
+-rw-r--r--   0        0        0    14549 2024-03-14 20:19:21.801908 carbon_python_sdk-0.1.9/carbon/paths/search_urls/get.py
+-rw-r--r--   0        0        0    14375 2024-03-14 20:19:21.802350 carbon_python_sdk-0.1.9/carbon/paths/search_urls/get.pyi
+-rw-r--r--   0        0        0      293 2024-03-14 20:19:21.802765 carbon_python_sdk-0.1.9/carbon/paths/text_chunks/__init__.py
+-rw-r--r--   0        0        0    19073 2024-03-14 20:19:21.803018 carbon_python_sdk-0.1.9/carbon/paths/text_chunks/post.py
+-rw-r--r--   0        0        0    18899 2024-03-14 20:19:21.803411 carbon_python_sdk-0.1.9/carbon/paths/text_chunks/post.pyi
+-rw-r--r--   0        0        0      327 2024-03-14 20:19:21.803607 carbon_python_sdk-0.1.9/carbon/paths/upload_chunks_and_embeddings/__init__.py
+-rw-r--r--   0        0        0    19841 2024-03-14 20:19:21.803858 carbon_python_sdk-0.1.9/carbon/paths/upload_chunks_and_embeddings/post.py
+-rw-r--r--   0        0        0    19667 2024-03-14 20:19:21.804148 carbon_python_sdk-0.1.9/carbon/paths/upload_chunks_and_embeddings/post.pyi
+-rw-r--r--   0        0        0      311 2024-03-14 20:19:21.804395 carbon_python_sdk-0.1.9/carbon/paths/upload_file_from_url/__init__.py
+-rw-r--r--   0        0        0    23090 2024-03-14 20:19:21.804659 carbon_python_sdk-0.1.9/carbon/paths/upload_file_from_url/post.py
+-rw-r--r--   0        0        0    22916 2024-03-14 20:19:21.804911 carbon_python_sdk-0.1.9/carbon/paths/upload_file_from_url/post.pyi
+-rw-r--r--   0        0        0      293 2024-03-14 20:19:21.805101 carbon_python_sdk-0.1.9/carbon/paths/upload_text/__init__.py
+-rw-r--r--   0        0        0    20504 2024-03-14 20:19:21.805305 carbon_python_sdk-0.1.9/carbon/paths/upload_text/post.py
+-rw-r--r--   0        0        0    20330 2024-03-14 20:19:21.805530 carbon_python_sdk-0.1.9/carbon/paths/upload_text/post.pyi
+-rw-r--r--   0        0        0      291 2024-03-14 20:19:21.805673 carbon_python_sdk-0.1.9/carbon/paths/uploadfile/__init__.py
+-rw-r--r--   0        0        0    29353 2024-03-14 20:19:21.805807 carbon_python_sdk-0.1.9/carbon/paths/uploadfile/post.py
+-rw-r--r--   0        0        0    29179 2024-03-14 20:19:21.805945 carbon_python_sdk-0.1.9/carbon/paths/uploadfile/post.pyi
+-rw-r--r--   0        0        0      279 2024-03-14 20:19:21.806066 carbon_python_sdk-0.1.9/carbon/paths/user/__init__.py
+-rw-r--r--   0        0        0    14161 2024-03-14 20:19:21.806194 carbon_python_sdk-0.1.9/carbon/paths/user/post.py
+-rw-r--r--   0        0        0    14019 2024-03-14 20:19:21.806506 carbon_python_sdk-0.1.9/carbon/paths/user/post.pyi
+-rw-r--r--   0        0        0      305 2024-03-14 20:19:21.806807 carbon_python_sdk-0.1.9/carbon/paths/user_data_sources/__init__.py
+-rw-r--r--   0        0        0    18865 2024-03-14 20:19:21.806936 carbon_python_sdk-0.1.9/carbon/paths/user_data_sources/post.py
+-rw-r--r--   0        0        0    18691 2024-03-14 20:19:21.807083 carbon_python_sdk-0.1.9/carbon/paths/user_data_sources/post.pyi
+-rw-r--r--   0        0        0      291 2024-03-14 20:19:21.807211 carbon_python_sdk-0.1.9/carbon/paths/user_files/__init__.py
+-rw-r--r--   0        0        0    22374 2024-03-14 20:19:21.807330 carbon_python_sdk-0.1.9/carbon/paths/user_files/post.py
+-rw-r--r--   0        0        0    22200 2024-03-14 20:19:21.807477 carbon_python_sdk-0.1.9/carbon/paths/user_files/post.pyi
+-rw-r--r--   0        0        0      297 2024-03-14 20:19:21.807608 carbon_python_sdk-0.1.9/carbon/paths/user_files_v2/__init__.py
+-rw-r--r--   0        0        0    21370 2024-03-14 20:19:21.807723 carbon_python_sdk-0.1.9/carbon/paths/user_files_v2/post.py
+-rw-r--r--   0        0        0    21196 2024-03-14 20:19:21.807848 carbon_python_sdk-0.1.9/carbon/paths/user_files_v2/post.pyi
+-rw-r--r--   0        0        0      291 2024-03-14 20:19:21.807965 carbon_python_sdk-0.1.9/carbon/paths/web_scrape/__init__.py
+-rw-r--r--   0        0        0    14274 2024-03-14 20:19:21.808080 carbon_python_sdk-0.1.9/carbon/paths/web_scrape/post.py
+-rw-r--r--   0        0        0    14100 2024-03-14 20:19:21.808341 carbon_python_sdk-0.1.9/carbon/paths/web_scrape/post.pyi
+-rw-r--r--   0        0        0      287 2024-03-14 20:19:21.808598 carbon_python_sdk-0.1.9/carbon/paths/webhooks/__init__.py
+-rw-r--r--   0        0        0    17372 2024-03-14 20:19:21.808709 carbon_python_sdk-0.1.9/carbon/paths/webhooks/post.py
+-rw-r--r--   0        0        0    17230 2024-03-14 20:19:21.808840 carbon_python_sdk-0.1.9/carbon/paths/webhooks/post.pyi
+-rw-r--r--   0        0        0        0 2024-03-14 20:19:21.808998 carbon_python_sdk-0.1.9/carbon/pydantic/__init__.py
+-rw-r--r--   0        0        0      496 2024-03-14 20:19:21.809109 carbon_python_sdk-0.1.9/carbon/pydantic/add_webhook_props.py
+-rw-r--r--   0        0        0      523 2024-03-14 20:19:21.809214 carbon_python_sdk-0.1.9/carbon/pydantic/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0      697 2024-03-14 20:19:21.809319 carbon_python_sdk-0.1.9/carbon/pydantic/chunk_properties.py
+-rw-r--r--   0        0        0      705 2024-03-14 20:19:21.809424 carbon_python_sdk-0.1.9/carbon/pydantic/chunk_properties_nullable.py
+-rw-r--r--   0        0        0      758 2024-03-14 20:19:21.809523 carbon_python_sdk-0.1.9/carbon/pydantic/chunks_and_embeddings.py
+-rw-r--r--   0        0        0      457 2024-03-14 20:19:21.809639 carbon_python_sdk-0.1.9/carbon/pydantic/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1180 2024-03-14 20:19:21.809755 carbon_python_sdk-0.1.9/carbon/pydantic/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0      406 2024-03-14 20:19:21.809863 carbon_python_sdk-0.1.9/carbon/pydantic/configuration_keys.py
+-rw-r--r--   0        0        0      772 2024-03-14 20:21:24.402931 carbon_python_sdk-0.1.9/carbon/pydantic/confluence_authentication.py
+-rw-r--r--   0        0        0     1635 2024-03-14 20:21:24.403027 carbon_python_sdk-0.1.9/carbon/pydantic/connect_data_source_input.py
+-rw-r--r--   0        0        0      702 2024-03-14 20:21:24.403115 carbon_python_sdk-0.1.9/carbon/pydantic/connect_data_source_response.py
+-rw-r--r--   0        0        0      444 2024-03-14 20:19:21.810321 carbon_python_sdk-0.1.9/carbon/pydantic/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      460 2024-03-14 20:19:21.810454 carbon_python_sdk-0.1.9/carbon/pydantic/data_source_sync_statuses.py
+-rw-r--r--   0        0        0      802 2024-03-14 20:19:21.810592 carbon_python_sdk-0.1.9/carbon/pydantic/data_source_type.py
+-rw-r--r--   0        0        0      810 2024-03-14 20:19:21.810707 carbon_python_sdk-0.1.9/carbon/pydantic/data_source_type_nullable.py
+-rw-r--r--   0        0        0     1124 2024-03-14 20:19:21.810810 carbon_python_sdk-0.1.9/carbon/pydantic/delete_files_query_input.py
+-rw-r--r--   0        0        0      436 2024-03-14 20:19:21.810915 carbon_python_sdk-0.1.9/carbon/pydantic/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0      627 2024-03-14 20:19:21.811022 carbon_python_sdk-0.1.9/carbon/pydantic/delete_users_input.py
+-rw-r--r--   0        0        0      418 2024-03-14 20:19:21.811128 carbon_python_sdk-0.1.9/carbon/pydantic/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0      631 2024-03-14 20:19:21.811228 carbon_python_sdk-0.1.9/carbon/pydantic/directory_item.py
+-rw-r--r--   0        0        0     1469 2024-03-14 20:19:21.811329 carbon_python_sdk-0.1.9/carbon/pydantic/document_response.py
+-rw-r--r--   0        0        0      602 2024-03-14 20:19:21.811445 carbon_python_sdk-0.1.9/carbon/pydantic/document_response_list.py
+-rw-r--r--   0        0        0      399 2024-03-14 20:19:21.811558 carbon_python_sdk-0.1.9/carbon/pydantic/document_response_tags.py
+-rw-r--r--   0        0        0      451 2024-03-14 20:19:21.811669 carbon_python_sdk-0.1.9/carbon/pydantic/document_response_vector.py
+-rw-r--r--   0        0        0      796 2024-03-14 20:19:21.811799 carbon_python_sdk-0.1.9/carbon/pydantic/embedding_and_chunk.py
+-rw-r--r--   0        0        0      455 2024-03-14 20:19:21.811922 carbon_python_sdk-0.1.9/carbon/pydantic/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0      715 2024-03-14 20:19:21.812031 carbon_python_sdk-0.1.9/carbon/pydantic/embedding_generators.py
+-rw-r--r--   0        0        0      723 2024-03-14 20:19:21.812136 carbon_python_sdk-0.1.9/carbon/pydantic/embedding_generators_nullable.py
+-rw-r--r--   0        0        0      603 2024-03-14 20:19:21.812236 carbon_python_sdk-0.1.9/carbon/pydantic/embedding_properties.py
+-rw-r--r--   0        0        0      717 2024-03-14 20:19:21.812348 carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0      458 2024-03-14 20:19:21.812459 carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0     1159 2024-03-14 20:19:21.812681 carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0      648 2024-03-14 20:19:21.812919 carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0      541 2024-03-14 20:19:21.813078 carbon_python_sdk-0.1.9/carbon/pydantic/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1647 2024-03-14 20:19:21.813217 carbon_python_sdk-0.1.9/carbon/pydantic/external_source_item.py
+-rw-r--r--   0        0        0      646 2024-03-14 20:19:21.813343 carbon_python_sdk-0.1.9/carbon/pydantic/fetch_urls_response.py
+-rw-r--r--   0        0        0      412 2024-03-14 20:19:21.813447 carbon_python_sdk-0.1.9/carbon/pydantic/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0      415 2024-03-14 20:19:21.813562 carbon_python_sdk-0.1.9/carbon/pydantic/file_content_types.py
+-rw-r--r--   0        0        0      423 2024-03-14 20:19:21.813666 carbon_python_sdk-0.1.9/carbon/pydantic/file_content_types_nullable.py
+-rw-r--r--   0        0        0      740 2024-03-14 20:19:21.813779 carbon_python_sdk-0.1.9/carbon/pydantic/file_formats.py
+-rw-r--r--   0        0        0      748 2024-03-14 20:19:21.813914 carbon_python_sdk-0.1.9/carbon/pydantic/file_formats_nullable.py
+-rw-r--r--   0        0        0      875 2024-03-14 20:19:21.814026 carbon_python_sdk-0.1.9/carbon/pydantic/file_statistics.py
+-rw-r--r--   0        0        0      883 2024-03-14 20:19:21.814151 carbon_python_sdk-0.1.9/carbon/pydantic/file_statistics_nullable.py
+-rw-r--r--   0        0        0      480 2024-03-14 20:19:21.814292 carbon_python_sdk-0.1.9/carbon/pydantic/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1566 2024-03-14 20:19:21.814422 carbon_python_sdk-0.1.9/carbon/pydantic/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0      660 2024-03-14 20:21:24.403203 carbon_python_sdk-0.1.9/carbon/pydantic/freskdesk_authentication.py
+-rw-r--r--   0        0        0      512 2024-03-14 20:19:21.814659 carbon_python_sdk-0.1.9/carbon/pydantic/generic_success_response.py
+-rw-r--r--   0        0        0     3076 2024-03-14 20:19:21.814790 carbon_python_sdk-0.1.9/carbon/pydantic/get_embedding_documents_body.py
+-rw-r--r--   0        0        0      440 2024-03-14 20:19:21.814923 carbon_python_sdk-0.1.9/carbon/pydantic/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0      446 2024-03-14 20:19:21.815058 carbon_python_sdk-0.1.9/carbon/pydantic/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0      465 2024-03-14 20:19:21.815192 carbon_python_sdk-0.1.9/carbon/pydantic/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0      408 2024-03-14 20:19:21.815356 carbon_python_sdk-0.1.9/carbon/pydantic/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0      689 2024-03-14 20:21:24.403286 carbon_python_sdk-0.1.9/carbon/pydantic/gitbook_authetication.py
+-rw-r--r--   0        0        0     1561 2024-03-14 20:19:21.815614 carbon_python_sdk-0.1.9/carbon/pydantic/gitbook_connect_request.py
+-rw-r--r--   0        0        0     1547 2024-03-14 20:19:21.815734 carbon_python_sdk-0.1.9/carbon/pydantic/gitbook_sync_request.py
+-rw-r--r--   0        0        0      417 2024-03-14 20:19:21.815860 carbon_python_sdk-0.1.9/carbon/pydantic/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0     1554 2024-03-14 20:19:21.815984 carbon_python_sdk-0.1.9/carbon/pydantic/gmail_sync_input.py
+-rw-r--r--   0        0        0      615 2024-03-14 20:19:21.816105 carbon_python_sdk-0.1.9/carbon/pydantic/http_validation_error.py
+-rw-r--r--   0        0        0      602 2024-03-14 20:19:21.816233 carbon_python_sdk-0.1.9/carbon/pydantic/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0      610 2024-03-14 20:19:21.816370 carbon_python_sdk-0.1.9/carbon/pydantic/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0      745 2024-03-14 20:19:21.816644 carbon_python_sdk-0.1.9/carbon/pydantic/list_data_source_items_request.py
+-rw-r--r--   0        0        0      647 2024-03-14 20:19:21.816832 carbon_python_sdk-0.1.9/carbon/pydantic/list_data_source_items_response.py
+-rw-r--r--   0        0        0      601 2024-03-14 20:19:21.816985 carbon_python_sdk-0.1.9/carbon/pydantic/list_request.py
+-rw-r--r--   0        0        0      575 2024-03-14 20:19:21.817111 carbon_python_sdk-0.1.9/carbon/pydantic/list_response.py
+-rw-r--r--   0        0        0      670 2024-03-14 20:19:21.817245 carbon_python_sdk-0.1.9/carbon/pydantic/modify_user_configuration_input.py
+-rw-r--r--   0        0        0      679 2024-03-14 20:21:24.403357 carbon_python_sdk-0.1.9/carbon/pydantic/notion_authentication.py
+-rw-r--r--   0        0        0      751 2024-03-14 20:21:24.403440 carbon_python_sdk-0.1.9/carbon/pydantic/o_auth_authentication.py
+-rw-r--r--   0        0        0     3224 2024-03-14 20:19:21.817669 carbon_python_sdk-0.1.9/carbon/pydantic/o_auth_url_request.py
+-rw-r--r--   0        0        0      405 2024-03-14 20:19:21.817848 carbon_python_sdk-0.1.9/carbon/pydantic/order_dir.py
+-rw-r--r--   0        0        0     1874 2024-03-14 20:19:21.817990 carbon_python_sdk-0.1.9/carbon/pydantic/organization_response.py
+-rw-r--r--   0        0        0     1724 2024-03-14 20:21:24.403571 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_api.py
+-rw-r--r--   0        0        0      935 2024-03-14 20:19:21.818255 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0      444 2024-03-14 20:19:21.818383 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0      450 2024-03-14 20:19:21.818516 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0     1150 2024-03-14 20:19:21.818656 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0      693 2024-03-14 20:19:21.818789 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_response.py
+-rw-r--r--   0        0        0      722 2024-03-14 20:19:21.818927 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0      412 2024-03-14 20:19:21.819179 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0      726 2024-03-14 20:19:21.819359 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0      425 2024-03-14 20:19:21.819494 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     2693 2024-03-14 20:19:21.819615 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0      457 2024-03-14 20:19:21.819735 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0      445 2024-03-14 20:19:21.819872 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0      470 2024-03-14 20:19:21.820070 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0      455 2024-03-14 20:19:21.820218 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0      417 2024-03-14 20:19:21.820396 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0      483 2024-03-14 20:19:21.820545 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1491 2024-03-14 20:19:21.820668 carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0      508 2024-03-14 20:19:21.820773 carbon_python_sdk-0.1.9/carbon/pydantic/outh_url_response.py
+-rw-r--r--   0        0        0     1637 2024-03-14 20:19:21.820894 carbon_python_sdk-0.1.9/carbon/pydantic/outlook_sync_input.py
+-rw-r--r--   0        0        0      582 2024-03-14 20:19:21.821007 carbon_python_sdk-0.1.9/carbon/pydantic/pagination.py
+-rw-r--r--   0        0        0      521 2024-03-14 20:19:21.821121 carbon_python_sdk-0.1.9/carbon/pydantic/presigned_url_response.py
+-rw-r--r--   0        0        0     1278 2024-03-14 20:19:21.821242 carbon_python_sdk-0.1.9/carbon/pydantic/raw_text_input.py
+-rw-r--r--   0        0        0      798 2024-03-14 20:19:21.821357 carbon_python_sdk-0.1.9/carbon/pydantic/resync_file_query_input.py
+-rw-r--r--   0        0        0      525 2024-03-14 20:19:21.821506 carbon_python_sdk-0.1.9/carbon/pydantic/revoke_access_token_input.py
+-rw-r--r--   0        0        0     1363 2024-03-14 20:19:21.821714 carbon_python_sdk-0.1.9/carbon/pydantic/rss_feed_input.py
+-rw-r--r--   0        0        0      571 2024-03-14 20:19:21.821880 carbon_python_sdk-0.1.9/carbon/pydantic/s3_auth_request.py
+-rw-r--r--   0        0        0      681 2024-03-14 20:21:24.403644 carbon_python_sdk-0.1.9/carbon/pydantic/s3_authentication.py
+-rw-r--r--   0        0        0     1748 2024-03-14 20:19:21.822276 carbon_python_sdk-0.1.9/carbon/pydantic/s3_file_sync_input.py
+-rw-r--r--   0        0        0      614 2024-03-14 20:19:21.822388 carbon_python_sdk-0.1.9/carbon/pydantic/s3_get_file_input.py
+-rw-r--r--   0        0        0      766 2024-03-14 20:21:24.403715 carbon_python_sdk-0.1.9/carbon/pydantic/salesforce_authentication.py
+-rw-r--r--   0        0        0      823 2024-03-14 20:21:24.403789 carbon_python_sdk-0.1.9/carbon/pydantic/sharepoint_authentication.py
+-rw-r--r--   0        0        0      482 2024-03-14 20:21:24.403880 carbon_python_sdk-0.1.9/carbon/pydantic/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0      879 2024-03-14 20:19:21.822916 carbon_python_sdk-0.1.9/carbon/pydantic/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     2274 2024-03-14 20:19:21.823405 carbon_python_sdk-0.1.9/carbon/pydantic/sitemap_scrape_request.py
+-rw-r--r--   0        0        0      444 2024-03-14 20:19:21.823629 carbon_python_sdk-0.1.9/carbon/pydantic/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      446 2024-03-14 20:19:21.823786 carbon_python_sdk-0.1.9/carbon/pydantic/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      442 2024-03-14 20:19:21.823971 carbon_python_sdk-0.1.9/carbon/pydantic/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      403 2024-03-14 20:19:21.824097 carbon_python_sdk-0.1.9/carbon/pydantic/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0      523 2024-03-14 20:19:21.824256 carbon_python_sdk-0.1.9/carbon/pydantic/sync_directory_request.py
+-rw-r--r--   0        0        0      534 2024-03-14 20:19:21.824492 carbon_python_sdk-0.1.9/carbon/pydantic/sync_files_ids.py
+-rw-r--r--   0        0        0     1759 2024-03-14 20:19:21.824612 carbon_python_sdk-0.1.9/carbon/pydantic/sync_files_request.py
+-rw-r--r--   0        0        0     1940 2024-03-14 20:21:24.403957 carbon_python_sdk-0.1.9/carbon/pydantic/sync_options.py
+-rw-r--r--   0        0        0      580 2024-03-14 20:19:21.824831 carbon_python_sdk-0.1.9/carbon/pydantic/text_embedding_generators.py
+-rw-r--r--   0        0        0      567 2024-03-14 20:19:21.824936 carbon_python_sdk-0.1.9/carbon/pydantic/token_response.py
+-rw-r--r--   0        0        0     1525 2024-03-14 20:19:21.825044 carbon_python_sdk-0.1.9/carbon/pydantic/upload_file_from_url_input.py
+-rw-r--r--   0        0        0     3106 2024-03-14 20:19:21.825146 carbon_python_sdk-0.1.9/carbon/pydantic/user_file.py
+-rw-r--r--   0        0        0      475 2024-03-14 20:19:21.825255 carbon_python_sdk-0.1.9/carbon/pydantic/user_file_embedding_properties.py
+-rw-r--r--   0        0        0      604 2024-03-14 20:19:21.825373 carbon_python_sdk-0.1.9/carbon/pydantic/user_files_v2.py
+-rw-r--r--   0        0        0      515 2024-03-14 20:19:21.825483 carbon_python_sdk-0.1.9/carbon/pydantic/user_request_content.py
+-rw-r--r--   0        0        0     1343 2024-03-14 20:19:21.825629 carbon_python_sdk-0.1.9/carbon/pydantic/user_response.py
+-rw-r--r--   0        0        0      420 2024-03-14 20:19:21.825781 carbon_python_sdk-0.1.9/carbon/pydantic/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0      492 2024-03-14 20:19:21.825897 carbon_python_sdk-0.1.9/carbon/pydantic/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0      651 2024-03-14 20:19:21.826015 carbon_python_sdk-0.1.9/carbon/pydantic/validation_error.py
+-rw-r--r--   0        0        0      454 2024-03-14 20:19:21.826159 carbon_python_sdk-0.1.9/carbon/pydantic/validation_error_loc.py
+-rw-r--r--   0        0        0      739 2024-03-14 20:19:21.826267 carbon_python_sdk-0.1.9/carbon/pydantic/webhook.py
+-rw-r--r--   0        0        0      598 2024-03-14 20:19:21.826393 carbon_python_sdk-0.1.9/carbon/pydantic/webhook_filters.py
+-rw-r--r--   0        0        0      425 2024-03-14 20:19:21.826687 carbon_python_sdk-0.1.9/carbon/pydantic/webhook_filters_ids.py
+-rw-r--r--   0        0        0      693 2024-03-14 20:19:21.826929 carbon_python_sdk-0.1.9/carbon/pydantic/webhook_no_key.py
+-rw-r--r--   0        0        0      431 2024-03-14 20:19:21.827236 carbon_python_sdk-0.1.9/carbon/pydantic/webhook_order_by_columns.py
+-rw-r--r--   0        0        0     1011 2024-03-14 20:19:21.827370 carbon_python_sdk-0.1.9/carbon/pydantic/webhook_query_input.py
+-rw-r--r--   0        0        0      626 2024-03-14 20:19:21.827580 carbon_python_sdk-0.1.9/carbon/pydantic/webhook_query_response.py
+-rw-r--r--   0        0        0     2317 2024-03-14 20:19:21.827724 carbon_python_sdk-0.1.9/carbon/pydantic/webscrape_request.py
+-rw-r--r--   0        0        0      440 2024-03-14 20:19:21.827883 carbon_python_sdk-0.1.9/carbon/pydantic/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      442 2024-03-14 20:19:21.828055 carbon_python_sdk-0.1.9/carbon/pydantic/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      438 2024-03-14 20:19:21.828189 carbon_python_sdk-0.1.9/carbon/pydantic/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      399 2024-03-14 20:19:21.828313 carbon_python_sdk-0.1.9/carbon/pydantic/webscrape_request_tags.py
+-rw-r--r--   0        0        0      664 2024-03-14 20:19:21.828612 carbon_python_sdk-0.1.9/carbon/pydantic/white_labeling_response.py
+-rw-r--r--   0        0        0      824 2024-03-14 20:19:21.828778 carbon_python_sdk-0.1.9/carbon/pydantic/youtube_transcript_response.py
+-rw-r--r--   0        0        0      604 2024-03-14 20:19:21.828920 carbon_python_sdk-0.1.9/carbon/pydantic/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0      421 2024-03-14 20:19:21.829046 carbon_python_sdk-0.1.9/carbon/pydantic/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0      674 2024-03-14 20:21:24.404036 carbon_python_sdk-0.1.9/carbon/pydantic/zendesk_authentication.py
+-rw-r--r--   0        0        0      785 2024-03-14 20:21:24.404106 carbon_python_sdk-0.1.9/carbon/pydantic/zotero_authentication.py
+-rw-r--r--   0        0        0      654 2024-03-14 20:19:21.829722 carbon_python_sdk-0.1.9/carbon/request_after_hook.py
+-rw-r--r--   0        0        0      712 2024-03-14 20:19:21.829996 carbon_python_sdk-0.1.9/carbon/request_before_hook.py
+-rw-r--r--   0        0        0      677 2024-03-14 20:19:21.830123 carbon_python_sdk-0.1.9/carbon/request_before_url_hook.py
+-rw-r--r--   0        0        0    10974 2024-03-14 20:19:21.830264 carbon_python_sdk-0.1.9/carbon/rest.py
+-rw-r--r--   0        0        0    96042 2024-03-14 20:19:21.830610 carbon_python_sdk-0.1.9/carbon/schemas.py
+-rw-r--r--   0        0        0        0 2024-03-14 20:19:21.830792 carbon_python_sdk-0.1.9/carbon/type/__init__.py
+-rw-r--r--   0        0        0      525 2024-03-14 20:19:21.831044 carbon_python_sdk-0.1.9/carbon/type/add_webhook_props.py
+-rw-r--r--   0        0        0      627 2024-03-14 20:19:21.831206 carbon_python_sdk-0.1.9/carbon/type/body_create_upload_file_uploadfile_post.py
+-rw-r--r--   0        0        0      628 2024-03-14 20:19:21.831489 carbon_python_sdk-0.1.9/carbon/type/chunk_properties.py
+-rw-r--r--   0        0        0      668 2024-03-14 20:19:21.831615 carbon_python_sdk-0.1.9/carbon/type/chunk_properties_nullable.py
+-rw-r--r--   0        0        0      707 2024-03-14 20:19:21.831897 carbon_python_sdk-0.1.9/carbon/type/chunks_and_embeddings.py
+-rw-r--r--   0        0        0      408 2024-03-14 20:19:21.832015 carbon_python_sdk-0.1.9/carbon/type/chunks_and_embeddings_embedding.py
+-rw-r--r--   0        0        0     1030 2024-03-14 20:19:21.832128 carbon_python_sdk-0.1.9/carbon/type/chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0      322 2024-03-14 20:19:21.832239 carbon_python_sdk-0.1.9/carbon/type/configuration_keys.py
+-rw-r--r--   0        0        0      713 2024-03-14 20:21:24.404193 carbon_python_sdk-0.1.9/carbon/type/confluence_authentication.py
+-rw-r--r--   0        0        0     1574 2024-03-14 20:21:24.404280 carbon_python_sdk-0.1.9/carbon/type/connect_data_source_input.py
+-rw-r--r--   0        0        0      733 2024-03-14 20:21:24.404367 carbon_python_sdk-0.1.9/carbon/type/connect_data_source_response.py
+-rw-r--r--   0        0        0      395 2024-03-14 20:19:21.833113 carbon_python_sdk-0.1.9/carbon/type/data_source_last_sync_actions.py
+-rw-r--r--   0        0        0      411 2024-03-14 20:19:21.833415 carbon_python_sdk-0.1.9/carbon/type/data_source_sync_statuses.py
+-rw-r--r--   0        0        0      753 2024-03-14 20:19:21.833539 carbon_python_sdk-0.1.9/carbon/type/data_source_type.py
+-rw-r--r--   0        0        0      761 2024-03-14 20:19:21.833653 carbon_python_sdk-0.1.9/carbon/type/data_source_type_nullable.py
+-rw-r--r--   0        0        0      912 2024-03-14 20:19:21.833866 carbon_python_sdk-0.1.9/carbon/type/delete_files_query_input.py
+-rw-r--r--   0        0        0      387 2024-03-14 20:19:21.834233 carbon_python_sdk-0.1.9/carbon/type/delete_files_query_input_file_ids.py
+-rw-r--r--   0        0        0      647 2024-03-14 20:19:21.834394 carbon_python_sdk-0.1.9/carbon/type/delete_users_input.py
+-rw-r--r--   0        0        0      369 2024-03-14 20:19:21.834521 carbon_python_sdk-0.1.9/carbon/type/delete_users_input_customer_ids.py
+-rw-r--r--   0        0        0      574 2024-03-14 20:19:21.834638 carbon_python_sdk-0.1.9/carbon/type/directory_item.py
+-rw-r--r--   0        0        0     1224 2024-03-14 20:19:21.834817 carbon_python_sdk-0.1.9/carbon/type/document_response.py
+-rw-r--r--   0        0        0      641 2024-03-14 20:19:21.834936 carbon_python_sdk-0.1.9/carbon/type/document_response_list.py
+-rw-r--r--   0        0        0      350 2024-03-14 20:19:21.835052 carbon_python_sdk-0.1.9/carbon/type/document_response_tags.py
+-rw-r--r--   0        0        0      402 2024-03-14 20:19:21.835165 carbon_python_sdk-0.1.9/carbon/type/document_response_vector.py
+-rw-r--r--   0        0        0      732 2024-03-14 20:19:21.835280 carbon_python_sdk-0.1.9/carbon/type/embedding_and_chunk.py
+-rw-r--r--   0        0        0      406 2024-03-14 20:19:21.835392 carbon_python_sdk-0.1.9/carbon/type/embedding_and_chunk_embedding.py
+-rw-r--r--   0        0        0      666 2024-03-14 20:19:21.835501 carbon_python_sdk-0.1.9/carbon/type/embedding_generators.py
+-rw-r--r--   0        0        0      674 2024-03-14 20:19:21.835606 carbon_python_sdk-0.1.9/carbon/type/embedding_generators_nullable.py
+-rw-r--r--   0        0        0      610 2024-03-14 20:19:21.835712 carbon_python_sdk-0.1.9/carbon/type/embedding_properties.py
+-rw-r--r--   0        0        0      711 2024-03-14 20:19:21.835822 carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_filters.py
+-rw-r--r--   0        0        0      409 2024-03-14 20:19:21.835935 carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_order_by_columns.py
+-rw-r--r--   0        0        0     1008 2024-03-14 20:19:21.836047 carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_query_input.py
+-rw-r--r--   0        0        0      694 2024-03-14 20:19:21.836164 carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_response.py
+-rw-r--r--   0        0        0      492 2024-03-14 20:19:21.836272 carbon_python_sdk-0.1.9/carbon/type/external_file_sync_statuses.py
+-rw-r--r--   0        0        0     1149 2024-03-14 20:19:21.836381 carbon_python_sdk-0.1.9/carbon/type/external_source_item.py
+-rw-r--r--   0        0        0      648 2024-03-14 20:19:21.836491 carbon_python_sdk-0.1.9/carbon/type/fetch_urls_response.py
+-rw-r--r--   0        0        0      363 2024-03-14 20:19:21.836616 carbon_python_sdk-0.1.9/carbon/type/fetch_urls_response_urls.py
+-rw-r--r--   0        0        0      366 2024-03-14 20:19:21.849682 carbon_python_sdk-0.1.9/carbon/type/file_content_types.py
+-rw-r--r--   0        0        0      374 2024-03-14 20:19:21.850110 carbon_python_sdk-0.1.9/carbon/type/file_content_types_nullable.py
+-rw-r--r--   0        0        0      691 2024-03-14 20:19:21.850253 carbon_python_sdk-0.1.9/carbon/type/file_formats.py
+-rw-r--r--   0        0        0      699 2024-03-14 20:19:21.850389 carbon_python_sdk-0.1.9/carbon/type/file_formats_nullable.py
+-rw-r--r--   0        0        0      769 2024-03-14 20:19:21.853449 carbon_python_sdk-0.1.9/carbon/type/file_statistics.py
+-rw-r--r--   0        0        0      809 2024-03-14 20:19:21.853593 carbon_python_sdk-0.1.9/carbon/type/file_statistics_nullable.py
+-rw-r--r--   0        0        0      427 2024-03-14 20:19:21.853741 carbon_python_sdk-0.1.9/carbon/type/files_query_user_files_deprecated_response.py
+-rw-r--r--   0        0        0     1117 2024-03-14 20:19:21.853889 carbon_python_sdk-0.1.9/carbon/type/fresh_desk_connect_request.py
+-rw-r--r--   0        0        0      669 2024-03-14 20:21:24.404447 carbon_python_sdk-0.1.9/carbon/type/freskdesk_authentication.py
+-rw-r--r--   0        0        0      565 2024-03-14 20:19:21.854181 carbon_python_sdk-0.1.9/carbon/type/generic_success_response.py
+-rw-r--r--   0        0        0     2436 2024-03-14 20:19:21.854310 carbon_python_sdk-0.1.9/carbon/type/get_embedding_documents_body.py
+-rw-r--r--   0        0        0      391 2024-03-14 20:19:21.854455 carbon_python_sdk-0.1.9/carbon/type/get_embedding_documents_body_file_ids.py
+-rw-r--r--   0        0        0      397 2024-03-14 20:19:21.854771 carbon_python_sdk-0.1.9/carbon/type/get_embedding_documents_body_parent_file_ids.py
+-rw-r--r--   0        0        0      416 2024-03-14 20:19:21.854946 carbon_python_sdk-0.1.9/carbon/type/get_embedding_documents_body_query_vector.py
+-rw-r--r--   0        0        0      359 2024-03-14 20:19:21.855084 carbon_python_sdk-0.1.9/carbon/type/get_embedding_documents_body_tags.py
+-rw-r--r--   0        0        0      670 2024-03-14 20:21:24.404535 carbon_python_sdk-0.1.9/carbon/type/gitbook_authetication.py
+-rw-r--r--   0        0        0     1093 2024-03-14 20:19:21.855332 carbon_python_sdk-0.1.9/carbon/type/gitbook_connect_request.py
+-rw-r--r--   0        0        0     1129 2024-03-14 20:19:21.856897 carbon_python_sdk-0.1.9/carbon/type/gitbook_sync_request.py
+-rw-r--r--   0        0        0      368 2024-03-14 20:19:21.857016 carbon_python_sdk-0.1.9/carbon/type/gitbook_sync_request_space_ids.py
+-rw-r--r--   0        0        0     1103 2024-03-14 20:19:21.857128 carbon_python_sdk-0.1.9/carbon/type/gmail_sync_input.py
+-rw-r--r--   0        0        0      630 2024-03-14 20:19:21.857241 carbon_python_sdk-0.1.9/carbon/type/http_validation_error.py
+-rw-r--r--   0        0        0      636 2024-03-14 20:19:21.857379 carbon_python_sdk-0.1.9/carbon/type/hybrid_search_tuning_params.py
+-rw-r--r--   0        0        0      676 2024-03-14 20:19:21.857540 carbon_python_sdk-0.1.9/carbon/type/hybrid_search_tuning_params_nullable.py
+-rw-r--r--   0        0        0      692 2024-03-14 20:19:21.857658 carbon_python_sdk-0.1.9/carbon/type/list_data_source_items_request.py
+-rw-r--r--   0        0        0      695 2024-03-14 20:19:21.857787 carbon_python_sdk-0.1.9/carbon/type/list_data_source_items_response.py
+-rw-r--r--   0        0        0      543 2024-03-14 20:19:21.857900 carbon_python_sdk-0.1.9/carbon/type/list_request.py
+-rw-r--r--   0        0        0      587 2024-03-14 20:19:21.858012 carbon_python_sdk-0.1.9/carbon/type/list_response.py
+-rw-r--r--   0        0        0      709 2024-03-14 20:19:21.858126 carbon_python_sdk-0.1.9/carbon/type/modify_user_configuration_input.py
+-rw-r--r--   0        0        0      665 2024-03-14 20:21:24.404622 carbon_python_sdk-0.1.9/carbon/type/notion_authentication.py
+-rw-r--r--   0        0        0      695 2024-03-14 20:21:24.404699 carbon_python_sdk-0.1.9/carbon/type/o_auth_authentication.py
+-rw-r--r--   0        0        0     2183 2024-03-14 20:19:21.858514 carbon_python_sdk-0.1.9/carbon/type/o_auth_url_request.py
+-rw-r--r--   0        0        0      356 2024-03-14 20:19:21.858632 carbon_python_sdk-0.1.9/carbon/type/order_dir.py
+-rw-r--r--   0        0        0     1494 2024-03-14 20:19:21.858744 carbon_python_sdk-0.1.9/carbon/type/organization_response.py
+-rw-r--r--   0        0        0     1359 2024-03-14 20:21:24.404839 carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_api.py
+-rw-r--r--   0        0        0      903 2024-03-14 20:19:21.858988 carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_filters.py
+-rw-r--r--   0        0        0      395 2024-03-14 20:19:21.859100 carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_filters_ids.py
+-rw-r--r--   0        0        0      401 2024-03-14 20:19:21.859231 carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_order_by_columns.py
+-rw-r--r--   0        0        0     1070 2024-03-14 20:19:21.859383 carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_query_input.py
+-rw-r--r--   0        0        0      767 2024-03-14 20:19:21.859531 carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_response.py
+-rw-r--r--   0        0        0      759 2024-03-14 20:19:21.859658 carbon_python_sdk-0.1.9/carbon/type/organization_user_file_tag_create.py
+-rw-r--r--   0        0        0      363 2024-03-14 20:19:21.859783 carbon_python_sdk-0.1.9/carbon/type/organization_user_file_tag_create_tags.py
+-rw-r--r--   0        0        0      767 2024-03-14 20:19:21.859921 carbon_python_sdk-0.1.9/carbon/type/organization_user_file_tags_remove.py
+-rw-r--r--   0        0        0      376 2024-03-14 20:19:21.860138 carbon_python_sdk-0.1.9/carbon/type/organization_user_file_tags_remove_tags.py
+-rw-r--r--   0        0        0     2200 2024-03-14 20:19:21.860305 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters.py
+-rw-r--r--   0        0        0      408 2024-03-14 20:19:21.860524 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters_external_file_ids.py
+-rw-r--r--   0        0        0      396 2024-03-14 20:19:21.860689 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters_ids.py
+-rw-r--r--   0        0        0      421 2024-03-14 20:19:21.860821 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters_organization_user_data_source_id.py
+-rw-r--r--   0        0        0      406 2024-03-14 20:19:21.860940 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters_parent_file_ids.py
+-rw-r--r--   0        0        0      368 2024-03-14 20:19:21.861707 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters_tags.py
+-rw-r--r--   0        0        0      434 2024-03-14 20:19:21.863419 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_order_by_types.py
+-rw-r--r--   0        0        0     1228 2024-03-14 20:19:21.865229 carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_query_input.py
+-rw-r--r--   0        0        0      531 2024-03-14 20:19:21.865400 carbon_python_sdk-0.1.9/carbon/type/outh_url_response.py
+-rw-r--r--   0        0        0     1147 2024-03-14 20:19:21.865530 carbon_python_sdk-0.1.9/carbon/type/outlook_sync_input.py
+-rw-r--r--   0        0        0      519 2024-03-14 20:19:21.865649 carbon_python_sdk-0.1.9/carbon/type/pagination.py
+-rw-r--r--   0        0        0      560 2024-03-14 20:19:21.865781 carbon_python_sdk-0.1.9/carbon/type/presigned_url_response.py
+-rw-r--r--   0        0        0      882 2024-03-14 20:19:21.865901 carbon_python_sdk-0.1.9/carbon/type/raw_text_input.py
+-rw-r--r--   0        0        0      661 2024-03-14 20:19:21.866026 carbon_python_sdk-0.1.9/carbon/type/resync_file_query_input.py
+-rw-r--r--   0        0        0      571 2024-03-14 20:19:21.866147 carbon_python_sdk-0.1.9/carbon/type/revoke_access_token_input.py
+-rw-r--r--   0        0        0      963 2024-03-14 20:19:21.866265 carbon_python_sdk-0.1.9/carbon/type/rss_feed_input.py
+-rw-r--r--   0        0        0      550 2024-03-14 20:19:21.866403 carbon_python_sdk-0.1.9/carbon/type/s3_auth_request.py
+-rw-r--r--   0        0        0      648 2024-03-14 20:21:24.404924 carbon_python_sdk-0.1.9/carbon/type/s3_authentication.py
+-rw-r--r--   0        0        0     1180 2024-03-14 20:19:21.866652 carbon_python_sdk-0.1.9/carbon/type/s3_file_sync_input.py
+-rw-r--r--   0        0        0      570 2024-03-14 20:19:21.866777 carbon_python_sdk-0.1.9/carbon/type/s3_get_file_input.py
+-rw-r--r--   0        0        0      710 2024-03-14 20:21:24.404996 carbon_python_sdk-0.1.9/carbon/type/salesforce_authentication.py
+-rw-r--r--   0        0        0      735 2024-03-14 20:21:24.405080 carbon_python_sdk-0.1.9/carbon/type/sharepoint_authentication.py
+-rw-r--r--   0        0        0      433 2024-03-14 20:21:24.405169 carbon_python_sdk-0.1.9/carbon/type/simple_o_auth_data_sources.py
+-rw-r--r--   0        0        0      830 2024-03-14 20:19:21.867251 carbon_python_sdk-0.1.9/carbon/type/single_chunks_and_embeddings_upload_input.py
+-rw-r--r--   0        0        0     1593 2024-03-14 20:19:21.867369 carbon_python_sdk-0.1.9/carbon/type/sitemap_scrape_request.py
+-rw-r--r--   0        0        0      395 2024-03-14 20:19:21.867490 carbon_python_sdk-0.1.9/carbon/type/sitemap_scrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      397 2024-03-14 20:19:21.867613 carbon_python_sdk-0.1.9/carbon/type/sitemap_scrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      393 2024-03-14 20:19:21.867732 carbon_python_sdk-0.1.9/carbon/type/sitemap_scrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      354 2024-03-14 20:19:21.867869 carbon_python_sdk-0.1.9/carbon/type/sitemap_scrape_request_tags.py
+-rw-r--r--   0        0        0      561 2024-03-14 20:19:21.867998 carbon_python_sdk-0.1.9/carbon/type/sync_directory_request.py
+-rw-r--r--   0        0        0      527 2024-03-14 20:19:21.868130 carbon_python_sdk-0.1.9/carbon/type/sync_files_ids.py
+-rw-r--r--   0        0        0     1218 2024-03-14 20:19:21.868250 carbon_python_sdk-0.1.9/carbon/type/sync_files_request.py
+-rw-r--r--   0        0        0     1381 2024-03-14 20:21:24.405244 carbon_python_sdk-0.1.9/carbon/type/sync_options.py
+-rw-r--r--   0        0        0      531 2024-03-14 20:19:21.868480 carbon_python_sdk-0.1.9/carbon/type/text_embedding_generators.py
+-rw-r--r--   0        0        0      548 2024-03-14 20:19:21.868763 carbon_python_sdk-0.1.9/carbon/type/token_response.py
+-rw-r--r--   0        0        0      986 2024-03-14 20:19:21.868945 carbon_python_sdk-0.1.9/carbon/type/upload_file_from_url_input.py
+-rw-r--r--   0        0        0     2196 2024-03-14 20:19:21.869084 carbon_python_sdk-0.1.9/carbon/type/user_file.py
+-rw-r--r--   0        0        0      422 2024-03-14 20:19:21.869222 carbon_python_sdk-0.1.9/carbon/type/user_file_embedding_properties.py
+-rw-r--r--   0        0        0      586 2024-03-14 20:19:21.869372 carbon_python_sdk-0.1.9/carbon/type/user_files_v2.py
+-rw-r--r--   0        0        0      548 2024-03-14 20:19:21.869506 carbon_python_sdk-0.1.9/carbon/type/user_request_content.py
+-rw-r--r--   0        0        0     1017 2024-03-14 20:19:21.869624 carbon_python_sdk-0.1.9/carbon/type/user_response.py
+-rw-r--r--   0        0        0      371 2024-03-14 20:19:21.869757 carbon_python_sdk-0.1.9/carbon/type/user_response_unique_file_tags.py
+-rw-r--r--   0        0        0      439 2024-03-14 20:19:21.870096 carbon_python_sdk-0.1.9/carbon/type/utilities_scrape_web_request.py
+-rw-r--r--   0        0        0      633 2024-03-14 20:19:21.870409 carbon_python_sdk-0.1.9/carbon/type/validation_error.py
+-rw-r--r--   0        0        0      405 2024-03-14 20:19:21.870892 carbon_python_sdk-0.1.9/carbon/type/validation_error_loc.py
+-rw-r--r--   0        0        0      598 2024-03-14 20:19:21.871039 carbon_python_sdk-0.1.9/carbon/type/webhook.py
+-rw-r--r--   0        0        0      596 2024-03-14 20:19:21.871170 carbon_python_sdk-0.1.9/carbon/type/webhook_filters.py
+-rw-r--r--   0        0        0      376 2024-03-14 20:19:21.871304 carbon_python_sdk-0.1.9/carbon/type/webhook_filters_ids.py
+-rw-r--r--   0        0        0      601 2024-03-14 20:19:21.871423 carbon_python_sdk-0.1.9/carbon/type/webhook_no_key.py
+-rw-r--r--   0        0        0      382 2024-03-14 20:19:21.871547 carbon_python_sdk-0.1.9/carbon/type/webhook_order_by_columns.py
+-rw-r--r--   0        0        0      855 2024-03-14 20:19:21.871685 carbon_python_sdk-0.1.9/carbon/type/webhook_query_input.py
+-rw-r--r--   0        0        0      644 2024-03-14 20:19:21.871838 carbon_python_sdk-0.1.9/carbon/type/webhook_query_response.py
+-rw-r--r--   0        0        0     1564 2024-03-14 20:19:21.871980 carbon_python_sdk-0.1.9/carbon/type/webscrape_request.py
+-rw-r--r--   0        0        0      391 2024-03-14 20:19:21.872279 carbon_python_sdk-0.1.9/carbon/type/webscrape_request_css_classes_to_skip.py
+-rw-r--r--   0        0        0      393 2024-03-14 20:19:21.872422 carbon_python_sdk-0.1.9/carbon/type/webscrape_request_css_selectors_to_skip.py
+-rw-r--r--   0        0        0      389 2024-03-14 20:19:21.872562 carbon_python_sdk-0.1.9/carbon/type/webscrape_request_html_tags_to_skip.py
+-rw-r--r--   0        0        0      350 2024-03-14 20:19:21.872681 carbon_python_sdk-0.1.9/carbon/type/webscrape_request_tags.py
+-rw-r--r--   0        0        0      675 2024-03-14 20:19:21.872805 carbon_python_sdk-0.1.9/carbon/type/white_labeling_response.py
+-rw-r--r--   0        0        0      809 2024-03-14 20:19:21.872938 carbon_python_sdk-0.1.9/carbon/type/youtube_transcript_response.py
+-rw-r--r--   0        0        0      551 2024-03-14 20:19:21.873072 carbon_python_sdk-0.1.9/carbon/type/youtube_transcript_response_raw_transcript.py
+-rw-r--r--   0        0        0      372 2024-03-14 20:19:21.873210 carbon_python_sdk-0.1.9/carbon/type/youtube_transcript_response_raw_transcript_item.py
+-rw-r--r--   0        0        0      667 2024-03-14 20:21:24.405345 carbon_python_sdk-0.1.9/carbon/type/zendesk_authentication.py
+-rw-r--r--   0        0        0      711 2024-03-14 20:21:24.405453 carbon_python_sdk-0.1.9/carbon/type/zotero_authentication.py
+-rw-r--r--   0        0        0      514 2024-03-14 20:19:21.873604 carbon_python_sdk-0.1.9/carbon/type_util.py
+-rw-r--r--   0        0        0     3162 2024-03-14 20:19:21.873725 carbon_python_sdk-0.1.9/carbon/validation_metadata.py
+-rw-r--r--   0        0        0      736 2024-03-14 20:21:24.405610 carbon_python_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    95328 1970-01-01 00:00:00.000000 carbon_python_sdk-0.1.9/PKG-INFO
```

### Comparing `carbon_python_sdk-0.1.8/LICENSE` & `carbon_python_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/README.md` & `carbon_python_sdk-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Visit Carbon](https://raw.githubusercontent.com/Carbon-for-Developers/carbon-sdks/HEAD/python/header.png)](https://carbon.ai)
 
 # Carbon<a id="carbon"></a>
 
 Connect external data to LLMs, no matter the source.
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v0.1.8-blue)](https://pypi.org/project/carbon-python-sdk/0.1.8)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.1.9-blue)](https://pypi.org/project/carbon-python-sdk/0.1.9)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/Carbon-for-Developers/carbon-sdks/tree/main/python#readme)
 
 </div>
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
@@ -38,14 +38,15 @@
   * [`carbon.files.query_user_files`](#carbonfilesquery_user_files)
   * [`carbon.files.query_user_files_deprecated`](#carbonfilesquery_user_files_deprecated)
   * [`carbon.files.resync`](#carbonfilesresync)
   * [`carbon.files.upload`](#carbonfilesupload)
   * [`carbon.files.upload_from_url`](#carbonfilesupload_from_url)
   * [`carbon.files.upload_text`](#carbonfilesupload_text)
   * [`carbon.health.check`](#carbonhealthcheck)
+  * [`carbon.integrations.connect_data_source`](#carbonintegrationsconnect_data_source)
   * [`carbon.integrations.connect_freshdesk`](#carbonintegrationsconnect_freshdesk)
   * [`carbon.integrations.connect_gitbook`](#carbonintegrationsconnect_gitbook)
   * [`carbon.integrations.create_aws_iam_user`](#carbonintegrationscreate_aws_iam_user)
   * [`carbon.integrations.get_oauth_url`](#carbonintegrationsget_oauth_url)
   * [`carbon.integrations.list_confluence_pages`](#carbonintegrationslist_confluence_pages)
   * [`carbon.integrations.list_data_source_items`](#carbonintegrationslist_data_source_items)
   * [`carbon.integrations.list_folders`](#carbonintegrationslist_folders)
@@ -79,15 +80,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install carbon-python-sdk==0.1.8
+pip install carbon-python-sdk==0.1.9
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from carbon import Carbon
 
@@ -1231,14 +1232,62 @@
 
 `/health` `get`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
+### `carbon.integrations.connect_data_source`<a id="carbonintegrationsconnect_data_source"></a>
+
+Connect Data Source
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+connect_data_source_response = carbon.integrations.connect_data_source(
+    authentication={
+        "source": "GOOGLE_DRIVE",
+        "access_token": "access_token_example",
+    },
+    sync_options={
+        "chunk_size": 1500,
+        "chunk_overlap": 20,
+        "skip_embedding_generation": False,
+        "embedding_model": "OPENAI",
+        "generate_sparse_vectors": False,
+        "prepend_filename_to_chunks": False,
+        "sync_files_on_connection": True,
+        "set_page_as_boundary": False,
+    },
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### authentication: Union[`OAuthAuthentication`, `NotionAuthentication`, `SharepointAuthentication`, `ConfluenceAuthentication`, `ZendeskAuthentication`, `ZoteroAuthentication`, `GitbookAuthetication`, `SalesforceAuthentication`, `FreskdeskAuthentication`, `S3Authentication`]<a id="authentication-unionoauthauthentication-notionauthentication-sharepointauthentication-confluenceauthentication-zendeskauthentication-zoteroauthentication-gitbookauthetication-salesforceauthentication-freskdeskauthentication-s3authentication"></a>
+
+
+##### sync_options: [`SyncOptions`](./carbon/type/sync_options.py)<a id="sync_options-syncoptionscarbontypesync_optionspy"></a>
+
+
+#### ⚙️ Request Body<a id="⚙️-request-body"></a>
+
+[`ConnectDataSourceInput`](./carbon/type/connect_data_source_input.py)
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`ConnectDataSourceResponse`](./carbon/pydantic/connect_data_source_response.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/integrations/connect` `post`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
 ### `carbon.integrations.connect_freshdesk`<a id="carbonintegrationsconnect_freshdesk"></a>
 
 Refer this article to obtain an API key https://support.freshdesk.com/en/support/solutions/articles/215517.
 Make sure that your API key has the permission to read solutions from your account and you are on a <b>paid</b> plan.
 Once you have an API key, you can make a request to this endpoint along with your freshdesk domain. This will 
 trigger an automatic sync of the articles in your "solutions" tab. Additional parameters below can be used to associate 
 data with the synced articles or modify the sync behavior.
```

### Comparing `carbon_python_sdk-0.1.8/carbon/__init__.py` & `carbon_python_sdk-0.1.9/carbon/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 # import ApiClient
 from carbon.api_client import ApiClient
 
 # import Configuration
 from carbon.configuration import Configuration
```

### Comparing `carbon_python_sdk-0.1.8/carbon/api_client.py` & `carbon_python_sdk-0.1.9/carbon/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2959,15 +2959,15 @@
 0000b8e0: 6465 725f 6e61 6d65 5d20 3d20 6865 6164  der_name] = head
 0000b8f0: 6572 5f76 616c 7565 0a20 2020 2020 2020  er_value.       
 0000b900: 2073 656c 662e 636f 6f6b 6965 203d 2063   self.cookie = c
 0000b910: 6f6f 6b69 650a 2020 2020 2020 2020 2320  ookie.        # 
 0000b920: 5365 7420 6465 6661 756c 7420 5573 6572  Set default User
 0000b930: 2d41 6765 6e74 2e0a 2020 2020 2020 2020  -Agent..        
 0000b940: 7365 6c66 2e75 7365 725f 6167 656e 7420  self.user_agent 
-0000b950: 3d20 274b 6f6e 6669 672f 302e 312e 382f  = 'Konfig/0.1.8/
+0000b950: 3d20 274b 6f6e 6669 672f 302e 312e 392f  = 'Konfig/0.1.9/
 0000b960: 7079 7468 6f6e 270a 0a20 2020 2064 6566  python'..    def
 0000b970: 205f 5f65 6e74 6572 5f5f 2873 656c 6629   __enter__(self)
 0000b980: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
 0000b990: 2073 656c 660a 0a20 2020 2064 6566 205f   self..    def _
 0000b9a0: 5f65 7869 745f 5f28 7365 6c66 2c20 6578  _exit__(self, ex
 0000b9b0: 635f 7479 7065 2c20 6578 635f 7661 6c75  c_type, exc_valu
 0000b9c0: 652c 2074 7261 6365 6261 636b 293a 0a20  e, traceback):.
```

### Comparing `carbon_python_sdk-0.1.8/carbon/api_response.py` & `carbon_python_sdk-0.1.9/carbon/api_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/path_to_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/path_to_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import typing_extensions
 
 from carbon.paths import PathValues
 from carbon.apis.paths.integrations_oauth_url import IntegrationsOauthUrl
+from carbon.apis.paths.integrations_connect import IntegrationsConnect
 from carbon.apis.paths.integrations_items_sync import IntegrationsItemsSync
 from carbon.apis.paths.integrations_items_list import IntegrationsItemsList
 from carbon.apis.paths.integrations_files_sync import IntegrationsFilesSync
 from carbon.apis.paths.integrations_confluence_list import IntegrationsConfluenceList
 from carbon.apis.paths.integrations_confluence_sync import IntegrationsConfluenceSync
 from carbon.apis.paths.integrations_s3 import IntegrationsS3
 from carbon.apis.paths.integrations_s3_files import IntegrationsS3Files
@@ -53,14 +54,15 @@
 from carbon.apis.paths.fetch_youtube_transcript import FetchYoutubeTranscript
 from carbon.apis.paths.health import Health
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.INTEGRATIONS_OAUTH_URL: IntegrationsOauthUrl,
+        PathValues.INTEGRATIONS_CONNECT: IntegrationsConnect,
         PathValues.INTEGRATIONS_ITEMS_SYNC: IntegrationsItemsSync,
         PathValues.INTEGRATIONS_ITEMS_LIST: IntegrationsItemsList,
         PathValues.INTEGRATIONS_FILES_SYNC: IntegrationsFilesSync,
         PathValues.INTEGRATIONS_CONFLUENCE_LIST: IntegrationsConfluenceList,
         PathValues.INTEGRATIONS_CONFLUENCE_SYNC: IntegrationsConfluenceSync,
         PathValues.INTEGRATIONS_S3: IntegrationsS3,
         PathValues.INTEGRATIONS_S3_FILES: IntegrationsS3Files,
@@ -109,14 +111,15 @@
         PathValues.HEALTH: Health,
     }
 )
 
 path_to_api = PathToApi(
     {
         PathValues.INTEGRATIONS_OAUTH_URL: IntegrationsOauthUrl,
+        PathValues.INTEGRATIONS_CONNECT: IntegrationsConnect,
         PathValues.INTEGRATIONS_ITEMS_SYNC: IntegrationsItemsSync,
         PathValues.INTEGRATIONS_ITEMS_LIST: IntegrationsItemsList,
         PathValues.INTEGRATIONS_FILES_SYNC: IntegrationsFilesSync,
         PathValues.INTEGRATIONS_CONFLUENCE_LIST: IntegrationsConfluenceList,
         PathValues.INTEGRATIONS_CONFLUENCE_SYNC: IntegrationsConfluenceSync,
         PathValues.INTEGRATIONS_S3: IntegrationsS3,
         PathValues.INTEGRATIONS_S3_FILES: IntegrationsS3Files,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tag_to_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/__init__.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/auth_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/auth_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/data_sources_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/data_sources_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/embeddings_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/embeddings_api_raw.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/embeddings_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/files_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/files_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/files_api_raw.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/files_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/health_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/health_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/integrations_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/integrations_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from carbon.paths.integrations_connect.post import ConnectDataSource
 from carbon.paths.integrations_freshdesk.post import ConnectFreshdesk
 from carbon.paths.integrations_gitbook.post import ConnectGitbook
 from carbon.paths.integrations_s3.post import CreateAwsIamUser
 from carbon.paths.integrations_oauth_url.post import GetOauthUrl
 from carbon.paths.integrations_confluence_list.post import ListConfluencePages
 from carbon.paths.integrations_items_list.post import ListDataSourceItems
 from carbon.paths.integrations_outlook_user_folders.get import ListFolders
@@ -27,14 +28,15 @@
 from carbon.paths.integrations_outlook_sync.post import SyncOutlook
 from carbon.paths.integrations_rss_feed.post import SyncRssFeed
 from carbon.paths.integrations_s3_files.post import SyncS3Files
 from carbon.apis.tags.integrations_api_raw import IntegrationsApiRaw
 
 
 class IntegrationsApi(
+    ConnectDataSource,
     ConnectFreshdesk,
     ConnectGitbook,
     CreateAwsIamUser,
     GetOauthUrl,
     ListConfluencePages,
     ListDataSourceItems,
     ListFolders,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/integrations_api_raw.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/integrations_api_raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
     Connect external data to LLMs, no matter the source.
 
     The version of the OpenAPI document: 1.0.0
     Generated by: https://konfigthis.com
 """
 
+from carbon.paths.integrations_connect.post import ConnectDataSourceRaw
 from carbon.paths.integrations_freshdesk.post import ConnectFreshdeskRaw
 from carbon.paths.integrations_gitbook.post import ConnectGitbookRaw
 from carbon.paths.integrations_s3.post import CreateAwsIamUserRaw
 from carbon.paths.integrations_oauth_url.post import GetOauthUrlRaw
 from carbon.paths.integrations_confluence_list.post import ListConfluencePagesRaw
 from carbon.paths.integrations_items_list.post import ListDataSourceItemsRaw
 from carbon.paths.integrations_outlook_user_folders.get import ListFoldersRaw
@@ -26,14 +27,15 @@
 from carbon.paths.integrations_gmail_sync.post import SyncGmailRaw
 from carbon.paths.integrations_outlook_sync.post import SyncOutlookRaw
 from carbon.paths.integrations_rss_feed.post import SyncRssFeedRaw
 from carbon.paths.integrations_s3_files.post import SyncS3FilesRaw
 
 
 class IntegrationsApiRaw(
+    ConnectDataSourceRaw,
     ConnectFreshdeskRaw,
     ConnectGitbookRaw,
     CreateAwsIamUserRaw,
     GetOauthUrlRaw,
     ListConfluencePagesRaw,
     ListDataSourceItemsRaw,
     ListFoldersRaw,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/organizations_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/organizations_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/users_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/users_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/users_api_raw.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/users_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/utilities_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/utilities_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/utilities_api_raw.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/utilities_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/webhooks_api.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/apis/tags/webhooks_api_raw.py` & `carbon_python_sdk-0.1.9/carbon/apis/tags/webhooks_api_raw.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/client.py` & `carbon_python_sdk-0.1.9/carbon/client.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/client.pyi` & `carbon_python_sdk-0.1.9/carbon/client.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/client_custom.py` & `carbon_python_sdk-0.1.9/carbon/client_custom.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/configuration.py` & `carbon_python_sdk-0.1.9/carbon/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -398,15 +398,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.1.8".\
+               "SDK Package Version: 0.1.9".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `carbon_python_sdk-0.1.8/carbon/exceptions.py` & `carbon_python_sdk-0.1.9/carbon/exceptions.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/exceptions_base.py` & `carbon_python_sdk-0.1.9/carbon/exceptions_base.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/add_webhook_props.py` & `carbon_python_sdk-0.1.9/carbon/model/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/add_webhook_props.pyi` & `carbon_python_sdk-0.1.9/carbon/model/add_webhook_props.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.1.9/carbon/model/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/body_create_upload_file_uploadfile_post.pyi` & `carbon_python_sdk-0.1.9/carbon/model/body_create_upload_file_uploadfile_post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunk_properties.py` & `carbon_python_sdk-0.1.9/carbon/model/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunk_properties.pyi` & `carbon_python_sdk-0.1.9/carbon/model/chunk_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunk_properties_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunk_properties_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/chunk_properties_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings.py` & `carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings.pyi` & `carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_embedding.py` & `carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_embedding.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_embedding.pyi` & `carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_embedding.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/chunks_and_embeddings_upload_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/chunks_and_embeddings_upload_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/configuration_keys.py` & `carbon_python_sdk-0.1.9/carbon/model/configuration_keys.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/configuration_keys.pyi` & `carbon_python_sdk-0.1.9/carbon/model/configuration_keys.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_last_sync_actions.py` & `carbon_python_sdk-0.1.9/carbon/model/data_source_last_sync_actions.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_last_sync_actions.pyi` & `carbon_python_sdk-0.1.9/carbon/model/data_source_last_sync_actions.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_sync_statuses.py` & `carbon_python_sdk-0.1.9/carbon/model/data_source_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_sync_statuses.pyi` & `carbon_python_sdk-0.1.9/carbon/model/data_source_sync_statuses.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_type.py` & `carbon_python_sdk-0.1.9/carbon/model/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_type.pyi` & `carbon_python_sdk-0.1.9/carbon/model/data_source_type.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_type_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/data_source_type_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/data_source_type_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input.py` & `carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input_file_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_files_query_input_file_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/delete_files_query_input_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_users_input.py` & `carbon_python_sdk-0.1.9/carbon/model/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_users_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/delete_users_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_users_input_customer_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/delete_users_input_customer_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/delete_users_input_customer_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/delete_users_input_customer_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/directory_item.py` & `carbon_python_sdk-0.1.9/carbon/model/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/directory_item.pyi` & `carbon_python_sdk-0.1.9/carbon/model/directory_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response.py` & `carbon_python_sdk-0.1.9/carbon/model/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/document_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response_list.py` & `carbon_python_sdk-0.1.9/carbon/model/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response_list.pyi` & `carbon_python_sdk-0.1.9/carbon/model/document_response_list.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/document_response_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/document_response_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response_vector.py` & `carbon_python_sdk-0.1.9/carbon/model/document_response_vector.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/document_response_vector.pyi` & `carbon_python_sdk-0.1.9/carbon/model/document_response_vector.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk.py` & `carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk_embedding.py` & `carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk_embedding.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_and_chunk_embedding.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embedding_and_chunk_embedding.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_generators.py` & `carbon_python_sdk-0.1.9/carbon/model/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_generators.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_generators_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_generators_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embedding_generators_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_properties.py` & `carbon_python_sdk-0.1.9/carbon/model/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embedding_properties.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embedding_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_filters.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_order_by_columns.py` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_order_by_columns.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_query_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/embeddings_and_chunks_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/embeddings_and_chunks_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/external_file_sync_statuses.py` & `carbon_python_sdk-0.1.9/carbon/model/external_file_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/external_file_sync_statuses.pyi` & `carbon_python_sdk-0.1.9/carbon/model/external_file_sync_statuses.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/external_source_item.py` & `carbon_python_sdk-0.1.9/carbon/model/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/external_source_item.pyi` & `carbon_python_sdk-0.1.9/carbon/model/external_source_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response.py` & `carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response_urls.py` & `carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response_urls.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/fetch_urls_response_urls.pyi` & `carbon_python_sdk-0.1.9/carbon/model/fetch_urls_response_urls.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_content_types.py` & `carbon_python_sdk-0.1.9/carbon/model/file_content_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_content_types.pyi` & `carbon_python_sdk-0.1.9/carbon/model/file_content_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_content_types_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/file_content_types_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_content_types_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/file_content_types_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_formats.py` & `carbon_python_sdk-0.1.9/carbon/model/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_formats.pyi` & `carbon_python_sdk-0.1.9/carbon/model/file_formats.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_formats_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_formats_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/file_formats_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_statistics.py` & `carbon_python_sdk-0.1.9/carbon/model/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_statistics.pyi` & `carbon_python_sdk-0.1.9/carbon/model/file_statistics.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_statistics_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/file_statistics_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/file_statistics_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/files_query_user_files_deprecated_response.py` & `carbon_python_sdk-0.1.9/carbon/model/files_query_user_files_deprecated_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/files_query_user_files_deprecated_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/files_query_user_files_deprecated_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/fresh_desk_connect_request.py` & `carbon_python_sdk-0.1.9/carbon/model/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/fresh_desk_connect_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/fresh_desk_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/generic_success_response.py` & `carbon_python_sdk-0.1.9/carbon/model/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/generic_success_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/generic_success_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body.py` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body.pyi` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_file_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_file_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_parent_file_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_parent_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_parent_file_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_parent_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_query_vector.py` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_query_vector.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_query_vector.pyi` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_query_vector.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/get_embedding_documents_body_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/get_embedding_documents_body_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gitbook_connect_request.py` & `carbon_python_sdk-0.1.9/carbon/model/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gitbook_connect_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/gitbook_connect_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request.py` & `carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request_space_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request_space_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gitbook_sync_request_space_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/gitbook_sync_request_space_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gmail_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/model/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/gmail_sync_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/gmail_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/http_validation_error.py` & `carbon_python_sdk-0.1.9/carbon/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/http_validation_error.pyi` & `carbon_python_sdk-0.1.9/carbon/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params.pyi` & `carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/hybrid_search_tuning_params_nullable.pyi` & `carbon_python_sdk-0.1.9/carbon/model/hybrid_search_tuning_params_nullable.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_request.py` & `carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_response.py` & `carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_data_source_items_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/list_data_source_items_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_request.py` & `carbon_python_sdk-0.1.9/carbon/model/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/list_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_response.py` & `carbon_python_sdk-0.1.9/carbon/model/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/list_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/list_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/modify_user_configuration_input.py` & `carbon_python_sdk-0.1.9/carbon/model/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/modify_user_configuration_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/modify_user_configuration_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/o_auth_url_request.py` & `carbon_python_sdk-0.1.9/carbon/model/o_auth_url_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/o_auth_url_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/o_auth_url_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/order_dir.py` & `carbon_python_sdk-0.1.9/carbon/model/order_dir.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/order_dir.pyi` & `carbon_python_sdk-0.1.9/carbon/model/order_dir.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_response.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_api.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     class MetaOapg:
         required = {
             "last_synced_at",
             "revoked_access",
             "created_at",
             "data_source_type",
             "organization_supplied_user_id",
+            "token",
             "updated_at",
             "source_items_synced_at",
             "organization_id",
             "organization_user_id",
             "last_sync_action",
             "sync_status",
             "id",
@@ -70,14 +71,36 @@
                         *args,
                         _configuration=_configuration,
                     )
         
             @staticmethod
             def data_source_type() -> typing.Type['DataSourceType']:
                 return DataSourceType
+            
+            
+            class token(
+                schemas.DictBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneFrozenDictMixin
+            ):
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, None, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'token':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
         
             @staticmethod
             def sync_status() -> typing.Type['DataSourceSyncStatuses']:
                 return DataSourceSyncStatuses
             
             
             class source_items_synced_at(
@@ -114,14 +137,15 @@
                 return DataSourceLastSyncActions
             created_at = schemas.DateTimeSchema
             updated_at = schemas.DateTimeSchema
             __annotations__ = {
                 "id": id,
                 "data_source_external_id": data_source_external_id,
                 "data_source_type": data_source_type,
+                "token": token,
                 "sync_status": sync_status,
                 "source_items_synced_at": source_items_synced_at,
                 "organization_user_id": organization_user_id,
                 "organization_id": organization_id,
                 "organization_supplied_user_id": organization_supplied_user_id,
                 "revoked_access": revoked_access,
                 "last_synced_at": last_synced_at,
@@ -131,14 +155,15 @@
             }
     
     last_synced_at: MetaOapg.properties.last_synced_at
     revoked_access: MetaOapg.properties.revoked_access
     created_at: MetaOapg.properties.created_at
     data_source_type: 'DataSourceType'
     organization_supplied_user_id: MetaOapg.properties.organization_supplied_user_id
+    token: MetaOapg.properties.token
     updated_at: MetaOapg.properties.updated_at
     source_items_synced_at: MetaOapg.properties.source_items_synced_at
     organization_id: MetaOapg.properties.organization_id
     organization_user_id: MetaOapg.properties.organization_user_id
     last_sync_action: 'DataSourceLastSyncActions'
     sync_status: 'DataSourceSyncStatuses'
     id: MetaOapg.properties.id
@@ -150,14 +175,17 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["data_source_external_id"]) -> MetaOapg.properties.data_source_external_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["data_source_type"]) -> 'DataSourceType': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["token"]) -> MetaOapg.properties.token: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sync_status"]) -> 'DataSourceSyncStatuses': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source_items_synced_at"]) -> MetaOapg.properties.source_items_synced_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["organization_user_id"]) -> MetaOapg.properties.organization_user_id: ...
@@ -182,29 +210,32 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "token", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["data_source_external_id"]) -> MetaOapg.properties.data_source_external_id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["data_source_type"]) -> 'DataSourceType': ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["token"]) -> MetaOapg.properties.token: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sync_status"]) -> 'DataSourceSyncStatuses': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source_items_synced_at"]) -> MetaOapg.properties.source_items_synced_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["organization_user_id"]) -> MetaOapg.properties.organization_user_id: ...
@@ -229,26 +260,27 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "token", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         last_synced_at: typing.Union[MetaOapg.properties.last_synced_at, str, datetime, ],
         revoked_access: typing.Union[MetaOapg.properties.revoked_access, bool, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         data_source_type: 'DataSourceType',
         organization_supplied_user_id: typing.Union[MetaOapg.properties.organization_supplied_user_id, str, ],
+        token: typing.Union[MetaOapg.properties.token, dict, frozendict.frozendict, None, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         source_items_synced_at: typing.Union[MetaOapg.properties.source_items_synced_at, None, str, datetime, ],
         organization_id: typing.Union[MetaOapg.properties.organization_id, decimal.Decimal, int, ],
         organization_user_id: typing.Union[MetaOapg.properties.organization_user_id, decimal.Decimal, int, ],
         last_sync_action: 'DataSourceLastSyncActions',
         sync_status: 'DataSourceSyncStatuses',
         id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
@@ -260,14 +292,15 @@
             cls,
             *args,
             last_synced_at=last_synced_at,
             revoked_access=revoked_access,
             created_at=created_at,
             data_source_type=data_source_type,
             organization_supplied_user_id=organization_supplied_user_id,
+            token=token,
             updated_at=updated_at,
             source_items_synced_at=source_items_synced_at,
             organization_id=organization_id,
             organization_user_id=organization_user_id,
             last_sync_action=last_sync_action,
             sync_status=sync_status,
             id=id,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_api.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_api.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     class MetaOapg:
         required = {
             "last_synced_at",
             "revoked_access",
             "created_at",
             "data_source_type",
             "organization_supplied_user_id",
+            "token",
             "updated_at",
             "source_items_synced_at",
             "organization_id",
             "organization_user_id",
             "last_sync_action",
             "sync_status",
             "id",
@@ -70,14 +71,36 @@
                         *args,
                         _configuration=_configuration,
                     )
         
             @staticmethod
             def data_source_type() -> typing.Type['DataSourceType']:
                 return DataSourceType
+            
+            
+            class token(
+                schemas.DictBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneFrozenDictMixin
+            ):
+            
+            
+                def __new__(
+                    cls,
+                    *args: typing.Union[dict, frozendict.frozendict, None, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'token':
+                    return super().__new__(
+                        cls,
+                        *args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
         
             @staticmethod
             def sync_status() -> typing.Type['DataSourceSyncStatuses']:
                 return DataSourceSyncStatuses
             
             
             class source_items_synced_at(
@@ -114,14 +137,15 @@
                 return DataSourceLastSyncActions
             created_at = schemas.DateTimeSchema
             updated_at = schemas.DateTimeSchema
             __annotations__ = {
                 "id": id,
                 "data_source_external_id": data_source_external_id,
                 "data_source_type": data_source_type,
+                "token": token,
                 "sync_status": sync_status,
                 "source_items_synced_at": source_items_synced_at,
                 "organization_user_id": organization_user_id,
                 "organization_id": organization_id,
                 "organization_supplied_user_id": organization_supplied_user_id,
                 "revoked_access": revoked_access,
                 "last_synced_at": last_synced_at,
@@ -131,14 +155,15 @@
             }
     
     last_synced_at: MetaOapg.properties.last_synced_at
     revoked_access: MetaOapg.properties.revoked_access
     created_at: MetaOapg.properties.created_at
     data_source_type: 'DataSourceType'
     organization_supplied_user_id: MetaOapg.properties.organization_supplied_user_id
+    token: MetaOapg.properties.token
     updated_at: MetaOapg.properties.updated_at
     source_items_synced_at: MetaOapg.properties.source_items_synced_at
     organization_id: MetaOapg.properties.organization_id
     organization_user_id: MetaOapg.properties.organization_user_id
     last_sync_action: 'DataSourceLastSyncActions'
     sync_status: 'DataSourceSyncStatuses'
     id: MetaOapg.properties.id
@@ -150,14 +175,17 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["data_source_external_id"]) -> MetaOapg.properties.data_source_external_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["data_source_type"]) -> 'DataSourceType': ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["token"]) -> MetaOapg.properties.token: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sync_status"]) -> 'DataSourceSyncStatuses': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["source_items_synced_at"]) -> MetaOapg.properties.source_items_synced_at: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["organization_user_id"]) -> MetaOapg.properties.organization_user_id: ...
@@ -182,29 +210,32 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "token", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["data_source_external_id"]) -> MetaOapg.properties.data_source_external_id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["data_source_type"]) -> 'DataSourceType': ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["token"]) -> MetaOapg.properties.token: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sync_status"]) -> 'DataSourceSyncStatuses': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["source_items_synced_at"]) -> MetaOapg.properties.source_items_synced_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["organization_user_id"]) -> MetaOapg.properties.organization_user_id: ...
@@ -229,26 +260,27 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["updated_at"]) -> MetaOapg.properties.updated_at: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "data_source_external_id", "data_source_type", "token", "sync_status", "source_items_synced_at", "organization_user_id", "organization_id", "organization_supplied_user_id", "revoked_access", "last_synced_at", "last_sync_action", "created_at", "updated_at", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *args: typing.Union[dict, frozendict.frozendict, ],
         last_synced_at: typing.Union[MetaOapg.properties.last_synced_at, str, datetime, ],
         revoked_access: typing.Union[MetaOapg.properties.revoked_access, bool, ],
         created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
         data_source_type: 'DataSourceType',
         organization_supplied_user_id: typing.Union[MetaOapg.properties.organization_supplied_user_id, str, ],
+        token: typing.Union[MetaOapg.properties.token, dict, frozendict.frozendict, None, ],
         updated_at: typing.Union[MetaOapg.properties.updated_at, str, datetime, ],
         source_items_synced_at: typing.Union[MetaOapg.properties.source_items_synced_at, None, str, datetime, ],
         organization_id: typing.Union[MetaOapg.properties.organization_id, decimal.Decimal, int, ],
         organization_user_id: typing.Union[MetaOapg.properties.organization_user_id, decimal.Decimal, int, ],
         last_sync_action: 'DataSourceLastSyncActions',
         sync_status: 'DataSourceSyncStatuses',
         id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
@@ -260,14 +292,15 @@
             cls,
             *args,
             last_synced_at=last_synced_at,
             revoked_access=revoked_access,
             created_at=created_at,
             data_source_type=data_source_type,
             organization_supplied_user_id=organization_supplied_user_id,
+            token=token,
             updated_at=updated_at,
             source_items_synced_at=source_items_synced_at,
             organization_id=organization_id,
             organization_user_id=organization_user_id,
             last_sync_action=last_sync_action,
             sync_status=sync_status,
             id=id,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_filters_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_order_by_columns.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_order_by_columns.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_query_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_response.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_data_source_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_data_source_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tag_create_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tag_create_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_file_tags_remove_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_file_tags_remove_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_external_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_external_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_organization_user_data_source_id.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_parent_file_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_filters_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_filters_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_order_by_types.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_order_by_types.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_order_by_types.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_order_by_types.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/organization_user_files_to_sync_query_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/organization_user_files_to_sync_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/outh_url_response.py` & `carbon_python_sdk-0.1.9/carbon/model/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/outh_url_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/outh_url_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/outlook_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/model/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/outlook_sync_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/outlook_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/pagination.py` & `carbon_python_sdk-0.1.9/carbon/model/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/pagination.pyi` & `carbon_python_sdk-0.1.9/carbon/model/pagination.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/presigned_url_response.py` & `carbon_python_sdk-0.1.9/carbon/model/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/presigned_url_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/presigned_url_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/raw_text_input.py` & `carbon_python_sdk-0.1.9/carbon/model/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/raw_text_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/raw_text_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/resync_file_query_input.py` & `carbon_python_sdk-0.1.9/carbon/model/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/resync_file_query_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/resync_file_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/revoke_access_token_input.py` & `carbon_python_sdk-0.1.9/carbon/model/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/revoke_access_token_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/revoke_access_token_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/rss_feed_input.py` & `carbon_python_sdk-0.1.9/carbon/model/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/rss_feed_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/rss_feed_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/s3_auth_request.py` & `carbon_python_sdk-0.1.9/carbon/model/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/s3_auth_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/s3_auth_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/s3_file_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/model/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/s3_file_sync_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/s3_file_sync_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/s3_get_file_input.py` & `carbon_python_sdk-0.1.9/carbon/model/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/s3_get_file_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/s3_get_file_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.1.9/carbon/model/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/single_chunks_and_embeddings_upload_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/single_chunks_and_embeddings_upload_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request.py` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,17 @@
                 schemas.IntBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneDecimalMixin
             ):
             
             
+                class MetaOapg:
+            
+            
                 def __new__(
                     cls,
                     *args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'max_pages_to_scrape':
                     return super().__new__(
                         cls,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,18 @@
                 schemas.IntBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneDecimalMixin
             ):
             
             
+                class MetaOapg:
+                    inclusive_minimum = 1
+            
+            
                 def __new__(
                     cls,
                     *args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'max_pages_to_scrape':
                     return super().__new__(
                         cls,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_classes_to_skip.py` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_classes_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_classes_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_selectors_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_css_selectors_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_html_tags_to_skip.py` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_html_tags_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_html_tags_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sitemap_scrape_request_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sitemap_scrape_request_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sync_directory_request.py` & `carbon_python_sdk-0.1.9/carbon/model/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sync_directory_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sync_directory_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sync_files_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sync_files_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sync_files_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sync_files_request.py` & `carbon_python_sdk-0.1.9/carbon/model/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/sync_files_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/sync_files_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/text_embedding_generators.py` & `carbon_python_sdk-0.1.9/carbon/model/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/text_embedding_generators.pyi` & `carbon_python_sdk-0.1.9/carbon/model/text_embedding_generators.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/token_response.py` & `carbon_python_sdk-0.1.9/carbon/model/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/token_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/token_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/upload_file_from_url_input.py` & `carbon_python_sdk-0.1.9/carbon/model/upload_file_from_url_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/upload_file_from_url_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/upload_file_from_url_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_file.py` & `carbon_python_sdk-0.1.9/carbon/model/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_file.pyi` & `carbon_python_sdk-0.1.9/carbon/model/user_file.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_file_embedding_properties.py` & `carbon_python_sdk-0.1.9/carbon/model/user_file_embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_file_embedding_properties.pyi` & `carbon_python_sdk-0.1.9/carbon/model/user_file_embedding_properties.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_files_v2.py` & `carbon_python_sdk-0.1.9/carbon/model/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_files_v2.pyi` & `carbon_python_sdk-0.1.9/carbon/model/user_files_v2.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_request_content.py` & `carbon_python_sdk-0.1.9/carbon/model/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_request_content.pyi` & `carbon_python_sdk-0.1.9/carbon/model/user_request_content.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_response.py` & `carbon_python_sdk-0.1.9/carbon/model/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/user_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_response_unique_file_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/user_response_unique_file_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/user_response_unique_file_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/user_response_unique_file_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/utilities_scrape_web_request.py` & `carbon_python_sdk-0.1.9/carbon/model/utilities_scrape_web_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/utilities_scrape_web_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/utilities_scrape_web_request.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/validation_error.py` & `carbon_python_sdk-0.1.9/carbon/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/validation_error.pyi` & `carbon_python_sdk-0.1.9/carbon/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/validation_error_loc.py` & `carbon_python_sdk-0.1.9/carbon/model/validation_error_loc.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/validation_error_loc.pyi` & `carbon_python_sdk-0.1.9/carbon/model/validation_error_loc.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_filters.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_filters.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook_filters.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_filters_ids.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook_filters_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_filters_ids.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook_filters_ids.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_no_key.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_no_key.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook_no_key.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_order_by_columns.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook_order_by_columns.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_order_by_columns.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook_order_by_columns.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_query_input.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_query_input.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook_query_input.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_query_response.py` & `carbon_python_sdk-0.1.9/carbon/model/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webhook_query_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webhook_query_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request.py` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,18 @@
                 schemas.IntBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneDecimalMixin
             ):
             
             
+                class MetaOapg:
+                    inclusive_minimum = 0
+            
+            
                 def __new__(
                     cls,
                     *args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'recursion_depth':
                     return super().__new__(
                         cls,
@@ -68,14 +72,18 @@
                 schemas.IntBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneDecimalMixin
             ):
             
             
+                class MetaOapg:
+                    inclusive_minimum = 1
+            
+            
                 def __new__(
                     cls,
                     *args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'max_pages_to_scrape':
                     return super().__new__(
                         cls,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,17 @@
                 schemas.IntBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneDecimalMixin
             ):
             
             
+                class MetaOapg:
+            
+            
                 def __new__(
                     cls,
                     *args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'recursion_depth':
                     return super().__new__(
                         cls,
@@ -68,14 +71,17 @@
                 schemas.IntBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneDecimalMixin
             ):
             
             
+                class MetaOapg:
+            
+            
                 def __new__(
                     cls,
                     *args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'max_pages_to_scrape':
                     return super().__new__(
                         cls,
```

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_classes_to_skip.py` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_classes_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_classes_to_skip.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_classes_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_selectors_to_skip.py` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_selectors_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_css_selectors_to_skip.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_css_selectors_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_html_tags_to_skip.py` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_html_tags_to_skip.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_html_tags_to_skip.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_html_tags_to_skip.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_tags.py` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_tags.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/webscrape_request_tags.pyi` & `carbon_python_sdk-0.1.9/carbon/model/webscrape_request_tags.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/white_labeling_response.py` & `carbon_python_sdk-0.1.9/carbon/model/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/white_labeling_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/white_labeling_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response.py` & `carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response.pyi` & `carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript.pyi` & `carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript_item.py` & `carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/model/youtube_transcript_response_raw_transcript_item.pyi` & `carbon_python_sdk-0.1.9/carbon/model/youtube_transcript_response_raw_transcript_item.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/models/__init__.py` & `carbon_python_sdk-0.1.9/carbon/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from carbon.model.body_create_upload_file_uploadfile_post import BodyCreateUploadFileUploadfilePost
 from carbon.model.chunk_properties import ChunkProperties
 from carbon.model.chunk_properties_nullable import ChunkPropertiesNullable
 from carbon.model.chunks_and_embeddings import ChunksAndEmbeddings
 from carbon.model.chunks_and_embeddings_embedding import ChunksAndEmbeddingsEmbedding
 from carbon.model.chunks_and_embeddings_upload_input import ChunksAndEmbeddingsUploadInput
 from carbon.model.configuration_keys import ConfigurationKeys
+from carbon.model.confluence_authentication import ConfluenceAuthentication
+from carbon.model.connect_data_source_input import ConnectDataSourceInput
+from carbon.model.connect_data_source_response import ConnectDataSourceResponse
 from carbon.model.data_source_last_sync_actions import DataSourceLastSyncActions
 from carbon.model.data_source_sync_statuses import DataSourceSyncStatuses
 from carbon.model.data_source_type import DataSourceType
 from carbon.model.data_source_type_nullable import DataSourceTypeNullable
 from carbon.model.delete_files_query_input import DeleteFilesQueryInput
 from carbon.model.delete_files_query_input_file_ids import DeleteFilesQueryInputFileIds
 from carbon.model.delete_users_input import DeleteUsersInput
@@ -49,32 +52,36 @@
 from carbon.model.file_content_types_nullable import FileContentTypesNullable
 from carbon.model.file_formats import FileFormats
 from carbon.model.file_formats_nullable import FileFormatsNullable
 from carbon.model.file_statistics import FileStatistics
 from carbon.model.file_statistics_nullable import FileStatisticsNullable
 from carbon.model.files_query_user_files_deprecated_response import FilesQueryUserFilesDeprecatedResponse
 from carbon.model.fresh_desk_connect_request import FreshDeskConnectRequest
+from carbon.model.freskdesk_authentication import FreskdeskAuthentication
 from carbon.model.generic_success_response import GenericSuccessResponse
 from carbon.model.get_embedding_documents_body import GetEmbeddingDocumentsBody
 from carbon.model.get_embedding_documents_body_file_ids import GetEmbeddingDocumentsBodyFileIds
 from carbon.model.get_embedding_documents_body_parent_file_ids import GetEmbeddingDocumentsBodyParentFileIds
 from carbon.model.get_embedding_documents_body_query_vector import GetEmbeddingDocumentsBodyQueryVector
 from carbon.model.get_embedding_documents_body_tags import GetEmbeddingDocumentsBodyTags
+from carbon.model.gitbook_authetication import GitbookAuthetication
 from carbon.model.gitbook_connect_request import GitbookConnectRequest
 from carbon.model.gitbook_sync_request import GitbookSyncRequest
 from carbon.model.gitbook_sync_request_space_ids import GitbookSyncRequestSpaceIds
 from carbon.model.gmail_sync_input import GmailSyncInput
 from carbon.model.http_validation_error import HTTPValidationError
 from carbon.model.hybrid_search_tuning_params import HybridSearchTuningParams
 from carbon.model.hybrid_search_tuning_params_nullable import HybridSearchTuningParamsNullable
 from carbon.model.list_data_source_items_request import ListDataSourceItemsRequest
 from carbon.model.list_data_source_items_response import ListDataSourceItemsResponse
 from carbon.model.list_request import ListRequest
 from carbon.model.list_response import ListResponse
 from carbon.model.modify_user_configuration_input import ModifyUserConfigurationInput
+from carbon.model.notion_authentication import NotionAuthentication
+from carbon.model.o_auth_authentication import OAuthAuthentication
 from carbon.model.o_auth_url_request import OAuthURLRequest
 from carbon.model.order_dir import OrderDir
 from carbon.model.organization_response import OrganizationResponse
 from carbon.model.organization_user_data_source_api import OrganizationUserDataSourceAPI
 from carbon.model.organization_user_data_source_filters import OrganizationUserDataSourceFilters
 from carbon.model.organization_user_data_source_filters_ids import OrganizationUserDataSourceFiltersIds
 from carbon.model.organization_user_data_source_order_by_columns import OrganizationUserDataSourceOrderByColumns
@@ -97,25 +104,30 @@
 from carbon.model.pagination import Pagination
 from carbon.model.presigned_url_response import PresignedURLResponse
 from carbon.model.rss_feed_input import RSSFeedInput
 from carbon.model.raw_text_input import RawTextInput
 from carbon.model.resync_file_query_input import ResyncFileQueryInput
 from carbon.model.revoke_access_token_input import RevokeAccessTokenInput
 from carbon.model.s3_auth_request import S3AuthRequest
+from carbon.model.s3_authentication import S3Authentication
 from carbon.model.s3_file_sync_input import S3FileSyncInput
 from carbon.model.s3_get_file_input import S3GetFileInput
+from carbon.model.salesforce_authentication import SalesforceAuthentication
+from carbon.model.sharepoint_authentication import SharepointAuthentication
+from carbon.model.simple_o_auth_data_sources import SimpleOAuthDataSources
 from carbon.model.single_chunks_and_embeddings_upload_input import SingleChunksAndEmbeddingsUploadInput
 from carbon.model.sitemap_scrape_request import SitemapScrapeRequest
 from carbon.model.sitemap_scrape_request_css_classes_to_skip import SitemapScrapeRequestCssClassesToSkip
 from carbon.model.sitemap_scrape_request_css_selectors_to_skip import SitemapScrapeRequestCssSelectorsToSkip
 from carbon.model.sitemap_scrape_request_html_tags_to_skip import SitemapScrapeRequestHtmlTagsToSkip
 from carbon.model.sitemap_scrape_request_tags import SitemapScrapeRequestTags
 from carbon.model.sync_directory_request import SyncDirectoryRequest
 from carbon.model.sync_files_ids import SyncFilesIds
 from carbon.model.sync_files_request import SyncFilesRequest
+from carbon.model.sync_options import SyncOptions
 from carbon.model.text_embedding_generators import TextEmbeddingGenerators
 from carbon.model.token_response import TokenResponse
 from carbon.model.upload_file_from_url_input import UploadFileFromUrlInput
 from carbon.model.user_file import UserFile
 from carbon.model.user_file_embedding_properties import UserFileEmbeddingProperties
 from carbon.model.user_files_v2 import UserFilesV2
 from carbon.model.user_request_content import UserRequestContent
@@ -136,7 +148,9 @@
 from carbon.model.webscrape_request_css_selectors_to_skip import WebscrapeRequestCssSelectorsToSkip
 from carbon.model.webscrape_request_html_tags_to_skip import WebscrapeRequestHtmlTagsToSkip
 from carbon.model.webscrape_request_tags import WebscrapeRequestTags
 from carbon.model.white_labeling_response import WhiteLabelingResponse
 from carbon.model.youtube_transcript_response import YoutubeTranscriptResponse
 from carbon.model.youtube_transcript_response_raw_transcript import YoutubeTranscriptResponseRawTranscript
 from carbon.model.youtube_transcript_response_raw_transcript_item import YoutubeTranscriptResponseRawTranscriptItem
+from carbon.model.zendesk_authentication import ZendeskAuthentication
+from carbon.model.zotero_authentication import ZoteroAuthentication
```

### Comparing `carbon_python_sdk-0.1.8/carbon/operation_parameter_map.py` & `carbon_python_sdk-0.1.9/carbon/operation_parameter_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,14 +339,24 @@
             },
         ]
     },
     '/health-GET': {
         'parameters': [
         ]
     },
+    '/integrations/connect-POST': {
+        'parameters': [
+            {
+                'name': 'authentication'
+            },
+            {
+                'name': 'sync_options'
+            },
+        ]
+    },
     '/integrations/freshdesk-POST': {
         'parameters': [
             {
                 'name': 'domain'
             },
             {
                 'name': 'api_key'
```

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/__init__.py` & `carbon_python_sdk-0.1.9/carbon/paths/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # from carbon.apis.path_to_api import path_to_api
 
 import enum
 
 
 class PathValues(str, enum.Enum):
     INTEGRATIONS_OAUTH_URL = "/integrations/oauth_url"
+    INTEGRATIONS_CONNECT = "/integrations/connect"
     INTEGRATIONS_ITEMS_SYNC = "/integrations/items/sync"
     INTEGRATIONS_ITEMS_LIST = "/integrations/items/list"
     INTEGRATIONS_FILES_SYNC = "/integrations/files/sync"
     INTEGRATIONS_CONFLUENCE_LIST = "/integrations/confluence/list"
     INTEGRATIONS_CONFLUENCE_SYNC = "/integrations/confluence/sync"
     INTEGRATIONS_S3 = "/integrations/s3"
     INTEGRATIONS_S3_FILES = "/integrations/s3/files"
```

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/add_webhook/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/add_webhook/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/add_webhook/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/add_webhook/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/auth_v1_access_token/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/auth_v1_access_token/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/auth_v1_access_token/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/auth_v1_access_token/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/auth_v1_white_labeling/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/auth_v1_white_labeling/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/auth_v1_white_labeling/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/auth_v1_white_labeling/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/create_user_file_tags/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/create_user_file_tags/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/create_user_file_tags/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/create_user_file_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_files/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/delete_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_files/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/delete_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_user_file_tags/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/delete_user_file_tags/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_user_file_tags/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/delete_user_file_tags/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_users/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/delete_users/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_users/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/delete_users/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_webhook_webhook_id/delete.py` & `carbon_python_sdk-0.1.9/carbon/paths/delete_webhook_webhook_id/delete.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/delete_webhook_webhook_id/delete.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/delete_webhook_webhook_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/deletefile_file_id/delete.py` & `carbon_python_sdk-0.1.9/carbon/paths/deletefile_file_id/delete.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/deletefile_file_id/delete.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/deletefile_file_id/delete.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/embeddings/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/embeddings/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/embeddings/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/embeddings/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/fetch_urls/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/fetch_urls/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/fetch_urls/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/fetch_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/fetch_youtube_transcript/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/fetch_youtube_transcript/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/fetch_youtube_transcript/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/fetch_youtube_transcript/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/health/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/health/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/health/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/health/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_list/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_list/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_list/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_list/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_sync/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_confluence_sync/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_confluence_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_files_sync/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_files_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_files_sync/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_files_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_freshdesk/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_freshdesk/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_freshdesk/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_freshdesk/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_spaces/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_spaces/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_spaces/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_spaces/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_sync/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gitbook_sync/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gitbook_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_sync/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_sync/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_user_labels/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_user_labels/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_gmail_user_labels/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_gmail_user_labels/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_items_list/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_items_list/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_items_list/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_items_list/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_items_sync/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_items_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_items_sync/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_items_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_oauth_url/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_oauth_url/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_oauth_url/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_oauth_url/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_sync/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_sync/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_sync/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_sync/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_categories/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_categories/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_categories/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_categories/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_folders/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_folders/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_outlook_user_folders/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_outlook_user_folders/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_rss_feed/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_rss_feed/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_rss_feed/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_rss_feed/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_s3/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_s3/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_s3/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_s3/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_s3_files/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_s3_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/integrations_s3_files/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/integrations_s3_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/modify_user_configuration/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/modify_user_configuration/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/modify_user_configuration/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/modify_user_configuration/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/organization/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/organization/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/organization/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/organization/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/parsed_file_file_id/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/parsed_file_file_id/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/parsed_file_file_id/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/parsed_file_file_id/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/process_sitemap/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/process_sitemap/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/process_sitemap/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/process_sitemap/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/raw_file_file_id/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/raw_file_file_id/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/raw_file_file_id/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/raw_file_file_id/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/resync_file/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/resync_file/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/resync_file/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/resync_file/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/revoke_access_token/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/revoke_access_token/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/revoke_access_token/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/revoke_access_token/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/scrape_sitemap/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/scrape_sitemap/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/scrape_sitemap/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/scrape_sitemap/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/search_urls/get.py` & `carbon_python_sdk-0.1.9/carbon/paths/search_urls/get.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/search_urls/get.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/search_urls/get.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/text_chunks/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/text_chunks/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/text_chunks/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/text_chunks/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/upload_chunks_and_embeddings/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/upload_chunks_and_embeddings/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/upload_chunks_and_embeddings/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/upload_chunks_and_embeddings/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/upload_file_from_url/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/upload_file_from_url/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/upload_file_from_url/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/upload_file_from_url/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/upload_text/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/upload_text/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/upload_text/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/upload_text/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/uploadfile/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/uploadfile/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/uploadfile/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/uploadfile/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/user/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/user/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user_data_sources/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/user_data_sources/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user_data_sources/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/user_data_sources/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user_files/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/user_files/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user_files/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/user_files/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user_files_v2/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/user_files_v2/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/user_files_v2/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/user_files_v2/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/web_scrape/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/web_scrape/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/web_scrape/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/web_scrape/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/webhooks/post.py` & `carbon_python_sdk-0.1.9/carbon/paths/webhooks/post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/paths/webhooks/post.pyi` & `carbon_python_sdk-0.1.9/carbon/paths/webhooks/post.pyi`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/chunk_properties.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/chunk_properties_nullable.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/chunks_and_embeddings.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/data_source_type.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/data_source_type_nullable.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/delete_files_query_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/delete_users_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/directory_item.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/document_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/document_response_list.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embedding_and_chunk.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embedding_generators.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embedding_generators_nullable.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embedding_properties.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/external_file_sync_statuses.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/external_file_sync_statuses.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/external_source_item.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/fetch_urls_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/file_formats.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/file_formats_nullable.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/file_statistics.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/file_statistics_nullable.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/fresh_desk_connect_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/generic_success_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/get_embedding_documents_body.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/gitbook_connect_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/gitbook_sync_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/gmail_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/http_validation_error.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/list_data_source_items_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/list_data_source_items_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/list_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/list_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/modify_user_configuration_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/o_auth_url_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/o_auth_url_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_filters.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_data_source_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_data_source_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_file_tag_create.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/outlook_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/pagination.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/presigned_url_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/raw_text_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/resync_file_query_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/revoke_access_token_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/rss_feed_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/s3_auth_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/s3_file_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/s3_get_file_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/sitemap_scrape_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/sync_directory_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/sync_files_ids.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/sync_files_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/text_embedding_generators.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/token_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/upload_file_from_url_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/upload_file_from_url_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/user_file.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/user_files_v2.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/user_request_content.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/user_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/validation_error.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/webhook.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/webhook_filters.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/webhook_no_key.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/webhook_query_input.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/webhook_query_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/webscrape_request.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/white_labeling_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/youtube_transcript_response.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/pydantic/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.1.9/carbon/pydantic/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/request_after_hook.py` & `carbon_python_sdk-0.1.9/carbon/request_after_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/request_before_hook.py` & `carbon_python_sdk-0.1.9/carbon/request_before_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/request_before_url_hook.py` & `carbon_python_sdk-0.1.9/carbon/request_before_url_hook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/rest.py` & `carbon_python_sdk-0.1.9/carbon/rest.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/schemas.py` & `carbon_python_sdk-0.1.9/carbon/schemas.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/add_webhook_props.py` & `carbon_python_sdk-0.1.9/carbon/type/add_webhook_props.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/body_create_upload_file_uploadfile_post.py` & `carbon_python_sdk-0.1.9/carbon/type/body_create_upload_file_uploadfile_post.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/chunk_properties.py` & `carbon_python_sdk-0.1.9/carbon/type/chunk_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/chunk_properties_nullable.py` & `carbon_python_sdk-0.1.9/carbon/type/chunk_properties_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/chunks_and_embeddings.py` & `carbon_python_sdk-0.1.9/carbon/type/chunks_and_embeddings.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.1.9/carbon/type/chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/data_source_type.py` & `carbon_python_sdk-0.1.9/carbon/type/data_source_type.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/data_source_type_nullable.py` & `carbon_python_sdk-0.1.9/carbon/type/data_source_type_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/delete_files_query_input.py` & `carbon_python_sdk-0.1.9/carbon/type/delete_files_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/delete_users_input.py` & `carbon_python_sdk-0.1.9/carbon/type/delete_users_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/directory_item.py` & `carbon_python_sdk-0.1.9/carbon/type/directory_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/document_response.py` & `carbon_python_sdk-0.1.9/carbon/type/document_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/document_response_list.py` & `carbon_python_sdk-0.1.9/carbon/type/document_response_list.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embedding_and_chunk.py` & `carbon_python_sdk-0.1.9/carbon/type/embedding_and_chunk.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embedding_generators.py` & `carbon_python_sdk-0.1.9/carbon/type/embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embedding_generators_nullable.py` & `carbon_python_sdk-0.1.9/carbon/type/embedding_generators_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embedding_properties.py` & `carbon_python_sdk-0.1.9/carbon/type/embedding_properties.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_filters.py` & `carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_query_input.py` & `carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/embeddings_and_chunks_response.py` & `carbon_python_sdk-0.1.9/carbon/type/embeddings_and_chunks_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/external_source_item.py` & `carbon_python_sdk-0.1.9/carbon/type/external_source_item.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/fetch_urls_response.py` & `carbon_python_sdk-0.1.9/carbon/type/fetch_urls_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/file_formats.py` & `carbon_python_sdk-0.1.9/carbon/type/file_formats.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/file_formats_nullable.py` & `carbon_python_sdk-0.1.9/carbon/type/file_formats_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/file_statistics.py` & `carbon_python_sdk-0.1.9/carbon/type/file_statistics.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/file_statistics_nullable.py` & `carbon_python_sdk-0.1.9/carbon/type/file_statistics_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/fresh_desk_connect_request.py` & `carbon_python_sdk-0.1.9/carbon/type/fresh_desk_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/generic_success_response.py` & `carbon_python_sdk-0.1.9/carbon/type/generic_success_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/get_embedding_documents_body.py` & `carbon_python_sdk-0.1.9/carbon/type/get_embedding_documents_body.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/gitbook_connect_request.py` & `carbon_python_sdk-0.1.9/carbon/type/gitbook_connect_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/gitbook_sync_request.py` & `carbon_python_sdk-0.1.9/carbon/type/gitbook_sync_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/gmail_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/type/gmail_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/http_validation_error.py` & `carbon_python_sdk-0.1.9/carbon/type/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/hybrid_search_tuning_params.py` & `carbon_python_sdk-0.1.9/carbon/type/hybrid_search_tuning_params.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/hybrid_search_tuning_params_nullable.py` & `carbon_python_sdk-0.1.9/carbon/type/hybrid_search_tuning_params_nullable.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/list_data_source_items_request.py` & `carbon_python_sdk-0.1.9/carbon/type/list_data_source_items_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/list_data_source_items_response.py` & `carbon_python_sdk-0.1.9/carbon/type/list_data_source_items_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/list_request.py` & `carbon_python_sdk-0.1.9/carbon/type/list_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/list_response.py` & `carbon_python_sdk-0.1.9/carbon/type/list_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/modify_user_configuration_input.py` & `carbon_python_sdk-0.1.9/carbon/type/modify_user_configuration_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/o_auth_url_request.py` & `carbon_python_sdk-0.1.9/carbon/type/o_auth_url_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_response.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_api.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,43 +10,22 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
-from carbon.type.data_source_last_sync_actions import DataSourceLastSyncActions
-from carbon.type.data_source_sync_statuses import DataSourceSyncStatuses
-from carbon.type.data_source_type import DataSourceType
+from carbon.type.data_source_type_nullable import DataSourceTypeNullable
+from carbon.type.organization_user_data_source_filters_ids import OrganizationUserDataSourceFiltersIds
 
-class RequiredOrganizationUserDataSourceAPI(TypedDict):
-    id: int
-
-    data_source_external_id: typing.Optional[str]
-
-    data_source_type: DataSourceType
-
-    sync_status: DataSourceSyncStatuses
-
-    source_items_synced_at: typing.Optional[datetime]
-
-    organization_user_id: int
-
-    organization_id: int
-
-    organization_supplied_user_id: str
-
-    revoked_access: bool
-
-    last_synced_at: datetime
-
-    last_sync_action: DataSourceLastSyncActions
+class RequiredOrganizationUserDataSourceFilters(TypedDict):
+    pass
 
-    created_at: datetime
+class OptionalOrganizationUserDataSourceFilters(TypedDict, total=False):
+    source: DataSourceTypeNullable
 
-    updated_at: datetime
+    ids: OrganizationUserDataSourceFiltersIds
 
-class OptionalOrganizationUserDataSourceAPI(TypedDict, total=False):
-    pass
+    revoked_access: typing.Optional[bool]
 
-class OrganizationUserDataSourceAPI(RequiredOrganizationUserDataSourceAPI, OptionalOrganizationUserDataSourceAPI):
+class OrganizationUserDataSourceFilters(RequiredOrganizationUserDataSourceFilters, OptionalOrganizationUserDataSourceFilters):
     pass
```

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_filters.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,22 +10,19 @@
 """
 
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
-from carbon.type.data_source_type_nullable import DataSourceTypeNullable
-from carbon.type.organization_user_data_source_filters_ids import OrganizationUserDataSourceFiltersIds
+from carbon.type.organization_user_data_source_api import OrganizationUserDataSourceAPI
 
-class RequiredOrganizationUserDataSourceFilters(TypedDict):
-    pass
-
-class OptionalOrganizationUserDataSourceFilters(TypedDict, total=False):
-    source: DataSourceTypeNullable
+class RequiredOrganizationUserDataSourceResponse(TypedDict):
+    results: typing.List[OrganizationUserDataSourceAPI]
 
-    ids: OrganizationUserDataSourceFiltersIds
+    count: int
 
-    revoked_access: typing.Optional[bool]
+class OptionalOrganizationUserDataSourceResponse(TypedDict, total=False):
+    pass
 
-class OrganizationUserDataSourceFilters(RequiredOrganizationUserDataSourceFilters, OptionalOrganizationUserDataSourceFilters):
+class OrganizationUserDataSourceResponse(RequiredOrganizationUserDataSourceResponse, OptionalOrganizationUserDataSourceResponse):
     pass
```

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_query_input.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_data_source_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_data_source_response.py` & `carbon_python_sdk-0.1.9/carbon/type/connect_data_source_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from datetime import datetime, date
 import typing
 from enum import Enum
 from typing_extensions import TypedDict, Literal, TYPE_CHECKING
 
 from carbon.type.organization_user_data_source_api import OrganizationUserDataSourceAPI
 
-class RequiredOrganizationUserDataSourceResponse(TypedDict):
-    results: typing.List[OrganizationUserDataSourceAPI]
+class RequiredConnectDataSourceResponse(TypedDict):
+    data_source: OrganizationUserDataSourceAPI
 
-    count: int
+    sync_url: typing.Optional[str]
 
-class OptionalOrganizationUserDataSourceResponse(TypedDict, total=False):
+class OptionalConnectDataSourceResponse(TypedDict, total=False):
     pass
 
-class OrganizationUserDataSourceResponse(RequiredOrganizationUserDataSourceResponse, OptionalOrganizationUserDataSourceResponse):
+class ConnectDataSourceResponse(RequiredConnectDataSourceResponse, OptionalConnectDataSourceResponse):
     pass
```

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_file_tag_create.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_file_tag_create.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_file_tags_remove.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_file_tags_remove.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_filters.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/organization_user_files_to_sync_query_input.py` & `carbon_python_sdk-0.1.9/carbon/type/organization_user_files_to_sync_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/outh_url_response.py` & `carbon_python_sdk-0.1.9/carbon/type/outh_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/outlook_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/type/outlook_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/pagination.py` & `carbon_python_sdk-0.1.9/carbon/type/pagination.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/presigned_url_response.py` & `carbon_python_sdk-0.1.9/carbon/type/presigned_url_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/raw_text_input.py` & `carbon_python_sdk-0.1.9/carbon/type/raw_text_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/resync_file_query_input.py` & `carbon_python_sdk-0.1.9/carbon/type/resync_file_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/revoke_access_token_input.py` & `carbon_python_sdk-0.1.9/carbon/type/revoke_access_token_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/rss_feed_input.py` & `carbon_python_sdk-0.1.9/carbon/type/rss_feed_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/s3_auth_request.py` & `carbon_python_sdk-0.1.9/carbon/type/s3_auth_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/s3_file_sync_input.py` & `carbon_python_sdk-0.1.9/carbon/type/s3_file_sync_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/s3_get_file_input.py` & `carbon_python_sdk-0.1.9/carbon/type/s3_get_file_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/single_chunks_and_embeddings_upload_input.py` & `carbon_python_sdk-0.1.9/carbon/type/single_chunks_and_embeddings_upload_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/sitemap_scrape_request.py` & `carbon_python_sdk-0.1.9/carbon/type/sitemap_scrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/sync_directory_request.py` & `carbon_python_sdk-0.1.9/carbon/type/sync_directory_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/sync_files_ids.py` & `carbon_python_sdk-0.1.9/carbon/type/sync_files_ids.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/sync_files_request.py` & `carbon_python_sdk-0.1.9/carbon/type/sync_files_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/text_embedding_generators.py` & `carbon_python_sdk-0.1.9/carbon/type/text_embedding_generators.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/token_response.py` & `carbon_python_sdk-0.1.9/carbon/type/token_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/upload_file_from_url_input.py` & `carbon_python_sdk-0.1.9/carbon/type/upload_file_from_url_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/user_file.py` & `carbon_python_sdk-0.1.9/carbon/type/user_file.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/user_files_v2.py` & `carbon_python_sdk-0.1.9/carbon/type/user_files_v2.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/user_request_content.py` & `carbon_python_sdk-0.1.9/carbon/type/user_request_content.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/user_response.py` & `carbon_python_sdk-0.1.9/carbon/type/user_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/validation_error.py` & `carbon_python_sdk-0.1.9/carbon/type/validation_error.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/webhook.py` & `carbon_python_sdk-0.1.9/carbon/type/webhook.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/webhook_filters.py` & `carbon_python_sdk-0.1.9/carbon/type/webhook_filters.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/webhook_no_key.py` & `carbon_python_sdk-0.1.9/carbon/type/webhook_no_key.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/webhook_query_input.py` & `carbon_python_sdk-0.1.9/carbon/type/webhook_query_input.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/webhook_query_response.py` & `carbon_python_sdk-0.1.9/carbon/type/webhook_query_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/webscrape_request.py` & `carbon_python_sdk-0.1.9/carbon/type/webscrape_request.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/white_labeling_response.py` & `carbon_python_sdk-0.1.9/carbon/type/white_labeling_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/youtube_transcript_response.py` & `carbon_python_sdk-0.1.9/carbon/type/youtube_transcript_response.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type/youtube_transcript_response_raw_transcript.py` & `carbon_python_sdk-0.1.9/carbon/type/youtube_transcript_response_raw_transcript.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/type_util.py` & `carbon_python_sdk-0.1.9/carbon/type_util.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/carbon/validation_metadata.py` & `carbon_python_sdk-0.1.9/carbon/validation_metadata.py`

 * *Files identical despite different names*

### Comparing `carbon_python_sdk-0.1.8/pyproject.toml` & `carbon_python_sdk-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "carbon-python-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = "Client for Carbon"
 authors = ["Konfig <engineering@konfigthis.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "carbon"}]
 
 [tool.poetry.dependencies]
```

### Comparing `carbon_python_sdk-0.1.8/PKG-INFO` & `carbon_python_sdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carbon-python-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client for Carbon
 License: MIT
 Author: Konfig
 Author-email: engineering@konfigthis.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 [![Visit Carbon](https://raw.githubusercontent.com/Carbon-for-Developers/carbon-sdks/HEAD/python/header.png)](https://carbon.ai)
 
 # Carbon<a id="carbon"></a>
 
 Connect external data to LLMs, no matter the source.
 
 
-[![PyPI](https://img.shields.io/badge/PyPI-v0.1.8-blue)](https://pypi.org/project/carbon-python-sdk/0.1.8)
+[![PyPI](https://img.shields.io/badge/PyPI-v0.1.9-blue)](https://pypi.org/project/carbon-python-sdk/0.1.9)
 [![README.md](https://img.shields.io/badge/README-Click%20Here-green)](https://github.com/Carbon-for-Developers/carbon-sdks/tree/main/python#readme)
 
 </div>
 
 ## Table of Contents<a id="table-of-contents"></a>
 
 <!-- toc -->
@@ -63,14 +63,15 @@
   * [`carbon.files.query_user_files`](#carbonfilesquery_user_files)
   * [`carbon.files.query_user_files_deprecated`](#carbonfilesquery_user_files_deprecated)
   * [`carbon.files.resync`](#carbonfilesresync)
   * [`carbon.files.upload`](#carbonfilesupload)
   * [`carbon.files.upload_from_url`](#carbonfilesupload_from_url)
   * [`carbon.files.upload_text`](#carbonfilesupload_text)
   * [`carbon.health.check`](#carbonhealthcheck)
+  * [`carbon.integrations.connect_data_source`](#carbonintegrationsconnect_data_source)
   * [`carbon.integrations.connect_freshdesk`](#carbonintegrationsconnect_freshdesk)
   * [`carbon.integrations.connect_gitbook`](#carbonintegrationsconnect_gitbook)
   * [`carbon.integrations.create_aws_iam_user`](#carbonintegrationscreate_aws_iam_user)
   * [`carbon.integrations.get_oauth_url`](#carbonintegrationsget_oauth_url)
   * [`carbon.integrations.list_confluence_pages`](#carbonintegrationslist_confluence_pages)
   * [`carbon.integrations.list_data_source_items`](#carbonintegrationslist_data_source_items)
   * [`carbon.integrations.list_folders`](#carbonintegrationslist_folders)
@@ -104,15 +105,15 @@
 ## Requirements<a id="requirements"></a>
 
 Python >=3.7
 
 ## Installation<a id="installation"></a>
 
 ```sh
-pip install carbon-python-sdk==0.1.8
+pip install carbon-python-sdk==0.1.9
 ```
 
 ## Getting Started<a id="getting-started"></a>
 
 ```python
 from carbon import Carbon
 
@@ -1256,14 +1257,62 @@
 
 `/health` `get`
 
 [🔙 **Back to Table of Contents**](#table-of-contents)
 
 ---
 
+### `carbon.integrations.connect_data_source`<a id="carbonintegrationsconnect_data_source"></a>
+
+Connect Data Source
+
+#### 🛠️ Usage<a id="🛠️-usage"></a>
+
+```python
+connect_data_source_response = carbon.integrations.connect_data_source(
+    authentication={
+        "source": "GOOGLE_DRIVE",
+        "access_token": "access_token_example",
+    },
+    sync_options={
+        "chunk_size": 1500,
+        "chunk_overlap": 20,
+        "skip_embedding_generation": False,
+        "embedding_model": "OPENAI",
+        "generate_sparse_vectors": False,
+        "prepend_filename_to_chunks": False,
+        "sync_files_on_connection": True,
+        "set_page_as_boundary": False,
+    },
+)
+```
+
+#### ⚙️ Parameters<a id="⚙️-parameters"></a>
+
+##### authentication: Union[`OAuthAuthentication`, `NotionAuthentication`, `SharepointAuthentication`, `ConfluenceAuthentication`, `ZendeskAuthentication`, `ZoteroAuthentication`, `GitbookAuthetication`, `SalesforceAuthentication`, `FreskdeskAuthentication`, `S3Authentication`]<a id="authentication-unionoauthauthentication-notionauthentication-sharepointauthentication-confluenceauthentication-zendeskauthentication-zoteroauthentication-gitbookauthetication-salesforceauthentication-freskdeskauthentication-s3authentication"></a>
+
+
+##### sync_options: [`SyncOptions`](./carbon/type/sync_options.py)<a id="sync_options-syncoptionscarbontypesync_optionspy"></a>
+
+
+#### ⚙️ Request Body<a id="⚙️-request-body"></a>
+
+[`ConnectDataSourceInput`](./carbon/type/connect_data_source_input.py)
+#### 🔄 Return<a id="🔄-return"></a>
+
+[`ConnectDataSourceResponse`](./carbon/pydantic/connect_data_source_response.py)
+
+#### 🌐 Endpoint<a id="🌐-endpoint"></a>
+
+`/integrations/connect` `post`
+
+[🔙 **Back to Table of Contents**](#table-of-contents)
+
+---
+
 ### `carbon.integrations.connect_freshdesk`<a id="carbonintegrationsconnect_freshdesk"></a>
 
 Refer this article to obtain an API key https://support.freshdesk.com/en/support/solutions/articles/215517.
 Make sure that your API key has the permission to read solutions from your account and you are on a <b>paid</b> plan.
 Once you have an API key, you can make a request to this endpoint along with your freshdesk domain. This will 
 trigger an automatic sync of the articles in your "solutions" tab. Additional parameters below can be used to associate 
 data with the synced articles or modify the sync behavior.
```

