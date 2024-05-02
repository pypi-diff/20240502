# Comparing `tmp/iparapheur-internal-1.11.5.tar.gz` & `tmp/iparapheur-internal-1.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-internal-1.11.5.tar", last modified: Thu May  2 09:51:45 2024, max compression
+gzip compressed data, was "iparapheur-internal-1.12.3.tar", last modified: Fri Apr 19 14:46:45 2024, max compression
```

## Comparing `iparapheur-internal-1.11.5.tar` & `iparapheur-internal-1.12.3.tar`

### file list

```diff
@@ -1,213 +1,197 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:51:45.227409 iparapheur-internal-1.11.5/
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-02 09:51:45.227409 iparapheur-internal-1.11.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13320 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:51:45.187408 iparapheur-internal-1.11.5/iparapheur_internal/
--rw-r--r--   0 root         (0) root         (0)     8059 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:51:45.191408 iparapheur-internal-1.11.5/iparapheur_internal/api/
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42170 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_advanced_config_api.py
--rw-r--r--   0 root         (0) root         (0)    18231 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)    93433 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_layer_api.py
--rw-r--r--   0 root         (0) root         (0)    26447 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)    35616 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_template_api.py
--rw-r--r--   0 root         (0) root         (0)    14505 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_trash_bin_api.py
--rw-r--r--   0 root         (0) root         (0)    18687 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    12402 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/admin_workflow_definition_api.py
--rw-r--r--   0 root         (0) root         (0)    11818 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/current_user_api.py
--rw-r--r--   0 root         (0) root         (0)    15950 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/desk_api.py
--rw-r--r--   0 root         (0) root         (0)    27573 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/folder_api.py
--rw-r--r--   0 root         (0) root         (0)    20001 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/server_info_api.py
--rw-r--r--   0 root         (0) root         (0)    13684 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/template_api.py
--rw-r--r--   0 root         (0) root         (0)    22740 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/typology_api.py
--rw-r--r--   0 root         (0) root         (0)    25503 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api/workflow_api.py
--rw-r--r--   0 root         (0) root         (0)    25875 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/api_response.py
--rw-r--r--   0 root         (0) root         (0)    14816 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/configuration.py
--rw-r--r--   0 root         (0) root         (0)     6025 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:51:45.203408 iparapheur-internal-1.11.5/iparapheur_internal/models/
--rw-r--r--   0 root         (0) root         (0)     6430 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/action.py
--rw-r--r--   0 root         (0) root         (0)     2579 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/composite_id.py
--rw-r--r--   0 root         (0) root         (0)     2960 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/create_file_stamp_request.py
--rw-r--r--   0 root         (0) root         (0)     9758 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/create_folder_request.py
--rw-r--r--   0 root         (0) root         (0)     3294 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     3562 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/detached_signature.py
--rw-r--r--   0 root         (0) root         (0)     8680 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/document_dto.py
--rw-r--r--   0 root         (0) root         (0)     2918 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/error_response.py
--rw-r--r--   0 root         (0) root         (0)     3428 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/external_signature_config.py
--rw-r--r--   0 root         (0) root         (0)     3295 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      909 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     1127 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/external_state.py
--rw-r--r--   0 root         (0) root         (0)     9125 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     4854 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/folder_filter_dto.py
--rw-r--r--   0 root         (0) root         (0)     6481 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)     1174 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      826 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/folder_visibility.py
--rw-r--r--   0 root         (0) root         (0)     6040 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_application.py
--rw-r--r--   0 root         (0) root         (0)     2737 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_cookie.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_data_element.py
--rw-r--r--   0 root         (0) root         (0)     2895 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_data_set.py
--rw-r--r--   0 root         (0) root         (0)     4361 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_declaring_entity.py
--rw-r--r--   0 root         (0) root         (0)     2799 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_declaring_entity_dpo.py
--rw-r--r--   0 root         (0) root         (0)     2835 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_declaring_entity_responsible.py
--rw-r--r--   0 root         (0) root         (0)     2904 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_entity.py
--rw-r--r--   0 root         (0) root         (0)     4705 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_information_details_dto.py
--rw-r--r--   0 root         (0) root         (0)     3785 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     3642 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     3091 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     2654 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/mail_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     3623 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/media_type.py
--rw-r--r--   0 root         (0) root         (0)     3100 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/metadata.py
--rw-r--r--   0 root         (0) root         (0)     4064 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     4768 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4686 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     4751 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)     4855 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     2767 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_info.py
--rw-r--r--   0 root         (0) root         (0)     4766 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     4782 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     4790 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/page_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3804 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/password_policies.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     2755 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/pdf_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     3633 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     3059 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/signature_info.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/signature_placement.py
--rw-r--r--   0 root         (0) root         (0)     9122 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/signature_proof.py
--rw-r--r--   0 root         (0) root         (0)      833 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     2719 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/sort_object.py
--rw-r--r--   0 root         (0) root         (0)     3652 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/stamp_dto.py
--rw-r--r--   0 root         (0) root         (0)      800 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/stamp_text_color.py
--rw-r--r--   0 root         (0) root         (0)      841 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/stamp_type.py
--rw-r--r--   0 root         (0) root         (0)     1103 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/state.py
--rw-r--r--   0 root         (0) root         (0)     6951 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/step_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)      830 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/step_definition_parallel_type.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/step_definition_type.py
--rw-r--r--   0 root         (0) root         (0)     7565 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype.py
--rw-r--r--   0 root         (0) root         (0)    13624 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     2994 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_layer.py
--rw-r--r--   0 root         (0) root         (0)      865 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     3561 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3619 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     7888 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/task.py
--rw-r--r--   0 root         (0) root         (0)     1302 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/template_type.py
--rw-r--r--   0 root         (0) root         (0)     3095 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     2722 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/test_signature_template_request.py
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     3558 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/typology_representation.py
--rw-r--r--   0 root         (0) root         (0)    12060 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/user_dto.py
--rw-r--r--   0 root         (0) root         (0)      887 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     2766 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/validation_service_configuration_dto.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/models/workflow_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/py.typed
--rw-r--r--   0 root         (0) root         (0)     9290 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/iparapheur_internal/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:51:45.227409 iparapheur-internal-1.11.5/iparapheur_internal.egg-info/
--rw-r--r--   0 root         (0) root         (0)      532 2024-05-02 09:51:45.000000 iparapheur-internal-1.11.5/iparapheur_internal.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8137 2024-05-02 09:51:45.000000 iparapheur-internal-1.11.5/iparapheur_internal.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 09:51:45.000000 iparapheur-internal-1.11.5/iparapheur_internal.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-02 09:51:45.000000 iparapheur-internal-1.11.5/iparapheur_internal.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-02 09:51:45.000000 iparapheur-internal-1.11.5/iparapheur_internal.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1952 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-02 09:51:45.227409 iparapheur-internal-1.11.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1420 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 09:51:45.227409 iparapheur-internal-1.11.5/test/
--rw-r--r--   0 root         (0) root         (0)      712 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_action.py
--rw-r--r--   0 root         (0) root         (0)     1449 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_advanced_config_api.py
--rw-r--r--   0 root         (0) root         (0)      838 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1818 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_layer_api.py
--rw-r--r--   0 root         (0) root         (0)     1084 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1229 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_template_api.py
--rw-r--r--   0 root         (0) root         (0)      898 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_trash_bin_api.py
--rw-r--r--   0 root         (0) root         (0)      889 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_admin_workflow_definition_api.py
--rw-r--r--   0 root         (0) root         (0)     1405 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_composite_id.py
--rw-r--r--   0 root         (0) root         (0)     2454 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_create_file_stamp_request.py
--rw-r--r--   0 root         (0) root         (0)    17455 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_create_folder_request.py
--rw-r--r--   0 root         (0) root         (0)      872 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_current_user_api.py
--rw-r--r--   0 root         (0) root         (0)      837 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_detached_signature.py
--rw-r--r--   0 root         (0) root         (0)     5048 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_document_dto.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)     1811 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_external_signature_config.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      847 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      762 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_external_state.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_folder_api.py
--rw-r--r--   0 root         (0) root         (0)    17042 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     2504 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_folder_filter_dto.py
--rw-r--r--   0 root         (0) root         (0)     6949 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      783 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_folder_visibility.py
--rw-r--r--   0 root         (0) root         (0)     2952 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_application.py
--rw-r--r--   0 root         (0) root         (0)     1498 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_cookie.py
--rw-r--r--   0 root         (0) root         (0)     1525 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_data_element.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_data_set.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_declaring_entity.py
--rw-r--r--   0 root         (0) root         (0)     1562 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_declaring_entity_dpo.py
--rw-r--r--   0 root         (0) root         (0)     1659 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_declaring_entity_responsible.py
--rw-r--r--   0 root         (0) root         (0)     1447 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_entity.py
--rw-r--r--   0 root         (0) root         (0)     4344 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_gdpr_information_details_dto.py
--rw-r--r--   0 root         (0) root         (0)     1834 2024-05-02 09:51:18.000000 iparapheur-internal-1.11.5/test/test_hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     1988 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     1597 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_mail_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     1710 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_media_type.py
--rw-r--r--   0 root         (0) root         (0)     1558 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1712 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     2695 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)    14915 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_folder_dto.py
--rw-r--r--   0 root         (0) root         (0)     7853 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_folder_listable_dto.py
--rw-r--r--   0 root         (0) root         (0)     2955 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_hierarchised_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     1432 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_info.py
--rw-r--r--   0 root         (0) root         (0)     2668 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     2696 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     2797 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_page_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     1752 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     1752 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_password_policies.py
--rw-r--r--   0 root         (0) root         (0)     1624 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1577 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_pdf_template_test_request.py
--rw-r--r--   0 root         (0) root         (0)     1854 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     1036 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_server_info_api.py
--rw-r--r--   0 root         (0) root         (0)      776 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1544 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_signature_info.py
--rw-r--r--   0 root         (0) root         (0)     1864 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_signature_placement.py
--rw-r--r--   0 root         (0) root         (0)     5196 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_signature_proof.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1456 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)     1649 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_stamp_dto.py
--rw-r--r--   0 root         (0) root         (0)      770 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_stamp_text_color.py
--rw-r--r--   0 root         (0) root         (0)      734 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_stamp_type.py
--rw-r--r--   0 root         (0) root         (0)      705 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_state.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_step_definition_dto.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_step_definition_parallel_type.py
--rw-r--r--   0 root         (0) root         (0)      798 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_step_definition_type.py
--rw-r--r--   0 root         (0) root         (0)     3715 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype.py
--rw-r--r--   0 root         (0) root         (0)     4811 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1535 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_layer.py
--rw-r--r--   0 root         (0) root         (0)      833 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_metadata.py
--rw-r--r--   0 root         (0) root         (0)     1969 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3578 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_task.py
--rw-r--r--   0 root         (0) root         (0)      860 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_template_api.py
--rw-r--r--   0 root         (0) root         (0)      755 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_template_type.py
--rw-r--r--   0 root         (0) root         (0)     1589 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1630 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_test_signature_template_request.py
--rw-r--r--   0 root         (0) root         (0)     1967 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      960 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_typology_api.py
--rw-r--r--   0 root         (0) root         (0)     1702 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     3993 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      762 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1776 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_validation_service_configuration_dto.py
--rw-r--r--   0 root         (0) root         (0)     1157 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_workflow_api.py
--rw-r--r--   0 root         (0) root         (0)     3965 2024-05-02 09:51:19.000000 iparapheur-internal-1.11.5/test/test_workflow_definition_dto.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/
+-rw-r--r--   0 root         (0) root         (0)      532 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12584 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.782265 iparapheur-internal-1.12.3/iparapheur_internal/
+-rw-r--r--   0 root         (0) root         (0)     7493 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.786265 iparapheur-internal-1.12.3/iparapheur_internal/api/
+-rw-r--r--   0 root         (0) root         (0)      994 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32735 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_advanced_config_api.py
+-rw-r--r--   0 root         (0) root         (0)    18231 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)    93433 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_layer_api.py
+-rw-r--r--   0 root         (0) root         (0)    26447 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)    35616 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_template_api.py
+-rw-r--r--   0 root         (0) root         (0)    14505 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_trash_bin_api.py
+-rw-r--r--   0 root         (0) root         (0)    18687 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    11818 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/current_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    15950 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/desk_api.py
+-rw-r--r--   0 root         (0) root         (0)    27573 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    20001 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/server_info_api.py
+-rw-r--r--   0 root         (0) root         (0)    13684 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/template_api.py
+-rw-r--r--   0 root         (0) root         (0)    22740 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    25503 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api/workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)    25875 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    14816 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.802265 iparapheur-internal-1.12.3/iparapheur_internal/models/
+-rw-r--r--   0 root         (0) root         (0)     5957 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/action.py
+-rw-r--r--   0 root         (0) root         (0)     2960 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/create_file_stamp_request.py
+-rw-r--r--   0 root         (0) root         (0)     8955 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)     3294 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3562 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/detached_signature.py
+-rw-r--r--   0 root         (0) root         (0)     8680 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/document_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      909 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/external_state.py
+-rw-r--r--   0 root         (0) root         (0)     8322 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4854 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_filter_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6481 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      826 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/folder_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_application.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_cookie.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_element.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_set.py
+-rw-r--r--   0 root         (0) root         (0)     4361 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_dpo.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_responsible.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_information_details_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3785 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/mail_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/media_type.py
+-rw-r--r--   0 root         (0) root         (0)     4064 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     4768 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4686 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4751 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4855 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_info.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4782 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/page_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3804 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/password_policies.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_info.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_placement.py
+-rw-r--r--   0 root         (0) root         (0)      833 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_dto.py
+-rw-r--r--   0 root         (0) root         (0)      800 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_text_color.py
+-rw-r--r--   0 root         (0) root         (0)      841 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_type.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/state.py
+-rw-r--r--   0 root         (0) root         (0)     6951 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)      830 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_parallel_type.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_type.py
+-rw-r--r--   0 root         (0) root         (0)    13624 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      865 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3210 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3619 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     7888 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/task.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/template_type.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/test_signature_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)    12060 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      887 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/validation_service_configuration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/models/workflow_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/py.typed
+-rw-r--r--   0 root         (0) root         (0)     9290 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/iparapheur_internal/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      532 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7530 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-19 14:46:45.000000 iparapheur-internal-1.12.3/iparapheur_internal.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1952 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 14:46:45.830265 iparapheur-internal-1.12.3/test/
+-rw-r--r--   0 root         (0) root         (0)      712 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_action.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_advanced_config_api.py
+-rw-r--r--   0 root         (0) root         (0)      838 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_layer_api.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1229 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_template_api.py
+-rw-r--r--   0 root         (0) root         (0)      898 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_trash_bin_api.py
+-rw-r--r--   0 root         (0) root         (0)      889 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_create_file_stamp_request.py
+-rw-r--r--   0 root         (0) root         (0)    13658 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_create_folder_request.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_current_user_api.py
+-rw-r--r--   0 root         (0) root         (0)      837 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_detached_signature.py
+-rw-r--r--   0 root         (0) root         (0)     5048 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_document_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      847 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_external_state.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_folder_api.py
+-rw-r--r--   0 root         (0) root         (0)    13245 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_filter_dto.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      783 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_folder_visibility.py
+-rw-r--r--   0 root         (0) root         (0)     2952 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_application.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_cookie.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_data_element.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_data_set.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1562 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_dpo.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_responsible.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4344 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_gdpr_information_details_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_mail_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_media_type.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      755 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)    14129 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_folder_dto.py
+-rw-r--r--   0 root         (0) root         (0)     7853 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_folder_listable_dto.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_hierarchised_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_info.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2696 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     2797 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_page_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_password_policies.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_pdf_template_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     1854 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_server_info_api.py
+-rw-r--r--   0 root         (0) root         (0)      776 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_info.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_placement.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_stamp_dto.py
+-rw-r--r--   0 root         (0) root         (0)      770 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_stamp_text_color.py
+-rw-r--r--   0 root         (0) root         (0)      734 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_stamp_type.py
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_state.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_step_definition_dto.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_step_definition_parallel_type.py
+-rw-r--r--   0 root         (0) root         (0)      798 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_step_definition_type.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      833 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_task.py
+-rw-r--r--   0 root         (0) root         (0)      860 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_template_api.py
+-rw-r--r--   0 root         (0) root         (0)      755 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_template_type.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2024-04-19 14:46:17.000000 iparapheur-internal-1.12.3/test/test_test_signature_template_request.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      960 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_typology_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      762 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1776 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_validation_service_configuration_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1157 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2024-04-19 14:46:18.000000 iparapheur-internal-1.12.3/test/test_workflow_definition_dto.py
```

### Comparing `iparapheur-internal-1.11.5/PKG-INFO` & `iparapheur-internal-1.12.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iparapheur-internal
-Version: 1.11.5
+Version: 1.12.3
 Summary: iparapheur
 Home-page: 
 Author: Libriciel SCOP
 Author-email: iparapheur@libriciel.coop
 License: Affero GPL 3.0
 Keywords: OpenAPI,OpenAPI-Generator,iparapheur
 Description-Content-Type: text/markdown
```

### Comparing `iparapheur-internal-1.11.5/README.md` & `iparapheur-internal-1.12.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.11.5
+- Package version: 1.12.3
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -74,28 +74,29 @@
 
 # Enter a context with an instance of the API client
 with iparapheur_internal.ApiClient(configuration) as api_client:
     # Create an instance of the API class
     api_instance = iparapheur_internal.AdminAdvancedConfigApi(api_client)
 
     try:
-        # Delete Chorus Pro configuration
-        api_instance.delete_chorus_configuration()
+        # Get Chorus Pro configuration
+        api_response = api_instance.get_chorus_configuration()
+        print("The response of AdminAdvancedConfigApi->get_chorus_configuration:\n")
+        pprint(api_response)
     except ApiException as e:
-        print("Exception when calling AdminAdvancedConfigApi->delete_chorus_configuration: %s\n" % e)
+        print("Exception when calling AdminAdvancedConfigApi->get_chorus_configuration: %s\n" % e)
 
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *http://localhost:8080*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
-*AdminAdvancedConfigApi* | [**delete_chorus_configuration**](docs/AdminAdvancedConfigApi.md#delete_chorus_configuration) | **DELETE** /api/internal/admin/config/chorus-configuration | Delete Chorus Pro configuration
 *AdminAdvancedConfigApi* | [**get_chorus_configuration**](docs/AdminAdvancedConfigApi.md#get_chorus_configuration) | **GET** /api/internal/admin/config/chorus | Get Chorus Pro configuration
 *AdminAdvancedConfigApi* | [**update_chorus_configuration**](docs/AdminAdvancedConfigApi.md#update_chorus_configuration) | **PUT** /api/internal/admin/config/chorus-configuration | Edit Chorus Pro configuration
 *AdminAdvancedConfigApi* | [**update_gdpr_information_details**](docs/AdminAdvancedConfigApi.md#update_gdpr_information_details) | **PUT** /api/internal/admin/config/gdpr | Register GDPR information details
 *AdminDeskApi* | [**list_hierarchic_desks**](docs/AdminDeskApi.md#list_hierarchic_desks) | **GET** /api/internal/admin/tenant/{tenantId}/desk | List desks
 *AdminLayerApi* | [**create_file_stamp**](docs/AdminLayerApi.md#create_file_stamp) | **POST** /api/internal/admin/tenant/{tenantId}/layer/{layerId}/stamp | Create a file stamp
 *AdminLayerApi* | [**create_layer**](docs/AdminLayerApi.md#create_layer) | **POST** /api/internal/admin/tenant/{tenantId}/layer | Create a layer
 *AdminLayerApi* | [**delete_file_stamp**](docs/AdminLayerApi.md#delete_file_stamp) | **DELETE** /api/internal/admin/tenant/{tenantId}/layer/{layerId}/stamp/{stampId} | Delete a stored image stamp
@@ -107,15 +108,14 @@
 *AdminSealCertificateApi* | [**get_seal_signature_image**](docs/AdminSealCertificateApi.md#get_seal_signature_image) | **GET** /api/internal/admin/tenant/{tenantId}/sealCertificate/{sealCertificateId}/signatureImage | Get seal&#39;s signature image
 *AdminSealCertificateApi* | [**list_subtype_usage**](docs/AdminSealCertificateApi.md#list_subtype_usage) | **GET** /api/internal/admin/tenant/{tenantId}/sealCertificate/{sealCertificateId}/subtypeUsage | List subtypes using the given certificate
 *AdminTemplateApi* | [**test_docket_pdf_template**](docs/AdminTemplateApi.md#test_docket_pdf_template) | **POST** /api/internal/admin/tenant/{tenantId}/test-docket-pdf-template | Test the given docket PDF template
 *AdminTemplateApi* | [**test_mail_template**](docs/AdminTemplateApi.md#test_mail_template) | **POST** /api/internal/admin/tenant/{tenantId}/test-mail-template | Test the given mail template
 *AdminTemplateApi* | [**test_signature_pdf_template**](docs/AdminTemplateApi.md#test_signature_pdf_template) | **POST** /api/internal/admin/tenant/{tenantId}/test-signature-pdf-template | Get the server default signature template
 *AdminTrashBinApi* | [**list_trash_bin_listable_folders**](docs/AdminTrashBinApi.md#list_trash_bin_listable_folders) | **GET** /api/internal/admin/tenant/{tenantId}/trash-bin | List folders in the trash-bin
 *AdminTypologyApi* | [**get_typology_hierarchy**](docs/AdminTypologyApi.md#get_typology_hierarchy) | **GET** /api/internal/admin/tenant/{tenantId}/typology | Get typology list, sorted by hierarchy.
-*AdminWorkflowDefinitionApi* | [**get_subtypes_referencing_workflow_definition_key**](docs/AdminWorkflowDefinitionApi.md#get_subtypes_referencing_workflow_definition_key) | **GET** /api/internal/admin/tenant/{tenantId}/workflowDefinitionByKey/{workflowDefinitionKey}/referencingSubtypes | Get subtypes referencing the given workflow definition key
 *CurrentUserApi* | [**update_current_user_password**](docs/CurrentUserApi.md#update_current_user_password) | **PUT** /api/internal/currentUser/password | Update user password
 *DeskApi* | [**get_associated_desks**](docs/DeskApi.md#get_associated_desks) | **GET** /api/internal/tenant/{tenantId}/desk/{deskId}/associatedDesks | Get the target desk&#39;s associated ones
 *FolderApi* | [**generate_document_signature_verification**](docs/FolderApi.md#generate_document_signature_verification) | **POST** /api/internal/tenant/{tenantId}/folder/{folderId}/signature-report | Get the document(s) signature validation report
 *FolderApi* | [**list_folders**](docs/FolderApi.md#list_folders) | **POST** /api/internal/tenant/{tenantId}/desk/{deskId}/search/{state} | Query folders
 *ServerInfoApi* | [**get_gdpr_information_details**](docs/ServerInfoApi.md#get_gdpr_information_details) | **GET** /api/internal/serverInfo/gdpr | Get the GDPR definition
 *ServerInfoApi* | [**get_password_policies**](docs/ServerInfoApi.md#get_password_policies) | **GET** /api/internal/serverInfo/passwordPolicies | Get Password rules for the server
 *TemplateApi* | [**test_signature_template**](docs/TemplateApi.md#test_signature_template) | **POST** /api/internal/tenant/{tenantId}/templates/{templateType}/example | Test the tenant signature template
@@ -124,22 +124,20 @@
 *WorkflowApi* | [**evaluate_workflow_selection_script**](docs/WorkflowApi.md#evaluate_workflow_selection_script) | **POST** /api/internal/tenant/{tenantId}/desk/{deskId}/evaluate-workflow-selection-script | Returns the evaluated workflow definition, using current parent desks, and given metadata on a possible selection script
 *WorkflowApi* | [**get_workflow_definition**](docs/WorkflowApi.md#get_workflow_definition) | **GET** /api/internal/tenant/{tenantId}/desk/{deskId}/workflow-definition/{workflowDefinitionKey} | Get a workflow definition with every information set
 
 
 ## Documentation For Models
 
  - [Action](docs/Action.md)
- - [CompositeId](docs/CompositeId.md)
  - [CreateFileStampRequest](docs/CreateFileStampRequest.md)
  - [CreateFolderRequest](docs/CreateFolderRequest.md)
  - [DeskRepresentation](docs/DeskRepresentation.md)
  - [DetachedSignature](docs/DetachedSignature.md)
  - [DocumentDto](docs/DocumentDto.md)
  - [ErrorResponse](docs/ErrorResponse.md)
- - [ExternalSignatureConfig](docs/ExternalSignatureConfig.md)
  - [ExternalSignatureConfigRepresentation](docs/ExternalSignatureConfigRepresentation.md)
  - [ExternalSignatureProvider](docs/ExternalSignatureProvider.md)
  - [ExternalState](docs/ExternalState.md)
  - [FolderDto](docs/FolderDto.md)
  - [FolderFilterDto](docs/FolderFilterDto.md)
  - [FolderListableDto](docs/FolderListableDto.md)
  - [FolderSortBy](docs/FolderSortBy.md)
@@ -154,15 +152,14 @@
  - [GdprEntity](docs/GdprEntity.md)
  - [GdprInformationDetailsDto](docs/GdprInformationDetailsDto.md)
  - [HierarchisedDeskRepresentation](docs/HierarchisedDeskRepresentation.md)
  - [LayerDto](docs/LayerDto.md)
  - [LayerRepresentation](docs/LayerRepresentation.md)
  - [MailTemplateTestRequest](docs/MailTemplateTestRequest.md)
  - [MediaType](docs/MediaType.md)
- - [Metadata](docs/Metadata.md)
  - [MetadataDto](docs/MetadataDto.md)
  - [MetadataType](docs/MetadataType.md)
  - [PageDeskRepresentation](docs/PageDeskRepresentation.md)
  - [PageFolderDto](docs/PageFolderDto.md)
  - [PageFolderListableDto](docs/PageFolderListableDto.md)
  - [PageHierarchisedDeskRepresentation](docs/PageHierarchisedDeskRepresentation.md)
  - [PageInfo](docs/PageInfo.md)
@@ -173,30 +170,26 @@
  - [PasswordPolicies](docs/PasswordPolicies.md)
  - [PdfSignaturePosition](docs/PdfSignaturePosition.md)
  - [PdfTemplateTestRequest](docs/PdfTemplateTestRequest.md)
  - [SealCertificateRepresentation](docs/SealCertificateRepresentation.md)
  - [SignatureFormat](docs/SignatureFormat.md)
  - [SignatureInfo](docs/SignatureInfo.md)
  - [SignaturePlacement](docs/SignaturePlacement.md)
- - [SignatureProof](docs/SignatureProof.md)
  - [SignatureProtocol](docs/SignatureProtocol.md)
  - [SortObject](docs/SortObject.md)
  - [StampDto](docs/StampDto.md)
  - [StampTextColor](docs/StampTextColor.md)
  - [StampType](docs/StampType.md)
  - [State](docs/State.md)
  - [StepDefinitionDto](docs/StepDefinitionDto.md)
  - [StepDefinitionParallelType](docs/StepDefinitionParallelType.md)
  - [StepDefinitionType](docs/StepDefinitionType.md)
- - [Subtype](docs/Subtype.md)
  - [SubtypeDto](docs/SubtypeDto.md)
- - [SubtypeLayer](docs/SubtypeLayer.md)
  - [SubtypeLayerAssociation](docs/SubtypeLayerAssociation.md)
  - [SubtypeLayerDto](docs/SubtypeLayerDto.md)
- - [SubtypeMetadata](docs/SubtypeMetadata.md)
  - [SubtypeMetadataDto](docs/SubtypeMetadataDto.md)
  - [SubtypeRepresentation](docs/SubtypeRepresentation.md)
  - [Task](docs/Task.md)
  - [TemplateType](docs/TemplateType.md)
  - [TenantRepresentation](docs/TenantRepresentation.md)
  - [TestSignatureTemplateRequest](docs/TestSignatureTemplateRequest.md)
  - [TypeDto](docs/TypeDto.md)
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/__init__.py` & `iparapheur-internal-1.12.3/iparapheur_internal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,24 @@
     Contact: iparapheur@libriciel.coop
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.11.5"
+__version__ = "1.12.3"
 
 # import apis into sdk package
 from iparapheur_internal.api.admin_advanced_config_api import AdminAdvancedConfigApi
 from iparapheur_internal.api.admin_desk_api import AdminDeskApi
 from iparapheur_internal.api.admin_layer_api import AdminLayerApi
 from iparapheur_internal.api.admin_seal_certificate_api import AdminSealCertificateApi
 from iparapheur_internal.api.admin_template_api import AdminTemplateApi
 from iparapheur_internal.api.admin_trash_bin_api import AdminTrashBinApi
 from iparapheur_internal.api.admin_typology_api import AdminTypologyApi
-from iparapheur_internal.api.admin_workflow_definition_api import AdminWorkflowDefinitionApi
 from iparapheur_internal.api.current_user_api import CurrentUserApi
 from iparapheur_internal.api.desk_api import DeskApi
 from iparapheur_internal.api.folder_api import FolderApi
 from iparapheur_internal.api.server_info_api import ServerInfoApi
 from iparapheur_internal.api.template_api import TemplateApi
 from iparapheur_internal.api.typology_api import TypologyApi
 from iparapheur_internal.api.workflow_api import WorkflowApi
@@ -43,22 +42,20 @@
 from iparapheur_internal.exceptions import ApiValueError
 from iparapheur_internal.exceptions import ApiKeyError
 from iparapheur_internal.exceptions import ApiAttributeError
 from iparapheur_internal.exceptions import ApiException
 
 # import models into sdk package
 from iparapheur_internal.models.action import Action
-from iparapheur_internal.models.composite_id import CompositeId
 from iparapheur_internal.models.create_file_stamp_request import CreateFileStampRequest
 from iparapheur_internal.models.create_folder_request import CreateFolderRequest
 from iparapheur_internal.models.desk_representation import DeskRepresentation
 from iparapheur_internal.models.detached_signature import DetachedSignature
 from iparapheur_internal.models.document_dto import DocumentDto
 from iparapheur_internal.models.error_response import ErrorResponse
-from iparapheur_internal.models.external_signature_config import ExternalSignatureConfig
 from iparapheur_internal.models.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_internal.models.external_signature_provider import ExternalSignatureProvider
 from iparapheur_internal.models.external_state import ExternalState
 from iparapheur_internal.models.folder_dto import FolderDto
 from iparapheur_internal.models.folder_filter_dto import FolderFilterDto
 from iparapheur_internal.models.folder_listable_dto import FolderListableDto
 from iparapheur_internal.models.folder_sort_by import FolderSortBy
@@ -73,15 +70,14 @@
 from iparapheur_internal.models.gdpr_entity import GdprEntity
 from iparapheur_internal.models.gdpr_information_details_dto import GdprInformationDetailsDto
 from iparapheur_internal.models.hierarchised_desk_representation import HierarchisedDeskRepresentation
 from iparapheur_internal.models.layer_dto import LayerDto
 from iparapheur_internal.models.layer_representation import LayerRepresentation
 from iparapheur_internal.models.mail_template_test_request import MailTemplateTestRequest
 from iparapheur_internal.models.media_type import MediaType
-from iparapheur_internal.models.metadata import Metadata
 from iparapheur_internal.models.metadata_dto import MetadataDto
 from iparapheur_internal.models.metadata_type import MetadataType
 from iparapheur_internal.models.page_desk_representation import PageDeskRepresentation
 from iparapheur_internal.models.page_folder_dto import PageFolderDto
 from iparapheur_internal.models.page_folder_listable_dto import PageFolderListableDto
 from iparapheur_internal.models.page_hierarchised_desk_representation import PageHierarchisedDeskRepresentation
 from iparapheur_internal.models.page_info import PageInfo
@@ -92,30 +88,26 @@
 from iparapheur_internal.models.password_policies import PasswordPolicies
 from iparapheur_internal.models.pdf_signature_position import PdfSignaturePosition
 from iparapheur_internal.models.pdf_template_test_request import PdfTemplateTestRequest
 from iparapheur_internal.models.seal_certificate_representation import SealCertificateRepresentation
 from iparapheur_internal.models.signature_format import SignatureFormat
 from iparapheur_internal.models.signature_info import SignatureInfo
 from iparapheur_internal.models.signature_placement import SignaturePlacement
-from iparapheur_internal.models.signature_proof import SignatureProof
 from iparapheur_internal.models.signature_protocol import SignatureProtocol
 from iparapheur_internal.models.sort_object import SortObject
 from iparapheur_internal.models.stamp_dto import StampDto
 from iparapheur_internal.models.stamp_text_color import StampTextColor
 from iparapheur_internal.models.stamp_type import StampType
 from iparapheur_internal.models.state import State
 from iparapheur_internal.models.step_definition_dto import StepDefinitionDto
 from iparapheur_internal.models.step_definition_parallel_type import StepDefinitionParallelType
 from iparapheur_internal.models.step_definition_type import StepDefinitionType
-from iparapheur_internal.models.subtype import Subtype
 from iparapheur_internal.models.subtype_dto import SubtypeDto
-from iparapheur_internal.models.subtype_layer import SubtypeLayer
 from iparapheur_internal.models.subtype_layer_association import SubtypeLayerAssociation
 from iparapheur_internal.models.subtype_layer_dto import SubtypeLayerDto
-from iparapheur_internal.models.subtype_metadata import SubtypeMetadata
 from iparapheur_internal.models.subtype_metadata_dto import SubtypeMetadataDto
 from iparapheur_internal.models.subtype_representation import SubtypeRepresentation
 from iparapheur_internal.models.task import Task
 from iparapheur_internal.models.template_type import TemplateType
 from iparapheur_internal.models.tenant_representation import TenantRepresentation
 from iparapheur_internal.models.test_signature_template_request import TestSignatureTemplateRequest
 from iparapheur_internal.models.type_dto import TypeDto
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/__init__.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from iparapheur_internal.api.admin_advanced_config_api import AdminAdvancedConfigApi
 from iparapheur_internal.api.admin_desk_api import AdminDeskApi
 from iparapheur_internal.api.admin_layer_api import AdminLayerApi
 from iparapheur_internal.api.admin_seal_certificate_api import AdminSealCertificateApi
 from iparapheur_internal.api.admin_template_api import AdminTemplateApi
 from iparapheur_internal.api.admin_trash_bin_api import AdminTrashBinApi
 from iparapheur_internal.api.admin_typology_api import AdminTypologyApi
-from iparapheur_internal.api.admin_workflow_definition_api import AdminWorkflowDefinitionApi
 from iparapheur_internal.api.current_user_api import CurrentUserApi
 from iparapheur_internal.api.desk_api import DeskApi
 from iparapheur_internal.api.folder_api import FolderApi
 from iparapheur_internal.api.server_info_api import ServerInfoApi
 from iparapheur_internal.api.template_api import TemplateApi
 from iparapheur_internal.api.typology_api import TypologyApi
 from iparapheur_internal.api.workflow_api import WorkflowApi
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_advanced_config_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_advanced_config_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,263 +35,14 @@
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def delete_chorus_configuration(
-        self,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> None:
-        """Delete Chorus Pro configuration
-
-
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._delete_chorus_configuration_serialize(
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '200': None,
-            '404': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        ).data
-
-
-    @validate_call
-    def delete_chorus_configuration_with_http_info(
-        self,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[None]:
-        """Delete Chorus Pro configuration
-
-
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._delete_chorus_configuration_serialize(
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '200': None,
-            '404': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        response_data.read()
-        return self.api_client.response_deserialize(
-            response_data=response_data,
-            response_types_map=_response_types_map,
-        )
-
-
-    @validate_call
-    def delete_chorus_configuration_without_preload_content(
-        self,
-        _request_timeout: Union[
-            None,
-            Annotated[StrictFloat, Field(gt=0)],
-            Tuple[
-                Annotated[StrictFloat, Field(gt=0)],
-                Annotated[StrictFloat, Field(gt=0)]
-            ]
-        ] = None,
-        _request_auth: Optional[Dict[StrictStr, Any]] = None,
-        _content_type: Optional[StrictStr] = None,
-        _headers: Optional[Dict[StrictStr, Any]] = None,
-        _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> RESTResponseType:
-        """Delete Chorus Pro configuration
-
-
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :type _request_timeout: int, tuple(int, int), optional
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the
-                              authentication in the spec for a single request.
-        :type _request_auth: dict, optional
-        :param _content_type: force content-type for the request.
-        :type _content_type: str, Optional
-        :param _headers: set to override the headers for a single
-                         request; this effectively ignores the headers
-                         in the spec for a single request.
-        :type _headers: dict, optional
-        :param _host_index: set to override the host_index for a single
-                            request; this effectively ignores the host_index
-                            in the spec for a single request.
-        :type _host_index: int, optional
-        :return: Returns the result object.
-        """ # noqa: E501
-
-        _param = self._delete_chorus_configuration_serialize(
-            _request_auth=_request_auth,
-            _content_type=_content_type,
-            _headers=_headers,
-            _host_index=_host_index
-        )
-
-        _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '200': None,
-            '404': "ErrorResponse",
-        }
-        response_data = self.api_client.call_api(
-            *_param,
-            _request_timeout=_request_timeout
-        )
-        return response_data.response
-
-
-    def _delete_chorus_configuration_serialize(
-        self,
-        _request_auth,
-        _content_type,
-        _headers,
-        _host_index,
-    ) -> RequestSerialized:
-
-        _host = None
-
-        _collection_formats: Dict[str, str] = {
-        }
-
-        _path_params: Dict[str, str] = {}
-        _query_params: List[Tuple[str, str]] = []
-        _header_params: Dict[str, Optional[str]] = _headers or {}
-        _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
-        _body_params: Optional[bytes] = None
-
-        # process the path parameters
-        # process the query parameters
-        # process the header parameters
-        # process the form parameters
-        # process the body parameter
-
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            [
-                'application/json'
-            ]
-        )
-
-
-        # authentication setting
-        _auth_settings: List[str] = [
-            'spring_oauth'
-        ]
-
-        return self.api_client.param_serialize(
-            method='DELETE',
-            resource_path='/api/internal/admin/config/chorus-configuration',
-            path_params=_path_params,
-            query_params=_query_params,
-            header_params=_header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            auth_settings=_auth_settings,
-            collection_formats=_collection_formats,
-            _host=_host,
-            _request_auth=_request_auth
-        )
-
-
-
-
-    @validate_call
     def get_chorus_configuration(
         self,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
@@ -332,17 +83,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "ValidationServiceConfigurationDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -397,17 +148,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "ValidationServiceConfigurationDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -462,17 +213,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "ValidationServiceConfigurationDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -585,18 +336,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -654,18 +405,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -723,18 +474,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -862,18 +613,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -931,18 +682,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -1000,18 +751,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': None,
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_desk_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_desk_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -113,18 +113,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "PageHierarchisedDeskRepresentation",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageHierarchisedDeskRepresentation",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -206,18 +206,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "PageHierarchisedDeskRepresentation",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageHierarchisedDeskRepresentation",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -299,18 +299,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "PageHierarchisedDeskRepresentation",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageHierarchisedDeskRepresentation",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_layer_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_layer_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,18 +103,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '201': "StampDto",
             '507': "ErrorResponse",
+            '201': "StampDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -185,18 +185,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '201': "StampDto",
             '507': "ErrorResponse",
+            '201': "StampDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -267,18 +267,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '201': "StampDto",
             '507': "ErrorResponse",
+            '201': "StampDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -420,19 +420,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '507': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
-            '507': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -495,19 +495,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '507': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
-            '507': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -570,19 +570,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '507': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
-            '507': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -722,17 +722,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
             '204': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -799,17 +799,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
             '204': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -876,17 +876,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
             '204': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1012,17 +1012,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
             '204': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1085,17 +1085,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
             '204': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1158,17 +1158,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
             '204': None,
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1291,17 +1291,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "LayerDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1364,17 +1364,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "LayerDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1437,17 +1437,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "LayerDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1570,17 +1570,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1643,17 +1643,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1716,17 +1716,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -1764,16 +1764,16 @@
         if layer_dto is not None:
             _body_params = layer_dto
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
@@ -1872,18 +1872,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "PageLayerRepresentation",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageLayerRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -1955,18 +1955,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "PageLayerRepresentation",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageLayerRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -2038,18 +2038,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "PageLayerRepresentation",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "PageLayerRepresentation",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -2189,18 +2189,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
             '200': "LayerDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -2268,18 +2268,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
             '200': "LayerDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
@@ -2347,18 +2347,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '201': "LayerDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '201': "LayerDto",
             '404': "ErrorResponse",
             '200': "LayerDto",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_seal_certificate_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_seal_certificate_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -166,17 +166,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -239,17 +239,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -287,16 +287,16 @@
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/octet-stream'
+                'application/octet-stream', 
+                'application/json'
             ]
         )
 
 
         # authentication setting
         _auth_settings: List[str] = [
             'spring_oauth'
@@ -385,17 +385,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageSubtypeRepresentation",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -470,17 +470,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageSubtypeRepresentation",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -555,17 +555,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageSubtypeRepresentation",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_template_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_template_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,18 +93,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
-            '200': None,
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -166,18 +166,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
-            '200': None,
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -239,18 +239,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
-            '200': None,
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -287,16 +287,16 @@
         if mail_template_test_request is not None:
             _body_params = mail_template_test_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
@@ -386,17 +386,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -458,17 +458,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -530,17 +530,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -675,18 +675,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
-            '200': None,
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -748,18 +748,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
-            '200': None,
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -821,18 +821,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
             '500': "ErrorResponse",
-            '200': None,
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -869,16 +869,16 @@
         if pdf_template_test_request is not None:
             _body_params = pdf_template_test_request
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
-                'application/json', 
-                'application/pdf'
+                'application/pdf', 
+                'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_trash_bin_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_trash_bin_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,17 +101,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageFolderListableDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -182,17 +182,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageFolderListableDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -263,17 +263,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageFolderListableDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_typology_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/admin_typology_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -114,19 +114,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '400': "ErrorResponse",
             '200': "PageTypologyRepresentation",
+            '401': "ErrorResponse",
             '406': "ErrorResponse",
+            '403': "ErrorResponse",
+            '400': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -210,19 +210,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '400': "ErrorResponse",
             '200': "PageTypologyRepresentation",
+            '401': "ErrorResponse",
             '406': "ErrorResponse",
+            '403': "ErrorResponse",
+            '400': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -306,19 +306,19 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
-            '400': "ErrorResponse",
             '200': "PageTypologyRepresentation",
+            '401': "ErrorResponse",
             '406': "ErrorResponse",
+            '403': "ErrorResponse",
+            '400': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/admin_workflow_definition_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/current_user_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,61 +13,56 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictStr
-from typing_extensions import Annotated
-from iparapheur_internal.models.subtype import Subtype
+from iparapheur_internal.models.user_dto import UserDto
 
 from iparapheur_internal.api_client import ApiClient, RequestSerialized
 from iparapheur_internal.api_response import ApiResponse
 from iparapheur_internal.rest import RESTResponseType
 
 
-class AdminWorkflowDefinitionApi:
+class CurrentUserApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def get_subtypes_referencing_workflow_definition_key(
+    def update_current_user_password(
         self,
-        tenant_id: Annotated[StrictStr, Field(description="Tenant id")],
-        workflow_definition_key: StrictStr,
+        user_dto: UserDto,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> List[Subtype]:
-        """Get subtypes referencing the given workflow definition key
+    ) -> None:
+        """(Deprecated) Update user password
 
 
-        :param tenant_id: Tenant id (required)
-        :type tenant_id: str
-        :param workflow_definition_key: (required)
-        :type workflow_definition_key: str
+        :param user_dto: (required)
+        :type user_dto: UserDto
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -81,66 +76,63 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/internal/currentUser/password is deprecated.", DeprecationWarning)
 
-        _param = self._get_subtypes_referencing_workflow_definition_key_serialize(
-            tenant_id=tenant_id,
-            workflow_definition_key=workflow_definition_key,
+        _param = self._update_current_user_password_serialize(
+            user_dto=user_dto,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
-            '200': "List[Subtype]",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def get_subtypes_referencing_workflow_definition_key_with_http_info(
+    def update_current_user_password_with_http_info(
         self,
-        tenant_id: Annotated[StrictStr, Field(description="Tenant id")],
-        workflow_definition_key: StrictStr,
+        user_dto: UserDto,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[List[Subtype]]:
-        """Get subtypes referencing the given workflow definition key
+    ) -> ApiResponse[None]:
+        """(Deprecated) Update user password
 
 
-        :param tenant_id: Tenant id (required)
-        :type tenant_id: str
-        :param workflow_definition_key: (required)
-        :type workflow_definition_key: str
+        :param user_dto: (required)
+        :type user_dto: UserDto
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -154,66 +146,63 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/internal/currentUser/password is deprecated.", DeprecationWarning)
 
-        _param = self._get_subtypes_referencing_workflow_definition_key_serialize(
-            tenant_id=tenant_id,
-            workflow_definition_key=workflow_definition_key,
+        _param = self._update_current_user_password_serialize(
+            user_dto=user_dto,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
-            '200': "List[Subtype]",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def get_subtypes_referencing_workflow_definition_key_without_preload_content(
+    def update_current_user_password_without_preload_content(
         self,
-        tenant_id: Annotated[StrictStr, Field(description="Tenant id")],
-        workflow_definition_key: StrictStr,
+        user_dto: UserDto,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """Get subtypes referencing the given workflow definition key
+        """(Deprecated) Update user password
 
 
-        :param tenant_id: Tenant id (required)
-        :type tenant_id: str
-        :param workflow_definition_key: (required)
-        :type workflow_definition_key: str
+        :param user_dto: (required)
+        :type user_dto: UserDto
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -227,41 +216,40 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
+        warnings.warn("PUT /api/internal/currentUser/password is deprecated.", DeprecationWarning)
 
-        _param = self._get_subtypes_referencing_workflow_definition_key_serialize(
-            tenant_id=tenant_id,
-            workflow_definition_key=workflow_definition_key,
+        _param = self._update_current_user_password_serialize(
+            user_dto=user_dto,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': None,
             '401': "ErrorResponse",
-            '200': "List[Subtype]",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _get_subtypes_referencing_workflow_definition_key_serialize(
+    def _update_current_user_password_serialize(
         self,
-        tenant_id,
-        workflow_definition_key,
+        user_dto,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -273,40 +261,51 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
-        if tenant_id is not None:
-            _path_params['tenantId'] = tenant_id
-        if workflow_definition_key is not None:
-            _path_params['workflowDefinitionKey'] = workflow_definition_key
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
+        if user_dto is not None:
+            _body_params = user_dto
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
                 'application/json'
             ]
         )
 
+        # set the HTTP header `Content-Type`
+        if _content_type:
+            _header_params['Content-Type'] = _content_type
+        else:
+            _default_content_type = (
+                self.api_client.select_header_content_type(
+                    [
+                        'application/json'
+                    ]
+                )
+            )
+            if _default_content_type is not None:
+                _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'spring_oauth'
         ]
 
         return self.api_client.param_serialize(
-            method='GET',
-            resource_path='/api/internal/admin/tenant/{tenantId}/workflowDefinitionByKey/{workflowDefinitionKey}/referencingSubtypes',
+            method='PUT',
+            resource_path='/api/internal/currentUser/password',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/current_user_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/template_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,56 +13,68 @@
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
-from iparapheur_internal.models.user_dto import UserDto
+from pydantic import Field, StrictBool, StrictBytes, StrictStr
+from typing import Optional, Union
+from typing_extensions import Annotated
+from iparapheur_internal.models.template_type import TemplateType
 
 from iparapheur_internal.api_client import ApiClient, RequestSerialized
 from iparapheur_internal.api_response import ApiResponse
 from iparapheur_internal.rest import RESTResponseType
 
 
-class CurrentUserApi:
+class TemplateApi:
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
 
     @validate_call
-    def update_current_user_password(
+    def test_signature_template(
         self,
-        user_dto: UserDto,
+        tenant_id: Annotated[StrictStr, Field(description="Tenant id")],
+        template_type: TemplateType,
+        use_small_doc: StrictBool,
+        signature_image: Optional[Union[StrictBytes, StrictStr]] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> None:
-        """(Deprecated) Update user password
+        """Test the tenant signature template
 
 
-        :param user_dto: (required)
-        :type user_dto: UserDto
+        :param tenant_id: Tenant id (required)
+        :type tenant_id: str
+        :param template_type: (required)
+        :type template_type: TemplateType
+        :param use_small_doc: (required)
+        :type use_small_doc: bool
+        :param signature_image:
+        :type signature_image: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -76,63 +88,73 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
-        warnings.warn("PUT /api/internal/currentUser/password is deprecated.", DeprecationWarning)
 
-        _param = self._update_current_user_password_serialize(
-            user_dto=user_dto,
+        _param = self._test_signature_template_serialize(
+            tenant_id=tenant_id,
+            template_type=template_type,
+            use_small_doc=use_small_doc,
+            signature_image=signature_image,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
-            '404': "ErrorResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         ).data
 
 
     @validate_call
-    def update_current_user_password_with_http_info(
+    def test_signature_template_with_http_info(
         self,
-        user_dto: UserDto,
+        tenant_id: Annotated[StrictStr, Field(description="Tenant id")],
+        template_type: TemplateType,
+        use_small_doc: StrictBool,
+        signature_image: Optional[Union[StrictBytes, StrictStr]] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[None]:
-        """(Deprecated) Update user password
+        """Test the tenant signature template
 
 
-        :param user_dto: (required)
-        :type user_dto: UserDto
+        :param tenant_id: Tenant id (required)
+        :type tenant_id: str
+        :param template_type: (required)
+        :type template_type: TemplateType
+        :param use_small_doc: (required)
+        :type use_small_doc: bool
+        :param signature_image:
+        :type signature_image: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -146,63 +168,73 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
-        warnings.warn("PUT /api/internal/currentUser/password is deprecated.", DeprecationWarning)
 
-        _param = self._update_current_user_password_serialize(
-            user_dto=user_dto,
+        _param = self._test_signature_template_serialize(
+            tenant_id=tenant_id,
+            template_type=template_type,
+            use_small_doc=use_small_doc,
+            signature_image=signature_image,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
-            '404': "ErrorResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
             response_data=response_data,
             response_types_map=_response_types_map,
         )
 
 
     @validate_call
-    def update_current_user_password_without_preload_content(
+    def test_signature_template_without_preload_content(
         self,
-        user_dto: UserDto,
+        tenant_id: Annotated[StrictStr, Field(description="Tenant id")],
+        template_type: TemplateType,
+        use_small_doc: StrictBool,
+        signature_image: Optional[Union[StrictBytes, StrictStr]] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
-        """(Deprecated) Update user password
+        """Test the tenant signature template
 
 
-        :param user_dto: (required)
-        :type user_dto: UserDto
+        :param tenant_id: Tenant id (required)
+        :type tenant_id: str
+        :param template_type: (required)
+        :type template_type: TemplateType
+        :param use_small_doc: (required)
+        :type use_small_doc: bool
+        :param signature_image:
+        :type signature_image: bytearray
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -216,40 +248,44 @@
         :type _headers: dict, optional
         :param _host_index: set to override the host_index for a single
                             request; this effectively ignores the host_index
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
-        warnings.warn("PUT /api/internal/currentUser/password is deprecated.", DeprecationWarning)
 
-        _param = self._update_current_user_password_serialize(
-            user_dto=user_dto,
+        _param = self._test_signature_template_serialize(
+            tenant_id=tenant_id,
+            template_type=template_type,
+            use_small_doc=use_small_doc,
+            signature_image=signature_image,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': None,
-            '404': "ErrorResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
 
-    def _update_current_user_password_serialize(
+    def _test_signature_template_serialize(
         self,
-        user_dto,
+        tenant_id,
+        template_type,
+        use_small_doc,
+        signature_image,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> RequestSerialized:
 
         _host = None
@@ -261,51 +297,60 @@
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
+        if tenant_id is not None:
+            _path_params['tenantId'] = tenant_id
+        if template_type is not None:
+            _path_params['templateType'] = template_type.value
         # process the query parameters
+        if use_small_doc is not None:
+            
+            _query_params.append(('useSmallDoc', use_small_doc))
+            
         # process the header parameters
         # process the form parameters
+        if signature_image is not None:
+            _files['signatureImage'] = signature_image
         # process the body parameter
-        if user_dto is not None:
-            _body_params = user_dto
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             [
+                'application/pdf', 
                 'application/json'
             ]
         )
 
         # set the HTTP header `Content-Type`
         if _content_type:
             _header_params['Content-Type'] = _content_type
         else:
             _default_content_type = (
                 self.api_client.select_header_content_type(
                     [
-                        'application/json'
+                        'multipart/form-data'
                     ]
                 )
             )
             if _default_content_type is not None:
                 _header_params['Content-Type'] = _default_content_type
 
         # authentication setting
         _auth_settings: List[str] = [
             'spring_oauth'
         ]
 
         return self.api_client.param_serialize(
-            method='PUT',
-            resource_path='/api/internal/currentUser/password',
+            method='POST',
+            resource_path='/api/internal/tenant/{tenantId}/templates/{templateType}/example',
             path_params=_path_params,
             query_params=_query_params,
             header_params=_header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             auth_settings=_auth_settings,
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/desk_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/desk_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageDeskRepresentation",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -198,17 +198,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageDeskRepresentation",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -287,17 +287,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageDeskRepresentation",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/folder_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/folder_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '201': "ErrorResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -169,17 +169,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '201': "ErrorResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -242,17 +242,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '201': "ErrorResponse",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -395,17 +395,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageFolderDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -488,17 +488,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageFolderDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -581,17 +581,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PageFolderDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/server_info_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/server_info_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -83,17 +83,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "GdprInformationDetailsDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -147,17 +147,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "GdprInformationDetailsDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -211,17 +211,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "GdprInformationDetailsDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
 
@@ -329,17 +329,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PasswordPolicies",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -393,17 +393,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PasswordPolicies",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
         return self.api_client.response_deserialize(
@@ -457,17 +457,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "PasswordPolicies",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/typology_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/typology_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -97,16 +97,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "SubtypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -173,16 +173,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "SubtypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -249,16 +249,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "SubtypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -384,16 +384,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "TypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -456,16 +456,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "TypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -528,16 +528,16 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '401': "ErrorResponse",
             '200': "TypeDto",
+            '401': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api/workflow_api.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api/workflow_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -97,18 +97,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "WorkflowDefinitionDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "WorkflowDefinitionDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -175,18 +175,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "WorkflowDefinitionDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "WorkflowDefinitionDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -253,18 +253,18 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
+            '200': "WorkflowDefinitionDto",
             '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '400': "ErrorResponse",
-            '200': "WorkflowDefinitionDto",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
@@ -407,17 +407,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "WorkflowDefinitionDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -484,17 +484,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "WorkflowDefinitionDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         response_data.read()
@@ -561,17 +561,17 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '403': "ErrorResponse",
-            '401': "ErrorResponse",
             '200': "WorkflowDefinitionDto",
+            '401': "ErrorResponse",
+            '403': "ErrorResponse",
             '404': "ErrorResponse",
         }
         response_data = self.api_client.call_api(
             *_param,
             _request_timeout=_request_timeout
         )
         return response_data.response
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api_client.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.11.5/python'
+        self.user_agent = 'OpenAPI-Generator/1.12.3/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/api_response.py` & `iparapheur-internal-1.12.3/iparapheur_internal/api_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/configuration.py` & `iparapheur-internal-1.12.3/iparapheur_internal/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,15 +375,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.11.5".\
+               "SDK Package Version: 1.12.3".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/exceptions.py` & `iparapheur-internal-1.12.3/iparapheur_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/__init__.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 # import models into model package
 from iparapheur_internal.models.action import Action
-from iparapheur_internal.models.composite_id import CompositeId
 from iparapheur_internal.models.create_file_stamp_request import CreateFileStampRequest
 from iparapheur_internal.models.create_folder_request import CreateFolderRequest
 from iparapheur_internal.models.desk_representation import DeskRepresentation
 from iparapheur_internal.models.detached_signature import DetachedSignature
 from iparapheur_internal.models.document_dto import DocumentDto
 from iparapheur_internal.models.error_response import ErrorResponse
-from iparapheur_internal.models.external_signature_config import ExternalSignatureConfig
 from iparapheur_internal.models.external_signature_config_representation import ExternalSignatureConfigRepresentation
 from iparapheur_internal.models.external_signature_provider import ExternalSignatureProvider
 from iparapheur_internal.models.external_state import ExternalState
 from iparapheur_internal.models.folder_dto import FolderDto
 from iparapheur_internal.models.folder_filter_dto import FolderFilterDto
 from iparapheur_internal.models.folder_listable_dto import FolderListableDto
 from iparapheur_internal.models.folder_sort_by import FolderSortBy
@@ -42,15 +40,14 @@
 from iparapheur_internal.models.gdpr_entity import GdprEntity
 from iparapheur_internal.models.gdpr_information_details_dto import GdprInformationDetailsDto
 from iparapheur_internal.models.hierarchised_desk_representation import HierarchisedDeskRepresentation
 from iparapheur_internal.models.layer_dto import LayerDto
 from iparapheur_internal.models.layer_representation import LayerRepresentation
 from iparapheur_internal.models.mail_template_test_request import MailTemplateTestRequest
 from iparapheur_internal.models.media_type import MediaType
-from iparapheur_internal.models.metadata import Metadata
 from iparapheur_internal.models.metadata_dto import MetadataDto
 from iparapheur_internal.models.metadata_type import MetadataType
 from iparapheur_internal.models.page_desk_representation import PageDeskRepresentation
 from iparapheur_internal.models.page_folder_dto import PageFolderDto
 from iparapheur_internal.models.page_folder_listable_dto import PageFolderListableDto
 from iparapheur_internal.models.page_hierarchised_desk_representation import PageHierarchisedDeskRepresentation
 from iparapheur_internal.models.page_info import PageInfo
@@ -61,30 +58,26 @@
 from iparapheur_internal.models.password_policies import PasswordPolicies
 from iparapheur_internal.models.pdf_signature_position import PdfSignaturePosition
 from iparapheur_internal.models.pdf_template_test_request import PdfTemplateTestRequest
 from iparapheur_internal.models.seal_certificate_representation import SealCertificateRepresentation
 from iparapheur_internal.models.signature_format import SignatureFormat
 from iparapheur_internal.models.signature_info import SignatureInfo
 from iparapheur_internal.models.signature_placement import SignaturePlacement
-from iparapheur_internal.models.signature_proof import SignatureProof
 from iparapheur_internal.models.signature_protocol import SignatureProtocol
 from iparapheur_internal.models.sort_object import SortObject
 from iparapheur_internal.models.stamp_dto import StampDto
 from iparapheur_internal.models.stamp_text_color import StampTextColor
 from iparapheur_internal.models.stamp_type import StampType
 from iparapheur_internal.models.state import State
 from iparapheur_internal.models.step_definition_dto import StepDefinitionDto
 from iparapheur_internal.models.step_definition_parallel_type import StepDefinitionParallelType
 from iparapheur_internal.models.step_definition_type import StepDefinitionType
-from iparapheur_internal.models.subtype import Subtype
 from iparapheur_internal.models.subtype_dto import SubtypeDto
-from iparapheur_internal.models.subtype_layer import SubtypeLayer
 from iparapheur_internal.models.subtype_layer_association import SubtypeLayerAssociation
 from iparapheur_internal.models.subtype_layer_dto import SubtypeLayerDto
-from iparapheur_internal.models.subtype_metadata import SubtypeMetadata
 from iparapheur_internal.models.subtype_metadata_dto import SubtypeMetadataDto
 from iparapheur_internal.models.subtype_representation import SubtypeRepresentation
 from iparapheur_internal.models.task import Task
 from iparapheur_internal.models.template_type import TemplateType
 from iparapheur_internal.models.tenant_representation import TenantRepresentation
 from iparapheur_internal.models.test_signature_template_request import TestSignatureTemplateRequest
 from iparapheur_internal.models.type_dto import TypeDto
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/action.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/action.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/composite_id.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/mail_template_test_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CompositeId(BaseModel):
+class MailTemplateTestRequest(BaseModel):
     """
-    CompositeId
+    body
     """ # noqa: E501
-    layer_id: Optional[StrictStr] = Field(default=None, alias="layerId")
-    __properties: ClassVar[List[str]] = ["layerId"]
+    template: Optional[StrictStr] = None
+    mail: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["template", "mail"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -44,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CompositeId from a JSON string"""
+        """Create an instance of MailTemplateTestRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,20 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CompositeId from a dict"""
+        """Create an instance of MailTemplateTestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "layerId": obj.get("layerId")
+            "template": obj.get("template"),
+            "mail": obj.get("mail")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/create_file_stamp_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/create_file_stamp_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/create_folder_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/create_folder_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from datetime import datetime
 from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from iparapheur_internal.models.desk_representation import DeskRepresentation
 from iparapheur_internal.models.document_dto import DocumentDto
 from iparapheur_internal.models.folder_visibility import FolderVisibility
-from iparapheur_internal.models.signature_proof import SignatureProof
 from iparapheur_internal.models.subtype_dto import SubtypeDto
 from iparapheur_internal.models.task import Task
 from iparapheur_internal.models.type_dto import TypeDto
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreateFolderRequest(BaseModel):
@@ -47,21 +46,20 @@
     final_desk: Optional[DeskRepresentation] = Field(default=None, alias="finalDesk")
     is_read_by_current_user: Optional[StrictBool] = Field(default=None, alias="isReadByCurrentUser")
     legacy_id: Optional[StrictStr] = Field(default=None, alias="legacyId")
     type_id: Optional[StrictStr] = Field(default=None, alias="typeId")
     subtype_id: Optional[StrictStr] = Field(default=None, alias="subtypeId")
     step_list: Optional[List[Task]] = Field(default=None, alias="stepList")
     document_list: Optional[List[DocumentDto]] = Field(default=None, alias="documentList")
-    signature_proof_list: Optional[List[SignatureProof]] = Field(default=None, alias="signatureProofList")
     read_by_user_ids: Optional[List[StrictStr]] = Field(default=None, alias="readByUserIds")
     variable_desks_ids: Optional[Dict[str, StrictStr]] = Field(default=None, alias="variableDesksIds")
     detached_signatures_mapping: Optional[Dict[str, List[StrictStr]]] = Field(default=None, alias="detachedSignaturesMapping")
     visibility: Optional[FolderVisibility] = None
     read_by_current_user: Optional[StrictBool] = Field(default=None, alias="readByCurrentUser")
-    __properties: ClassVar[List[str]] = ["id", "name", "dueDate", "metadata", "draftCreationDate", "type", "subtype", "originDesk", "finalDesk", "isReadByCurrentUser", "legacyId", "typeId", "subtypeId", "stepList", "documentList", "signatureProofList", "readByUserIds", "variableDesksIds", "detachedSignaturesMapping", "visibility", "readByCurrentUser"]
+    __properties: ClassVar[List[str]] = ["id", "name", "dueDate", "metadata", "draftCreationDate", "type", "subtype", "originDesk", "finalDesk", "isReadByCurrentUser", "legacyId", "typeId", "subtypeId", "stepList", "documentList", "readByUserIds", "variableDesksIds", "detachedSignaturesMapping", "visibility", "readByCurrentUser"]
 
     @field_validator('name')
     def name_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[^\r\n ]*$", value):
             raise ValueError(r"must validate the regular expression /^[^\r\n ]*$/")
         return value
@@ -98,23 +96,21 @@
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "id",
             "draft_creation_date",
             "is_read_by_current_user",
             "step_list",
             "document_list",
-            "signature_proof_list",
             "read_by_user_ids",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
@@ -141,21 +137,14 @@
         # override the default output from pydantic by calling `to_dict()` of each item in document_list (list)
         _items = []
         if self.document_list:
             for _item in self.document_list:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['documentList'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in signature_proof_list (list)
-        _items = []
-        if self.signature_proof_list:
-            for _item in self.signature_proof_list:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['signatureProofList'] = _items
         # set to None if due_date (nullable) is None
         # and model_fields_set contains the field
         if self.due_date is None and "due_date" in self.model_fields_set:
             _dict['dueDate'] = None
 
         # set to None if origin_desk (nullable) is None
         # and model_fields_set contains the field
@@ -190,15 +179,14 @@
             "finalDesk": DeskRepresentation.from_dict(obj["finalDesk"]) if obj.get("finalDesk") is not None else None,
             "isReadByCurrentUser": obj.get("isReadByCurrentUser"),
             "legacyId": obj.get("legacyId"),
             "typeId": obj.get("typeId"),
             "subtypeId": obj.get("subtypeId"),
             "stepList": [Task.from_dict(_item) for _item in obj["stepList"]] if obj.get("stepList") is not None else None,
             "documentList": [DocumentDto.from_dict(_item) for _item in obj["documentList"]] if obj.get("documentList") is not None else None,
-            "signatureProofList": [SignatureProof.from_dict(_item) for _item in obj["signatureProofList"]] if obj.get("signatureProofList") is not None else None,
             "readByUserIds": obj.get("readByUserIds"),
             "variableDesksIds": obj.get("variableDesksIds"),
             "detachedSignaturesMapping": obj.get("detachedSignaturesMapping"),
             "visibility": obj.get("visibility"),
             "readByCurrentUser": obj.get("readByCurrentUser")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/detached_signature.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/detached_signature.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/document_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/document_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/error_response.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/external_signature_config.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_cookie.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,33 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from iparapheur_internal.models.external_signature_provider import ExternalSignatureProvider
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ExternalSignatureConfig(BaseModel):
+class GdprCookie(BaseModel):
     """
-    ExternalSignatureConfig
+    GdprCookie
     """ # noqa: E501
-    id: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
-    service_name: Optional[ExternalSignatureProvider] = Field(default=None, alias="serviceName")
-    url: Optional[StrictStr] = None
-    token: Optional[StrictStr] = None
-    password: Optional[StrictStr] = None
-    login: Optional[StrictStr] = None
-    transaction_ids: Optional[List[StrictStr]] = Field(default=None, alias="transactionIds")
-    __properties: ClassVar[List[str]] = ["id", "name", "serviceName", "url", "token", "password", "login", "transactionIds"]
+    elements: Optional[List[StrictStr]] = None
+    description: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["name", "elements", "description"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -52,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ExternalSignatureConfig from a JSON string"""
+        """Create an instance of GdprCookie from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,27 +71,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ExternalSignatureConfig from a dict"""
+        """Create an instance of GdprCookie from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
             "name": obj.get("name"),
-            "serviceName": obj.get("serviceName"),
-            "url": obj.get("url"),
-            "token": obj.get("token"),
-            "password": obj.get("password"),
-            "login": obj.get("login"),
-            "transactionIds": obj.get("transactionIds")
+            "elements": obj.get("elements"),
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/external_signature_config_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/external_signature_provider.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/external_state.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/external_state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/folder_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_dto.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 from datetime import datetime
 from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from iparapheur_internal.models.desk_representation import DeskRepresentation
 from iparapheur_internal.models.document_dto import DocumentDto
-from iparapheur_internal.models.signature_proof import SignatureProof
 from iparapheur_internal.models.subtype_dto import SubtypeDto
 from iparapheur_internal.models.task import Task
 from iparapheur_internal.models.type_dto import TypeDto
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FolderDto(BaseModel):
@@ -46,18 +45,17 @@
     final_desk: Optional[DeskRepresentation] = Field(default=None, alias="finalDesk")
     is_read_by_current_user: Optional[StrictBool] = Field(default=None, alias="isReadByCurrentUser")
     legacy_id: Optional[StrictStr] = Field(default=None, alias="legacyId")
     type_id: Optional[StrictStr] = Field(default=None, alias="typeId")
     subtype_id: Optional[StrictStr] = Field(default=None, alias="subtypeId")
     step_list: Optional[List[Task]] = Field(default=None, alias="stepList")
     document_list: Optional[List[DocumentDto]] = Field(default=None, alias="documentList")
-    signature_proof_list: Optional[List[SignatureProof]] = Field(default=None, alias="signatureProofList")
     read_by_user_ids: Optional[List[StrictStr]] = Field(default=None, alias="readByUserIds")
     read_by_current_user: Optional[StrictBool] = Field(default=None, alias="readByCurrentUser")
-    __properties: ClassVar[List[str]] = ["id", "name", "dueDate", "metadata", "draftCreationDate", "type", "subtype", "originDesk", "finalDesk", "isReadByCurrentUser", "legacyId", "typeId", "subtypeId", "stepList", "documentList", "signatureProofList", "readByUserIds", "readByCurrentUser"]
+    __properties: ClassVar[List[str]] = ["id", "name", "dueDate", "metadata", "draftCreationDate", "type", "subtype", "originDesk", "finalDesk", "isReadByCurrentUser", "legacyId", "typeId", "subtypeId", "stepList", "documentList", "readByUserIds", "readByCurrentUser"]
 
     @field_validator('name')
     def name_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[^\r\n ]*$", value):
             raise ValueError(r"must validate the regular expression /^[^\r\n ]*$/")
         return value
@@ -94,23 +92,21 @@
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
         * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "id",
             "draft_creation_date",
             "is_read_by_current_user",
             "step_list",
             "document_list",
-            "signature_proof_list",
             "read_by_user_ids",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
@@ -137,21 +133,14 @@
         # override the default output from pydantic by calling `to_dict()` of each item in document_list (list)
         _items = []
         if self.document_list:
             for _item in self.document_list:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['documentList'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in signature_proof_list (list)
-        _items = []
-        if self.signature_proof_list:
-            for _item in self.signature_proof_list:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['signatureProofList'] = _items
         # set to None if due_date (nullable) is None
         # and model_fields_set contains the field
         if self.due_date is None and "due_date" in self.model_fields_set:
             _dict['dueDate'] = None
 
         # set to None if origin_desk (nullable) is None
         # and model_fields_set contains the field
@@ -186,14 +175,13 @@
             "finalDesk": DeskRepresentation.from_dict(obj["finalDesk"]) if obj.get("finalDesk") is not None else None,
             "isReadByCurrentUser": obj.get("isReadByCurrentUser"),
             "legacyId": obj.get("legacyId"),
             "typeId": obj.get("typeId"),
             "subtypeId": obj.get("subtypeId"),
             "stepList": [Task.from_dict(_item) for _item in obj["stepList"]] if obj.get("stepList") is not None else None,
             "documentList": [DocumentDto.from_dict(_item) for _item in obj["documentList"]] if obj.get("documentList") is not None else None,
-            "signatureProofList": [SignatureProof.from_dict(_item) for _item in obj["signatureProofList"]] if obj.get("signatureProofList") is not None else None,
             "readByUserIds": obj.get("readByUserIds"),
             "readByCurrentUser": obj.get("readByCurrentUser")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/folder_filter_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_filter_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/folder_listable_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_listable_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/folder_sort_by.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/folder_visibility.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/folder_visibility.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_application.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_application.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_cookie.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_responsible.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field
 from typing import Any, ClassVar, Dict, List, Optional
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GdprCookie(BaseModel):
+class GdprDeclaringEntityResponsible(BaseModel):
     """
-    GdprCookie
+    GdprDeclaringEntityResponsible
     """ # noqa: E501
-    name: Optional[StrictStr] = None
-    elements: Optional[List[StrictStr]] = None
-    description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["name", "elements", "description"]
+    name: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
+    title: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
+    __properties: ClassVar[List[str]] = ["name", "title"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -46,15 +46,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GdprCookie from a JSON string"""
+        """Create an instance of GdprDeclaringEntityResponsible from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,22 +71,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GdprCookie from a dict"""
+        """Create an instance of GdprDeclaringEntityResponsible from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "elements": obj.get("elements"),
-            "description": obj.get("description")
+            "title": obj.get("title")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_data_element.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_element.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_data_set.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_data_set.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_declaring_entity.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_declaring_entity_dpo.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_declaring_entity_dpo.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_declaring_entity_responsible.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 
 from pydantic import BaseModel, Field
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GdprDeclaringEntityResponsible(BaseModel):
+class GdprEntity(BaseModel):
     """
-    GdprDeclaringEntityResponsible
+    GdprEntity
     """ # noqa: E501
     name: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
-    title: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
-    __properties: ClassVar[List[str]] = ["name", "title"]
+    address: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
+    siret: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
+    __properties: ClassVar[List[str]] = ["name", "address", "siret"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -46,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GdprDeclaringEntityResponsible from a JSON string"""
+        """Create an instance of GdprEntity from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +72,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GdprDeclaringEntityResponsible from a dict"""
+        """Create an instance of GdprEntity from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
-            "title": obj.get("title")
+            "address": obj.get("address"),
+            "siret": obj.get("siret")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_entity.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/validation_service_configuration_dto.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field
-from typing import Any, ClassVar, Dict, List, Optional
-from typing_extensions import Annotated
+from pydantic import BaseModel, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GdprEntity(BaseModel):
+class ValidationServiceConfigurationDto(BaseModel):
     """
-    GdprEntity
+    ValidationServiceConfigurationDto
     """ # noqa: E501
-    name: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
-    address: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
-    siret: Optional[Annotated[str, Field(min_length=0, strict=True, max_length=255)]] = None
-    __properties: ClassVar[List[str]] = ["name", "address", "siret"]
+    client_id: StrictStr = Field(alias="clientId")
+    client_secret: StrictStr = Field(alias="clientSecret")
+    __properties: ClassVar[List[str]] = ["clientId", "clientSecret"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GdprEntity from a JSON string"""
+        """Create an instance of ValidationServiceConfigurationDto from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,22 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GdprEntity from a dict"""
+        """Create an instance of ValidationServiceConfigurationDto from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "name": obj.get("name"),
-            "address": obj.get("address"),
-            "siret": obj.get("siret")
+            "clientId": obj.get("clientId"),
+            "clientSecret": obj.get("clientSecret")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/gdpr_information_details_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/gdpr_information_details_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/hierarchised_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/layer_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/layer_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/mail_template_test_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/test_signature_template_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, Field, StrictBytes, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MailTemplateTestRequest(BaseModel):
+class TestSignatureTemplateRequest(BaseModel):
     """
-    body
+    TestSignatureTemplateRequest
     """ # noqa: E501
-    template: Optional[StrictStr] = None
-    mail: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["template", "mail"]
+    signature_image: Optional[Union[StrictBytes, StrictStr]] = Field(default=None, alias="signatureImage")
+    __properties: ClassVar[List[str]] = ["signatureImage"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -45,15 +44,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MailTemplateTestRequest from a JSON string"""
+        """Create an instance of TestSignatureTemplateRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,21 +69,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MailTemplateTestRequest from a dict"""
+        """Create an instance of TestSignatureTemplateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "template": obj.get("template"),
-            "mail": obj.get("mail")
+            "signatureImage": obj.get("signatureImage")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/media_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/media_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/metadata.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,28 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from iparapheur_internal.models.metadata_type import MetadataType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Metadata(BaseModel):
+class SignatureInfo(BaseModel):
     """
-    Metadata
+    SignatureInfo
     """ # noqa: E501
-    id: Optional[StrictStr] = None
-    key: Optional[StrictStr] = None
+    signature_date_time: Optional[StrictInt] = Field(default=None, alias="signatureDateTime")
+    is_signature_valid: Optional[StrictBool] = Field(default=None, alias="isSignatureValid")
     name: Optional[StrictStr] = None
-    index: Optional[StrictInt] = None
-    type: Optional[MetadataType] = None
-    restricted_values: Optional[List[StrictStr]] = Field(default=None, alias="restrictedValues")
-    __properties: ClassVar[List[str]] = ["id", "key", "name", "index", "type", "restrictedValues"]
+    issuer_name: Optional[StrictStr] = Field(default=None, alias="issuerName")
+    __properties: ClassVar[List[str]] = ["signatureDateTime", "isSignatureValid", "name", "issuerName"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Metadata from a JSON string"""
+        """Create an instance of SignatureInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,25 +72,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Metadata from a dict"""
+        """Create an instance of SignatureInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "key": obj.get("key"),
+            "signatureDateTime": obj.get("signatureDateTime"),
+            "isSignatureValid": obj.get("isSignatureValid"),
             "name": obj.get("name"),
-            "index": obj.get("index"),
-            "type": obj.get("type"),
-            "restrictedValues": obj.get("restrictedValues")
+            "issuerName": obj.get("issuerName")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/metadata_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/metadata_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_folder_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_folder_listable_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_folder_listable_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_hierarchised_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_info.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_info.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_layer_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_subtype_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/page_typology_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/page_typology_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/pageable_object.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/password_policies.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/password_policies.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/pdf_signature_position.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/pdf_template_test_request.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/pdf_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/seal_certificate_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/signature_format.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/signature_info.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_representation.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,28 +14,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SignatureInfo(BaseModel):
+class SubtypeRepresentation(BaseModel):
     """
-    SignatureInfo
+    SubtypeRepresentation
     """ # noqa: E501
-    signature_date_time: Optional[StrictInt] = Field(default=None, alias="signatureDateTime")
-    is_signature_valid: Optional[StrictBool] = Field(default=None, alias="isSignatureValid")
-    name: Optional[StrictStr] = None
-    issuer_name: Optional[StrictStr] = Field(default=None, alias="issuerName")
-    __properties: ClassVar[List[str]] = ["signatureDateTime", "isSignatureValid", "name", "issuerName"]
+    id: Optional[StrictStr] = None
+    name: Annotated[str, Field(min_length=2, strict=True, max_length=255)]
+    __properties: ClassVar[List[str]] = ["id", "name"]
+
+    @field_validator('name')
+    def name_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^[^\r\n ]*$", value):
+            raise ValueError(r"must validate the regular expression /^[^\r\n ]*$/")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,48 +53,48 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SignatureInfo from a JSON string"""
+        """Create an instance of SubtypeRepresentation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SignatureInfo from a dict"""
+        """Create an instance of SubtypeRepresentation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "signatureDateTime": obj.get("signatureDateTime"),
-            "isSignatureValid": obj.get("isSignatureValid"),
-            "name": obj.get("name"),
-            "issuerName": obj.get("issuerName")
+            "id": obj.get("id"),
+            "name": obj.get("name")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/signature_placement.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_placement.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/signature_protocol.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/sort_object.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/stamp_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/stamp_text_color.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_text_color.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/stamp_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/stamp_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/state.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/step_definition_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/step_definition_parallel_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_parallel_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/step_definition_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/step_definition_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/task.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,48 +14,53 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from datetime import datetime
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from iparapheur_internal.models.external_signature_config import ExternalSignatureConfig
-from iparapheur_internal.models.subtype_layer import SubtypeLayer
-from iparapheur_internal.models.subtype_metadata import SubtypeMetadata
+from iparapheur_internal.models.action import Action
+from iparapheur_internal.models.desk_representation import DeskRepresentation
+from iparapheur_internal.models.external_state import ExternalState
+from iparapheur_internal.models.state import State
+from iparapheur_internal.models.user_representation import UserRepresentation
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Subtype(BaseModel):
+class Task(BaseModel):
     """
-    Subtype
+    Task
     """ # noqa: E501
     id: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    description: Optional[StrictStr] = None
-    creation_workflow_id: Optional[StrictStr] = Field(default=None, alias="creationWorkflowId")
-    validation_workflow_id: Optional[StrictStr] = Field(default=None, alias="validationWorkflowId")
-    workflow_selection_script: Optional[StrictStr] = Field(default=None, alias="workflowSelectionScript")
-    annotations_allowed: Optional[StrictBool] = Field(default=None, alias="annotationsAllowed")
-    external_signature_automatic: Optional[StrictBool] = Field(default=None, alias="externalSignatureAutomatic")
-    max_main_documents: Optional[StrictInt] = Field(default=None, alias="maxMainDocuments")
-    secure_mail_server_id: Optional[StrictInt] = Field(default=None, alias="secureMailServerId")
-    seal_certificate_id: Optional[StrictStr] = Field(default=None, alias="sealCertificateId")
-    external_signature_config: Optional[ExternalSignatureConfig] = Field(default=None, alias="externalSignatureConfig")
-    subtype_metadata_list: Optional[List[SubtypeMetadata]] = Field(default=None, alias="subtypeMetadataList")
-    subtype_layers: Optional[List[SubtypeLayer]] = Field(default=None, alias="subtypeLayers")
-    creation_permitted_desk_ids: Optional[List[StrictStr]] = Field(default=None, alias="creationPermittedDeskIds")
-    filterable_by_desk_ids: Optional[List[StrictStr]] = Field(default=None, alias="filterableByDeskIds")
-    multi_documents: Optional[StrictBool] = Field(default=None, alias="multiDocuments")
-    annexe_included: Optional[StrictBool] = Field(default=None, alias="annexeIncluded")
-    digital_signature_mandatory: Optional[StrictBool] = Field(default=None, alias="digitalSignatureMandatory")
-    reading_mandatory: Optional[StrictBool] = Field(default=None, alias="readingMandatory")
-    seal_automatic: Optional[StrictBool] = Field(default=None, alias="sealAutomatic")
-    __properties: ClassVar[List[str]] = ["id", "name", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "maxMainDocuments", "secureMailServerId", "sealCertificateId", "externalSignatureConfig", "subtypeMetadataList", "subtypeLayers", "creationPermittedDeskIds", "filterableByDeskIds", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic"]
+    metadata: Optional[Dict[str, StrictStr]] = None
+    action: Optional[Action] = None
+    performed_action: Optional[Action] = Field(default=None, alias="performedAction")
+    external_state: Optional[ExternalState] = Field(default=None, alias="externalState")
+    state: Optional[State] = None
+    desks: Optional[List[Optional[DeskRepresentation]]] = None
+    delegated_by_desk: Optional[DeskRepresentation] = Field(default=None, alias="delegatedByDesk")
+    user: Optional[UserRepresentation] = None
+    read_by_user_ids: Optional[List[StrictStr]] = Field(default=None, alias="readByUserIds")
+    public_certificate_base64: Optional[StrictStr] = Field(default=None, alias="publicCertificateBase64")
+    external_signature_procedure_id: Optional[StrictStr] = Field(default=None, alias="externalSignatureProcedureId")
+    begin_date: Optional[datetime] = Field(default=None, alias="beginDate")
+    var_date: Optional[datetime] = Field(default=None, alias="date")
+    draft_creation_date: Optional[datetime] = Field(default=None, alias="draftCreationDate")
+    public_annotation: Optional[StrictStr] = Field(default=None, alias="publicAnnotation")
+    private_annotation: Optional[StrictStr] = Field(default=None, alias="privateAnnotation")
+    notified_desks: Optional[List[Optional[DeskRepresentation]]] = Field(default=None, alias="notifiedDesks")
+    workflow_index: Optional[StrictInt] = Field(default=None, alias="workflowIndex")
+    step_index: Optional[StrictInt] = Field(default=None, alias="stepIndex")
+    mandatory_validation_metadata: Optional[List[StrictStr]] = Field(default=None, alias="mandatoryValidationMetadata")
+    mandatory_rejection_metadata: Optional[List[StrictStr]] = Field(default=None, alias="mandatoryRejectionMetadata")
+    instance_name: Optional[StrictStr] = Field(default=None, alias="instanceName")
+    __properties: ClassVar[List[str]] = ["id", "metadata", "action", "performedAction", "externalState", "state", "desks", "delegatedByDesk", "user", "readByUserIds", "publicCertificateBase64", "externalSignatureProcedureId", "beginDate", "date", "draftCreationDate", "publicAnnotation", "privateAnnotation", "notifiedDesks", "workflowIndex", "stepIndex", "mandatoryValidationMetadata", "mandatoryRejectionMetadata", "instanceName"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -67,15 +72,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Subtype from a JSON string"""
+        """Create an instance of Task from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -88,61 +93,71 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of external_signature_config
-        if self.external_signature_config:
-            _dict['externalSignatureConfig'] = self.external_signature_config.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in subtype_metadata_list (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in desks (list)
         _items = []
-        if self.subtype_metadata_list:
-            for _item in self.subtype_metadata_list:
+        if self.desks:
+            for _item in self.desks:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['subtypeMetadataList'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in subtype_layers (list)
+            _dict['desks'] = _items
+        # override the default output from pydantic by calling `to_dict()` of delegated_by_desk
+        if self.delegated_by_desk:
+            _dict['delegatedByDesk'] = self.delegated_by_desk.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of user
+        if self.user:
+            _dict['user'] = self.user.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in notified_desks (list)
         _items = []
-        if self.subtype_layers:
-            for _item in self.subtype_layers:
+        if self.notified_desks:
+            for _item in self.notified_desks:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['subtypeLayers'] = _items
+            _dict['notifiedDesks'] = _items
+        # set to None if delegated_by_desk (nullable) is None
+        # and model_fields_set contains the field
+        if self.delegated_by_desk is None and "delegated_by_desk" in self.model_fields_set:
+            _dict['delegatedByDesk'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Subtype from a dict"""
+        """Create an instance of Task from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "name": obj.get("name"),
-            "description": obj.get("description"),
-            "creationWorkflowId": obj.get("creationWorkflowId"),
-            "validationWorkflowId": obj.get("validationWorkflowId"),
-            "workflowSelectionScript": obj.get("workflowSelectionScript"),
-            "annotationsAllowed": obj.get("annotationsAllowed"),
-            "externalSignatureAutomatic": obj.get("externalSignatureAutomatic"),
-            "maxMainDocuments": obj.get("maxMainDocuments"),
-            "secureMailServerId": obj.get("secureMailServerId"),
-            "sealCertificateId": obj.get("sealCertificateId"),
-            "externalSignatureConfig": ExternalSignatureConfig.from_dict(obj["externalSignatureConfig"]) if obj.get("externalSignatureConfig") is not None else None,
-            "subtypeMetadataList": [SubtypeMetadata.from_dict(_item) for _item in obj["subtypeMetadataList"]] if obj.get("subtypeMetadataList") is not None else None,
-            "subtypeLayers": [SubtypeLayer.from_dict(_item) for _item in obj["subtypeLayers"]] if obj.get("subtypeLayers") is not None else None,
-            "creationPermittedDeskIds": obj.get("creationPermittedDeskIds"),
-            "filterableByDeskIds": obj.get("filterableByDeskIds"),
-            "multiDocuments": obj.get("multiDocuments"),
-            "annexeIncluded": obj.get("annexeIncluded"),
-            "digitalSignatureMandatory": obj.get("digitalSignatureMandatory"),
-            "readingMandatory": obj.get("readingMandatory"),
-            "sealAutomatic": obj.get("sealAutomatic")
+            "metadata": obj.get("metadata"),
+            "action": obj.get("action"),
+            "performedAction": obj.get("performedAction"),
+            "externalState": obj.get("externalState"),
+            "state": obj.get("state"),
+            "desks": [DeskRepresentation.from_dict(_item) for _item in obj["desks"]] if obj.get("desks") is not None else None,
+            "delegatedByDesk": DeskRepresentation.from_dict(obj["delegatedByDesk"]) if obj.get("delegatedByDesk") is not None else None,
+            "user": UserRepresentation.from_dict(obj["user"]) if obj.get("user") is not None else None,
+            "readByUserIds": obj.get("readByUserIds"),
+            "publicCertificateBase64": obj.get("publicCertificateBase64"),
+            "externalSignatureProcedureId": obj.get("externalSignatureProcedureId"),
+            "beginDate": obj.get("beginDate"),
+            "date": obj.get("date"),
+            "draftCreationDate": obj.get("draftCreationDate"),
+            "publicAnnotation": obj.get("publicAnnotation"),
+            "privateAnnotation": obj.get("privateAnnotation"),
+            "notifiedDesks": [DeskRepresentation.from_dict(_item) for _item in obj["notifiedDesks"]] if obj.get("notifiedDesks") is not None else None,
+            "workflowIndex": obj.get("workflowIndex"),
+            "stepIndex": obj.get("stepIndex"),
+            "mandatoryValidationMetadata": obj.get("mandatoryValidationMetadata"),
+            "mandatoryRejectionMetadata": obj.get("mandatoryRejectionMetadata"),
+            "instanceName": obj.get("instanceName")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_layer.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_dto.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from iparapheur_internal.models.composite_id import CompositeId
+from iparapheur_internal.models.layer_representation import LayerRepresentation
 from iparapheur_internal.models.subtype_layer_association import SubtypeLayerAssociation
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SubtypeLayer(BaseModel):
+class SubtypeLayerDto(BaseModel):
     """
-    SubtypeLayer
+    SubtypeLayerDto
     """ # noqa: E501
-    id: Optional[CompositeId] = None
+    layer_id: Optional[StrictStr] = Field(default=None, alias="layerId")
+    layer: Optional[LayerRepresentation] = None
     association: Optional[SubtypeLayerAssociation] = None
-    __properties: ClassVar[List[str]] = ["id", "association"]
+    __properties: ClassVar[List[str]] = ["layerId", "layer", "association"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -47,15 +48,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SubtypeLayer from a JSON string"""
+        """Create an instance of SubtypeLayerDto from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,28 +69,29 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of id
-        if self.id:
-            _dict['id'] = self.id.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of layer
+        if self.layer:
+            _dict['layer'] = self.layer.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SubtypeLayer from a dict"""
+        """Create an instance of SubtypeLayerDto from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": CompositeId.from_dict(obj["id"]) if obj.get("id") is not None else None,
+            "layerId": obj.get("layerId"),
+            "layer": LayerRepresentation.from_dict(obj["layer"]) if obj.get("layer") is not None else None,
             "association": obj.get("association")
         })
         return _obj
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_layer_association.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_layer_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/tenant_representation.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,29 +14,34 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from iparapheur_internal.models.layer_representation import LayerRepresentation
-from iparapheur_internal.models.subtype_layer_association import SubtypeLayerAssociation
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SubtypeLayerDto(BaseModel):
+class TenantRepresentation(BaseModel):
     """
-    SubtypeLayerDto
+    TenantRepresentation
     """ # noqa: E501
-    layer_id: Optional[StrictStr] = Field(default=None, alias="layerId")
-    layer: Optional[LayerRepresentation] = None
-    association: Optional[SubtypeLayerAssociation] = None
-    __properties: ClassVar[List[str]] = ["layerId", "layer", "association"]
+    id: Optional[StrictStr] = None
+    name: Annotated[str, Field(min_length=2, strict=True, max_length=255)]
+    __properties: ClassVar[List[str]] = ["id", "name"]
+
+    @field_validator('name')
+    def name_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^[^\r\n ]*$", value):
+            raise ValueError(r"must validate the regular expression /^[^\r\n ]*$/")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -48,50 +53,48 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SubtypeLayerDto from a JSON string"""
+        """Create an instance of TenantRepresentation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of layer
-        if self.layer:
-            _dict['layer'] = self.layer.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SubtypeLayerDto from a dict"""
+        """Create an instance of TenantRepresentation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "layerId": obj.get("layerId"),
-            "layer": LayerRepresentation.from_dict(obj["layer"]) if obj.get("layer") is not None else None,
-            "association": obj.get("association")
+            "id": obj.get("id"),
+            "name": obj.get("name")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_metadata.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/typology_representation.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,31 +14,36 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from iparapheur_internal.models.composite_id import CompositeId
-from iparapheur_internal.models.metadata import Metadata
+from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SubtypeMetadata(BaseModel):
+class TypologyRepresentation(BaseModel):
     """
-    SubtypeMetadata
+    TypologyRepresentation
     """ # noqa: E501
-    id: Optional[CompositeId] = None
-    metadata: Optional[Metadata] = None
-    default_value: Optional[StrictStr] = Field(default=None, alias="defaultValue")
-    mandatory: Optional[StrictBool] = None
-    editable: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["id", "metadata", "defaultValue", "mandatory", "editable"]
+    id: Optional[StrictStr] = None
+    name: Annotated[str, Field(min_length=2, strict=True, max_length=255)]
+    parent_id: Optional[StrictStr] = Field(default=None, alias="parentId")
+    children_count: Optional[StrictInt] = Field(default=None, alias="childrenCount")
+    __properties: ClassVar[List[str]] = ["id", "name", "parentId", "childrenCount"]
+
+    @field_validator('name')
+    def name_validate_regular_expression(cls, value):
+        """Validates the regular expression"""
+        if not re.match(r"^[^\r\n ]*$", value):
+            raise ValueError(r"must validate the regular expression /^[^\r\n ]*$/")
+        return value
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -50,55 +55,54 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SubtypeMetadata from a JSON string"""
+        """Create an instance of TypologyRepresentation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "id",
+            "parent_id",
+            "children_count",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of id
-        if self.id:
-            _dict['id'] = self.id.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of metadata
-        if self.metadata:
-            _dict['metadata'] = self.metadata.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SubtypeMetadata from a dict"""
+        """Create an instance of TypologyRepresentation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "id": CompositeId.from_dict(obj["id"]) if obj.get("id") is not None else None,
-            "metadata": Metadata.from_dict(obj["metadata"]) if obj.get("metadata") is not None else None,
-            "defaultValue": obj.get("defaultValue"),
-            "mandatory": obj.get("mandatory"),
-            "editable": obj.get("editable")
+            "id": obj.get("id"),
+            "name": obj.get("name"),
+            "parentId": obj.get("parentId"),
+            "childrenCount": obj.get("childrenCount")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/subtype_metadata_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/template_type.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/tenant_representation.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/user_representation.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,34 +14,33 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
+from iparapheur_internal.models.user_privilege import UserPrivilege
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TenantRepresentation(BaseModel):
+class UserRepresentation(BaseModel):
     """
-    TenantRepresentation
+    UserRepresentation
     """ # noqa: E501
     id: Optional[StrictStr] = None
-    name: Annotated[str, Field(min_length=2, strict=True, max_length=255)]
-    __properties: ClassVar[List[str]] = ["id", "name"]
-
-    @field_validator('name')
-    def name_validate_regular_expression(cls, value):
-        """Validates the regular expression"""
-        if not re.match(r"^[^\r\n ]*$", value):
-            raise ValueError(r"must validate the regular expression /^[^\r\n ]*$/")
-        return value
+    user_name: Annotated[str, Field(min_length=1, strict=True, max_length=128)] = Field(alias="userName")
+    first_name: Annotated[str, Field(min_length=0, strict=True, max_length=128)] = Field(alias="firstName")
+    last_name: Annotated[str, Field(min_length=0, strict=True, max_length=128)] = Field(alias="lastName")
+    email: StrictStr
+    privilege: UserPrivilege
+    is_ldap_synchronized: Optional[StrictBool] = Field(default=None, alias="isLdapSynchronized")
+    __properties: ClassVar[List[str]] = ["id", "userName", "firstName", "lastName", "email", "privilege", "isLdapSynchronized"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
@@ -53,48 +52,55 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TenantRepresentation from a JSON string"""
+        """Create an instance of UserRepresentation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
         * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
             "id",
+            "is_ldap_synchronized",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TenantRepresentation from a dict"""
+        """Create an instance of UserRepresentation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "id": obj.get("id"),
-            "name": obj.get("name")
+            "userName": obj.get("userName"),
+            "firstName": obj.get("firstName"),
+            "lastName": obj.get("lastName"),
+            "email": obj.get("email"),
+            "privilege": obj.get("privilege"),
+            "isLdapSynchronized": obj.get("isLdapSynchronized")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/type_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/user_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/user_privilege.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/models/workflow_definition_dto.py` & `iparapheur-internal-1.12.3/iparapheur_internal/models/workflow_definition_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal/rest.py` & `iparapheur-internal-1.12.3/iparapheur_internal/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal.egg-info/PKG-INFO` & `iparapheur-internal-1.12.3/iparapheur_internal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iparapheur-internal
-Version: 1.11.5
+Version: 1.12.3
 Summary: iparapheur
 Home-page: 
 Author: Libriciel SCOP
 Author-email: iparapheur@libriciel.coop
 License: Affero GPL 3.0
 Keywords: OpenAPI,OpenAPI-Generator,iparapheur
 Description-Content-Type: text/markdown
```

### Comparing `iparapheur-internal-1.11.5/iparapheur_internal.egg-info/SOURCES.txt` & `iparapheur-internal-1.12.3/iparapheur_internal.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,32 +18,29 @@
 iparapheur_internal/api/admin_advanced_config_api.py
 iparapheur_internal/api/admin_desk_api.py
 iparapheur_internal/api/admin_layer_api.py
 iparapheur_internal/api/admin_seal_certificate_api.py
 iparapheur_internal/api/admin_template_api.py
 iparapheur_internal/api/admin_trash_bin_api.py
 iparapheur_internal/api/admin_typology_api.py
-iparapheur_internal/api/admin_workflow_definition_api.py
 iparapheur_internal/api/current_user_api.py
 iparapheur_internal/api/desk_api.py
 iparapheur_internal/api/folder_api.py
 iparapheur_internal/api/server_info_api.py
 iparapheur_internal/api/template_api.py
 iparapheur_internal/api/typology_api.py
 iparapheur_internal/api/workflow_api.py
 iparapheur_internal/models/__init__.py
 iparapheur_internal/models/action.py
-iparapheur_internal/models/composite_id.py
 iparapheur_internal/models/create_file_stamp_request.py
 iparapheur_internal/models/create_folder_request.py
 iparapheur_internal/models/desk_representation.py
 iparapheur_internal/models/detached_signature.py
 iparapheur_internal/models/document_dto.py
 iparapheur_internal/models/error_response.py
-iparapheur_internal/models/external_signature_config.py
 iparapheur_internal/models/external_signature_config_representation.py
 iparapheur_internal/models/external_signature_provider.py
 iparapheur_internal/models/external_state.py
 iparapheur_internal/models/folder_dto.py
 iparapheur_internal/models/folder_filter_dto.py
 iparapheur_internal/models/folder_listable_dto.py
 iparapheur_internal/models/folder_sort_by.py
@@ -58,15 +55,14 @@
 iparapheur_internal/models/gdpr_entity.py
 iparapheur_internal/models/gdpr_information_details_dto.py
 iparapheur_internal/models/hierarchised_desk_representation.py
 iparapheur_internal/models/layer_dto.py
 iparapheur_internal/models/layer_representation.py
 iparapheur_internal/models/mail_template_test_request.py
 iparapheur_internal/models/media_type.py
-iparapheur_internal/models/metadata.py
 iparapheur_internal/models/metadata_dto.py
 iparapheur_internal/models/metadata_type.py
 iparapheur_internal/models/page_desk_representation.py
 iparapheur_internal/models/page_folder_dto.py
 iparapheur_internal/models/page_folder_listable_dto.py
 iparapheur_internal/models/page_hierarchised_desk_representation.py
 iparapheur_internal/models/page_info.py
@@ -77,30 +73,26 @@
 iparapheur_internal/models/password_policies.py
 iparapheur_internal/models/pdf_signature_position.py
 iparapheur_internal/models/pdf_template_test_request.py
 iparapheur_internal/models/seal_certificate_representation.py
 iparapheur_internal/models/signature_format.py
 iparapheur_internal/models/signature_info.py
 iparapheur_internal/models/signature_placement.py
-iparapheur_internal/models/signature_proof.py
 iparapheur_internal/models/signature_protocol.py
 iparapheur_internal/models/sort_object.py
 iparapheur_internal/models/stamp_dto.py
 iparapheur_internal/models/stamp_text_color.py
 iparapheur_internal/models/stamp_type.py
 iparapheur_internal/models/state.py
 iparapheur_internal/models/step_definition_dto.py
 iparapheur_internal/models/step_definition_parallel_type.py
 iparapheur_internal/models/step_definition_type.py
-iparapheur_internal/models/subtype.py
 iparapheur_internal/models/subtype_dto.py
-iparapheur_internal/models/subtype_layer.py
 iparapheur_internal/models/subtype_layer_association.py
 iparapheur_internal/models/subtype_layer_dto.py
-iparapheur_internal/models/subtype_metadata.py
 iparapheur_internal/models/subtype_metadata_dto.py
 iparapheur_internal/models/subtype_representation.py
 iparapheur_internal/models/task.py
 iparapheur_internal/models/template_type.py
 iparapheur_internal/models/tenant_representation.py
 iparapheur_internal/models/test_signature_template_request.py
 iparapheur_internal/models/type_dto.py
@@ -114,25 +106,22 @@
 test/test_admin_advanced_config_api.py
 test/test_admin_desk_api.py
 test/test_admin_layer_api.py
 test/test_admin_seal_certificate_api.py
 test/test_admin_template_api.py
 test/test_admin_trash_bin_api.py
 test/test_admin_typology_api.py
-test/test_admin_workflow_definition_api.py
-test/test_composite_id.py
 test/test_create_file_stamp_request.py
 test/test_create_folder_request.py
 test/test_current_user_api.py
 test/test_desk_api.py
 test/test_desk_representation.py
 test/test_detached_signature.py
 test/test_document_dto.py
 test/test_error_response.py
-test/test_external_signature_config.py
 test/test_external_signature_config_representation.py
 test/test_external_signature_provider.py
 test/test_external_state.py
 test/test_folder_api.py
 test/test_folder_dto.py
 test/test_folder_filter_dto.py
 test/test_folder_listable_dto.py
@@ -148,15 +137,14 @@
 test/test_gdpr_entity.py
 test/test_gdpr_information_details_dto.py
 test/test_hierarchised_desk_representation.py
 test/test_layer_dto.py
 test/test_layer_representation.py
 test/test_mail_template_test_request.py
 test/test_media_type.py
-test/test_metadata.py
 test/test_metadata_dto.py
 test/test_metadata_type.py
 test/test_page_desk_representation.py
 test/test_page_folder_dto.py
 test/test_page_folder_listable_dto.py
 test/test_page_hierarchised_desk_representation.py
 test/test_page_info.py
@@ -168,30 +156,26 @@
 test/test_pdf_signature_position.py
 test/test_pdf_template_test_request.py
 test/test_seal_certificate_representation.py
 test/test_server_info_api.py
 test/test_signature_format.py
 test/test_signature_info.py
 test/test_signature_placement.py
-test/test_signature_proof.py
 test/test_signature_protocol.py
 test/test_sort_object.py
 test/test_stamp_dto.py
 test/test_stamp_text_color.py
 test/test_stamp_type.py
 test/test_state.py
 test/test_step_definition_dto.py
 test/test_step_definition_parallel_type.py
 test/test_step_definition_type.py
-test/test_subtype.py
 test/test_subtype_dto.py
-test/test_subtype_layer.py
 test/test_subtype_layer_association.py
 test/test_subtype_layer_dto.py
-test/test_subtype_metadata.py
 test/test_subtype_metadata_dto.py
 test/test_subtype_representation.py
 test/test_task.py
 test/test_template_api.py
 test/test_template_type.py
 test/test_tenant_representation.py
 test/test_test_signature_template_request.py
```

### Comparing `iparapheur-internal-1.11.5/pyproject.toml` & `iparapheur-internal-1.12.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iparapheur_internal"
-version = "1.11.5"
+version = "1.12.3"
 description = "iparapheur"
 authors = ["Libriciel SCOP <iparapheur@libriciel.coop>"]
 license = "Affero GPL 3.0"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "iparapheur"]
 include = ["iparapheur_internal/py.typed"]
```

### Comparing `iparapheur-internal-1.11.5/setup.py` & `iparapheur-internal-1.12.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "iparapheur-internal"
-VERSION = "1.11.5"
+VERSION = "1.12.3"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `iparapheur-internal-1.11.5/test/test_action.py` & `iparapheur-internal-1.12.3/test/test_action.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_advanced_config_api.py` & `iparapheur-internal-1.12.3/test/test_admin_advanced_config_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,21 +23,14 @@
 
     def setUp(self) -> None:
         self.api = AdminAdvancedConfigApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_delete_chorus_configuration(self) -> None:
-        """Test case for delete_chorus_configuration
-
-        Delete Chorus Pro configuration
-        """
-        pass
-
     def test_get_chorus_configuration(self) -> None:
         """Test case for get_chorus_configuration
 
         Get Chorus Pro configuration
         """
         pass
```

### Comparing `iparapheur-internal-1.11.5/test/test_admin_desk_api.py` & `iparapheur-internal-1.12.3/test/test_admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_layer_api.py` & `iparapheur-internal-1.12.3/test/test_admin_layer_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_seal_certificate_api.py` & `iparapheur-internal-1.12.3/test/test_admin_seal_certificate_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_template_api.py` & `iparapheur-internal-1.12.3/test/test_admin_template_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_trash_bin_api.py` & `iparapheur-internal-1.12.3/test/test_admin_trash_bin_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_typology_api.py` & `iparapheur-internal-1.12.3/test/test_admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_admin_workflow_definition_api.py` & `iparapheur-internal-1.12.3/test/test_workflow_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,29 +11,36 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.api.admin_workflow_definition_api import AdminWorkflowDefinitionApi
+from iparapheur_internal.api.workflow_api import WorkflowApi
 
 
-class TestAdminWorkflowDefinitionApi(unittest.TestCase):
-    """AdminWorkflowDefinitionApi unit test stubs"""
+class TestWorkflowApi(unittest.TestCase):
+    """WorkflowApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = AdminWorkflowDefinitionApi()
+        self.api = WorkflowApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_subtypes_referencing_workflow_definition_key(self) -> None:
-        """Test case for get_subtypes_referencing_workflow_definition_key
+    def test_evaluate_workflow_selection_script(self) -> None:
+        """Test case for evaluate_workflow_selection_script
 
-        Get subtypes referencing the given workflow definition key
+        Returns the evaluated workflow definition, using current parent desks, and given metadata on a possible selection script
+        """
+        pass
+
+    def test_get_workflow_definition(self) -> None:
+        """Test case for get_workflow_definition
+
+        Get a workflow definition with every information set
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_composite_id.py` & `iparapheur-internal-1.12.3/test/test_gdpr_entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,42 +11,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.composite_id import CompositeId
+from iparapheur_internal.models.gdpr_entity import GdprEntity
 
-class TestCompositeId(unittest.TestCase):
-    """CompositeId unit test stubs"""
+class TestGdprEntity(unittest.TestCase):
+    """GdprEntity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CompositeId:
-        """Test CompositeId
+    def make_instance(self, include_optional) -> GdprEntity:
+        """Test GdprEntity
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CompositeId`
+        # uncomment below to create an instance of `GdprEntity`
         """
-        model = CompositeId()
+        model = GdprEntity()
         if include_optional:
-            return CompositeId(
-                layer_id = ''
+            return GdprEntity(
+                name = '',
+                address = '',
+                siret = ''
             )
         else:
-            return CompositeId(
+            return GdprEntity(
         )
         """
 
-    def testCompositeId(self):
-        """Test CompositeId"""
+    def testGdprEntity(self):
+        """Test GdprEntity"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_create_file_stamp_request.py` & `iparapheur-internal-1.12.3/test/test_create_file_stamp_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_create_folder_request.py` & `iparapheur-internal-1.12.3/test/test_create_folder_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -259,89 +259,14 @@
                                 name = '', 
                                 issuer_name = '', )
                             ], 
                         signature_proof = True, 
                         deletable = True, 
                         is_main_document = True, )
                     ],
-                signature_proof_list = [
-                    iparapheur_internal.models.signature_proof.SignatureProof(
-                        id = '', 
-                        name = '', 
-                        index = 56, 
-                        page_count = 56, 
-                        content_length = 56, 
-                        media_type = iparapheur_internal.models.media_type.MediaType(
-                            type = '', 
-                            subtype = '', 
-                            parameters = {
-                                'key' : ''
-                                }, 
-                            quality_value = 1.337, 
-                            wildcard_type = True, 
-                            wildcard_subtype = True, 
-                            subtype_suffix = '', 
-                            charset = '', 
-                            concrete = True, ), 
-                        pages_properties = {
-                            'key' : iparapheur_internal.models.page_info.PageInfo(
-                                width = 1.337, 
-                                height = 1.337, 
-                                rotation = 56, )
-                            }, 
-                        pdf_visual_id = '', 
-                        signature_placement_annotations = [
-                            iparapheur_internal.models.signature_placement.SignaturePlacement(
-                                id = '', 
-                                page = 1, 
-                                width = 15, 
-                                height = 15, 
-                                x = 56, 
-                                y = 56, 
-                                page_rotation = 0, 
-                                page_width = 276, 
-                                page_height = 308, 
-                                rectangle_origin = 'TOP_RIGHT', 
-                                signature_number = 0, 
-                                template_type = 'MAIL_NOTIFICATION_SINGLE', )
-                            ], 
-                        signature_tags = {
-                            'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
-                                x = 1.337, 
-                                y = 1.337, 
-                                page = 56, )
-                            }, 
-                        seal_tags = {
-                            'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
-                                x = 1.337, 
-                                y = 1.337, 
-                                page = 56, )
-                            }, 
-                        detached_signatures = [
-                            iparapheur_internal.models.detached_signature.DetachedSignature(
-                                id = '', 
-                                name = '', 
-                                content_length = 56, 
-                                target_document_id = '', 
-                                target_task_id = '', )
-                            ], 
-                        embedded_signature_infos = [
-                            iparapheur_internal.models.signature_info.SignatureInfo(
-                                signature_date_time = 56, 
-                                is_signature_valid = True, 
-                                name = '', 
-                                issuer_name = '', )
-                            ], 
-                        proof_target_task_id = '', 
-                        error_message = '', 
-                        internal = True, 
-                        signature_proof = True, 
-                        deletable = True, 
-                        is_main_document = True, )
-                    ],
                 read_by_user_ids = [
                     ''
                     ],
                 variable_desks_ids = {
                     'key' : ''
                     },
                 detached_signatures_mapping = {
```

### Comparing `iparapheur-internal-1.11.5/test/test_current_user_api.py` & `iparapheur-internal-1.12.3/test/test_current_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_desk_api.py` & `iparapheur-internal-1.12.3/test/test_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_detached_signature.py` & `iparapheur-internal-1.12.3/test/test_detached_signature.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_document_dto.py` & `iparapheur-internal-1.12.3/test/test_document_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_error_response.py` & `iparapheur-internal-1.12.3/test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_external_signature_config.py` & `iparapheur-internal-1.12.3/test/test_external_signature_config_representation.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,51 +11,46 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.external_signature_config import ExternalSignatureConfig
+from iparapheur_internal.models.external_signature_config_representation import ExternalSignatureConfigRepresentation
 
-class TestExternalSignatureConfig(unittest.TestCase):
-    """ExternalSignatureConfig unit test stubs"""
+class TestExternalSignatureConfigRepresentation(unittest.TestCase):
+    """ExternalSignatureConfigRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ExternalSignatureConfig:
-        """Test ExternalSignatureConfig
+    def make_instance(self, include_optional) -> ExternalSignatureConfigRepresentation:
+        """Test ExternalSignatureConfigRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ExternalSignatureConfig`
+        # uncomment below to create an instance of `ExternalSignatureConfigRepresentation`
         """
-        model = ExternalSignatureConfig()
+        model = ExternalSignatureConfigRepresentation()
         if include_optional:
-            return ExternalSignatureConfig(
+            return ExternalSignatureConfigRepresentation(
                 id = '',
-                name = '',
+                name = '01',
                 service_name = 'YOUSIGN_V2',
                 url = '',
-                token = '',
-                password = '',
-                login = '',
-                transaction_ids = [
-                    ''
-                    ]
+                login = ''
             )
         else:
-            return ExternalSignatureConfig(
+            return ExternalSignatureConfigRepresentation(
         )
         """
 
-    def testExternalSignatureConfig(self):
-        """Test ExternalSignatureConfig"""
+    def testExternalSignatureConfigRepresentation(self):
+        """Test ExternalSignatureConfigRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_external_signature_config_representation.py` & `iparapheur-internal-1.12.3/test/test_hierarchised_desk_representation.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,46 +11,47 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.external_signature_config_representation import ExternalSignatureConfigRepresentation
+from iparapheur_internal.models.hierarchised_desk_representation import HierarchisedDeskRepresentation
 
-class TestExternalSignatureConfigRepresentation(unittest.TestCase):
-    """ExternalSignatureConfigRepresentation unit test stubs"""
+class TestHierarchisedDeskRepresentation(unittest.TestCase):
+    """HierarchisedDeskRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ExternalSignatureConfigRepresentation:
-        """Test ExternalSignatureConfigRepresentation
+    def make_instance(self, include_optional) -> HierarchisedDeskRepresentation:
+        """Test HierarchisedDeskRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ExternalSignatureConfigRepresentation`
+        # uncomment below to create an instance of `HierarchisedDeskRepresentation`
         """
-        model = ExternalSignatureConfigRepresentation()
+        model = HierarchisedDeskRepresentation()
         if include_optional:
-            return ExternalSignatureConfigRepresentation(
+            return HierarchisedDeskRepresentation(
                 id = '',
-                name = '01',
-                service_name = 'YOUSIGN_V2',
-                url = '',
-                login = ''
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+                tenant_id = '',
+                direct_children_count = 56,
+                level = 56
             )
         else:
-            return ExternalSignatureConfigRepresentation(
+            return HierarchisedDeskRepresentation(
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
         )
         """
 
-    def testExternalSignatureConfigRepresentation(self):
-        """Test ExternalSignatureConfigRepresentation"""
+    def testHierarchisedDeskRepresentation(self):
+        """Test HierarchisedDeskRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_external_signature_provider.py` & `iparapheur-internal-1.12.3/test/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_external_state.py` & `iparapheur-internal-1.12.3/test/test_external_state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_folder_api.py` & `iparapheur-internal-1.12.3/test/test_folder_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_folder_dto.py` & `iparapheur-internal-1.12.3/test/test_folder_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -259,89 +259,14 @@
                                 name = '', 
                                 issuer_name = '', )
                             ], 
                         signature_proof = True, 
                         deletable = True, 
                         is_main_document = True, )
                     ],
-                signature_proof_list = [
-                    iparapheur_internal.models.signature_proof.SignatureProof(
-                        id = '', 
-                        name = '', 
-                        index = 56, 
-                        page_count = 56, 
-                        content_length = 56, 
-                        media_type = iparapheur_internal.models.media_type.MediaType(
-                            type = '', 
-                            subtype = '', 
-                            parameters = {
-                                'key' : ''
-                                }, 
-                            quality_value = 1.337, 
-                            wildcard_type = True, 
-                            wildcard_subtype = True, 
-                            subtype_suffix = '', 
-                            charset = '', 
-                            concrete = True, ), 
-                        pages_properties = {
-                            'key' : iparapheur_internal.models.page_info.PageInfo(
-                                width = 1.337, 
-                                height = 1.337, 
-                                rotation = 56, )
-                            }, 
-                        pdf_visual_id = '', 
-                        signature_placement_annotations = [
-                            iparapheur_internal.models.signature_placement.SignaturePlacement(
-                                id = '', 
-                                page = 1, 
-                                width = 15, 
-                                height = 15, 
-                                x = 56, 
-                                y = 56, 
-                                page_rotation = 0, 
-                                page_width = 276, 
-                                page_height = 308, 
-                                rectangle_origin = 'TOP_RIGHT', 
-                                signature_number = 0, 
-                                template_type = 'MAIL_NOTIFICATION_SINGLE', )
-                            ], 
-                        signature_tags = {
-                            'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
-                                x = 1.337, 
-                                y = 1.337, 
-                                page = 56, )
-                            }, 
-                        seal_tags = {
-                            'key' : iparapheur_internal.models.pdf_signature_position.PdfSignaturePosition(
-                                x = 1.337, 
-                                y = 1.337, 
-                                page = 56, )
-                            }, 
-                        detached_signatures = [
-                            iparapheur_internal.models.detached_signature.DetachedSignature(
-                                id = '', 
-                                name = '', 
-                                content_length = 56, 
-                                target_document_id = '', 
-                                target_task_id = '', )
-                            ], 
-                        embedded_signature_infos = [
-                            iparapheur_internal.models.signature_info.SignatureInfo(
-                                signature_date_time = 56, 
-                                is_signature_valid = True, 
-                                name = '', 
-                                issuer_name = '', )
-                            ], 
-                        proof_target_task_id = '', 
-                        error_message = '', 
-                        internal = True, 
-                        signature_proof = True, 
-                        deletable = True, 
-                        is_main_document = True, )
-                    ],
                 read_by_user_ids = [
                     ''
                     ],
                 read_by_current_user = True
             )
         else:
             return FolderDto(
```

### Comparing `iparapheur-internal-1.11.5/test/test_folder_filter_dto.py` & `iparapheur-internal-1.12.3/test/test_folder_filter_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_folder_listable_dto.py` & `iparapheur-internal-1.12.3/test/test_folder_listable_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_folder_sort_by.py` & `iparapheur-internal-1.12.3/test/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_folder_visibility.py` & `iparapheur-internal-1.12.3/test/test_folder_visibility.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_application.py` & `iparapheur-internal-1.12.3/test/test_gdpr_application.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_cookie.py` & `iparapheur-internal-1.12.3/test/test_gdpr_cookie.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_data_element.py` & `iparapheur-internal-1.12.3/test/test_gdpr_data_element.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_data_set.py` & `iparapheur-internal-1.12.3/test/test_gdpr_data_set.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_declaring_entity.py` & `iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_declaring_entity_dpo.py` & `iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_dpo.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_declaring_entity_responsible.py` & `iparapheur-internal-1.12.3/test/test_gdpr_declaring_entity_responsible.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_entity.py` & `iparapheur-internal-1.12.3/test/test_page_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,44 +11,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.gdpr_entity import GdprEntity
+from iparapheur_internal.models.page_info import PageInfo
 
-class TestGdprEntity(unittest.TestCase):
-    """GdprEntity unit test stubs"""
+class TestPageInfo(unittest.TestCase):
+    """PageInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> GdprEntity:
-        """Test GdprEntity
+    def make_instance(self, include_optional) -> PageInfo:
+        """Test PageInfo
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GdprEntity`
+        # uncomment below to create an instance of `PageInfo`
         """
-        model = GdprEntity()
+        model = PageInfo()
         if include_optional:
-            return GdprEntity(
-                name = '',
-                address = '',
-                siret = ''
+            return PageInfo(
+                width = 1.337,
+                height = 1.337,
+                rotation = 56
             )
         else:
-            return GdprEntity(
+            return PageInfo(
         )
         """
 
-    def testGdprEntity(self):
-        """Test GdprEntity"""
+    def testPageInfo(self):
+        """Test PageInfo"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_gdpr_information_details_dto.py` & `iparapheur-internal-1.12.3/test/test_gdpr_information_details_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_page_hierarchised_desk_representation.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,47 +11,71 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.hierarchised_desk_representation import HierarchisedDeskRepresentation
+from iparapheur_internal.models.page_hierarchised_desk_representation import PageHierarchisedDeskRepresentation
 
-class TestHierarchisedDeskRepresentation(unittest.TestCase):
-    """HierarchisedDeskRepresentation unit test stubs"""
+class TestPageHierarchisedDeskRepresentation(unittest.TestCase):
+    """PageHierarchisedDeskRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> HierarchisedDeskRepresentation:
-        """Test HierarchisedDeskRepresentation
+    def make_instance(self, include_optional) -> PageHierarchisedDeskRepresentation:
+        """Test PageHierarchisedDeskRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `HierarchisedDeskRepresentation`
+        # uncomment below to create an instance of `PageHierarchisedDeskRepresentation`
         """
-        model = HierarchisedDeskRepresentation()
+        model = PageHierarchisedDeskRepresentation()
         if include_optional:
-            return HierarchisedDeskRepresentation(
-                id = '',
-                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
-                tenant_id = '',
-                direct_children_count = 56,
-                level = 56
+            return PageHierarchisedDeskRepresentation(
+                total_elements = 56,
+                total_pages = 56,
+                size = 56,
+                content = [
+                    iparapheur_internal.models.hierarchised_desk_representation.HierarchisedDeskRepresentation(
+                        id = '', 
+                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                        tenant_id = '', 
+                        direct_children_count = 56, 
+                        level = 56, )
+                    ],
+                number = 56,
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
+                first = True,
+                last = True,
+                number_of_elements = 56,
+                pageable = iparapheur_internal.models.pageable_object.PageableObject(
+                    offset = 56, 
+                    sort = iparapheur_internal.models.sort_object.SortObject(
+                        empty = True, 
+                        sorted = True, 
+                        unsorted = True, ), 
+                    page_size = 56, 
+                    paged = True, 
+                    page_number = 56, 
+                    unpaged = True, ),
+                empty = True
             )
         else:
-            return HierarchisedDeskRepresentation(
-                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+            return PageHierarchisedDeskRepresentation(
         )
         """
 
-    def testHierarchisedDeskRepresentation(self):
-        """Test HierarchisedDeskRepresentation"""
+    def testPageHierarchisedDeskRepresentation(self):
+        """Test PageHierarchisedDeskRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_layer_dto.py` & `iparapheur-internal-1.12.3/test/test_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_layer_representation.py` & `iparapheur-internal-1.12.3/test/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_mail_template_test_request.py` & `iparapheur-internal-1.12.3/test/test_mail_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_media_type.py` & `iparapheur-internal-1.12.3/test/test_media_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_metadata.py` & `iparapheur-internal-1.12.3/test/test_stamp_dto.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,49 +11,51 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.metadata import Metadata
+from iparapheur_internal.models.stamp_dto import StampDto
 
-class TestMetadata(unittest.TestCase):
-    """Metadata unit test stubs"""
+class TestStampDto(unittest.TestCase):
+    """StampDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Metadata:
-        """Test Metadata
+    def make_instance(self, include_optional) -> StampDto:
+        """Test StampDto
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Metadata`
+        # uncomment below to create an instance of `StampDto`
         """
-        model = Metadata()
+        model = StampDto()
         if include_optional:
-            return Metadata(
+            return StampDto(
                 id = '',
-                key = '',
-                name = '',
-                index = 56,
-                type = 'TEXT',
-                restricted_values = [
-                    ''
-                    ]
+                page = 56,
+                x = 56,
+                y = 56,
+                signature_rank = 56,
+                after_signature = True,
+                type = 'SIGNATURE',
+                value = '',
+                font_size = 56,
+                text_color = 'BLACK'
             )
         else:
-            return Metadata(
+            return StampDto(
         )
         """
 
-    def testMetadata(self):
-        """Test Metadata"""
+    def testStampDto(self):
+        """Test StampDto"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_metadata_dto.py` & `iparapheur-internal-1.12.3/test/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_metadata_type.py` & `iparapheur-internal-1.12.3/test/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_page_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_page_folder_dto.py` & `iparapheur-internal-1.12.3/test/test_page_folder_dto.py`

 * *Files 6% similar despite different names*

```diff
@@ -234,29 +234,14 @@
                                         name = '', 
                                         issuer_name = '', )
                                     ], 
                                 signature_proof = True, 
                                 deletable = True, 
                                 is_main_document = True, )
                             ], 
-                        signature_proof_list = [
-                            iparapheur_internal.models.signature_proof.SignatureProof(
-                                id = '', 
-                                name = '', 
-                                index = 56, 
-                                page_count = 56, 
-                                content_length = 56, 
-                                pdf_visual_id = '', 
-                                proof_target_task_id = '', 
-                                error_message = '', 
-                                internal = True, 
-                                signature_proof = True, 
-                                deletable = True, 
-                                is_main_document = True, )
-                            ], 
                         read_by_user_ids = [
                             ''
                             ], 
                         read_by_current_user = True, )
                     ],
                 number = 56,
                 sort = iparapheur_internal.models.sort_object.SortObject(
```

### Comparing `iparapheur-internal-1.11.5/test/test_page_folder_listable_dto.py` & `iparapheur-internal-1.12.3/test/test_page_folder_listable_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_page_hierarchised_desk_representation.py` & `iparapheur-internal-1.12.3/test/test_page_layer_representation.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,45 +11,42 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_hierarchised_desk_representation import PageHierarchisedDeskRepresentation
+from iparapheur_internal.models.page_layer_representation import PageLayerRepresentation
 
-class TestPageHierarchisedDeskRepresentation(unittest.TestCase):
-    """PageHierarchisedDeskRepresentation unit test stubs"""
+class TestPageLayerRepresentation(unittest.TestCase):
+    """PageLayerRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageHierarchisedDeskRepresentation:
-        """Test PageHierarchisedDeskRepresentation
+    def make_instance(self, include_optional) -> PageLayerRepresentation:
+        """Test PageLayerRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageHierarchisedDeskRepresentation`
+        # uncomment below to create an instance of `PageLayerRepresentation`
         """
-        model = PageHierarchisedDeskRepresentation()
+        model = PageLayerRepresentation()
         if include_optional:
-            return PageHierarchisedDeskRepresentation(
+            return PageLayerRepresentation(
                 total_elements = 56,
                 total_pages = 56,
                 size = 56,
                 content = [
-                    iparapheur_internal.models.hierarchised_desk_representation.HierarchisedDeskRepresentation(
+                    iparapheur_internal.models.layer_representation.LayerRepresentation(
                         id = '', 
-                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
-                        tenant_id = '', 
-                        direct_children_count = 56, 
-                        level = 56, )
+                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', )
                     ],
                 number = 56,
                 sort = iparapheur_internal.models.sort_object.SortObject(
                     empty = True, 
                     sorted = True, 
                     unsorted = True, ),
                 first = True,
@@ -64,18 +61,18 @@
                     page_size = 56, 
                     paged = True, 
                     page_number = 56, 
                     unpaged = True, ),
                 empty = True
             )
         else:
-            return PageHierarchisedDeskRepresentation(
+            return PageLayerRepresentation(
         )
         """
 
-    def testPageHierarchisedDeskRepresentation(self):
-        """Test PageHierarchisedDeskRepresentation"""
+    def testPageLayerRepresentation(self):
+        """Test PageLayerRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_page_info.py` & `iparapheur-internal-1.12.3/test/test_pageable_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,44 +11,50 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_info import PageInfo
+from iparapheur_internal.models.pageable_object import PageableObject
 
-class TestPageInfo(unittest.TestCase):
-    """PageInfo unit test stubs"""
+class TestPageableObject(unittest.TestCase):
+    """PageableObject unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageInfo:
-        """Test PageInfo
+    def make_instance(self, include_optional) -> PageableObject:
+        """Test PageableObject
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageInfo`
+        # uncomment below to create an instance of `PageableObject`
         """
-        model = PageInfo()
+        model = PageableObject()
         if include_optional:
-            return PageInfo(
-                width = 1.337,
-                height = 1.337,
-                rotation = 56
+            return PageableObject(
+                offset = 56,
+                sort = iparapheur_internal.models.sort_object.SortObject(
+                    empty = True, 
+                    sorted = True, 
+                    unsorted = True, ),
+                page_size = 56,
+                paged = True,
+                page_number = 56,
+                unpaged = True
             )
         else:
-            return PageInfo(
+            return PageableObject(
         )
         """
 
-    def testPageInfo(self):
-        """Test PageInfo"""
+    def testPageableObject(self):
+        """Test PageableObject"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_page_layer_representation.py` & `iparapheur-internal-1.12.3/test/test_sort_object.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,68 +11,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.page_layer_representation import PageLayerRepresentation
+from iparapheur_internal.models.sort_object import SortObject
 
-class TestPageLayerRepresentation(unittest.TestCase):
-    """PageLayerRepresentation unit test stubs"""
+class TestSortObject(unittest.TestCase):
+    """SortObject unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageLayerRepresentation:
-        """Test PageLayerRepresentation
+    def make_instance(self, include_optional) -> SortObject:
+        """Test SortObject
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageLayerRepresentation`
+        # uncomment below to create an instance of `SortObject`
         """
-        model = PageLayerRepresentation()
+        model = SortObject()
         if include_optional:
-            return PageLayerRepresentation(
-                total_elements = 56,
-                total_pages = 56,
-                size = 56,
-                content = [
-                    iparapheur_internal.models.layer_representation.LayerRepresentation(
-                        id = '', 
-                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', )
-                    ],
-                number = 56,
-                sort = iparapheur_internal.models.sort_object.SortObject(
-                    empty = True, 
-                    sorted = True, 
-                    unsorted = True, ),
-                first = True,
-                last = True,
-                number_of_elements = 56,
-                pageable = iparapheur_internal.models.pageable_object.PageableObject(
-                    offset = 56, 
-                    sort = iparapheur_internal.models.sort_object.SortObject(
-                        empty = True, 
-                        sorted = True, 
-                        unsorted = True, ), 
-                    page_size = 56, 
-                    paged = True, 
-                    page_number = 56, 
-                    unpaged = True, ),
-                empty = True
+            return SortObject(
+                empty = True,
+                sorted = True,
+                unsorted = True
             )
         else:
-            return PageLayerRepresentation(
+            return SortObject(
         )
         """
 
-    def testPageLayerRepresentation(self):
-        """Test PageLayerRepresentation"""
+    def testSortObject(self):
+        """Test SortObject"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_page_subtype_representation.py` & `iparapheur-internal-1.12.3/test/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_page_typology_representation.py` & `iparapheur-internal-1.12.3/test/test_page_typology_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_pageable_object.py` & `iparapheur-internal-1.12.3/test/test_tenant_representation.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,50 +11,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.pageable_object import PageableObject
+from iparapheur_internal.models.tenant_representation import TenantRepresentation
 
-class TestPageableObject(unittest.TestCase):
-    """PageableObject unit test stubs"""
+class TestTenantRepresentation(unittest.TestCase):
+    """TenantRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> PageableObject:
-        """Test PageableObject
+    def make_instance(self, include_optional) -> TenantRepresentation:
+        """Test TenantRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `PageableObject`
+        # uncomment below to create an instance of `TenantRepresentation`
         """
-        model = PageableObject()
+        model = TenantRepresentation()
         if include_optional:
-            return PageableObject(
-                offset = 56,
-                sort = iparapheur_internal.models.sort_object.SortObject(
-                    empty = True, 
-                    sorted = True, 
-                    unsorted = True, ),
-                page_size = 56,
-                paged = True,
-                page_number = 56,
-                unpaged = True
+            return TenantRepresentation(
+                id = '',
+                name = 'Example tenant'
             )
         else:
-            return PageableObject(
+            return TenantRepresentation(
+                name = 'Example tenant',
         )
         """
 
-    def testPageableObject(self):
-        """Test PageableObject"""
+    def testTenantRepresentation(self):
+        """Test TenantRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_password_policies.py` & `iparapheur-internal-1.12.3/test/test_password_policies.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_pdf_signature_position.py` & `iparapheur-internal-1.12.3/test/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_pdf_template_test_request.py` & `iparapheur-internal-1.12.3/test/test_pdf_template_test_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_seal_certificate_representation.py` & `iparapheur-internal-1.12.3/test/test_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_server_info_api.py` & `iparapheur-internal-1.12.3/test/test_server_info_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_signature_format.py` & `iparapheur-internal-1.12.3/test/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_signature_info.py` & `iparapheur-internal-1.12.3/test/test_signature_info.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_signature_placement.py` & `iparapheur-internal-1.12.3/test/test_signature_placement.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_signature_protocol.py` & `iparapheur-internal-1.12.3/test/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_stamp_dto.py` & `iparapheur-internal-1.12.3/test/test_user_representation.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,51 +11,53 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.stamp_dto import StampDto
+from iparapheur_internal.models.user_representation import UserRepresentation
 
-class TestStampDto(unittest.TestCase):
-    """StampDto unit test stubs"""
+class TestUserRepresentation(unittest.TestCase):
+    """UserRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> StampDto:
-        """Test StampDto
+    def make_instance(self, include_optional) -> UserRepresentation:
+        """Test UserRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `StampDto`
+        # uncomment below to create an instance of `UserRepresentation`
         """
-        model = StampDto()
+        model = UserRepresentation()
         if include_optional:
-            return StampDto(
+            return UserRepresentation(
                 id = '',
-                page = 56,
-                x = 56,
-                y = 56,
-                signature_rank = 56,
-                after_signature = True,
-                type = 'SIGNATURE',
-                value = '',
-                font_size = 56,
-                text_color = 'BLACK'
+                user_name = '0',
+                first_name = '',
+                last_name = '',
+                email = '',
+                privilege = 'NONE',
+                is_ldap_synchronized = True
             )
         else:
-            return StampDto(
+            return UserRepresentation(
+                user_name = '0',
+                first_name = '',
+                last_name = '',
+                email = '',
+                privilege = 'NONE',
         )
         """
 
-    def testStampDto(self):
-        """Test StampDto"""
+    def testUserRepresentation(self):
+        """Test UserRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_stamp_text_color.py` & `iparapheur-internal-1.12.3/test/test_stamp_text_color.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_stamp_type.py` & `iparapheur-internal-1.12.3/test/test_stamp_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_state.py` & `iparapheur-internal-1.12.3/test/test_state.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_step_definition_dto.py` & `iparapheur-internal-1.12.3/test/test_step_definition_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_step_definition_parallel_type.py` & `iparapheur-internal-1.12.3/test/test_step_definition_parallel_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_step_definition_type.py` & `iparapheur-internal-1.12.3/test/test_step_definition_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_subtype.py` & `iparapheur-internal-1.12.3/test/test_subtype_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,96 +11,112 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.subtype import Subtype
+from iparapheur_internal.models.subtype_dto import SubtypeDto
 
-class TestSubtype(unittest.TestCase):
-    """Subtype unit test stubs"""
+class TestSubtypeDto(unittest.TestCase):
+    """SubtypeDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Subtype:
-        """Test Subtype
+    def make_instance(self, include_optional) -> SubtypeDto:
+        """Test SubtypeDto
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Subtype`
+        # uncomment below to create an instance of `SubtypeDto`
         """
-        model = Subtype()
+        model = SubtypeDto()
         if include_optional:
-            return Subtype(
+            return SubtypeDto(
                 id = '',
-                name = '',
-                description = '',
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+                description = '012',
                 creation_workflow_id = '',
                 validation_workflow_id = '',
                 workflow_selection_script = '',
                 annotations_allowed = True,
                 external_signature_automatic = True,
-                max_main_documents = 56,
                 secure_mail_server_id = 56,
                 seal_certificate_id = '',
-                external_signature_config = iparapheur_internal.models.external_signature_config.ExternalSignatureConfig(
+                seal_certificate = iparapheur_internal.models.seal_certificate_representation.SealCertificateRepresentation(
                     id = '', 
-                    name = '', 
-                    service_name = 'YOUSIGN_V2', 
-                    url = '', 
-                    token = '', 
-                    password = '', 
-                    login = '', 
-                    transaction_ids = [
-                        ''
-                        ], ),
+                    name = 'Example certificate', 
+                    expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    usage_count = 56, ),
                 subtype_metadata_list = [
-                    iparapheur_internal.models.subtype_metadata.SubtypeMetadata(
-                        id = iparapheur_internal.models.composite_id.CompositeId(
-                            layer_id = '', ), 
-                        metadata = iparapheur_internal.models.metadata.Metadata(
-                            key = '', 
-                            name = '', 
+                    iparapheur_internal.models.subtype_metadata_dto.SubtypeMetadataDto(
+                        metadata_id = '', 
+                        metadata = iparapheur_internal.models.metadata_dto.MetadataDto(
+                            id = '', 
+                            name = 'Example metadata', 
+                            key = 'example_metadata', 
                             index = 56, 
                             type = 'TEXT', 
                             restricted_values = [
                                 ''
                                 ], ), 
                         default_value = '', 
                         mandatory = True, 
                         editable = True, )
                     ],
                 subtype_layers = [
-                    iparapheur_internal.models.subtype_layer.SubtypeLayer(
-                        id = iparapheur_internal.models.composite_id.CompositeId(
-                            layer_id = '', ), 
+                    iparapheur_internal.models.subtype_layer_dto.SubtypeLayerDto(
+                        layer_id = '', 
+                        layer = iparapheur_internal.models.layer_representation.LayerRepresentation(
+                            id = '', 
+                            name = 'jXAuKb%@;_5)#fEb-bx%oZ01', ), 
                         association = 'ALL', )
                     ],
+                external_signature_config_id = '',
+                external_signature_config = iparapheur_internal.models.external_signature_config_representation.ExternalSignatureConfigRepresentation(
+                    id = '', 
+                    name = '01', 
+                    service_name = 'YOUSIGN_V2', 
+                    url = '', 
+                    login = '', ),
                 creation_permitted_desk_ids = [
                     ''
                     ],
+                creation_permitted_desks = [
+                    iparapheur_internal.models.desk_representation.DeskRepresentation(
+                        id = '', 
+                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                        tenant_id = '', )
+                    ],
                 filterable_by_desk_ids = [
                     ''
                     ],
+                filterable_by_desks = [
+                    iparapheur_internal.models.desk_representation.DeskRepresentation(
+                        id = '', 
+                        name = 'jXAuKb%@;_5)#fEb-bx%oZ01', 
+                        tenant_id = '', )
+                    ],
+                max_main_documents = 56,
                 multi_documents = True,
                 annexe_included = True,
                 digital_signature_mandatory = True,
                 reading_mandatory = True,
                 seal_automatic = True
             )
         else:
-            return Subtype(
+            return SubtypeDto(
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
         )
         """
 
-    def testSubtype(self):
-        """Test Subtype"""
+    def testSubtypeDto(self):
+        """Test SubtypeDto"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_subtype_layer.py` & `iparapheur-internal-1.12.3/test/test_subtype_layer_dto.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,44 +11,46 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.subtype_layer import SubtypeLayer
+from iparapheur_internal.models.subtype_layer_dto import SubtypeLayerDto
 
-class TestSubtypeLayer(unittest.TestCase):
-    """SubtypeLayer unit test stubs"""
+class TestSubtypeLayerDto(unittest.TestCase):
+    """SubtypeLayerDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SubtypeLayer:
-        """Test SubtypeLayer
+    def make_instance(self, include_optional) -> SubtypeLayerDto:
+        """Test SubtypeLayerDto
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SubtypeLayer`
+        # uncomment below to create an instance of `SubtypeLayerDto`
         """
-        model = SubtypeLayer()
+        model = SubtypeLayerDto()
         if include_optional:
-            return SubtypeLayer(
-                id = iparapheur_internal.models.composite_id.CompositeId(
-                    layer_id = '', ),
+            return SubtypeLayerDto(
+                layer_id = '',
+                layer = iparapheur_internal.models.layer_representation.LayerRepresentation(
+                    id = '', 
+                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', ),
                 association = 'ALL'
             )
         else:
-            return SubtypeLayer(
+            return SubtypeLayerDto(
         )
         """
 
-    def testSubtypeLayer(self):
-        """Test SubtypeLayer"""
+    def testSubtypeLayerDto(self):
+        """Test SubtypeLayerDto"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_subtype_layer_association.py` & `iparapheur-internal-1.12.3/test/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_subtype_layer_dto.py` & `iparapheur-internal-1.12.3/test/test_subtype_representation.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,46 +11,44 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.subtype_layer_dto import SubtypeLayerDto
+from iparapheur_internal.models.subtype_representation import SubtypeRepresentation
 
-class TestSubtypeLayerDto(unittest.TestCase):
-    """SubtypeLayerDto unit test stubs"""
+class TestSubtypeRepresentation(unittest.TestCase):
+    """SubtypeRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SubtypeLayerDto:
-        """Test SubtypeLayerDto
+    def make_instance(self, include_optional) -> SubtypeRepresentation:
+        """Test SubtypeRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SubtypeLayerDto`
+        # uncomment below to create an instance of `SubtypeRepresentation`
         """
-        model = SubtypeLayerDto()
+        model = SubtypeRepresentation()
         if include_optional:
-            return SubtypeLayerDto(
-                layer_id = '',
-                layer = iparapheur_internal.models.layer_representation.LayerRepresentation(
-                    id = '', 
-                    name = 'jXAuKb%@;_5)#fEb-bx%oZ01', ),
-                association = 'ALL'
+            return SubtypeRepresentation(
+                id = '',
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01'
             )
         else:
-            return SubtypeLayerDto(
+            return SubtypeRepresentation(
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
         )
         """
 
-    def testSubtypeLayerDto(self):
-        """Test SubtypeLayerDto"""
+    def testSubtypeRepresentation(self):
+        """Test SubtypeRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_subtype_metadata.py` & `iparapheur-internal-1.12.3/test/test_subtype_metadata_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,55 +11,54 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.subtype_metadata import SubtypeMetadata
+from iparapheur_internal.models.subtype_metadata_dto import SubtypeMetadataDto
 
-class TestSubtypeMetadata(unittest.TestCase):
-    """SubtypeMetadata unit test stubs"""
+class TestSubtypeMetadataDto(unittest.TestCase):
+    """SubtypeMetadataDto unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SubtypeMetadata:
-        """Test SubtypeMetadata
+    def make_instance(self, include_optional) -> SubtypeMetadataDto:
+        """Test SubtypeMetadataDto
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SubtypeMetadata`
+        # uncomment below to create an instance of `SubtypeMetadataDto`
         """
-        model = SubtypeMetadata()
+        model = SubtypeMetadataDto()
         if include_optional:
-            return SubtypeMetadata(
-                id = iparapheur_internal.models.composite_id.CompositeId(
-                    layer_id = '', ),
-                metadata = iparapheur_internal.models.metadata.Metadata(
+            return SubtypeMetadataDto(
+                metadata_id = '',
+                metadata = iparapheur_internal.models.metadata_dto.MetadataDto(
                     id = '', 
-                    key = '', 
-                    name = '', 
+                    name = 'Example metadata', 
+                    key = 'example_metadata', 
                     index = 56, 
                     type = 'TEXT', 
                     restricted_values = [
                         ''
                         ], ),
                 default_value = '',
                 mandatory = True,
                 editable = True
             )
         else:
-            return SubtypeMetadata(
+            return SubtypeMetadataDto(
         )
         """
 
-    def testSubtypeMetadata(self):
-        """Test SubtypeMetadata"""
+    def testSubtypeMetadataDto(self):
+        """Test SubtypeMetadataDto"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_subtype_representation.py` & `iparapheur-internal-1.12.3/test/test_typology_representation.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,44 +11,46 @@
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from iparapheur_internal.models.subtype_representation import SubtypeRepresentation
+from iparapheur_internal.models.typology_representation import TypologyRepresentation
 
-class TestSubtypeRepresentation(unittest.TestCase):
-    """SubtypeRepresentation unit test stubs"""
+class TestTypologyRepresentation(unittest.TestCase):
+    """TypologyRepresentation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SubtypeRepresentation:
-        """Test SubtypeRepresentation
+    def make_instance(self, include_optional) -> TypologyRepresentation:
+        """Test TypologyRepresentation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SubtypeRepresentation`
+        # uncomment below to create an instance of `TypologyRepresentation`
         """
-        model = SubtypeRepresentation()
+        model = TypologyRepresentation()
         if include_optional:
-            return SubtypeRepresentation(
+            return TypologyRepresentation(
                 id = '',
-                name = 'jXAuKb%@;_5)#fEb-bx%oZ01'
+                name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
+                parent_id = '',
+                children_count = 56
             )
         else:
-            return SubtypeRepresentation(
+            return TypologyRepresentation(
                 name = 'jXAuKb%@;_5)#fEb-bx%oZ01',
         )
         """
 
-    def testSubtypeRepresentation(self):
-        """Test SubtypeRepresentation"""
+    def testTypologyRepresentation(self):
+        """Test TypologyRepresentation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-internal-1.11.5/test/test_task.py` & `iparapheur-internal-1.12.3/test/test_task.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_template_api.py` & `iparapheur-internal-1.12.3/test/test_template_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_template_type.py` & `iparapheur-internal-1.12.3/test/test_template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_test_signature_template_request.py` & `iparapheur-internal-1.12.3/test/test_test_signature_template_request.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_type_dto.py` & `iparapheur-internal-1.12.3/test/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_typology_api.py` & `iparapheur-internal-1.12.3/test/test_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_user_dto.py` & `iparapheur-internal-1.12.3/test/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_user_privilege.py` & `iparapheur-internal-1.12.3/test/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_validation_service_configuration_dto.py` & `iparapheur-internal-1.12.3/test/test_validation_service_configuration_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-internal-1.11.5/test/test_workflow_definition_dto.py` & `iparapheur-internal-1.12.3/test/test_workflow_definition_dto.py`

 * *Files identical despite different names*

