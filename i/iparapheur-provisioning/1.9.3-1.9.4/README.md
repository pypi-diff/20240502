# Comparing `tmp/iparapheur-provisioning-1.9.3.tar.gz` & `tmp/iparapheur-provisioning-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.9.3.tar", last modified: Mon Oct 23 09:15:30 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.9.4.tar", last modified: Wed Oct 25 09:08:37 2023, max compression
```

## Comparing `iparapheur-provisioning-1.9.3.tar` & `iparapheur-provisioning-1.9.4.tar`

### file list

```diff
@@ -1,342 +1,342 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-10-23 09:15:05.000000 iparapheur-provisioning-1.9.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23088 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.007213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.007213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8817 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.011213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      261 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      315 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
--rw-r--r--   0 root         (0) root         (0)      490 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
--rw-r--r--   0 root         (0) root         (0)      338 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      210 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
--rw-r--r--   0 root         (0) root         (0)      264 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
--rw-r--r--   0 root         (0) root         (0)      255 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_templates_template_type.py
--rw-r--r--   0 root         (0) root         (0)      206 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.011213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      659 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_template_api.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6643 2023-10-23 09:14:30.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/certificate_informations.py
--rw-r--r--   0 root         (0) root         (0)    24041 2023-10-23 09:14:31.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-10-23 09:14:31.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7908 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9141 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     9205 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     9232 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     8300 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/seal_certificate_dto.py
--rw-r--r--   0 root         (0) root         (0)     4500 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    29448 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/template_type.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-10-23 09:14:39.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-10-23 09:14:39.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-10-23 09:14:39.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4499 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     4377 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     2934 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13070 2023-10-23 09:14:54.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-10-23 09:14:53.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-10-23 09:14:53.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-10-23 09:14:53.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-10-23 09:14:54.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11862 2023-10-23 09:14:43.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-10-23 09:14:43.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-10-23 09:14:43.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.019213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)      407 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15486 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
--rw-r--r--   0 root         (0) root         (0)    16907 2023-10-23 09:14:45.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)      431 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11938 2023-10-23 09:14:45.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-10-23 09:14:45.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16979 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
--rw-r--r--   0 root         (0) root         (0)      423 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14894 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
--rw-r--r--   0 root         (0) root         (0)    19934 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
--rw-r--r--   0 root         (0) root         (0)      463 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12091 2023-10-23 09:14:48.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    12371 2023-10-23 09:14:48.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
--rw-r--r--   0 root         (0) root         (0)    20252 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)      437 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11569 2023-10-23 09:14:51.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py
--rw-r--r--   0 root         (0) root         (0)    15581 2023-10-23 09:14:50.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py
--rw-r--r--   0 root         (0) root         (0)    15574 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-10-23 09:15:01.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-10-23 09:14:59.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-10-23 09:14:59.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-10-23 09:15:00.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-10-23 09:15:00.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-10-23 09:14:58.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.023213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-10-23 09:14:59.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-10-23 09:15:00.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-10-23 09:15:01.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-10-23 09:14:56.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    16306 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11932 2023-10-23 09:14:56.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
--rw-r--r--   0 root         (0) root         (0)      429 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15256 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
--rw-r--r--   0 root         (0) root         (0)      477 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12148 2023-10-23 09:15:03.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-10-23 09:14:41.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
--rw-r--r--   0 root         (0) root         (0)    13883 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-10-23 09:14:41.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-10-23 09:14:41.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)      391 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10817 2023-10-23 09:14:51.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.027213 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)      425 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11613 2023-10-23 09:14:51.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/get.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.007213 iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-10-23 09:15:29.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21063 2023-10-23 09:15:29.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-23 09:15:29.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-10-23 09:15:29.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-10-23 09:15:29.000000 iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.003213 iparapheur-provisioning-1.9.3/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-10-23 09:14:30.000000 iparapheur-provisioning-1.9.3/test/test_models/test_certificate_informations.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-10-23 09:14:31.000000 iparapheur-provisioning-1.9.3/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-10-23 09:14:31.000000 iparapheur-provisioning-1.9.3/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-10-23 09:14:32.000000 iparapheur-provisioning-1.9.3/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      751 2023-10-23 09:14:33.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      714 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-10-23 09:14:34.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      763 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/test/test_models/test_page_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-10-23 09:14:35.000000 iparapheur-provisioning-1.9.3/test/test_models/test_seal_certificate_dto.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/test/test_models/test_seal_certificate_representation.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-10-23 09:14:36.000000 iparapheur-provisioning-1.9.3/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-10-23 09:14:37.000000 iparapheur-provisioning-1.9.3/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_template_type.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-10-23 09:14:38.000000 iparapheur-provisioning-1.9.3/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-10-23 09:14:39.000000 iparapheur-provisioning-1.9.3/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-10-23 09:14:39.000000 iparapheur-provisioning-1.9.3/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/test/test_models/test_workflow_definition_representation.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-10-23 09:14:40.000000 iparapheur-provisioning-1.9.3/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      887 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-10-23 09:14:55.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-10-23 09:14:44.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.035213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-10-23 09:14:46.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-10-23 09:14:47.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.043213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      970 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.043213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1064 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1051 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-10-23 09:14:49.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.043213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.043213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.047213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.047213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.047213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1056 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-10-23 09:15:02.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.047213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.047213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-10-23 09:14:57.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.047213 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-10-23 09:15:04.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-10-23 09:14:42.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_templates_template_type/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-23 09:15:30.051214 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-10-23 09:14:52.000000 iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23088 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.818505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.822505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8817 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.822505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      261 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      315 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      490 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id.py
+-rw-r--r--   0 root         (0) root         (0)      338 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      210 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition.py
+-rw-r--r--   0 root         (0) root         (0)      264 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key.py
+-rw-r--r--   0 root         (0) root         (0)      255 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_templates_template_type.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.826505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      659 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_template_api.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.830505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6643 2023-10-25 09:07:51.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/certificate_informations.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-10-25 09:07:52.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7908 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9141 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9205 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     8300 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4500 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    29448 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/template_type.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-10-25 09:07:59.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-10-25 09:07:59.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-10-25 09:07:59.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4499 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.830505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     4377 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.830505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13070 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11862 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15486 2023-10-25 09:08:03.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py
+-rw-r--r--   0 root         (0) root         (0)    16907 2023-10-25 09:08:03.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)      431 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11938 2023-10-25 09:08:03.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-10-25 09:08:03.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16979 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14894 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py
+-rw-r--r--   0 root         (0) root         (0)    19934 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.834505 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)      463 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12091 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    12371 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    20252 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.838506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11569 2023-10-25 09:08:06.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py
+-rw-r--r--   0 root         (0) root         (0)    15581 2023-10-25 09:08:06.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py
+-rw-r--r--   0 root         (0) root         (0)    15574 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.838506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-10-25 09:08:13.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-10-25 09:08:11.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.838506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-10-25 09:08:11.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-10-25 09:08:12.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.838506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-10-25 09:08:12.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-10-25 09:08:11.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.838506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-10-25 09:08:11.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-10-25 09:08:12.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-10-25 09:08:13.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-10-25 09:08:09.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    16306 2023-10-25 09:08:09.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11932 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-10-25 09:08:09.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)      429 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15256 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12148 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    13883 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)      391 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10817 2023-10-25 09:08:06.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.842506 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)      425 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11613 2023-10-25 09:08:06.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.822505 iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-10-25 09:08:37.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21063 2023-10-25 09:08:37.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-25 09:08:37.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-10-25 09:08:37.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-10-25 09:08:37.000000 iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.818505 iparapheur-provisioning-1.9.4/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.850506 iparapheur-provisioning-1.9.4/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:16.000000 iparapheur-provisioning-1.9.4/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-10-25 09:07:51.000000 iparapheur-provisioning-1.9.4/test/test_models/test_certificate_informations.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-10-25 09:07:53.000000 iparapheur-provisioning-1.9.4/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-10-25 09:07:54.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      751 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      714 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-10-25 09:07:55.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      763 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_page_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_seal_certificate_dto.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_seal_certificate_representation.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-10-25 09:07:56.000000 iparapheur-provisioning-1.9.4/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-10-25 09:07:57.000000 iparapheur-provisioning-1.9.4/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_template_type.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-10-25 09:07:58.000000 iparapheur-provisioning-1.9.4/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-10-25 09:07:59.000000 iparapheur-provisioning-1.9.4/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-10-25 09:07:59.000000 iparapheur-provisioning-1.9.4/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-10-25 09:07:59.000000 iparapheur-provisioning-1.9.4/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/test/test_models/test_workflow_definition_representation.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-10-25 09:08:00.000000 iparapheur-provisioning-1.9.4/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.850506 iparapheur-provisioning-1.9.4/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.850506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      887 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.850506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-10-25 09:08:08.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.850506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-10-25 09:08:02.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-10-25 09:08:04.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-10-25 09:08:05.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.854506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-10-25 09:08:14.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-10-25 09:08:10.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-10-25 09:08:15.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-10-25 09:08:01.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_templates_template_type/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 09:08:37.858506 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-10-25 09:08:07.000000 iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/test_get.py
```

### Comparing `iparapheur-provisioning-1.9.3/LICENSE.md` & `iparapheur-provisioning-1.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/README.md` & `iparapheur-provisioning-1.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.9.3
+- Package version: 1.9.4
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.9.3"
+__version__ = "1.9.4"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.9.3/python'
+        self.user_agent = 'OpenAPI-Generator/1.9.4/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/__init__.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_metadata_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_metadata_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_seal_certificate_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_template_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_template_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/apis/tags/admin_workflow_definition_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.9.3".\
+               "SDK Package Version: 1.9.4".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/certificate_informations.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/certificate_informations.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_metadata_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_seal_certificate_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_tenant_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/page_workflow_definition_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/page_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/pageable_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,101 +34,101 @@
     """
 
 
     class MetaOapg:
         
         class properties:
             pageNumber = schemas.Int32Schema
-            paged = schemas.BoolSchema
-            pageSize = schemas.Int32Schema
             unpaged = schemas.BoolSchema
+            pageSize = schemas.Int32Schema
+            paged = schemas.BoolSchema
             offset = schemas.Int64Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
             __annotations__ = {
                 "pageNumber": pageNumber,
-                "paged": paged,
-                "pageSize": pageSize,
                 "unpaged": unpaged,
+                "pageSize": pageSize,
+                "paged": paged,
                 "offset": offset,
                 "sort": sort,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["pageNumber"]) -> MetaOapg.properties.pageNumber: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["paged"]) -> MetaOapg.properties.paged: ...
+    def __getitem__(self, name: typing_extensions.Literal["unpaged"]) -> MetaOapg.properties.unpaged: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["pageSize"]) -> MetaOapg.properties.pageSize: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["unpaged"]) -> MetaOapg.properties.unpaged: ...
+    def __getitem__(self, name: typing_extensions.Literal["paged"]) -> MetaOapg.properties.paged: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["offset"]) -> MetaOapg.properties.offset: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["pageNumber", "paged", "pageSize", "unpaged", "offset", "sort", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["pageNumber", "unpaged", "pageSize", "paged", "offset", "sort", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["pageNumber"]) -> typing.Union[MetaOapg.properties.pageNumber, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["paged"]) -> typing.Union[MetaOapg.properties.paged, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["unpaged"]) -> typing.Union[MetaOapg.properties.unpaged, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["pageSize"]) -> typing.Union[MetaOapg.properties.pageSize, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["unpaged"]) -> typing.Union[MetaOapg.properties.unpaged, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["paged"]) -> typing.Union[MetaOapg.properties.paged, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["offset"]) -> typing.Union[MetaOapg.properties.offset, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["pageNumber", "paged", "pageSize", "unpaged", "offset", "sort", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["pageNumber", "unpaged", "pageSize", "paged", "offset", "sort", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         pageNumber: typing.Union[MetaOapg.properties.pageNumber, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        paged: typing.Union[MetaOapg.properties.paged, bool, schemas.Unset] = schemas.unset,
-        pageSize: typing.Union[MetaOapg.properties.pageSize, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         unpaged: typing.Union[MetaOapg.properties.unpaged, bool, schemas.Unset] = schemas.unset,
+        pageSize: typing.Union[MetaOapg.properties.pageSize, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        paged: typing.Union[MetaOapg.properties.paged, bool, schemas.Unset] = schemas.unset,
         offset: typing.Union[MetaOapg.properties.offset, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageableObject':
         return super().__new__(
             cls,
             *_args,
             pageNumber=pageNumber,
-            paged=paged,
-            pageSize=pageSize,
             unpaged=unpaged,
+            pageSize=pageSize,
+            paged=paged,
             offset=offset,
             sort=sort,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/seal_certificate_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/seal_certificate_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/seal_certificate_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,18 +374,18 @@
                 ) -> 'filterableByDesks':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
             maxMainDocuments = schemas.Int32Schema
-            sealAutomatic = schemas.BoolSchema
-            readingMandatory = schemas.BoolSchema
             digitalSignatureMandatory = schemas.BoolSchema
+            readingMandatory = schemas.BoolSchema
             annexeIncluded = schemas.BoolSchema
+            sealAutomatic = schemas.BoolSchema
             multiDocuments = schemas.BoolSchema
             __annotations__ = {
                 "name": name,
                 "id": id,
                 "description": description,
                 "creationWorkflowId": creationWorkflowId,
                 "validationWorkflowId": validationWorkflowId,
@@ -400,18 +400,18 @@
                 "externalSignatureConfigId": externalSignatureConfigId,
                 "externalSignatureConfig": externalSignatureConfig,
                 "creationPermittedDeskIds": creationPermittedDeskIds,
                 "creationPermittedDesks": creationPermittedDesks,
                 "filterableByDeskIds": filterableByDeskIds,
                 "filterableByDesks": filterableByDesks,
                 "maxMainDocuments": maxMainDocuments,
-                "sealAutomatic": sealAutomatic,
-                "readingMandatory": readingMandatory,
                 "digitalSignatureMandatory": digitalSignatureMandatory,
+                "readingMandatory": readingMandatory,
                 "annexeIncluded": annexeIncluded,
+                "sealAutomatic": sealAutomatic,
                 "multiDocuments": multiDocuments,
             }
     
     name: MetaOapg.properties.name
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
@@ -470,32 +470,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["filterableByDesks"]) -> MetaOapg.properties.filterableByDesks: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["maxMainDocuments"]) -> MetaOapg.properties.maxMainDocuments: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sealAutomatic"]) -> MetaOapg.properties.sealAutomatic: ...
+    def __getitem__(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> MetaOapg.properties.digitalSignatureMandatory: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["readingMandatory"]) -> MetaOapg.properties.readingMandatory: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> MetaOapg.properties.digitalSignatureMandatory: ...
+    def __getitem__(self, name: typing_extensions.Literal["annexeIncluded"]) -> MetaOapg.properties.annexeIncluded: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["annexeIncluded"]) -> MetaOapg.properties.annexeIncluded: ...
+    def __getitem__(self, name: typing_extensions.Literal["sealAutomatic"]) -> MetaOapg.properties.sealAutomatic: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["multiDocuments"]) -> MetaOapg.properties.multiDocuments: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "sealCertificate", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "sealAutomatic", "readingMandatory", "digitalSignatureMandatory", "annexeIncluded", "multiDocuments", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "sealCertificate", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "digitalSignatureMandatory", "readingMandatory", "annexeIncluded", "sealAutomatic", "multiDocuments", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
@@ -553,32 +553,32 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["filterableByDesks"]) -> typing.Union[MetaOapg.properties.filterableByDesks, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["maxMainDocuments"]) -> typing.Union[MetaOapg.properties.maxMainDocuments, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sealAutomatic"]) -> typing.Union[MetaOapg.properties.sealAutomatic, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> typing.Union[MetaOapg.properties.digitalSignatureMandatory, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["readingMandatory"]) -> typing.Union[MetaOapg.properties.readingMandatory, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> typing.Union[MetaOapg.properties.digitalSignatureMandatory, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["annexeIncluded"]) -> typing.Union[MetaOapg.properties.annexeIncluded, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["annexeIncluded"]) -> typing.Union[MetaOapg.properties.annexeIncluded, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sealAutomatic"]) -> typing.Union[MetaOapg.properties.sealAutomatic, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["multiDocuments"]) -> typing.Union[MetaOapg.properties.multiDocuments, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "sealCertificate", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "sealAutomatic", "readingMandatory", "digitalSignatureMandatory", "annexeIncluded", "multiDocuments", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "sealCertificate", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "digitalSignatureMandatory", "readingMandatory", "annexeIncluded", "sealAutomatic", "multiDocuments", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
@@ -597,18 +597,18 @@
         externalSignatureConfigId: typing.Union[MetaOapg.properties.externalSignatureConfigId, None, str, schemas.Unset] = schemas.unset,
         externalSignatureConfig: typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset] = schemas.unset,
         creationPermittedDeskIds: typing.Union[MetaOapg.properties.creationPermittedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
         creationPermittedDesks: typing.Union[MetaOapg.properties.creationPermittedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
         filterableByDeskIds: typing.Union[MetaOapg.properties.filterableByDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
         filterableByDesks: typing.Union[MetaOapg.properties.filterableByDesks, list, tuple, None, schemas.Unset] = schemas.unset,
         maxMainDocuments: typing.Union[MetaOapg.properties.maxMainDocuments, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        sealAutomatic: typing.Union[MetaOapg.properties.sealAutomatic, bool, schemas.Unset] = schemas.unset,
-        readingMandatory: typing.Union[MetaOapg.properties.readingMandatory, bool, schemas.Unset] = schemas.unset,
         digitalSignatureMandatory: typing.Union[MetaOapg.properties.digitalSignatureMandatory, bool, schemas.Unset] = schemas.unset,
+        readingMandatory: typing.Union[MetaOapg.properties.readingMandatory, bool, schemas.Unset] = schemas.unset,
         annexeIncluded: typing.Union[MetaOapg.properties.annexeIncluded, bool, schemas.Unset] = schemas.unset,
+        sealAutomatic: typing.Union[MetaOapg.properties.sealAutomatic, bool, schemas.Unset] = schemas.unset,
         multiDocuments: typing.Union[MetaOapg.properties.multiDocuments, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'SubtypeDto':
         return super().__new__(
             cls,
             *_args,
@@ -628,18 +628,18 @@
             externalSignatureConfigId=externalSignatureConfigId,
             externalSignatureConfig=externalSignatureConfig,
             creationPermittedDeskIds=creationPermittedDeskIds,
             creationPermittedDesks=creationPermittedDesks,
             filterableByDeskIds=filterableByDeskIds,
             filterableByDesks=filterableByDesks,
             maxMainDocuments=maxMainDocuments,
-            sealAutomatic=sealAutomatic,
-            readingMandatory=readingMandatory,
             digitalSignatureMandatory=digitalSignatureMandatory,
+            readingMandatory=readingMandatory,
             annexeIncluded=annexeIncluded,
+            sealAutomatic=sealAutomatic,
             multiDocuments=multiDocuments,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
 from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/template_type.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/workflow_definition_representation.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/models/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -136,76 +136,76 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,31 +40,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -78,77 +78,77 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '201': _response_for_201,
-    '403': _response_for_403,
     '400': _response_for_400,
+    '201': _response_for_201,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -66,31 +66,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -104,38 +104,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,50 +55,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -142,39 +142,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -162,76 +162,76 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,69 +66,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = DeskDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -142,59 +142,59 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '404': _response_for_404,
     '201': _response_for_201,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,96 +74,96 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
-    '406': _response_for_406,
     '404': _response_for_404,
+    '406': _response_for_406,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,69 +74,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -150,59 +150,59 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,50 +151,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageMetadataRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageMetadataRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -208,38 +208,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -123,98 +123,98 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
-    '201': _response_for_201,
-    '403': _response_for_403,
+    '404': _response_for_404,
     '400': _response_for_400,
+    '201': _response_for_201,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -74,96 +74,96 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '409': _response_for_409,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=MetadataIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = MetadataDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = MetadataDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,63 +74,63 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor406ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor406ResponseBodyApplicationJson),
+    },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -162,60 +162,60 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
+    '404': _response_for_404,
+    '406': _response_for_406,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '406': _response_for_406,
-    '404': _response_for_404,
+    '403': _response_for_403,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,50 +135,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageSealCertificateRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSealCertificateRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -192,38 +192,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -144,31 +144,31 @@
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
 SchemaFor201ResponseBodyApplicationJson = SealCertificateDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -182,77 +182,77 @@
 _response_for_201 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '201': _response_for_201,
-    '403': _response_for_403,
     '400': _response_for_400,
+    '201': _response_for_201,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,96 +74,96 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
-    '406': _response_for_406,
     '404': _response_for_404,
+    '406': _response_for_406,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SealCertificateIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -139,39 +139,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -150,50 +150,50 @@
         'multipart/form-data': api_client.MediaType(
             schema=SchemaForRequestBodyMultipartFormData),
     },
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SealCertificateDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -226,39 +226,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -63,44 +63,44 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TemplateTypeSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor404ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
+    },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -113,38 +113,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,44 +74,44 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor404ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
+    },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -124,38 +124,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,44 +74,44 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor404ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
+    },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
+    body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -124,38 +124,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,50 +135,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -192,38 +192,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,115 +66,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = TypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
     '201': _response_for_201,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -112,38 +112,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,50 +74,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -131,38 +131,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,50 +143,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -200,38 +200,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,69 +74,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SubtypeDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -150,59 +150,59 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '404': _response_for_404,
     '201': _response_for_201,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,31 +82,31 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,50 +71,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -128,38 +128,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -101,31 +101,31 @@
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor204ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -139,31 +139,31 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -179,17 +179,17 @@
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,50 +151,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -227,39 +227,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,69 +66,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = UserDto
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -142,59 +142,59 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
+    '404': _response_for_404,
     '201': _response_for_201,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,96 +74,96 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
-    '401': _response_for_401,
-    '406': _response_for_406,
     '404': _response_for_404,
+    '406': _response_for_406,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -63,50 +63,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
@@ -120,38 +120,38 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,115 +74,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor406ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor406ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor406ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor406(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor406ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_406 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor406,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor406ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
+    '406': _response_for_406,
     '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
-    '406': _response_for_406,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,50 +143,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = PageWorkflowDefinitionRepresentation
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageWorkflowDefinitionRepresentation
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -200,38 +200,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,96 +74,96 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '409': _response_for_409,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -136,76 +136,76 @@
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/post.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,115 +40,115 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor507ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor507(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor507ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_507 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor507,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor507ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
-SchemaFor409ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor409(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor409ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_409 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor409,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor409ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor201(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor201ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_201 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor201,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor201ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor507ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor507(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor507ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_507 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor409(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor409ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_409 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor409,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor409ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '507': _response_for_507,
-    '409': _response_for_409,
     '201': _response_for_201,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '507': _response_for_507,
+    '409': _response_for_409,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,76 +66,76 @@
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_204 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor204,
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor400ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor400(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor400ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_400 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor400,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor400ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
     '204': _response_for_204,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,50 +55,50 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -131,39 +131,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor400(api_client.ApiResponse):
@@ -142,39 +142,39 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
+    '404': _response_for_404,
     '200': _response_for_200,
-    '403': _response_for_403,
     '400': _response_for_400,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_templates_template_type/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -55,29 +55,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TemplateTypeSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        schemas.Unset,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
-        'text/plain': api_client.MediaType(),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
 SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor403(api_client.ApiResponse):
@@ -91,41 +93,39 @@
 _response_for_403 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        schemas.Unset,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+        'text/plain': api_client.MediaType(),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
+    '200': _response_for_200,
 }
 _all_accept_content_types = (
-    'text/plain',
     'application/json',
+    'text/plain',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
     def _get_default_template_oapg(
         self,
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/get.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/paths/api_provisioning_v1_tenant_tenant_id_templates_template_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,97 +63,97 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TemplateTypeSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
+SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor404(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        schemas.Unset,
+        SchemaFor404ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_404 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor404,
     content={
-        'text/plain': api_client.MediaType(),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor404ResponseBodyApplicationJson),
     },
 )
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
+        SchemaFor401ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
+_response_for_401 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
+            schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor401ResponseBodyApplicationJson = ErrorResponse
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        schemas.Unset,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+        'text/plain': api_client.MediaType(),
     },
 )
 _status_code_to_response = {
-    '200': _response_for_200,
-    '403': _response_for_403,
-    '401': _response_for_401,
     '404': _response_for_404,
+    '401': _response_for_401,
+    '403': _response_for_403,
+    '200': _response_for_200,
 }
 _all_accept_content_types = (
-    'text/plain',
     'application/json',
+    'text/plain',
 )
 
 
 class BaseApi(api_client.Api):
     @typing.overload
     def _get_custom_template_oapg(
         self,
```

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.9.4/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/setup.py` & `iparapheur-provisioning-1.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.9.3"
+VERSION = "1.9.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_certificate_informations.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_certificate_informations.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_metadata_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_seal_certificate_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_tenant_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_page_workflow_definition_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_page_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_seal_certificate_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_seal_certificate_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_seal_certificate_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_seal_certificate_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_template_type.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_template_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_workflow_definition_representation.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_workflow_definition_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_models/test_workflow_definition_sort_by.py` & `iparapheur-provisioning-1.9.4/test/test_models/test_workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/__init__.py` & `iparapheur-provisioning-1.9.4/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_get.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user/test_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenant unit test stubs
-        Create a new tenant  # noqa: E501
+    ApiProvisioningV1AdminUser unit test stubs
+        Create a new super admin user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 201
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Get a full tenant description  # noqa: E501
+        Edit a tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantId unit test stubs
-        Edit a tenant  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
+        List desks  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
     response_status = 200
 
 
 
 
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDesk(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDesk unit test stubs
-        List desks  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Get a full desk description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Get a full desk description  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Get a full user description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
-        Edit a desk  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
+        Edit a metadata  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_metadata_metadata_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdMetadataMetadataId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdMetadataMetadataId unit test stubs
-        Edit a metadata  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdSealCertificate(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdSealCertificate unit test stubs
-        List seal certificates  # noqa: E501
+        Create a seal certificate  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 400
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdSealCertificate(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdSealCertificate unit test stubs
-        Create a seal certificate  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate_seal_certificate_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,33 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Delete a custom template  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Get a full tenant description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
+    response_status = 404
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_delete.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,35 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Create a custom template  # noqa: E501
+        Delete a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-    response_body = ''
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,35 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
-        Update a custom template  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 204
     response_body = ''
 
 
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        List types  # noqa: E501
+        Create a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 201
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        Create a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
+        Edit a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
-        Edit a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
+        Edit a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 204
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
-        Create a subtype  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
+        Get a subtype with every information set  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
-
-
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Get a subtype with every information set  # noqa: E501
+    ApiProvisioningV1AdminUser unit test stubs
+        List all users on the instance  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtypeSubtypeId unit test stubs
-        Edit a subtype  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Remove the given user from the tenant, deleting it if it was the last tenant linked  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeIdSubtype unit test stubs
+        Create a subtype  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 404
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Delete a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenant(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenant unit test stubs
+        Create a new tenant  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 400
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_workflow_definition_workflow_definition_key/test_delete.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_put.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUser unit test stubs
-        List all users on the instance  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
+        Update a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user/test_post.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_templates_template_type/test_post.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_templates_template_type import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUser unit test stubs
-        Create a new super admin user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTemplatesTemplateType unit test stubs
+        Create a custom template  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 507
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,33 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdDeskDeskId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Delete a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdDeskDeskId unit test stubs
+        Edit a desk  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 204
-    response_body = ''
+    response_status = 404
+
+
+
+
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_seal_certificate/test_get.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_seal_certificate import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdSealCertificate(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdSealCertificate unit test stubs
+        List seal certificates  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminUserUserId unit test stubs
-        Edit a user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
+        List types  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
-
-
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_templates_template_type/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_templates_template_type/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.9.3/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/test_get.py` & `iparapheur-provisioning-1.9.4/test/test_paths/test_api_provisioning_v1_tenant_tenant_id_templates_template_type/test_get.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 200
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

