# Comparing `tmp/xingchen-1.1.1.tar.gz` & `tmp/xingchen-1.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingchen-1.1.1.tar", last modified: Thu May  2 15:18:37 2024, max compression
+gzip compressed data, was "xingchen-1.1.1.1.tar", last modified: Mon Apr  1 09:21:23 2024, max compression
```

## Comparing `xingchen-1.1.1.tar` & `xingchen-1.1.1.1.tar`

### file list

```diff
@@ -1,150 +1,119 @@
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.538490 xingchen-1.1.1/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-02 15:18:37.538590 xingchen-1.1.1/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)    11848 2024-05-02 15:15:25.000000 xingchen-1.1.1/README.md
--rw-r--r--   0 frankin    (501) staff       (20)      771 2024-05-02 15:02:56.000000 xingchen-1.1.1/pyproject.toml
--rw-r--r--   0 frankin    (501) staff       (20)       69 2024-05-02 15:18:37.538930 xingchen-1.1.1/setup.cfg
--rw-r--r--   0 frankin    (501) staff       (20)     1152 2024-05-02 15:03:02.000000 xingchen-1.1.1/setup.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.486548 xingchen-1.1.1/test/
--rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.1/test/test_base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     3120 2024-04-11 03:27:03.000000 xingchen-1.1.1/test/test_base_chat_request_aca_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.1/test/test_character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.1/test/test_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.1/test/test_character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.1/test/test_character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.1/test/test_character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.1/test/test_chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.1/test/test_chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_message.py
--rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.1/test/test_message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.1/test/test_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.1/test/test_result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.1/test/test_result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.1/test/test_result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.1/test/test_sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.1/test/test_user_profile.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.489544 xingchen-1.1.1/xingchen/
--rw-r--r--   0 frankin    (501) staff       (20)     6093 2024-04-25 08:50:36.000000 xingchen-1.1.1/xingchen/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     3290 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/aca_util.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.493831 xingchen-1.1.1/xingchen/api/
--rw-r--r--   0 frankin    (501) staff       (20)      410 2024-04-25 08:50:36.000000 xingchen-1.1.1/xingchen/api/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)    60683 2024-04-25 09:41:08.000000 xingchen-1.1.1/xingchen/api/character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    12628 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     8021 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/chat_extract_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    29175 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     7592 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/api/common_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     5384 2024-04-11 06:12:19.000000 xingchen-1.1.1/xingchen/api/groupchat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/api_client.py
--rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/api_response.py
--rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/configuration.py
--rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/exceptions.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.534247 xingchen-1.1.1/xingchen/models/
--rw-r--r--   0 frankin    (501) staff       (20)     3374 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.1/xingchen/models/advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2618 2024-04-11 03:27:03.000000 xingchen-1.1.1/xingchen/models/base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     4766 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.1/xingchen/models/character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2023 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/character_desc_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2345 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/character_desc_generated_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.1/xingchen/models/character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2686 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     5138 2024-04-25 09:41:54.000000 xingchen-1.1.1/xingchen/models/character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4759 2024-04-25 09:19:54.000000 xingchen-1.1.1/xingchen/models/character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.1/xingchen/models/chat_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     6915 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.1/xingchen/models/context.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.536452 xingchen-1.1.1/xingchen/models/custom/
--rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/custom/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/custom/base_response.py
--rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.1/xingchen/models/custom/character_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4815 2024-03-05 07:11:26.000000 xingchen-1.1.1/xingchen/models/custom/chat_response.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.538106 xingchen-1.1.1/xingchen/models/custom/groupchat/
--rw-r--r--   0 frankin    (501) staff       (20)       92 2024-04-09 12:57:52.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2778 2024-04-11 07:45:59.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     1763 2024-04-09 13:04:39.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_reply_setting.py
--rw-r--r--   0 frankin    (501) staff       (20)     1303 2024-04-11 02:56:10.000000 xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_room_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.1/xingchen/models/custom/platform_publish_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.1/xingchen/models/custom/reset_history_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1778 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/extract_data.py
--rw-r--r--   0 frankin    (501) staff       (20)     2162 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/extract_kv_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2399 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/extract_memory_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/extract_summary_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1718 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/file_conver_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1712 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/file_conver_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.1/xingchen/models/function_call.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2494 2024-04-11 07:26:08.000000 xingchen-1.1.1/xingchen/models/input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1506 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/keyword.py
--rw-r--r--   0 frankin    (501) staff       (20)     1698 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/kv_memory_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     2237 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/long_term_memory.py
--rw-r--r--   0 frankin    (501) staff       (20)     2089 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/memory.py
--rw-r--r--   0 frankin    (501) staff       (20)     1582 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/memory_summary.py
--rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.1/xingchen/models/message.py
--rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.1/xingchen/models/model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1681 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/platform_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2009 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/polling_image_detail_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1965 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/reject_answer_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2303 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/reject_condition.py
--rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     2561 2024-04-25 05:48:37.000000 xingchen-1.1.1/xingchen/models/result_dto_character_desc_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2517 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_extract_kv_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2573 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_extract_summary_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2539 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_file_conver_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2617 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/result_dto_polling_image_detail_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.1/xingchen/models/scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1702 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/stop_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.1/xingchen/models/sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2193 2024-04-24 06:58:03.000000 xingchen-1.1.1/xingchen/models/text_to_image_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/models/user_profile.py
--rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/py.typed
--rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.1/xingchen/rest.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-02 15:18:37.490853 xingchen-1.1.1/xingchen.egg-info/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)     5014 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/SOURCES.txt
--rw-r--r--   0 frankin    (501) staff       (20)        1 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/dependency_links.txt
--rw-r--r--   0 frankin    (501) staff       (20)       85 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/requires.txt
--rw-r--r--   0 frankin    (501) staff       (20)        9 2024-05-02 15:18:37.000000 xingchen-1.1.1/xingchen.egg-info/top_level.txt
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.269419 xingchen-1.1.1.1/
+-rw-r--r--   0 frankin    (501) staff       (20)      335 2024-04-01 09:21:23.269535 xingchen-1.1.1.1/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)    11507 2024-03-05 07:56:13.000000 xingchen-1.1.1.1/README.md
+-rw-r--r--   0 frankin    (501) staff       (20)      773 2024-04-01 09:19:09.000000 xingchen-1.1.1.1/pyproject.toml
+-rw-r--r--   0 frankin    (501) staff       (20)       69 2024-04-01 09:21:23.269965 xingchen-1.1.1.1/setup.cfg
+-rw-r--r--   0 frankin    (501) staff       (20)     1154 2024-04-01 09:18:50.000000 xingchen-1.1.1.1/setup.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.223782 xingchen-1.1.1.1/test/
+-rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.1.1/test/test_base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3169 2024-03-05 07:23:22.000000 xingchen-1.1.1.1/test/test_base_chat_request_aca_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.1.1/test/test_character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.1.1/test/test_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.1.1/test/test_character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.1.1/test/test_character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.1.1/test/test_character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.1.1/test/test_chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.1.1/test/test_chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.1.1/test/test_message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.1.1/test/test_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.1.1/test/test_result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.1.1/test/test_result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.1.1/test/test_result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.1.1/test/test_sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/test/test_user_profile.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.226255 xingchen-1.1.1.1/xingchen/
+-rw-r--r--   0 frankin    (501) staff       (20)     4083 2024-03-06 06:57:10.000000 xingchen-1.1.1.1/xingchen/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2161 2024-02-01 06:42:31.000000 xingchen-1.1.1.1/xingchen/aca_util.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.229699 xingchen-1.1.1.1/xingchen/api/
+-rw-r--r--   0 frankin    (501) staff       (20)      220 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)    55637 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api/character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     9376 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api/chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    25469 2024-02-01 06:52:29.000000 xingchen-1.1.1.1/xingchen/api/chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api_client.py
+-rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/api_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/configuration.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/exceptions.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.265954 xingchen-1.1.1.1/xingchen/models/
+-rw-r--r--   0 frankin    (501) staff       (20)     2988 2024-03-05 07:09:19.000000 xingchen-1.1.1.1/xingchen/models/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.1.1/xingchen/models/advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2973 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3093 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/base_chat_request_aca_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4106 2024-03-07 08:00:51.000000 xingchen-1.1.1.1/xingchen/models/character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.1.1/xingchen/models/character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.1.1/xingchen/models/character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2408 2023-11-24 13:03:37.000000 xingchen-1.1.1.1/xingchen/models/character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5127 2024-03-07 08:02:16.000000 xingchen-1.1.1.1/xingchen/models/character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4748 2024-03-06 06:39:36.000000 xingchen-1.1.1.1/xingchen/models/character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.1.1/xingchen/models/chat_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     6702 2024-03-05 07:40:25.000000 xingchen-1.1.1.1/xingchen/models/chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.1.1/xingchen/models/context.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.268890 xingchen-1.1.1.1/xingchen/models/custom/
+-rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/custom/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/custom/base_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.1.1/xingchen/models/custom/character_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4815 2024-03-05 07:11:26.000000 xingchen-1.1.1.1/xingchen/models/custom/chat_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.1.1/xingchen/models/custom/platform_publish_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.1.1/xingchen/models/custom/reset_history_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.1.1/xingchen/models/function_call.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2505 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.1.1/xingchen/models/message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.1.1/xingchen/models/model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.1.1/xingchen/models/scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.1.1/xingchen/models/sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/models/user_profile.py
+-rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/py.typed
+-rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.1.1/xingchen/rest.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-04-01 09:21:23.227676 xingchen-1.1.1.1/xingchen.egg-info/
+-rw-r--r--   0 frankin    (501) staff       (20)      335 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)     3793 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/SOURCES.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        1 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/dependency_links.txt
+-rw-r--r--   0 frankin    (501) staff       (20)       85 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/requires.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        9 2024-04-01 09:21:23.000000 xingchen-1.1.1.1/xingchen.egg-info/top_level.txt
```

### Comparing `xingchen-1.1.1/README.md` & `xingchen-1.1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # [通义星尘](https://tongyi.aliyun.com/xingchen) Python SDK
 
 - API 版本: v2
-- Package 版本: 1.1.1
+- Package 版本: 1.0.5
 
 ## 运行环境
 
 Python 3.7+
 
 ## 安装/使用
 
@@ -19,26 +19,26 @@
 
 认证信息可在[通义星尘/接入管理](https://tongyi.aliyun.com/xingchen/accessManagement)官网创建。
 
 ```python
 
 import unittest
 
-from xingchen import Configuration, ApiClient, GroupChatApiSub, ChatReqParams, CharacterKey, Message, UserProfile,
+from xingchen import Configuration, ApiClient, ChatApiSub, ChatReqParams, CharacterKey, Message, UserProfile, \
     ModelParameters
 
 
 def build_chat_param():
     return ChatReqParams(
         bot_profile=CharacterKey(
             character_id="c39797a35ad243f1a85baaa6e1ec37e0",
             version=1
         ),
         model_parameters=ModelParameters(
-            top_p=0.8,
+            top_p=0.8,    
             temperature=0.8,
             seed=1683806810
         ),
         messages=[
             Message(
                 name='小明',
                 role='user',
@@ -77,15 +77,15 @@
     @staticmethod
     def init_client():
         configuration = Configuration(
             host="https://nlp.aliyuncs.com"
         )
         configuration.access_token = "{API-KEY}"
         with ApiClient(configuration) as api_client:
-            api_instance = GroupChatApiSub(api_client)
+            api_instance = ChatApiSub(api_client)
         return api_instance
 
     # 非流式回复
     def test_chat_sync(self):
         api = self.init_client()
         chat_param = build_chat_param()
         res = api.chat(chat_param)
@@ -248,19 +248,14 @@
 
 7. 验证
 ```commandline
 pip install {包名}=={版本名} -i https://www.pypi.org/simple/
 ```
 
 ## 版本变更
-### 1.1.1
-- 添加群聊逻辑 `GroupChatApiSub.chat(非流式)`, `GroupChatApiSub.streamOut(流式)` 
-- 添加通义万相图片轮训接口 `ChatMessageApiSub.polling_image_detail`
-- 添加角色描述自动生成接口 `CharacterApiSub.auto_generate_desc`
-- 添加角色记忆抽取接口 `ChatExtractMessageApiSub.extract_memory_kv`
 
 ### 1.1.0
 - 角色创建/更新接口，添加短长期记忆配置 `CharacterAdvancedConfig.shortTermMemory`, `CharacterAdvancedConfig.memory`
 - 角色创建/更新接口，添加模型配置 `CharacterPermissionConfig.modelConfig`
 - 对话接口支持返回结果数量配置 `ChatContext.resultCount`
```

### Comparing `xingchen-1.1.1/pyproject.toml` & `xingchen-1.1.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xingchen"
-version = "1.1.1"
+version = "1.1.1.1"
 description = "XingChen 开放接口定义"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "XingChen 开放接口定义"]
 include = ["xingchen/py.typed"]
```

### Comparing `xingchen-1.1.1/setup.py` & `xingchen-1.1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "xingchen"
-VERSION = "1.1.1"
+VERSION = "1.1.1.1"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum",
     "sseclient-py >= 1.8.0"
```

### Comparing `xingchen-1.1.1/test/test_advanced_settings.py` & `xingchen-1.1.1.1/test/test_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_base_chat_request.py` & `xingchen-1.1.1.1/test/test_base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_base_chat_request_aca_chat_ext_param.py` & `xingchen-1.1.1.1/test/test_base_chat_request_aca_chat_ext_param.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,26 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 import datetime
 
-from xingchen.models.base_chat_request import BaseChatRequest  # noqa: E501
+from xingchen.models.base_chat_request_aca_chat_ext_param import BaseChatRequestAcaChatExtParam  # noqa: E501
 
 class TestBaseChatRequestAcaChatExtParam(unittest.TestCase):
     """BaseChatRequestAcaChatExtParam unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> BaseChatRequest:
+    def make_instance(self, include_optional) -> BaseChatRequestAcaChatExtParam:
         """Test BaseChatRequestAcaChatExtParam
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `BaseChatRequestAcaChatExtParam`
         """
         model = BaseChatRequestAcaChatExtParam()  # noqa: E501
```

### Comparing `xingchen-1.1.1/test/test_character_advanced_config.py` & `xingchen-1.1.1.1/test/test_character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_api_sub.py` & `xingchen-1.1.1.1/test/test_character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_create_dto.py` & `xingchen-1.1.1.1/test/test_character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_dto.py` & `xingchen-1.1.1.1/test/test_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_key.py` & `xingchen-1.1.1.1/test/test_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_permission_config.py` & `xingchen-1.1.1.1/test/test_character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_query_dto.py` & `xingchen-1.1.1.1/test/test_character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_query_where.py` & `xingchen-1.1.1.1/test/test_character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_update_dto.py` & `xingchen-1.1.1.1/test/test_character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_character_version_create_or_update_dto.py` & `xingchen-1.1.1.1/test/test_character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_api_sub.py` & `xingchen-1.1.1.1/test/test_chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_history_query_dto.py` & `xingchen-1.1.1.1/test/test_chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_history_query_where.py` & `xingchen-1.1.1.1/test/test_chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_message_api_sub.py` & `xingchen-1.1.1.1/test/test_chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_message_dto.py` & `xingchen-1.1.1.1/test/test_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_req_params.py` & `xingchen-1.1.1.1/test/test_chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_chat_room_user_dto.py` & `xingchen-1.1.1.1/test/test_chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_context.py` & `xingchen-1.1.1.1/test/test_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_file_info_vo.py` & `xingchen-1.1.1.1/test/test_file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_gateway_context.py` & `xingchen-1.1.1.1/test/test_gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_gateway_issued_params.py` & `xingchen-1.1.1.1/test/test_gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_input.py` & `xingchen-1.1.1.1/test/test_input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_message.py` & `xingchen-1.1.1.1/test/test_message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_message_rating_request.py` & `xingchen-1.1.1.1/test/test_message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_meta.py` & `xingchen-1.1.1.1/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_model_parameters.py` & `xingchen-1.1.1.1/test/test_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_page_result_character_dto.py` & `xingchen-1.1.1.1/test/test_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_page_result_chat_message_dto.py` & `xingchen-1.1.1.1/test/test_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_repository.py` & `xingchen-1.1.1.1/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_repository_info.py` & `xingchen-1.1.1.1/test/test_repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_boolean.py` & `xingchen-1.1.1.1/test/test_result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_character_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_character_key.py` & `xingchen-1.1.1.1/test/test_result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_list_character_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_page_result_character_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.1.1/test/test_result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_scenario.py` & `xingchen-1.1.1.1/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_sys_reminder_request.py` & `xingchen-1.1.1.1/test/test_sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/test/test_user_profile.py` & `xingchen-1.1.1.1/test/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/__init__.py` & `xingchen-1.1.1.1/xingchen/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 
 __version__ = "1.0.7"
 
 # import apis into sdk package
 from xingchen.api.character_api_sub import CharacterApiSub
 from xingchen.api.chat_api_sub import ChatApiSub
 from xingchen.api.chat_message_api_sub import ChatMessageApiSub
-from xingchen.api.groupchat_api_sub import GroupChatApiSub
-from xingchen.api.chat_extract_message_api_sub import ChatExtractMessageApiSub
-from xingchen.api.common_api_sub import CommonApiSub
 
 # import ApiClient
 from xingchen.api_response import ApiResponse
 from xingchen.api_client import ApiClient
 from xingchen.configuration import Configuration
 from xingchen.exceptions import OpenApiException
 from xingchen.exceptions import ApiTypeError
@@ -33,15 +30,15 @@
 from xingchen.exceptions import ApiKeyError
 from xingchen.exceptions import ApiAttributeError
 from xingchen.exceptions import ApiException
 
 # import models into sdk package
 from xingchen.models.advanced_settings import AdvancedSettings
 from xingchen.models.base_chat_request import BaseChatRequest
-from xingchen.models.base_chat_request import BaseChatRequest
+from xingchen.models.base_chat_request_aca_chat_ext_param import BaseChatRequestAcaChatExtParam
 from xingchen.models.character_advanced_config import CharacterAdvancedConfig
 from xingchen.models.character_create_dto import CharacterCreateDTO
 from xingchen.models.character_dto import CharacterDTO
 from xingchen.models.character_key import CharacterKey
 from xingchen.models.character_permission_config import CharacterPermissionConfig
 from xingchen.models.character_query_dto import CharacterQueryDTO
 from xingchen.models.character_query_where import CharacterQueryWhere
@@ -76,35 +73,7 @@
 from xingchen.models.user_profile import UserProfile
 from xingchen.models.chat_context import ChatContext
 from xingchen.models.function_call import Function, FunctionChoice, FunctionCall, FunctionChoiceType, Plugin, \
     PlanningApiInfo
 from xingchen.models.custom.reset_history_request import ResetChatHistoryRequest
 from xingchen.models.custom.character_model_parameters import CharacterModelParameters
 from xingchen.models.custom.platform_publish_config import PlatformPublishConfig
-from xingchen.models.custom.groupchat.group_chat_reply_setting import GroupChatReplySetting
-from xingchen.models.custom.groupchat.group_chat_room_info import GroupChatRoomInfo
-from xingchen.models.custom.groupchat.group_chat_ext_param import GroupChatExtParam
-from xingchen.models.extract_data import ExtractData
-from xingchen.models.stop_chat_request import StopChatRequest
-from xingchen.models.character_desc_generated_request import CharacterDescGeneratedRequest
-from xingchen.models.keyword import Keyword
-from xingchen.models.memory import Memory
-from xingchen.models.kv_memory_config import KVMemoryConfig
-from xingchen.models.long_term_memory import LongTermMemory
-from xingchen.models.reject_answer_plugin import RejectAnswerPlugin
-from xingchen.models.reject_condition import RejectCondition
-from xingchen.models.text_to_image_plugin import TextToImagePlugin
-from xingchen.models.platform_plugin import PlatformPlugin
-from xingchen.models.extract_memory_request import ExtractMemoryRequest
-from xingchen.models.extract_data import ExtractData
-from xingchen.models.extract_kv_dto import ExtractKVDTO
-from xingchen.models.extract_summary_dto import ExtractSummaryDTO
-from xingchen.models.file_conver_dto import FileConvertDTO
-from xingchen.models.file_conver_request import FileConvertRequest
-from xingchen.models.memory_summary import MemorySummary
-from xingchen.models.polling_image_detail_dto import PollingImageDetailDTO
-from xingchen.models.result_dto_character_desc_dto import ResultDTOCharacterDescDTO
-from xingchen.models.result_dto_file_conver_dto import ResultDTOFileConvertDTO
-from xingchen.models.result_dto_polling_image_detail_dto import ResultDTOPollingImageDetailDTO
-from xingchen.models.result_dto_extract_kv_dto import ResultDTOExtractKVDTO
-from xingchen.models.result_dto_extract_summary_dto import ResultDTOExtractSummaryDTO
-
```

### Comparing `xingchen-1.1.1/xingchen/api/character_api_sub.py` & `xingchen-1.1.1.1/xingchen/api/character_api_sub.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,42 +10,36 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import re  # noqa: F401
 import io
 import warnings
-from typing import List, Optional
 
 from pydantic import validate_arguments, ValidationError
 
 from typing_extensions import Annotated
 from pydantic import Field, StrictInt, StrictStr
 
 from xingchen.models.character_create_dto import CharacterCreateDTO
-from xingchen.models.character_desc_generated_request import CharacterDescGeneratedRequest
 from xingchen.models.character_query_dto import CharacterQueryDTO
 from xingchen.models.character_update_dto import CharacterUpdateDTO
 from xingchen.models.character_version_create_or_update_dto import CharacterVersionCreateOrUpdateDTO
-from xingchen.models.platform_plugin import PlatformPlugin
-from xingchen.models.reject_answer_plugin import RejectAnswerPlugin
 from xingchen.models.result_dto_boolean import ResultDTOBoolean
-from xingchen.models.result_dto_character_desc_dto import ResultDTOCharacterDescDTO
 from xingchen.models.result_dto_character_dto import ResultDTOCharacterDTO
 from xingchen.models.result_dto_character_key import ResultDTOCharacterKey
 from xingchen.models.result_dto_list_character_dto import ResultDTOListCharacterDTO
 from xingchen.models.result_dto_page_result_character_dto import ResultDTOPageResultCharacterDTO
 
 from xingchen.api_client import ApiClient
 from xingchen.api_response import ApiResponse
 from xingchen.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
-from xingchen.models.text_to_image_plugin import TextToImagePlugin
 
 
 class CharacterApiSub:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -54,22 +48,23 @@
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
     def character_details(self, character_id: Annotated[StrictStr, Field(..., description="角色ID")],
+                          version: Annotated[StrictInt, Field(..., description="角色版本")],
                           **kwargs) -> ResultDTOCharacterDTO:  # noqa: E501
         """角色详情  # noqa: E501
 
         获取角色详细信息  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.character_details(character_id, 1, async_req=True)
+        >>> thread = api.character_details(character_id, version, async_req=True)
         >>> result = thread.get()
 
         :param character_id: 角色ID (required)
         :type character_id: str
         :param version: 角色版本 (required)
         :type version: int
         :param async_req: Whether to execute the request asynchronously.
@@ -83,15 +78,15 @@
                  returns the request thread.
         :rtype: ResultDTOCharacterDTO
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the character_details_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.character_details_with_http_info(character_id, 1, **kwargs)  # noqa: E501
+        return self.character_details_with_http_info(character_id, version, **kwargs)  # noqa: E501
 
     @validate_arguments
     def character_details_with_http_info(self, character_id: Annotated[StrictStr, Field(..., description="角色ID")],
                                          version: Annotated[StrictInt, Field(..., description="角色版本")],
                                          **kwargs) -> ApiResponse:  # noqa: E501
         """角色详情  # noqa: E501
 
@@ -270,16 +265,15 @@
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ResultDTOCharacterKey, status_code(int), headers(HTTPHeaderDict))
         """
-        if character_create_dto.advanced_config is not None:
-            self.pre_check_plugin_process(character_create_dto.advanced_config.platform_plugins)
+
         _params = locals()
 
         _all_params = [
             'character_create_dto'
         ]
         _all_params.extend(
             [
@@ -505,22 +499,23 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
     def delete(self, character_id: Annotated[StrictStr, Field(..., description="待删除的 characterId")],
+               version: Annotated[StrictInt, Field(..., description="待删除的版本")],
                **kwargs) -> ResultDTOBoolean:  # noqa: E501
         """删除角色  # noqa: E501
 
         （逻辑）删除 character。返回成功或失败。  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete(character_id, 1, async_req=True)
+        >>> thread = api.delete(character_id, version, async_req=True)
         >>> result = thread.get()
 
         :param character_id: 待删除的 characterId (required)
         :type character_id: str
         :param version: 待删除的版本 (required)
         :type version: int
         :param async_req: Whether to execute the request asynchronously.
@@ -534,15 +529,15 @@
                  returns the request thread.
         :rtype: ResultDTOBoolean
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the delete_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
-        return self.delete_with_http_info(character_id, 1, **kwargs)  # noqa: E501
+        return self.delete_with_http_info(character_id, version, **kwargs)  # noqa: E501
 
     @validate_arguments
     def delete_with_http_info(self, character_id: Annotated[StrictStr, Field(..., description="待删除的 characterId")],
                               version: Annotated[StrictInt, Field(..., description="待删除的版本")],
                               **kwargs) -> ApiResponse:  # noqa: E501
         """删除角色  # noqa: E501
 
@@ -1169,16 +1164,14 @@
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: tuple(ResultDTOBoolean, status_code(int), headers(HTTPHeaderDict))
         """
-        if character_update_dto.advanced_config is not None:
-            self.pre_check_plugin_process(platform_plugins=character_update_dto.advanced_config.platform_plugins)
 
         _params = locals()
 
         _all_params = [
             'character_update_dto'
         ]
         _all_params.extend(
@@ -1243,123 +1236,14 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @staticmethod
-    def pre_check_plugin_process(platform_plugins: List[PlatformPlugin]):
-        if platform_plugins is None or len(platform_plugins) == 0:
-            return
-        for platform_plugin in platform_plugins:
-            if isinstance(platform_plugin, TextToImagePlugin):
-                platform_plugin.enabled = False if platform_plugin.enabled is None else platform_plugin.enabled
-                if not platform_plugin.name:
-                    platform_plugin.name = "text_to_image_plugin"
-                continue
-            if isinstance(platform_plugin, RejectAnswerPlugin):
-                platform_plugin.enabled = False if platform_plugin.enabled is None else platform_plugin.enabled
-                if not platform_plugin.name:
-                    platform_plugin.name = "reject_answer_plugin"
-                continue
-            raise TypeError("Wrong plugin class type")
-
-    @validate_arguments
-    def auto_generate_desc(self, character_desc_generate_request: CharacterDescGeneratedRequest,
-                           **kwargs) -> ResultDTOCharacterDescDTO:  # noqa: E501
-        kwargs['_return_http_data_only'] = True
-        if '_preload_content' in kwargs:
-            message = "Error! Please call the create_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.auto_generate_desc_with_http_info(character_desc_generate_request, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def auto_generate_desc_with_http_info(self, character_desc_generate_request: CharacterDescGeneratedRequest,
-                                          **kwargs) -> ApiResponse:  # noqa: E501
-
-        _params = locals()
-
-        _all_params = [
-            'character_desc_generate_request'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method auto_generate_desc" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        if _params['character_desc_generate_request'] is not None:
-            _body_params = _params['character_desc_generate_request']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['*/*'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-                                          self.api_client.select_header_content_type(
-                                              ['application/json']))
-        if _content_types_list:
-            _header_params['Content-Type'] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ['Authorization']  # noqa: E501
-
-        _response_types_map = {
-            '200': "ResultDTOCharacterDescDTO",
-        }
-
-        return self.api_client.call_api(
-            '/{0}/api/character/auto/desc'.format(self.api_client.api_version()), 'POST',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `xingchen-1.1.1/xingchen/api/chat_api_sub.py` & `xingchen-1.1.1.1/xingchen/api/chat_api_sub.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,28 +11,45 @@
     Do not edit the class manually.
 """
 
 import re  # noqa: F401
 from typing import Union, Generator
 
 import requests
-from pydantic import Field
 from pydantic import validate_arguments
-from sseclient import SSEClient
+
 from typing_extensions import Annotated
-from xingchen.api_response import ApiResponse
-from xingchen.models.result_dto_boolean import ResultDTOBoolean
-from xingchen.aca_util import convert_chat_params, handle_sse_response
+from pydantic import Field
+
+from xingchen.models.chat_req_params import ChatReqParams
+
 from xingchen.api_client import ApiClient
 from xingchen.exceptions import (
     ApiTypeError
 )
-from xingchen.models.chat_req_params import ChatReqParams
-from xingchen.models.custom import ChatResponse
-from xingchen.models.stop_chat_request import StopChatRequest
+from xingchen.aca_util import convert_chat_params
+from sseclient import SSEClient
+import json
+
+from xingchen.models.custom import ChatResponse, ChatResult
+
+
+def handle_sse_response(client: SSEClient):
+    events = client.events()
+    for event in events:
+        d = json.loads(event.data)
+        error_code = d.get('errorCode', None)
+        if error_code is not None:
+            yield ChatResponse.from_dict(d)
+        yield ChatResponse(
+            success=True,
+            http_status_code=200,
+            code=200,
+            data=ChatResult.from_dict(d)
+        )
 
 
 class ChatApiSub:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -221,99 +238,7 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
         return ChatResponse.from_dict(response)
-
-    @validate_arguments
-    def stop_chat(self, stop_chat_request: Annotated[StopChatRequest, Field(..., description="停止对话请求")],
-                  **kwargs) -> ResultDTOBoolean:  # noqa: E501
-        kwargs['_return_http_data_only'] = True
-        if '_preload_content' in kwargs:
-            message = "Error! Please call the stop_chat_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.stop_chat_with_http_info(stop_chat_request, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def stop_chat_with_http_info(self, stop_chat_request: Annotated[
-        StopChatRequest, Field(..., description="停止对话请求")], **kwargs) -> ApiResponse:  # noqa: E501
-
-        _params = locals()
-
-        _all_params = [
-            'extract_memory_request'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method  stop_chat" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        if _params['stop_chat_request'] is not None:
-            _body_params = _params['stop_chat_request']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['*/*'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-                                          self.api_client.select_header_content_type(
-                                              ['application/json']))
-        if _content_types_list:
-            _header_params['Content-Type'] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ['Authorization']  # noqa: E501
-
-        _response_types_map = {
-            '200': "ResultDTOBoolean",
-        }
-
-        return self.api_client.call_api(
-            '/{0}/api/chat/stop'.format(self.version()), 'POST',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
```

### Comparing `xingchen-1.1.1/xingchen/api/chat_message_api_sub.py` & `xingchen-1.1.1.1/xingchen/api/chat_message_api_sub.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from pydantic import validate_arguments, ValidationError
 
 from typing_extensions import Annotated
 from pydantic import Field, StrictInt, StrictStr
 
 from typing import Optional
 
-from xingchen.models import ResultDTOPollingImageDetailDTO
 from xingchen.models.chat_history_query_dto import ChatHistoryQueryDTO
 from xingchen.models.message_rating_request import MessageRatingRequest
 from xingchen.models.result_dto_boolean import ResultDTOBoolean
 from xingchen.models.result_dto_page_result_chat_message_dto import ResultDTOPageResultChatMessageDTO
 from xingchen.models.sys_reminder_request import SysReminderRequest
 from xingchen.models.custom.reset_history_request import ResetChatHistoryRequest
 
@@ -584,104 +583,14 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def polling_image_detail(self, message_id: Annotated[StrictStr, Field(..., description="消息ID")],
-                          user_id: Annotated[StrictInt, Field(..., description="用户ID")],
-                          **kwargs) -> ResultDTOPollingImageDetailDTO:  # noqa: E501
-        kwargs['_return_http_data_only'] = True
-        if '_preload_content' in kwargs:
-            message = "Error! Please call the character_details_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
-            raise ValueError(message)
-        return self.polling_image_detail_with_http_info(message_id, user_id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def polling_image_detail_with_http_info(self, message_id: Annotated[StrictStr, Field(..., description="角色ID")],
-                                         user_id: Annotated[StrictInt, Field(..., description="用户ID")],
-                                         **kwargs) -> ApiResponse:  # noqa: E501
-        _params = locals()
-
-        _all_params = [
-            'message_id',
-            'user_id'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method polling_image_detail" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-        if _params.get('message_id') is not None:  # noqa: E501
-            _query_params.append(('messageId', _params['message_id']))
-
-        if _params.get('user_id') is not None:  # noqa: E501
-            _query_params.append(('userId', _params['user_id']))
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['*/*'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['Authorization']  # noqa: E501
-
-        _response_types_map = {
-            '200': "ResultDTOPollingImageDetailDTO",
-        }
-
-        return self.api_client.call_api(
-            '/{api_version}/api/chat/polling/image'.format(api_version=self.api_client.configuration.api_version), 'GET',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `xingchen-1.1.1/xingchen/api_client.py` & `xingchen-1.1.1.1/xingchen/api_client.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/api_response.py` & `xingchen-1.1.1.1/xingchen/api_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/configuration.py` & `xingchen-1.1.1.1/xingchen/configuration.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/exceptions.py` & `xingchen-1.1.1.1/xingchen/exceptions.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/__init__.py` & `xingchen-1.1.1.1/xingchen/models/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from xingchen.models.advanced_settings import AdvancedSettings
 from xingchen.models.base_chat_request import BaseChatRequest
-from xingchen.models.base_chat_request import BaseChatRequest
+from xingchen.models.base_chat_request_aca_chat_ext_param import BaseChatRequestAcaChatExtParam
 from xingchen.models.character_advanced_config import CharacterAdvancedConfig
 from xingchen.models.character_create_dto import CharacterCreateDTO
 from xingchen.models.character_dto import CharacterDTO
 from xingchen.models.character_key import CharacterKey
 from xingchen.models.character_permission_config import CharacterPermissionConfig
 from xingchen.models.character_query_dto import CharacterQueryDTO
 from xingchen.models.character_query_where import CharacterQueryWhere
@@ -49,12 +49,7 @@
 from xingchen.models.result_dto_character_key import ResultDTOCharacterKey
 from xingchen.models.result_dto_list_character_dto import ResultDTOListCharacterDTO
 from xingchen.models.result_dto_page_result_character_dto import ResultDTOPageResultCharacterDTO
 from xingchen.models.result_dto_page_result_chat_message_dto import ResultDTOPageResultChatMessageDTO
 from xingchen.models.scenario import Scenario
 from xingchen.models.sys_reminder_request import SysReminderRequest
 from xingchen.models.user_profile import UserProfile
-from xingchen.models.result_dto_extract_summary_dto import ResultDTOExtractSummaryDTO
-from xingchen.models.result_dto_extract_kv_dto import ResultDTOExtractKVDTO
-from xingchen.models.result_dto_polling_image_detail_dto import ResultDTOPollingImageDetailDTO
-from xingchen.models.result_dto_file_conver_dto import ResultDTOFileConvertDTO
-from xingchen.models.result_dto_character_desc_dto import ResultDTOCharacterDescDTO
```

### Comparing `xingchen-1.1.1/xingchen/models/advanced_settings.py` & `xingchen-1.1.1.1/xingchen/models/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/base_chat_request.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_character_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,42 @@
 # coding: utf-8
 
-from __future__ import annotations
+"""
+    XingChen 开放接口定义
 
-import json
-import pprint
-import re
-from typing import Optional
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from xingchen.models.input import Input
-from xingchen.models.model_parameters import ModelParameters
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from xingchen.models.character_dto import CharacterDTO
 
-class BaseChatRequest(BaseModel):
+class ResultDTOCharacterDTO(BaseModel):
     """
-    BaseChatRequestAcaChatExtParam
+    ResultDTOCharacterDTO
     """
-    model: Optional[StrictStr] = None
-    parameters: Optional[ModelParameters] = None
-    input: Input = Field(...)
-    servicename: Optional[StrictStr] = None
-    debug: Optional[StrictBool] = None
-    __properties = ["model", "parameters", "input", "servicename", "debug"]
+    request_id: Optional[StrictStr] = Field(None, alias="requestId")
+    code: Optional[StrictInt] = None
+    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
+    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
+    data: Optional[CharacterDTO] = None
+    success: Optional[StrictBool] = None
+    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -34,44 +44,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> BaseChatRequest:
-        """Create an instance of BaseChatRequestAcaChatExtParam from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultDTOCharacterDTO:
+        """Create an instance of ResultDTOCharacterDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of parameters
-        if self.parameters:
-            _dict['parameters'] = self.parameters.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of input
-        if self.input:
-            _dict['input'] = self.input.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> BaseChatRequest:
-        """Create an instance of BaseChatRequestAcaChatExtParam from a dict"""
+    def from_dict(cls, obj: dict) -> ResultDTOCharacterDTO:
+        """Create an instance of ResultDTOCharacterDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return BaseChatRequest.parse_obj(obj)
+            return ResultDTOCharacterDTO.parse_obj(obj)
 
-        _obj = BaseChatRequest.parse_obj({
-            "model": obj.get("model"),
-            "parameters": ModelParameters.from_dict(obj.get("parameters")) if obj.get("parameters") is not None else None,
-            "input": Input.from_dict(obj.get("input")) if obj.get("input") is not None else None,
-            "servicename": obj.get("servicename"),
-            "debug": obj.get("debug")
+        _obj = ResultDTOCharacterDTO.parse_obj({
+            "request_id": obj.get("requestId"),
+            "code": obj.get("code"),
+            "error_message": obj.get("errorMessage"),
+            "error_message_key": obj.get("errorMessageKey"),
+            "data": CharacterDTO.from_dict(obj.get("data")) if obj.get("data") is not None else None,
+            "success": obj.get("success")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/character_advanced_config.py` & `xingchen-1.1.1.1/xingchen/models/character_advanced_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding: utf-8
 
 
 from __future__ import annotations
 
 import json
 import pprint
-from typing import Optional, Any
+from typing import Optional
 
 from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist, StrictInt
 
-from xingchen.models.long_term_memory import LongTermMemory
 from xingchen.models.repository_info import RepositoryInfo
 from xingchen.models.custom.character_model_parameters import CharacterModelParameters
 
 
 class CharacterAdvancedConfig(BaseModel):
     """
     角色高级配置
@@ -26,20 +25,16 @@
     allow_send_asr: Optional[StrictBool] = Field(None, alias="allowSendAsr", description="是否允许角色发送语音")
     asr_style: Optional[StrictStr] = Field(None, alias="asrStyle", description="角色发送语音风格")
     chat_description: Optional[StrictStr] = Field(None, alias="chatDescription", description="对话介绍")
     is_real_time: Optional[StrictBool] = Field(None, alias="isRealTime", description="是否获取真实时间")
     short_term_memory_round: Optional[StrictInt] = Field(None, alias="shortTermMemoryRound", description="""
     短期记忆轮数，若使用平台对话历史，可以通过该参数获取指定轮数的对话历史作为短期记忆，超过该轮数，会到长期记忆库中搜索用户query相关问题答案
     """)
-    long_term_memories: Optional[conlist(LongTermMemory)] = Field(None, alias="longTermMemories",
-                                                                  description="打开长期记忆设置")
-    platform_plugins: Optional[conlist(Any)] = Field(None, alias="platformPlugins", description="平台插件")
-
     __properties = ["repositoryInfo", "isRealInfo", "searchKeyword", "allowSendImage", "imageStyle", "allowSendAsr",
-                    "asrStyle", "chatDescription", "shortTermMemoryRound", "longTermMemories", "platformPlugins"]
+                    "asrStyle", "chatDescription", "shortTermMemoryRound"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -83,12 +78,9 @@
             "allow_send_image": obj.get("allowSendImage"),
             "image_style": obj.get("imageStyle"),
             "allow_send_asr": obj.get("allowSendAsr"),
             "asr_style": obj.get("asrStyle"),
             "chat_description": obj.get("chatDescription"),
             "is_real_time": obj.get("isRealTime"),
             "short_term_memory_round": obj.get("shortTermMemoryRound"),
-            "long_term_memories": [LongTermMemory.from_dict(_item) for _item in obj.get("longTermMemories")] if obj.get(
-                "longTermMemories") is not None else None,
-            "platform_plugins": obj.get("platformPlugins")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/character_create_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_desc_dto.py` & `xingchen-1.1.1.1/xingchen/models/page_result_character_dto.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,41 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
-import pprint
-import re  # noqa: F401
-from typing import Optional
+"""
+    XingChen 开放接口定义
 
-from pydantic import BaseModel, Field, StrictStr
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-from xingchen.models import Context
-from xingchen.models.custom import Usage
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-class CharacterDescDTO(BaseModel):
-    content: Optional[StrictStr] = Field(None, alias="content")
-    usage: Optional[Usage] = Field(None, alias="usage")
-    context: Optional[Context] = Field(None, alias="context")
-    __properties = ["content", "usage", "context"]
+
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictInt, conlist
+from xingchen.models.character_dto import CharacterDTO
+
+class PageResultCharacterDTO(BaseModel):
+    """
+    PageResultCharacterDTO
+    """
+    list: Optional[conlist(CharacterDTO)] = None
+    page: Optional[StrictInt] = None
+    page_size: Optional[StrictInt] = Field(None, alias="pageSize")
+    total: Optional[StrictInt] = None
+    page_offset_value: Optional[StrictInt] = Field(None, alias="pageOffsetValue")
+    __properties = ["list", "page", "pageSize", "total", "pageOffsetValue"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -27,34 +43,45 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CharacterDescDTO:
-        """Create an instance of CharacterDescDTO from a JSON string"""
+    def from_json(cls, json_str: str) -> PageResultCharacterDTO:
+        """Create an instance of PageResultCharacterDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in list (list)
+        _items = []
+        if self.list:
+            for _item in self.list:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['list'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CharacterDescDTO:
-        """Create an instance of CharacterDescDTO from a dict"""
+    def from_dict(cls, obj: dict) -> PageResultCharacterDTO:
+        """Create an instance of PageResultCharacterDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CharacterDescDTO.parse_obj(obj)
+            return PageResultCharacterDTO.parse_obj(obj)
 
-        _obj = CharacterDescDTO.parse_obj({
-            "content": obj.get("content"),
-            "usage": Usage.from_dict(obj.get("usage")) if obj.get("usage") is not None else None,
-            "context": Context.from_dict(obj.get("context")) if obj.get("context") is not None else None
+        _obj = PageResultCharacterDTO.parse_obj({
+            "list": [CharacterDTO.from_dict(_item) for _item in obj.get("list")] if obj.get("list") is not None else None,
+            "page": obj.get("page"),
+            "page_size": obj.get("pageSize"),
+            "total": obj.get("total"),
+            "page_offset_value": obj.get("pageOffsetValue")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/character_desc_generated_request.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_character_key.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
 import re  # noqa: F401
-from typing import Optional
-
-from pydantic import BaseModel, Field, StrictStr
+import json
 
-from xingchen.models.model_parameters import ModelParameters
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from xingchen.models.character_key import CharacterKey
 
-class CharacterDescGeneratedRequest(BaseModel):
-    type: Optional[StrictStr] = Field(None, alias="type")
-    file_url: Optional[StrictStr] = Field(None, alias="fileUrl")
-    text: Optional[StrictStr] = Field(None, alias="text")
-    file_name: Optional[StrictStr] = Field(None, alias="fileName")
-    model_parameter: Optional[ModelParameters] = Field(None, alias="modelParameter")
-    __properties = ["type", "fileUrl", "text", "fileName", "modelParameter"]
+class ResultDTOCharacterKey(BaseModel):
+    """
+    ResultDTOCharacterKey
+    """
+    request_id: Optional[StrictStr] = Field(None, alias="requestId")
+    code: Optional[StrictInt] = None
+    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
+    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
+    data: Optional[CharacterKey] = None
+    success: Optional[StrictBool] = None
+    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -28,37 +44,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> CharacterDescGeneratedRequest:
-        """Create an instance of CharacterDescGeneratedRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultDTOCharacterKey:
+        """Create an instance of ResultDTOCharacterKey from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> CharacterDescGeneratedRequest:
-        """Create an instance of CharacterDescGeneratedRequest from a dict"""
+    def from_dict(cls, obj: dict) -> ResultDTOCharacterKey:
+        """Create an instance of ResultDTOCharacterKey from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return CharacterDescGeneratedRequest.parse_obj(obj)
+            return ResultDTOCharacterKey.parse_obj(obj)
 
-        _obj = CharacterDescGeneratedRequest.parse_obj({
-            "type": obj.get("type"),
-            "file_url": obj.get("fileUrl"),
-            "text": obj.get("text"),
-            "file_name": obj.get("fileName"),
-            "model_parameter": ModelParameters.from_dict(obj.get("modelParameter")) if obj.get(
-                "modelParameter") is not None else None
+        _obj = ResultDTOCharacterKey.parse_obj({
+            "request_id": obj.get("requestId"),
+            "code": obj.get("code"),
+            "error_message": obj.get("errorMessage"),
+            "error_message_key": obj.get("errorMessageKey"),
+            "data": CharacterKey.from_dict(obj.get("data")) if obj.get("data") is not None else None,
+            "success": obj.get("success")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/character_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_key.py` & `xingchen-1.1.1.1/xingchen/models/character_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,15 @@
     CharacterKey
     """
     character_id: Optional[StrictStr] = Field(None, alias="characterId")
     version: Optional[StrictInt] = None
     name: Optional[StrictStr] = None
     content: Optional[StrictStr] = None
     type: Optional[StrictStr] = Field(None, alias="type", description="角色类型，虚拟角色-virtual（默认）, 角色复刻-reproduction，助手-assistant")
-    task: Optional[StrictStr] = Field(None, alias="task", description="角色群聊任务")
-    traits: Optional[StrictStr] = Field(None, alias="traits", description="强制要求")
-    __properties = ["characterId", "version", "name", "content", "type", "task", "traits"]
+    __properties = ["characterId", "version", "name", "content", "type"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -69,14 +67,12 @@
         if not isinstance(obj, dict):
             return CharacterKey.parse_obj(obj)
 
         _obj = CharacterKey.parse_obj({
             "character_id": obj.get("characterId"),
             "version": obj.get("version"),
             "name": obj.get("name"),
-            "content": obj.get("content"),
-            "task": obj.get("task"),
-            "traits": obj.get("traits")
+            "content": obj.get("content")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/character_permission_config.py` & `xingchen-1.1.1.1/xingchen/models/character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_query_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_query_where.py` & `xingchen-1.1.1.1/xingchen/models/character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/character_update_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_update_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     opening_line: Optional[StrictStr] = Field(None, alias="openingLine", description="开场白")
     traits: Optional[StrictStr] = Field(None, description="角色特点")
     chat_example: Optional[StrictStr] = Field(None, alias="chatExample", description="聊天示例")
     type: Optional[StrictStr] = Field(None, description="角色类型，virtual:虚拟角色，reproduction:已知角色复刻")
     chat_objective: Optional[StrictStr] = Field(None, alias="chatObjective", description="对话目标")
     advanced_config: Optional[CharacterAdvancedConfig] = Field(None, alias="advancedConfig")
     character_id: StrictStr = Field(..., alias="characterId", description="角色ID")
-    version: Optional[StrictInt] = Field(None, description="角色版本")
+    version: StrictInt = Field(..., description="角色版本")
     perm_config: Optional[CharacterPermissionConfig] = Field(None, alias="permConfig")
     role_types: Optional[conlist(StrictStr)] = Field(None, alias="roleTypes", description="角色类型")
     __properties = ["name", "avatar", "introduction", "basicInformation", "openingLine", "traits",
                     "chatExample", "type", "chatObjective", "advancedConfig", "characterId", "version", "permConfig",
                     "roleTypes"]
 
     class Config:
```

### Comparing `xingchen-1.1.1/xingchen/models/character_version_create_or_update_dto.py` & `xingchen-1.1.1.1/xingchen/models/character_version_create_or_update_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     opening_line: Optional[StrictStr] = Field(None, alias="openingLine", description="开场白")
     traits: Optional[StrictStr] = Field(None, description="角色特点")
     chat_example: Optional[StrictStr] = Field(None, alias="chatExample", description="聊天示例")
     type: Optional[StrictStr] = Field(None, description="角色类型，virtual:虚拟角色，reproduction:已知角色复刻")
     chat_objective: Optional[StrictStr] = Field(None, alias="chatObjective", description="对话目标")
     advanced_config: Optional[CharacterAdvancedConfig] = Field(None, alias="advancedConfig")
     character_id: StrictStr = Field(..., alias="characterId", description="角色标识")
-    version: Optional[StrictInt] = Field(None, description="角色版本，相同角色版本号唯一")
+    version: StrictInt = Field(..., description="角色版本，相同角色版本号唯一")
     role_types: Optional[conlist(StrictStr)] = Field(None, alias="roleTypes", description="角色类型")
     __properties = ["name", "avatar", "introduction", "basicInformation", "openingLine", "traits", "chatExample",
                     "type", "chatObjective", "advancedConfig", "characterId", "version", "roleTypes"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
```

### Comparing `xingchen-1.1.1/xingchen/models/chat_context.py` & `xingchen-1.1.1.1/xingchen/models/chat_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_history_query_dto.py` & `xingchen-1.1.1.1/xingchen/models/chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_history_query_where.py` & `xingchen-1.1.1.1/xingchen/models/chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_message_dto.py` & `xingchen-1.1.1.1/xingchen/models/chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/chat_req_params.py` & `xingchen-1.1.1.1/xingchen/models/chat_req_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 from pydantic import BaseModel, Field, StrictBool, StrictStr, conlist
 
 from xingchen.models.advanced_settings import AdvancedSettings
 from xingchen.models.character_key import CharacterKey
 from xingchen.models.chat_context import ChatContext
 from xingchen.models.function_call import Function, FunctionChoice, Plugin
-from xingchen.models.memory import Memory
 from xingchen.models.message import Message
 from xingchen.models.model_parameters import ModelParameters
 from xingchen.models.scenario import Scenario
 from xingchen.models.user_profile import UserProfile
 
 
 class ChatReqParams(BaseModel):
@@ -44,19 +43,18 @@
     scenario: Optional[Scenario] = None
     streaming: Optional[StrictBool] = None
     source: Optional[StrictStr] = None
     functions: conlist(Function, max_items=50) = Field(None, alias="functionList")
     function_choice: Optional[FunctionChoice] = Field(None, alias="functionChoice")
     plugins: conlist(Plugin, max_items=50) = Field(None, alias="pluginList")
     context: Optional[ChatContext] = Field(None, alias="context")
-    memory: Optional[Memory] = Field(None, alias="memory")
 
     __properties = ["botProfile", "messages", "sampleMessages", "advancedSettings",
                     "modelParameters", "userProfile", "scenario", "streaming", "context", "source", "functionList",
-                    "functionChoice", "pluginList", "context", "memory"]
+                    "functionChoice", "pluginList", "context"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -143,11 +141,10 @@
                 "userProfile") is not None else None,
             "scenario": Scenario.from_dict(obj.get("scenario")) if obj.get("scenario") is not None else None,
             "streaming": obj.get("streaming"),
             "source": obj.get("source"),
             "functions": [Function.from_dict(_item) for _item in obj.get("functionList")] if obj.get("functionList") is not None else None,
             "plugins": [Plugin.from_dict(_item) for _item in obj.get("pluginList")] if obj.get("pluginList") is not None else None,
             "function_choice": FunctionChoice.from_dict(obj.get("functionChoice")) if obj.get("functionChoice") is not None else None,
-            "context": ChatContext.from_dict(obj.get("context")) if obj.get("context") is not None else None,
-            "memory": Memory.from_dict(obj.get("memory")) if obj.get("memory") is not None else None
+            "context": ChatContext.from_dict(obj.get("context")) if obj.get("context") is not None else None
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/chat_room_user_dto.py` & `xingchen-1.1.1.1/xingchen/models/chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/context.py` & `xingchen-1.1.1.1/xingchen/models/context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/base_response.py` & `xingchen-1.1.1.1/xingchen/models/custom/base_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/character_model_parameters.py` & `xingchen-1.1.1.1/xingchen/models/custom/character_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/chat_response.py` & `xingchen-1.1.1.1/xingchen/models/custom/chat_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/custom/groupchat/group_chat_reply_setting.py` & `xingchen-1.1.1.1/xingchen/models/custom/platform_publish_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 # coding: utf-8
 
+
+from __future__ import annotations
+
 import json
-from typing import Optional
+import pprint
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictStr, StrictBool
+from typing import Optional
 
 
-class GroupChatReplySetting(BaseModel):
-    bot_name: StrictStr = Field(..., alias="botName", description="回复角色名称，必须为群聊角色中的一名角色")
-    thought: Optional[StrictStr] = Field(None, alias="thought", description="希望角色如何回复")
+class PlatformPublishConfig(BaseModel):
+    """
+    平台发布配置
+    """
+    enabled: Optional[StrictBool] = Field(..., alias="enabled", description="是否开启")
+    private_share_type: StrictStr = Field(..., alias="privateShareType", description="""
+     私密分享类型
+     * selfShare - 仅自己可与角色聊天 （permConfig.allowChat=0）
+     * linkShare - 通过链接分享（允许获得链接的星尘用户可与ta聊天）  （permConfig.allowChat=0）
+     * allShare  - 所有星尘用户可见（需要平台审核）  （permConfig.allowChat=1）
+    """)
+    __properties = ["enabled", "privateShareType"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
-        # 直接使用 json.dumps 序列化，提高性能效率
-        return json.dumps(self.dict(by_alias=True, exclude_none=True), indent=4)
+        return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
-        # 同样，直接序列化，避免不必要的中间步骤
-        return json.dumps(self.dict(by_alias=True, exclude_none=True))
+        return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'GroupChatReplySetting':
-        # 增加异常处理来确保输入的 JSON 字符串是有效的
-        try:
-            obj_dict = json.loads(json_str)
-            return cls.from_dict(obj_dict)
-        except json.JSONDecodeError:
-            raise ValueError("Invalid JSON string")
+    def from_json(cls, json_str: str) -> PlatformPublishConfig:
+        """Create an instance of SysReminderRequest from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
-        # 简化了代码风格
-        return self.dict(by_alias=True, exclude_none=True)
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'GroupChatReplySetting':
-        # 移除了对 `obj` 是否为 `None` 的判断，因为 `parse_obj` 已经能够处理 `None` 的情况
-        # 同时，明确使用 `cls.__init__` 来创建实例，提高代码的可维护性和健壮性
+    def from_dict(cls, obj: dict) -> PlatformPublishConfig:
+        """Create an instance of SysReminderRequest from a dict"""
+        if obj is None:
+            return None
+
         if not isinstance(obj, dict):
-            raise TypeError("Expected a dictionary object")
+            return PlatformPublishConfig.parse_obj(obj)
+
+        _obj = PlatformPublishConfig.parse_obj({
+            "enabled": obj.get("enabled"),
+            "private_share_type": obj.get("privateShareType")
+        })
+        return _obj
+
 
-        return cls(bot_name=obj.get("botName"), thought=obj.get("thought"))
```

### Comparing `xingchen-1.1.1/xingchen/models/custom/reset_history_request.py` & `xingchen-1.1.1.1/xingchen/models/custom/reset_history_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/extract_data.py` & `xingchen-1.1.1.1/xingchen/models/file_info_vo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,38 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
 import re  # noqa: F401
-from typing import Optional
-
-from pydantic import BaseModel, Field, conlist, StrictStr
+import json
 
 
-class ExtractData(BaseModel):
-    role: Optional[StrictStr] = Field(None, alias="role")
-    key: Optional[StrictStr] = Field(None, alias="key")
-    value: Optional[conlist(StrictStr)] = Field(None, alias="value")
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-    __properties = ["role", "key", "value"]
+class FileInfoVO(BaseModel):
+    """
+    角色头像  # noqa: E501
+    """
+    file_save_path: Optional[StrictStr] = Field(None, alias="fileSavePath")
+    filename: Optional[StrictStr] = None
+    file_url: Optional[StrictStr] = Field(None, alias="fileUrl")
+    __properties = ["fileSavePath", "filename", "fileUrl"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -25,34 +40,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ExtractData:
-        """Create an instance of ExtractData from a JSON string"""
+    def from_json(cls, json_str: str) -> FileInfoVO:
+        """Create an instance of FileInfoVO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ExtractData:
-        """Create an instance of ExtractData from a dict"""
+    def from_dict(cls, obj: dict) -> FileInfoVO:
+        """Create an instance of FileInfoVO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ExtractData.parse_obj(obj)
+            return FileInfoVO.parse_obj(obj)
 
-        _obj = ExtractData.parse_obj({
-            "role": obj.get("role"),
-            "key": obj.get("key"),
-            "value": obj.get("value")
+        _obj = FileInfoVO.parse_obj({
+            "file_save_path": obj.get("fileSavePath"),
+            "filename": obj.get("filename"),
+            "file_url": obj.get("fileUrl")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/extract_memory_request.py` & `xingchen-1.1.1.1/xingchen/models/message_rating_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
 import re  # noqa: F401
-from typing import Optional
-
-from pydantic import BaseModel, Field, conlist
+import json
 
-from xingchen.models import Message, ModelParameters
-from xingchen.models.kv_memory_config import KVMemoryConfig
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr, conint
+from xingchen.models.gateway_issued_params import GatewayIssuedParams
 
-class ExtractMemoryRequest(BaseModel):
-    messages: Optional[conlist(Message, min_items=1)] = Field(...)
-    kv_memory_configs: Optional[conlist(KVMemoryConfig)] = Field(None, alias="kvMemoryConfigs")
-    model_parameter: Optional[ModelParameters] = Field(None, alias="modelParameter")
-    __properties = ["messages", "kvMemoryConfigs", "modelParameter"]
+class MessageRatingRequest(BaseModel):
+    """
+    MessageRatingRequest
+    """
+    message_id: StrictStr = Field(..., alias="messageId", description="待评分消息ID")
+    rating: conint(strict=True, le=5, ge=-1) = Field(..., description="评分")
+    __properties = ["messageId", "rating"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -27,37 +40,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ExtractMemoryRequest:
-        """Create an instance of ExtractMemoryRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> MessageRatingRequest:
+        """Create an instance of MessageRatingRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ExtractMemoryRequest:
-        """Create an instance of ExtractMemoryRequest from a dict"""
+    def from_dict(cls, obj: dict) -> MessageRatingRequest:
+        """Create an instance of MessageRatingRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ExtractMemoryRequest.parse_obj(obj)
+            return MessageRatingRequest.parse_obj(obj)
 
-        _obj = ExtractMemoryRequest.parse_obj({
-            "messages": [Message.from_dict(_item) for _item in obj.get("messages")] if obj.get(
-                "messages") is not None else None,
-            "kv_memory_configs": [KVMemoryConfig.from_dict(_item) for _item in obj.get("kvMemoryConfigs")] if obj.get(
-                "kvMemoryConfigs") is not None else None,
-            "model_parameter": ModelParameters.from_dict(obj.get("modelParameter")) if obj.get(
-                "modelParameter") is not None else None
+        _obj = MessageRatingRequest.parse_obj({
+            "message_id": obj.get("messageId"),
+            "rating": obj.get("rating")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/extract_summary_dto.py` & `xingchen-1.1.1.1/xingchen/models/gateway_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,38 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
 import re  # noqa: F401
-from typing import Optional
-
-from pydantic import BaseModel, Field, conlist
+import json
 
-from xingchen.models import Context
-from xingchen.models.custom import Usage
-from xingchen.models.memory_summary import MemorySummary
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-class ExtractSummaryDTO(BaseModel):
-    memory_results: conlist(MemorySummary) = Field(None, alias="memoryResults")
-    usage: Optional[Usage] = Field(None, alias="usage")
-    context: Optional[Context] = Field(None, alias="context")
-    __properties = ["memoryResults", "usage", "context"]
+class GatewayContext(BaseModel):
+    """
+    GatewayContext
+    """
+    service_type: Optional[StrictStr] = Field(None, alias="serviceType")
+    fc_url: Optional[StrictStr] = Field(None, alias="fcUrl")
+    flow_json_path: Optional[StrictStr] = Field(None, alias="flowJsonPath")
+    __properties = ["serviceType", "fcUrl", "flowJsonPath"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -28,35 +40,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ExtractSummaryDTO:
-        """Create an instance of ExtractMemoryRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> GatewayContext:
+        """Create an instance of GatewayContext from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ExtractSummaryDTO:
-        """Create an instance of ExtractMemoryRequest from a dict"""
+    def from_dict(cls, obj: dict) -> GatewayContext:
+        """Create an instance of GatewayContext from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ExtractSummaryDTO.parse_obj(obj)
+            return GatewayContext.parse_obj(obj)
 
-        _obj = ExtractSummaryDTO.parse_obj({
-            "memory_results": [MemorySummary.from_dict(_item) for _item in obj.get("memoryResults")] if obj.get(
-                "memoryResults") is not None else None,
-            "usage": Usage.from_dict(obj.get("usage")) if obj.get("usage") is not None else None,
-            "context": Context.from_dict(obj.get("context")) if obj.get("context") is not None else None
+        _obj = GatewayContext.parse_obj({
+            "service_type": obj.get("serviceType"),
+            "fc_url": obj.get("fcUrl"),
+            "flow_json_path": obj.get("flowJsonPath")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/file_conver_dto.py` & `xingchen-1.1.1.1/xingchen/models/scenario.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,37 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
 import re  # noqa: F401
-from typing import Optional
-
-from pydantic import BaseModel, StrictStr, StrictInt
+import json
 
 
-class FileConvertDTO(BaseModel):
-    id: Optional[StrictInt] = None
-    status: Optional[StrictStr] = None
-    url: Optional[StrictStr] = None
+from typing import Optional
+from pydantic import BaseModel, StrictStr, Field
 
-    __properties = ["id", "status", "url"]
+class Scenario(BaseModel):
+    """
+    Scenario
+    """
+    description: Optional[StrictStr] = None
+    safety_prompt: Optional[StrictStr] = Field(None, alias="safetyPrompt", description="命中安全风险后，给大模型的提示信息")
+    __properties = ["description", "safetyPrompt"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -25,34 +39,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> FileConvertDTO:
-        """Create an instance of FileConvertDTO from a JSON string"""
+    def from_json(cls, json_str: str) -> Scenario:
+        """Create an instance of Scenario from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> FileConvertDTO:
-        """Create an instance of FileConvertDTO from a dict"""
+    def from_dict(cls, obj: dict) -> Scenario:
+        """Create an instance of Scenario from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return FileConvertDTO.parse_obj(obj)
+            return Scenario.parse_obj(obj)
 
-        _obj = FileConvertDTO.parse_obj({
-            "id": obj.get("id"),
-            "status": obj.get("status"),
-            "url": obj.get("url")
+        _obj = Scenario.parse_obj({
+            "description": obj.get("description")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/file_conver_request.py` & `xingchen-1.1.1.1/xingchen/models/gateway_issued_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,38 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
 import re  # noqa: F401
-from typing import Optional
-
-from pydantic import BaseModel, Field, StrictStr
+import json
 
 
-class FileConvertRequest(BaseModel):
-    type: Optional[StrictStr] = None
-    source_url: Optional[StrictStr] = Field(None, alias="sourceUrl")
+from typing import Dict, Optional
+from pydantic import BaseModel, Field, StrictStr
+from xingchen.models.gateway_context import GatewayContext
 
-    __properties = ["type", "sourceUrl"]
+class GatewayIssuedParams(BaseModel):
+    """
+    GatewayIssuedParams
+    """
+    user_info: Optional[Dict[str, StrictStr]] = Field(None, alias="userInfo")
+    context: Optional[GatewayContext] = None
+    __properties = ["userInfo", "context"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -24,33 +40,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> FileConvertRequest:
-        """Create an instance of FileConvertRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> GatewayIssuedParams:
+        """Create an instance of GatewayIssuedParams from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of context
+        if self.context:
+            _dict['context'] = self.context.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> FileConvertRequest:
-        """Create an instance of FileConvertRequest from a dict"""
+    def from_dict(cls, obj: dict) -> GatewayIssuedParams:
+        """Create an instance of GatewayIssuedParams from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return FileConvertRequest.parse_obj(obj)
+            return GatewayIssuedParams.parse_obj(obj)
 
-        _obj = FileConvertRequest.parse_obj({
-            "type": obj.get("type"),
-            "source_url": obj.get("sourceUrl")
+        _obj = GatewayIssuedParams.parse_obj({
+            "user_info": obj.get("userInfo"),
+            "context": GatewayContext.from_dict(obj.get("context")) if obj.get("context") is not None else None
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/file_info_vo.py` & `xingchen-1.1.1.1/xingchen/models/sys_reminder_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
+from xingchen.models.gateway_issued_params import GatewayIssuedParams
 
-class FileInfoVO(BaseModel):
+class SysReminderRequest(BaseModel):
     """
-    角色头像  # noqa: E501
+    系统提醒参数  # noqa: E501
     """
-    file_save_path: Optional[StrictStr] = Field(None, alias="fileSavePath")
-    filename: Optional[StrictStr] = None
-    file_url: Optional[StrictStr] = Field(None, alias="fileUrl")
-    __properties = ["fileSavePath", "filename", "fileUrl"]
+    character_id: StrictStr = Field(..., alias="characterId", description="角色ID")
+    content: StrictStr = Field(..., description="系统提醒内容")
+    biz_user_id: StrictStr = Field(..., alias="bizUserId", description="业务系统ID")
+    __properties = ["characterId", "content", "bizUserId"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,36 +41,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> FileInfoVO:
-        """Create an instance of FileInfoVO from a JSON string"""
+    def from_json(cls, json_str: str) -> SysReminderRequest:
+        """Create an instance of SysReminderRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> FileInfoVO:
-        """Create an instance of FileInfoVO from a dict"""
+    def from_dict(cls, obj: dict) -> SysReminderRequest:
+        """Create an instance of SysReminderRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return FileInfoVO.parse_obj(obj)
+            return SysReminderRequest.parse_obj(obj)
 
-        _obj = FileInfoVO.parse_obj({
-            "file_save_path": obj.get("fileSavePath"),
-            "filename": obj.get("filename"),
-            "file_url": obj.get("fileUrl")
+        _obj = SysReminderRequest.parse_obj({
+            "character_id": obj.get("characterId"),
+            "content": obj.get("content"),
+            "biz_user_id": obj.get("bizUserId")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/function_call.py` & `xingchen-1.1.1.1/xingchen/models/function_call.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/gateway_context.py` & `xingchen-1.1.1.1/xingchen/models/user_profile.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class GatewayContext(BaseModel):
+class UserProfile(BaseModel):
     """
-    GatewayContext
+    UserProfile
     """
-    service_type: Optional[StrictStr] = Field(None, alias="serviceType")
-    fc_url: Optional[StrictStr] = Field(None, alias="fcUrl")
-    flow_json_path: Optional[StrictStr] = Field(None, alias="flowJsonPath")
-    __properties = ["serviceType", "fcUrl", "flowJsonPath"]
+    user_id: StrictStr = Field(..., alias="userId")
+    user_name: Optional[StrictStr] = Field(None, alias="userName")
+    basic_info: Optional[StrictStr] = Field(None, alias="basicInfo")
+    __properties = ["userId", "userName", "basicInfo"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,36 +40,36 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GatewayContext:
-        """Create an instance of GatewayContext from a JSON string"""
+    def from_json(cls, json_str: str) -> UserProfile:
+        """Create an instance of UserProfile from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GatewayContext:
-        """Create an instance of GatewayContext from a dict"""
+    def from_dict(cls, obj: dict) -> UserProfile:
+        """Create an instance of UserProfile from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return GatewayContext.parse_obj(obj)
+            return UserProfile.parse_obj(obj)
 
-        _obj = GatewayContext.parse_obj({
-            "service_type": obj.get("serviceType"),
-            "fc_url": obj.get("fcUrl"),
-            "flow_json_path": obj.get("flowJsonPath")
+        _obj = UserProfile.parse_obj({
+            "user_id": obj.get("userId"),
+            "user_name": obj.get("userName"),
+            "basic_info": obj.get("basicInfo")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/gateway_issued_params.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_page_result_chat_message_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,25 +14,29 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Dict, Optional
-from pydantic import BaseModel, Field, StrictStr
-from xingchen.models.gateway_context import GatewayContext
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from xingchen.models.page_result_chat_message_dto import PageResultChatMessageDTO
 
-class GatewayIssuedParams(BaseModel):
+class ResultDTOPageResultChatMessageDTO(BaseModel):
     """
-    GatewayIssuedParams
+    ResultDTOPageResultChatMessageDTO
     """
-    user_info: Optional[Dict[str, StrictStr]] = Field(None, alias="userInfo")
-    context: Optional[GatewayContext] = None
-    __properties = ["userInfo", "context"]
+    request_id: Optional[StrictStr] = Field(None, alias="requestId")
+    code: Optional[StrictInt] = None
+    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
+    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
+    data: Optional[PageResultChatMessageDTO] = None
+    success: Optional[StrictBool] = None
+    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,38 +44,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GatewayIssuedParams:
-        """Create an instance of GatewayIssuedParams from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultDTOPageResultChatMessageDTO:
+        """Create an instance of ResultDTOPageResultChatMessageDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of context
-        if self.context:
-            _dict['context'] = self.context.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GatewayIssuedParams:
-        """Create an instance of GatewayIssuedParams from a dict"""
+    def from_dict(cls, obj: dict) -> ResultDTOPageResultChatMessageDTO:
+        """Create an instance of ResultDTOPageResultChatMessageDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return GatewayIssuedParams.parse_obj(obj)
+            return ResultDTOPageResultChatMessageDTO.parse_obj(obj)
 
-        _obj = GatewayIssuedParams.parse_obj({
-            "user_info": obj.get("userInfo"),
-            "context": GatewayContext.from_dict(obj.get("context")) if obj.get("context") is not None else None
+        _obj = ResultDTOPageResultChatMessageDTO.parse_obj({
+            "request_id": obj.get("requestId"),
+            "code": obj.get("code"),
+            "error_message": obj.get("errorMessage"),
+            "error_message_key": obj.get("errorMessageKey"),
+            "data": PageResultChatMessageDTO.from_dict(obj.get("data")) if obj.get("data") is not None else None,
+            "success": obj.get("success")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/input.py` & `xingchen-1.1.1.1/xingchen/models/input.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class Input(BaseModel):
     """
     Input
     """
     prompt: Optional[StrictStr] = None
     messages: Optional[conlist(Message)] = None
-    aca: Optional[Any] = None
+    aca: Optional[Dict[str, Any]] = None
     __properties = ["prompt", "messages", "aca"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `xingchen-1.1.1/xingchen/models/keyword.py` & `xingchen-1.1.1.1/xingchen/models/meta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,37 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
+
+
+from __future__ import annotations
 import pprint
-from typing import Optional
+import re  # noqa: F401
+import json
 
-from pydantic import BaseModel, Field, StrictStr
 
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class Keyword(BaseModel):
-    value: Optional[StrictStr] = Field(None, alias="value")
-    __properties = ["value"]
+class Meta(BaseModel):
+    """
+    Meta
+    """
+    has_risk: Optional[StrictBool] = Field(None, alias="hasRisk")
+    safety_std_answer: Optional[StrictStr] = Field(None, alias="safetyStdAnswer")
+    __properties = ["hasRisk", "safetyStdAnswer"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -21,32 +39,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Keyword:
-        """Create an instance of Keyword from a JSON string"""
+    def from_json(cls, json_str: str) -> Meta:
+        """Create an instance of Meta from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Keyword:
-        """Create an instance of Keyword from a dict"""
+    def from_dict(cls, obj: dict) -> Meta:
+        """Create an instance of Meta from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Keyword.parse_obj(obj)
+            return Meta.parse_obj(obj)
 
-        _obj = Keyword.parse_obj({
-            "value": obj.get("value")
+        _obj = Meta.parse_obj({
+            "has_risk": obj.get("hasRisk"),
+            "safety_std_answer": obj.get("safetyStdAnswer")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/long_term_memory.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_boolean.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,41 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
-import pprint
-from typing import Optional
+"""
+    XingChen 开放接口定义
+
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
+
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""  # noqa: E501
 
-from pydantic import BaseModel, Field, StrictStr, StrictBool, conlist
 
-from xingchen.models.kv_memory_config import KVMemoryConfig
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class LongTermMemory(BaseModel):
-    enabled: Optional[StrictBool] = Field(None, description="是否启动")
-    memory_type: Optional[StrictStr] = Field(None, alias="memoryType", description="记忆类型")
-    kv_memory_configs: Optional[conlist(KVMemoryConfig)] = Field(None, alias="kvMemoryConfigs",
-                                                                 description="kv记忆配置,当memoryType为kv时生效")
-    __properties = ["enabled", "memoryType", "kvMemoryConfigs"]
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+
+class ResultDTOBoolean(BaseModel):
+    """
+    ResultDTOBoolean
+    """
+    request_id: Optional[StrictStr] = Field(None, alias="requestId")
+    code: Optional[StrictInt] = None
+    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
+    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
+    data: Optional[StrictBool] = None
+    success: Optional[StrictBool] = None
+    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -26,35 +43,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> LongTermMemory:
-        """Create an instance of LongTermMemory from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultDTOBoolean:
+        """Create an instance of ResultDTOBoolean from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> LongTermMemory:
-        """Create an instance of LongTermMemory from a dict"""
+    def from_dict(cls, obj: dict) -> ResultDTOBoolean:
+        """Create an instance of ResultDTOBoolean from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return KVMemoryConfig.parse_obj(obj)
+            return ResultDTOBoolean.parse_obj(obj)
 
-        _obj = KVMemoryConfig.parse_obj({
-            "enabled": obj.get("enabled"),
-            "memory_type": obj.get("memoryType"),
-            "kv_memory_configs": [KVMemoryConfig.from_dict(_item) for _item in obj.get("kvMemoryConfigs")] if obj.get(
-                "kvMemoryConfigs") is not None else None
+        _obj = ResultDTOBoolean.parse_obj({
+            "request_id": obj.get("requestId"),
+            "code": obj.get("code"),
+            "error_message": obj.get("errorMessage"),
+            "error_message_key": obj.get("errorMessageKey"),
+            "data": obj.get("data"),
+            "success": obj.get("success")
         })
         return _obj
+
+
```

### Comparing `xingchen-1.1.1/xingchen/models/memory.py` & `xingchen-1.1.1.1/xingchen/models/message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,44 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
-import pprint
-from typing import Optional
+"""
+    XingChen 开放接口定义
 
-from pydantic import BaseModel, Field, StrictStr, conlist
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-from xingchen.models.message import Message
-from xingchen.models.extract_data import ExtractData
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-class Memory(BaseModel):
-    summaries: Optional[conlist(StrictStr)] = Field(None, alias="summaries")
-    originals: Optional[conlist(Message)] = Field(None, alias="originals")
-    tags: Optional[conlist(ExtractData)] = Field(None, alias="tags")
-    __properties = ["summaries", "originals", "tags"]
+
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
+from xingchen.models.meta import Meta
+from xingchen.models.function_call import FunctionCall
+
+
+class Message(BaseModel):
+    """
+    Message
+    """
+    name: Optional[StrictStr] = None
+    role: Optional[StrictStr] = None
+    content: Optional[StrictStr] = None
+    finish_reason: Optional[StrictStr] = Field(None, alias="finishReason")
+    meta: Optional[Meta] = None
+    function_call: Optional[FunctionCall] = Field(None, alias="functionCall", description="函数调用")
+    __properties = ["name", "role", "content", "finishReason", "meta", "functionCall"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -26,36 +46,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Memory:
-        """Create an instance of Memory from a JSON string"""
+    def from_json(cls, json_str: str) -> Message:
+        """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of meta
+        if self.meta:
+            _dict['meta'] = self.meta.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Memory:
-        """Create an instance of Memory from a dict"""
+    def from_dict(cls, obj: dict) -> Message:
+        """Create an instance of Message from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Memory.parse_obj(obj)
+            return Message.parse_obj(obj)
 
-        _obj = Memory.parse_obj({
-            "summaries": obj.get("summaries"),
-            "originals": [Message.from_dict(_item) for _item in obj.get("originals")] if obj.get(
-                "originals") is not None else None,
-            "tags": [ExtractData.from_dict(_item) for _item in obj.get("tags")] if obj.get(
-                "tags") is not None else None
+        _obj = Message.parse_obj({
+            "name": obj.get("name"),
+            "role": obj.get("role"),
+            "content": obj.get("content"),
+            "finish_reason": obj.get("finishReason"),
+            "meta": Meta.from_dict(obj.get("meta")) if obj.get("meta") is not None else None
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/models/message.py` & `xingchen-1.1.1.1/xingchen/models/base_chat_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,30 +15,29 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
-from xingchen.models.meta import Meta
-from xingchen.models.function_call import FunctionCall
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from xingchen.models.gateway_issued_params import GatewayIssuedParams
+from xingchen.models.input import Input
+from xingchen.models.model_parameters import ModelParameters
 
-
-class Message(BaseModel):
+class BaseChatRequest(BaseModel):
     """
-    Message
+    BaseChatRequest
     """
-    name: Optional[StrictStr] = None
-    role: Optional[StrictStr] = None
-    content: Optional[StrictStr] = None
-    finish_reason: Optional[StrictStr] = Field(None, alias="finishReason")
-    meta: Optional[Meta] = None
-    function_call: Optional[FunctionCall] = Field(None, alias="functionCall", description="函数调用")
-    __properties = ["name", "role", "content", "finishReason", "meta", "functionCall"]
+    model: Optional[StrictStr] = None
+    parameters: Optional[ModelParameters] = None
+    input: Input = Field(...)
+    servicename: Optional[StrictStr] = None
+    debug: Optional[StrictBool] = None
+    __properties = ["model", "parameters", "input", "servicename", "debug"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -46,41 +45,44 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Message:
-        """Create an instance of Message from a JSON string"""
+    def from_json(cls, json_str: str) -> BaseChatRequest:
+        """Create an instance of BaseChatRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of meta
-        if self.meta:
-            _dict['meta'] = self.meta.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of parameters
+        if self.parameters:
+            _dict['parameters'] = self.parameters.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of input
+        if self.input:
+            _dict['input'] = self.input.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Message:
-        """Create an instance of Message from a dict"""
+    def from_dict(cls, obj: dict) -> BaseChatRequest:
+        """Create an instance of BaseChatRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Message.parse_obj(obj)
+            return BaseChatRequest.parse_obj(obj)
 
-        _obj = Message.parse_obj({
-            "name": obj.get("name"),
-            "role": obj.get("role"),
-            "content": obj.get("content"),
-            "finish_reason": obj.get("finishReason"),
-            "meta": Meta.from_dict(obj.get("meta")) if obj.get("meta") is not None else None
+        _obj = BaseChatRequest.parse_obj({
+            "model": obj.get("model"),
+            "parameters": ModelParameters.from_dict(obj.get("parameters")) if obj.get("parameters") is not None else None,
+            "input": Input.from_dict(obj.get("input")) if obj.get("input") is not None else None,
+            "servicename": obj.get("servicename"),
+            "debug": obj.get("debug")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/message_rating_request.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_page_result_character_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,24 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictStr, conint
-from xingchen.models.gateway_issued_params import GatewayIssuedParams
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from xingchen.models.page_result_character_dto import PageResultCharacterDTO
 
-class MessageRatingRequest(BaseModel):
+class ResultDTOPageResultCharacterDTO(BaseModel):
     """
-    MessageRatingRequest
+    ResultDTOPageResultCharacterDTO
     """
-    message_id: StrictStr = Field(..., alias="messageId", description="待评分消息ID")
-    rating: conint(strict=True, le=5, ge=-1) = Field(..., description="评分")
-    __properties = ["messageId", "rating"]
+    request_id: Optional[StrictStr] = Field(None, alias="requestId")
+    code: Optional[StrictInt] = None
+    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
+    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
+    data: Optional[PageResultCharacterDTO] = None
+    success: Optional[StrictBool] = None
+    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -40,35 +44,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> MessageRatingRequest:
-        """Create an instance of MessageRatingRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultDTOPageResultCharacterDTO:
+        """Create an instance of ResultDTOPageResultCharacterDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of data
+        if self.data:
+            _dict['data'] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> MessageRatingRequest:
-        """Create an instance of MessageRatingRequest from a dict"""
+    def from_dict(cls, obj: dict) -> ResultDTOPageResultCharacterDTO:
+        """Create an instance of ResultDTOPageResultCharacterDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return MessageRatingRequest.parse_obj(obj)
+            return ResultDTOPageResultCharacterDTO.parse_obj(obj)
 
-        _obj = MessageRatingRequest.parse_obj({
-            "message_id": obj.get("messageId"),
-            "rating": obj.get("rating")
+        _obj = ResultDTOPageResultCharacterDTO.parse_obj({
+            "request_id": obj.get("requestId"),
+            "code": obj.get("code"),
+            "error_message": obj.get("errorMessage"),
+            "error_message_key": obj.get("errorMessageKey"),
+            "data": PageResultCharacterDTO.from_dict(obj.get("data")) if obj.get("data") is not None else None,
+            "success": obj.get("success")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/meta.py` & `xingchen-1.1.1.1/xingchen/models/model_parameters.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,24 +14,32 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from typing import Optional, Union
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, StrictBool
 
-class Meta(BaseModel):
+
+class ModelParameters(BaseModel):
     """
-    Meta
+    ModelParameters
     """
-    has_risk: Optional[StrictBool] = Field(None, alias="hasRisk")
-    safety_std_answer: Optional[StrictStr] = Field(None, alias="safetyStdAnswer")
-    __properties = ["hasRisk", "safetyStdAnswer"]
+    model_name: Optional[StrictStr] = Field(None, alias="modelName")
+    top_p: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="topP")
+    top_k: Optional[StrictInt] = Field(None, alias="topK")
+    seed: Optional[StrictInt] = None
+    max_length: Optional[StrictInt] = Field(None, alias="maxLength")
+    min_length: Optional[StrictInt] = Field(None, alias="minLength")
+    temperature: Optional[Union[StrictFloat, StrictInt]] = None
+    incremental_output: Optional[StrictBool] = Field(False, alias="incrementalOutput")
+
+    __properties = ["modelName", "topP", "topK", "seed", "maxLength", "minLength", "temperature", "incrementalOutput"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -39,35 +47,41 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Meta:
-        """Create an instance of Meta from a JSON string"""
+    def from_json(cls, json_str: str) -> ModelParameters:
+        """Create an instance of ModelParameters from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Meta:
-        """Create an instance of Meta from a dict"""
+    def from_dict(cls, obj: dict) -> ModelParameters:
+        """Create an instance of ModelParameters from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return Meta.parse_obj(obj)
+            return ModelParameters.parse_obj(obj)
 
-        _obj = Meta.parse_obj({
-            "has_risk": obj.get("hasRisk"),
-            "safety_std_answer": obj.get("safetyStdAnswer")
+        _obj = ModelParameters.parse_obj({
+            "model_name": obj.get("modelName"),
+            "top_p": obj.get("topP"),
+            "top_k": obj.get("topK"),
+            "seed": obj.get("seed"),
+            "max_length": obj.get("maxLength"),
+            "min_length": obj.get("minLength"),
+            "temperature": obj.get("temperature"),
+            "incremental_output": obj.get("incrementalOutput")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/model_parameters.py` & `xingchen-1.1.1.1/xingchen/models/page_result_chat_message_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,32 +14,28 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional, Union
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, StrictBool
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictInt, conlist
+from xingchen.models.chat_message_dto import ChatMessageDTO
 
-
-class ModelParameters(BaseModel):
+class PageResultChatMessageDTO(BaseModel):
     """
-    ModelParameters
+    PageResultChatMessageDTO
     """
-    model_name: Optional[StrictStr] = Field(None, alias="modelName")
-    top_p: Optional[Union[StrictFloat, StrictInt]] = Field(None, alias="topP")
-    top_k: Optional[StrictInt] = Field(None, alias="topK")
-    seed: Optional[StrictInt] = None
-    max_length: Optional[StrictInt] = Field(None, alias="maxLength")
-    min_length: Optional[StrictInt] = Field(None, alias="minLength")
-    temperature: Optional[Union[StrictFloat, StrictInt]] = None
-    incremental_output: Optional[StrictBool] = Field(False, alias="incrementalOutput")
-
-    __properties = ["modelName", "topP", "topK", "seed", "maxLength", "minLength", "temperature", "incrementalOutput"]
+    list: Optional[conlist(ChatMessageDTO)] = None
+    page: Optional[StrictInt] = None
+    page_size: Optional[StrictInt] = Field(None, alias="pageSize")
+    total: Optional[StrictInt] = None
+    page_offset_value: Optional[StrictInt] = Field(None, alias="pageOffsetValue")
+    __properties = ["list", "page", "pageSize", "total", "pageOffsetValue"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -47,41 +43,45 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ModelParameters:
-        """Create an instance of ModelParameters from a JSON string"""
+    def from_json(cls, json_str: str) -> PageResultChatMessageDTO:
+        """Create an instance of PageResultChatMessageDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in list (list)
+        _items = []
+        if self.list:
+            for _item in self.list:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['list'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ModelParameters:
-        """Create an instance of ModelParameters from a dict"""
+    def from_dict(cls, obj: dict) -> PageResultChatMessageDTO:
+        """Create an instance of PageResultChatMessageDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ModelParameters.parse_obj(obj)
+            return PageResultChatMessageDTO.parse_obj(obj)
 
-        _obj = ModelParameters.parse_obj({
-            "model_name": obj.get("modelName"),
-            "top_p": obj.get("topP"),
-            "top_k": obj.get("topK"),
-            "seed": obj.get("seed"),
-            "max_length": obj.get("maxLength"),
-            "min_length": obj.get("minLength"),
-            "temperature": obj.get("temperature"),
-            "incremental_output": obj.get("incrementalOutput")
+        _obj = PageResultChatMessageDTO.parse_obj({
+            "list": [ChatMessageDTO.from_dict(_item) for _item in obj.get("list")] if obj.get("list") is not None else None,
+            "page": obj.get("page"),
+            "page_size": obj.get("pageSize"),
+            "total": obj.get("total"),
+            "page_offset_value": obj.get("pageOffsetValue")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/page_result_character_dto.py` & `xingchen-1.1.1.1/xingchen/models/result_dto_list_character_dto.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, conlist
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, conlist
 from xingchen.models.character_dto import CharacterDTO
 
-class PageResultCharacterDTO(BaseModel):
+class ResultDTOListCharacterDTO(BaseModel):
     """
-    PageResultCharacterDTO
+    ResultDTOListCharacterDTO
     """
-    list: Optional[conlist(CharacterDTO)] = None
-    page: Optional[StrictInt] = None
-    page_size: Optional[StrictInt] = Field(None, alias="pageSize")
-    total: Optional[StrictInt] = None
-    page_offset_value: Optional[StrictInt] = Field(None, alias="pageOffsetValue")
-    __properties = ["list", "page", "pageSize", "total", "pageOffsetValue"]
+    request_id: Optional[StrictStr] = Field(None, alias="requestId")
+    code: Optional[StrictInt] = None
+    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
+    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
+    data: Optional[conlist(CharacterDTO)] = None
+    success: Optional[StrictBool] = None
+    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -43,45 +44,46 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PageResultCharacterDTO:
-        """Create an instance of PageResultCharacterDTO from a JSON string"""
+    def from_json(cls, json_str: str) -> ResultDTOListCharacterDTO:
+        """Create an instance of ResultDTOListCharacterDTO from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in list (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
         _items = []
-        if self.list:
-            for _item in self.list:
+        if self.data:
+            for _item in self.data:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['list'] = _items
+            _dict['data'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PageResultCharacterDTO:
-        """Create an instance of PageResultCharacterDTO from a dict"""
+    def from_dict(cls, obj: dict) -> ResultDTOListCharacterDTO:
+        """Create an instance of ResultDTOListCharacterDTO from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PageResultCharacterDTO.parse_obj(obj)
+            return ResultDTOListCharacterDTO.parse_obj(obj)
 
-        _obj = PageResultCharacterDTO.parse_obj({
-            "list": [CharacterDTO.from_dict(_item) for _item in obj.get("list")] if obj.get("list") is not None else None,
-            "page": obj.get("page"),
-            "page_size": obj.get("pageSize"),
-            "total": obj.get("total"),
-            "page_offset_value": obj.get("pageOffsetValue")
+        _obj = ResultDTOListCharacterDTO.parse_obj({
+            "request_id": obj.get("requestId"),
+            "code": obj.get("code"),
+            "error_message": obj.get("errorMessage"),
+            "error_message_key": obj.get("errorMessageKey"),
+            "data": [CharacterDTO.from_dict(_item) for _item in obj.get("data")] if obj.get("data") is not None else None,
+            "success": obj.get("success")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/page_result_chat_message_dto.py` & `xingchen-1.1.1.1/xingchen/models/repository.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, conlist
-from xingchen.models.chat_message_dto import ChatMessageDTO
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-class PageResultChatMessageDTO(BaseModel):
+class Repository(BaseModel):
     """
-    PageResultChatMessageDTO
+    知识库文件信息  # noqa: E501
     """
-    list: Optional[conlist(ChatMessageDTO)] = None
-    page: Optional[StrictInt] = None
-    page_size: Optional[StrictInt] = Field(None, alias="pageSize")
-    total: Optional[StrictInt] = None
-    page_offset_value: Optional[StrictInt] = Field(None, alias="pageOffsetValue")
-    __properties = ["list", "page", "pageSize", "total", "pageOffsetValue"]
+    file_save_path: Optional[StrictStr] = Field(None, alias="fileSavePath")
+    filename: Optional[StrictStr] = None
+    file_url: Optional[StrictStr] = Field(None, alias="fileUrl")
+    status: Optional[StrictStr] = None
+    __properties = ["fileSavePath", "filename", "fileUrl", "status"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -43,45 +41,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PageResultChatMessageDTO:
-        """Create an instance of PageResultChatMessageDTO from a JSON string"""
+    def from_json(cls, json_str: str) -> Repository:
+        """Create an instance of Repository from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in list (list)
-        _items = []
-        if self.list:
-            for _item in self.list:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['list'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PageResultChatMessageDTO:
-        """Create an instance of PageResultChatMessageDTO from a dict"""
+    def from_dict(cls, obj: dict) -> Repository:
+        """Create an instance of Repository from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return PageResultChatMessageDTO.parse_obj(obj)
+            return Repository.parse_obj(obj)
 
-        _obj = PageResultChatMessageDTO.parse_obj({
-            "list": [ChatMessageDTO.from_dict(_item) for _item in obj.get("list")] if obj.get("list") is not None else None,
-            "page": obj.get("page"),
-            "page_size": obj.get("pageSize"),
-            "total": obj.get("total"),
-            "page_offset_value": obj.get("pageOffsetValue")
+        _obj = Repository.parse_obj({
+            "file_save_path": obj.get("fileSavePath"),
+            "filename": obj.get("filename"),
+            "file_url": obj.get("fileUrl"),
+            "status": obj.get("status")
         })
         return _obj
```

### Comparing `xingchen-1.1.1/xingchen/models/repository_info.py` & `xingchen-1.1.1.1/xingchen/models/repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen/models/result_dto_character_desc_dto.py` & `xingchen-1.1.1.1/xingchen/models/base_chat_request_aca_chat_ext_param.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-from __future__ import annotations
+# coding: utf-8
 
-import json
-import pprint
-import re  # noqa: F401
-from typing import Optional
+"""
+    XingChen 开放接口定义
 
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+    No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)
 
-from xingchen.models.character_desc_dto import CharacterDescDTO
+    The version of the OpenAPI document: v2
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""  # noqa: E501
 
-class ResultDTOCharacterDescDTO(BaseModel):
-    request_id: Optional[StrictStr] = Field(None, alias="requestId")
-    code: Optional[StrictInt] = None
-    error_message: Optional[StrictStr] = Field(None, alias="errorMessage")
-    error_message_key: Optional[StrictStr] = Field(None, alias="errorMessageKey")
-    data: Optional[CharacterDescDTO] = None
-    success: Optional[StrictBool] = None
-    __properties = ["requestId", "code", "errorMessage", "errorMessageKey", "data", "success"]
+
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from xingchen.models.gateway_issued_params import GatewayIssuedParams
+from xingchen.models.input import Input
+from xingchen.models.model_parameters import ModelParameters
+
+class BaseChatRequestAcaChatExtParam(BaseModel):
+    """
+    BaseChatRequestAcaChatExtParam
+    """
+    model: Optional[StrictStr] = None
+    parameters: Optional[ModelParameters] = None
+    input: Input = Field(...)
+    servicename: Optional[StrictStr] = None
+    debug: Optional[StrictBool] = None
+    __properties = ["model", "parameters", "input", "servicename", "debug"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -29,40 +45,44 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ResultDTOCharacterDescDTO:
-        """Create an instance of ResultDTOCharacterDescDTO from a JSON string"""
+    def from_json(cls, json_str: str) -> BaseChatRequestAcaChatExtParam:
+        """Create an instance of BaseChatRequestAcaChatExtParam from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of data
-        if self.data:
-            _dict['data'] = self.data.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of parameters
+        if self.parameters:
+            _dict['parameters'] = self.parameters.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of input
+        if self.input:
+            _dict['input'] = self.input.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ResultDTOCharacterDescDTO:
-        """Create an instance of ResultDTOCharacterDescDTO from a dict"""
+    def from_dict(cls, obj: dict) -> BaseChatRequestAcaChatExtParam:
+        """Create an instance of BaseChatRequestAcaChatExtParam from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return ResultDTOCharacterDescDTO.parse_obj(obj)
+            return BaseChatRequestAcaChatExtParam.parse_obj(obj)
 
-        _obj = ResultDTOCharacterDescDTO.parse_obj({
-            "request_id": obj.get("requestId"),
-            "code": obj.get("code"),
-            "error_message": obj.get("errorMessage"),
-            "error_message_key": obj.get("errorMessageKey"),
-            "data": CharacterDescDTO.from_dict(obj.get("data")) if obj.get("data") is not None else None,
-            "success": obj.get("success")
+        _obj = BaseChatRequestAcaChatExtParam.parse_obj({
+            "model": obj.get("model"),
+            "parameters": ModelParameters.from_dict(obj.get("parameters")) if obj.get("parameters") is not None else None,
+            "input": Input.from_dict(obj.get("input")) if obj.get("input") is not None else None,
+            "servicename": obj.get("servicename"),
+            "debug": obj.get("debug")
         })
         return _obj
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.1/xingchen/rest.py` & `xingchen-1.1.1.1/xingchen/rest.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.1/xingchen.egg-info/SOURCES.txt` & `xingchen-1.1.1.1/xingchen.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -56,86 +56,56 @@
 xingchen.egg-info/SOURCES.txt
 xingchen.egg-info/dependency_links.txt
 xingchen.egg-info/requires.txt
 xingchen.egg-info/top_level.txt
 xingchen/api/__init__.py
 xingchen/api/character_api_sub.py
 xingchen/api/chat_api_sub.py
-xingchen/api/chat_extract_message_api_sub.py
 xingchen/api/chat_message_api_sub.py
-xingchen/api/common_api_sub.py
-xingchen/api/groupchat_api_sub.py
 xingchen/models/__init__.py
 xingchen/models/advanced_settings.py
 xingchen/models/base_chat_request.py
+xingchen/models/base_chat_request_aca_chat_ext_param.py
 xingchen/models/character_advanced_config.py
 xingchen/models/character_create_dto.py
-xingchen/models/character_desc_dto.py
-xingchen/models/character_desc_generated_request.py
 xingchen/models/character_dto.py
 xingchen/models/character_key.py
 xingchen/models/character_permission_config.py
 xingchen/models/character_query_dto.py
 xingchen/models/character_query_where.py
 xingchen/models/character_update_dto.py
 xingchen/models/character_version_create_or_update_dto.py
 xingchen/models/chat_context.py
 xingchen/models/chat_history_query_dto.py
 xingchen/models/chat_history_query_where.py
 xingchen/models/chat_message_dto.py
 xingchen/models/chat_req_params.py
 xingchen/models/chat_room_user_dto.py
 xingchen/models/context.py
-xingchen/models/extract_data.py
-xingchen/models/extract_kv_dto.py
-xingchen/models/extract_memory_request.py
-xingchen/models/extract_summary_dto.py
-xingchen/models/file_conver_dto.py
-xingchen/models/file_conver_request.py
 xingchen/models/file_info_vo.py
 xingchen/models/function_call.py
 xingchen/models/gateway_context.py
 xingchen/models/gateway_issued_params.py
 xingchen/models/input.py
-xingchen/models/keyword.py
-xingchen/models/kv_memory_config.py
-xingchen/models/long_term_memory.py
-xingchen/models/memory.py
-xingchen/models/memory_summary.py
 xingchen/models/message.py
 xingchen/models/message_rating_request.py
 xingchen/models/meta.py
 xingchen/models/model_parameters.py
 xingchen/models/page_result_character_dto.py
 xingchen/models/page_result_chat_message_dto.py
-xingchen/models/platform_plugin.py
-xingchen/models/polling_image_detail_dto.py
-xingchen/models/reject_answer_plugin.py
-xingchen/models/reject_condition.py
 xingchen/models/repository.py
 xingchen/models/repository_info.py
 xingchen/models/result_dto_boolean.py
-xingchen/models/result_dto_character_desc_dto.py
 xingchen/models/result_dto_character_dto.py
 xingchen/models/result_dto_character_key.py
-xingchen/models/result_dto_extract_kv_dto.py
-xingchen/models/result_dto_extract_summary_dto.py
-xingchen/models/result_dto_file_conver_dto.py
 xingchen/models/result_dto_list_character_dto.py
 xingchen/models/result_dto_page_result_character_dto.py
 xingchen/models/result_dto_page_result_chat_message_dto.py
-xingchen/models/result_dto_polling_image_detail_dto.py
 xingchen/models/scenario.py
-xingchen/models/stop_chat_request.py
 xingchen/models/sys_reminder_request.py
-xingchen/models/text_to_image_plugin.py
 xingchen/models/user_profile.py
 xingchen/models/custom/__init__.py
 xingchen/models/custom/base_response.py
 xingchen/models/custom/character_model_parameters.py
 xingchen/models/custom/chat_response.py
 xingchen/models/custom/platform_publish_config.py
-xingchen/models/custom/reset_history_request.py
-xingchen/models/custom/groupchat/__init__.py
-xingchen/models/custom/groupchat/group_chat_ext_param.py
-xingchen/models/custom/groupchat/group_chat_reply_setting.py
-xingchen/models/custom/groupchat/group_chat_room_info.py
+xingchen/models/custom/reset_history_request.py
```

