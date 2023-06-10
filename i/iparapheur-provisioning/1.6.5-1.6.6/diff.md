# Comparing `tmp/iparapheur-provisioning-1.6.5.tar.gz` & `tmp/iparapheur-provisioning-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iparapheur-provisioning-1.6.5.tar", last modified: Wed May 31 09:42:12 2023, max compression
+gzip compressed data, was "iparapheur-provisioning-1.6.6.tar", last modified: Sat Jun 10 12:31:44 2023, max compression
```

## Comparing `iparapheur-provisioning-1.6.5.tar` & `iparapheur-provisioning-1.6.6.tar`

### file list

```diff
@@ -1,243 +1,241 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/
--rw-r--r--   0 root         (0) root         (0)     1111 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17390 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.065018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/
--rw-r--r--   0 root         (0) root         (0)      907 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58620 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.069018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/
--rw-r--r--   0 root         (0) root         (0)      214 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/path_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.069018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
--rw-r--r--   0 root         (0) root         (0)      493 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
--rw-r--r--   0 root         (0) root         (0)      566 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tag_to_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.073018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/
--rw-r--r--   0 root         (0) root         (0)      475 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_all_users_api.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_desk_api.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_tenant_api.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_typology_api.py
--rw-r--r--   0 root         (0) root         (0)    15677 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/configuration.py
--rw-r--r--   0 root         (0) root         (0)     4598 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.081019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/
--rw-r--r--   0 root         (0) root         (0)      357 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-05-31 09:40:33.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    30320 2023-05-31 09:40:34.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/desk_dto.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-05-31 09:40:35.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     4553 2023-05-31 09:40:35.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/error_response.py
--rw-r--r--   0 root         (0) root         (0)     4891 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)     2680 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3284 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/layer_representation.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     5805 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)     1356 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_type.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)     9132 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)     9105 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)     5251 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/pageable_object.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/signature_format.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/sort_object.py
--rw-r--r--   0 root         (0) root         (0)    28616 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)     1307 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)     3930 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)     5468 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)     3274 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     9365 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/type_dto.py
--rw-r--r--   0 root         (0) root         (0)     4044 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/type_representation.py
--rw-r--r--   0 root         (0) root         (0)     4436 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/typology_representation.py
--rw-r--r--   0 root         (0) root         (0)     1144 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)    29666 2023-05-31 09:40:42.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_dto.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_privilege.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_representation.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1256 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.081019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/models/
--rw-r--r--   0 root         (0) root         (0)     3734 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.081019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.081019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)      369 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13629 2023-05-31 09:40:48.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.081019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11083 2023-05-31 09:40:48.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11332 2023-05-31 09:40:48.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15808 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.085018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15034 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
--rw-r--r--   0 root         (0) root         (0)    16302 2023-05-31 09:40:46.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.085018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-05-31 09:40:46.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11677 2023-05-31 09:40:46.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16545 2023-05-31 09:40:46.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.085018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)      417 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14728 2023-05-31 09:40:54.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
--rw-r--r--   0 root         (0) root         (0)    15777 2023-05-31 09:40:52.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.085018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11337 2023-05-31 09:40:53.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11590 2023-05-31 09:40:53.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15521 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.085018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)      449 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15050 2023-05-31 09:40:54.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
--rw-r--r--   0 root         (0) root         (0)    16640 2023-05-31 09:40:52.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.085018 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11672 2023-05-31 09:40:52.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11934 2023-05-31 09:40:53.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16645 2023-05-31 09:40:54.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.089019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)      399 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15944 2023-05-31 09:40:50.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.089019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      415 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-05-31 09:40:50.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11580 2023-05-31 09:40:50.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    16046 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.089019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)      365 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-05-31 09:40:44.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.089019 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11207 2023-05-31 09:40:44.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
--rw-r--r--   0 root         (0) root         (0)    11978 2023-05-31 09:40:44.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
--rw-r--r--   0 root         (0) root         (0)    15946 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
--rw-r--r--   0 root         (0) root         (0)    10635 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/rest.py
--rw-r--r--   0 root         (0) root         (0)    97752 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.069018 iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      421 2023-05-31 09:42:12.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13603 2023-05-31 09:42:12.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 09:42:12.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-05-31 09:42:12.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-31 09:42:12.000000 iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1322 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.065018 iparapheur-provisioning-1.6.5/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.093019 iparapheur-provisioning-1.6.5/test/test_models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:56.000000 iparapheur-provisioning-1.6.5/test/test_models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-31 09:40:33.000000 iparapheur-provisioning-1.6.5/test/test_models/test_delegation_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-31 09:40:34.000000 iparapheur-provisioning-1.6.5/test/test_models/test_desk_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-31 09:40:35.000000 iparapheur-provisioning-1.6.5/test/test_models/test_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)      767 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_external_signature_config_representation.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_external_signature_config_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_external_signature_provider.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_folder_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_internal_metadata.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_layer_representation.py
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-31 09:40:36.000000 iparapheur-provisioning-1.6.5/test/test_models/test_layer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/test/test_models/test_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/test/test_models/test_metadata_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/test/test_models/test_metadata_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      665 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/test/test_models/test_metadata_type.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-31 09:40:37.000000 iparapheur-provisioning-1.6.5/test/test_models/test_page_desk_representation.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/test/test_models/test_page_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/test/test_models/test_page_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/test/test_models/test_page_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-05-31 09:40:38.000000 iparapheur-provisioning-1.6.5/test/test_models/test_pageable_object.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/test/test_models/test_pdf_signature_position.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/test/test_models/test_seal_certificate_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/test/test_models/test_signature_format.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/test/test_models/test_signature_protocol.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-31 09:40:39.000000 iparapheur-provisioning-1.6.5/test/test_models/test_sort_object.py
--rw-r--r--   0 root         (0) root         (0)      657 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/test/test_models/test_subtype_dto.py
--rw-r--r--   0 root         (0) root         (0)      710 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/test/test_models/test_subtype_layer_association.py
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/test/test_models/test_subtype_layer_dto.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/test/test_models/test_subtype_metadata_dto.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-31 09:40:40.000000 iparapheur-provisioning-1.6.5/test/test_models/test_subtype_representation.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_tenant_dto.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_tenant_representation.py
--rw-r--r--   0 root         (0) root         (0)      666 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_tenant_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_type_dto.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_type_representation.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_typology_representation.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-31 09:40:41.000000 iparapheur-provisioning-1.6.5/test/test_models/test_typology_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-05-31 09:40:42.000000 iparapheur-provisioning-1.6.5/test/test_models/test_user_dto.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/test/test_models/test_user_privilege.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/test/test_models/test_user_representation.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/test/test_models/test_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-31 09:40:43.000000 iparapheur-provisioning-1.6.5/test/test_models/test_workflow_definition_sort_by.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.093019 iparapheur-provisioning-1.6.5/test/test_paths/
--rw-r--r--   0 root         (0) root         (0)     1995 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.093019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.097019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      930 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-31 09:40:49.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.097019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.097019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-31 09:40:47.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.097019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
--rw-r--r--   0 root         (0) root         (0)      949 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.097019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      981 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.097019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-31 09:40:55.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-05-31 09:40:51.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
--rw-r--r--   0 root         (0) root         (0)      899 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 09:42:12.101019 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-05-31 09:40:45.000000 iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.257931 iparapheur-provisioning-1.6.6/
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-10 12:31:44.257931 iparapheur-provisioning-1.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    17323 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.641916 iparapheur-provisioning-1.6.6/iparapheur_provisioning/
+-rw-r--r--   0 root         (0) root         (0)      907 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58620 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.649917 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4776 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/path_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.677917 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/
+-rw-r--r--   0 root         (0) root         (0)      250 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id.py
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type.py
+-rw-r--r--   0 root         (0) root         (0)      493 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_user_user_id.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tag_to_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.681917 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_all_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_desk_api.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_api.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_typology_api.py
+-rw-r--r--   0 root         (0) root         (0)    15677 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4598 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.881922 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2023-06-10 12:24:51.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    24041 2023-06-10 12:24:53.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4891 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3284 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     7233 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9132 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     9105 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_format.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/sort_object.py
+-rw-r--r--   0 root         (0) root         (0)    28616 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1307 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)     3274 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     9365 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_dto.py
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)    29666 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_dto.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_representation.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.893922 iparapheur-provisioning-1.6.6/iparapheur_provisioning/models/
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.901923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.905923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-10 12:25:11.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13629 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.909923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)      389 2023-06-10 12:25:11.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11083 2023-06-10 12:25:10.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11332 2023-06-10 12:25:10.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15808 2023-06-10 12:25:10.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.909923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15034 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py
+-rw-r--r--   0 root         (0) root         (0)    16302 2023-06-10 12:25:07.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.917923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-06-10 12:25:07.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11677 2023-06-10 12:25:08.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16545 2023-06-10 12:25:07.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.917923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14728 2023-06-10 12:25:34.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py
+-rw-r--r--   0 root         (0) root         (0)    15777 2023-06-10 12:25:15.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.933923 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11337 2023-06-10 12:25:28.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2023-06-10 12:25:33.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15521 2023-06-10 12:25:35.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.949924 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15050 2023-06-10 12:25:34.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-06-10 12:25:15.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.953924 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11672 2023-06-10 12:25:21.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11934 2023-06-10 12:25:32.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16645 2023-06-10 12:25:35.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.977924 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15944 2023-06-10 12:25:13.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.997925 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-06-10 12:25:13.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    16046 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.001925 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.041926 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11207 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py
+-rw-r--r--   0 root         (0) root         (0)    11978 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py
+-rw-r--r--   0 root         (0) root         (0)    10635 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/rest.py
+-rw-r--r--   0 root         (0) root         (0)    97752 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.649917 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13497 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-10 12:31:43.000000 iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-10 12:31:44.261931 iparapheur-provisioning-1.6.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1322 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:43.609916 iparapheur-provisioning-1.6.6/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.153928 iparapheur-provisioning-1.6.6/test/test_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:37.000000 iparapheur-provisioning-1.6.6/test/test_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-10 12:24:51.000000 iparapheur-provisioning-1.6.6/test/test_models/test_delegation_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-10 12:24:54.000000 iparapheur-provisioning-1.6.6/test/test_models/test_desk_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/test/test_models/test_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-10 12:24:55.000000 iparapheur-provisioning-1.6.6/test/test_models/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)      767 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_representation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_provider.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_folder_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_internal_metadata.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_layer_representation.py
+-rw-r--r--   0 root         (0) root         (0)      662 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_layer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      705 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-10 12:24:56.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      665 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_metadata_type.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_desk_representation.py
+-rw-r--r--   0 root         (0) root         (0)      718 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-06-10 12:24:57.000000 iparapheur-provisioning-1.6.6/test/test_models/test_page_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_pageable_object.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_pdf_signature_position.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_seal_certificate_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_signature_format.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_signature_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-10 12:24:58.000000 iparapheur-provisioning-1.6.6/test/test_models/test_sort_object.py
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_dto.py
+-rw-r--r--   0 root         (0) root         (0)      710 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_association.py
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-10 12:24:59.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_dto.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_metadata_dto.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_subtype_representation.py
+-rw-r--r--   0 root         (0) root         (0)      653 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_tenant_dto.py
+-rw-r--r--   0 root         (0) root         (0)      697 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_tenant_representation.py
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_tenant_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-10 12:25:00.000000 iparapheur-provisioning-1.6.6/test/test_models/test_type_dto.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/test/test_models/test_type_representation.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-10 12:25:01.000000 iparapheur-provisioning-1.6.6/test/test_models/test_typology_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_dto.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-10 12:25:02.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_privilege.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_representation.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/test/test_models/test_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-10 12:25:05.000000 iparapheur-provisioning-1.6.6/test/test_models/test_workflow_definition_sort_by.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.153928 iparapheur-provisioning-1.6.6/test/test_paths/
+-rw-r--r--   0 root         (0) root         (0)     1995 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.153928 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.157929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      925 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-10 12:25:12.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.157929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      924 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.161929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      956 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-10 12:25:09.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.161929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      949 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.161929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      981 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.173929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.189929 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-10 12:25:36.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.205930 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.233930 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-06-10 12:25:14.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.241930 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      899 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-10 12:31:44.245931 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py
+-rw-r--r--   0 root         (0) root         (0)      902 2023-06-10 12:25:06.000000 iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py
```

### Comparing `iparapheur-provisioning-1.6.5/LICENSE.md` & `iparapheur-provisioning-1.6.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/README.md` & `iparapheur-provisioning-1.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 The main link between every sub-services, integrating business code logic.
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: DEVELOP
-- Package version: 1.6.5
+- Package version: 1.6.6
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://libriciel.fr](https://libriciel.fr)
 
 ## Requirements.
 
 Python &gt;&#x3D;3.7
 
@@ -246,15 +246,14 @@
  - [SubtypeMetadataDto](docs/models/SubtypeMetadataDto.md)
  - [SubtypeRepresentation](docs/models/SubtypeRepresentation.md)
  - [TenantDto](docs/models/TenantDto.md)
  - [TenantRepresentation](docs/models/TenantRepresentation.md)
  - [TenantSortBy](docs/models/TenantSortBy.md)
  - [TypeDto](docs/models/TypeDto.md)
  - [TypeRepresentation](docs/models/TypeRepresentation.md)
- - [TypologyRepresentation](docs/models/TypologyRepresentation.md)
  - [TypologySortBy](docs/models/TypologySortBy.md)
  - [UserDto](docs/models/UserDto.md)
  - [UserPrivilege](docs/models/UserPrivilege.md)
  - [UserRepresentation](docs/models/UserRepresentation.md)
  - [UserSortBy](docs/models/UserSortBy.md)
  - [WorkflowDefinitionSortBy](docs/models/WorkflowDefinitionSortBy.md)
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/__init__.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     iparapheur v5.x main core application.  The main link between every sub-services, integrating business code logic.   # noqa: E501
 
     The version of the OpenAPI document: DEVELOP
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
-__version__ = "1.6.5"
+__version__ = "1.6.6"
 
 # import ApiClient
 from iparapheur_provisioning.api_client import ApiClient
 
 # import Configuration
 from iparapheur_provisioning.configuration import Configuration
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/api_client.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1000,15 +1000,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = HTTPHeaderDict()
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.6.5/python'
+        self.user_agent = 'OpenAPI-Generator/1.6.6/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/path_to_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tag_to_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_all_users_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_all_users_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_desk_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_desk_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_tenant_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_tenant_user_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/apis/tags/admin_typology_api.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/apis/tags/admin_typology_api.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/configuration.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: DEVELOP\n"\
-               "SDK Package Version: 1.6.5".\
+               "SDK Package Version: 1.6.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/exceptions.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/exceptions.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/delegation_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/desk_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_dto.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,31 +20,27 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class DeskDto(
+class SubtypeDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-
-    body
     """
 
 
     class MetaOapg:
         required = {
-            "ownerIds",
             "name",
-            "shortName",
         }
         
         class properties:
             
             
             class name(
                 schemas.StrSchema
@@ -53,638 +49,586 @@
             
                 class MetaOapg:
                     max_length = 255
                     min_length = 2
                     regex=[{
                         'pattern': r'^[^\r\n ]+$',  # noqa: E501
                     }]
+            id = schemas.StrSchema
             
             
-            class shortName(
+            class description(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
                     max_length = 255
-                    min_length = 2
+                    min_length = 3
             
             
-            class ownerIds(
-                schemas.ListSchema
+            class creationWorkflowId(
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
             ):
             
             
-                class MetaOapg:
-                    max_items = 256
-                    min_items = 0
-                    items = schemas.StrSchema
-            
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'ownerIds':
+                ) -> 'creationWorkflowId':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
+            validationWorkflowId = schemas.StrSchema
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            id = schemas.StrSchema
-            tenantId = schemas.StrSchema
-            description = schemas.StrSchema
-            folderCreationAllowed = schemas.BoolSchema
-            actionAllowed = schemas.BoolSchema
-            archivingAllowed = schemas.BoolSchema
-            chainAllowed = schemas.BoolSchema
-            parentDeskId = schemas.StrSchema
-        
-            @staticmethod
-            def parentDesk() -> typing.Type['DeskRepresentation']:
-                return DeskRepresentation
             
-            
-            class owners(
-                schemas.ListSchema
+            class workflowSelectionScript(
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
             ):
             
             
                 class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['UserRepresentation']:
-                        return UserRepresentation
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'owners':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'UserRepresentation':
-                    return super().__getitem__(i)
+                    max_length = 65535
+                    min_length = 0
             
             
-            class associatedDeskIds(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'associatedDeskIds':
+                ) -> 'workflowSelectionScript':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
+            annotationsAllowed = schemas.BoolSchema
+            externalSignatureAutomatic = schemas.BoolSchema
             
             
-            class associatedDesks(
-                schemas.ListSchema
+            class secureMailServerId(
+                schemas.Int64Base,
+                schemas.IntBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneDecimalMixin
             ):
             
             
                 class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['DeskRepresentation']:
-                        return DeskRepresentation
+                    format = 'int64'
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['DeskRepresentation'], typing.List['DeskRepresentation']],
+                    *_args: typing.Union[None, decimal.Decimal, int, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'associatedDesks':
+                ) -> 'secureMailServerId':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'DeskRepresentation':
-                    return super().__getitem__(i)
             
-            
-            class filterableMetadataIds(
-                schemas.ListSchema
+            class sealCertificateId(
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
             ):
             
             
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'filterableMetadataIds':
+                ) -> 'sealCertificateId':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            
             
-            class filterableMetadata(
+            class subtypeMetadataList(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['MetadataRepresentation']:
-                        return MetadataRepresentation
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['MetadataRepresentation'], typing.List['MetadataRepresentation']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'filterableMetadata':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'MetadataRepresentation':
-                    return super().__getitem__(i)
-            
-            
-            class filterableSubtypeIds(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
+                    def items() -> typing.Type['SubtypeMetadataDto']:
+                        return SubtypeMetadataDto
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    _arg: typing.Union[typing.Tuple['SubtypeMetadataDto'], typing.List['SubtypeMetadataDto']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'filterableSubtypeIds':
+                ) -> 'subtypeMetadataList':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
+                def __getitem__(self, i: int) -> 'SubtypeMetadataDto':
                     return super().__getitem__(i)
             
             
-            class filterableSubtypes(
+            class subtypeLayers(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['TypologyRepresentation']:
-                        return TypologyRepresentation
+                    def items() -> typing.Type['SubtypeLayerDto']:
+                        return SubtypeLayerDto
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['TypologyRepresentation'], typing.List['TypologyRepresentation']],
+                    _arg: typing.Union[typing.Tuple['SubtypeLayerDto'], typing.List['SubtypeLayerDto']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'filterableSubtypes':
+                ) -> 'subtypeLayers':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'TypologyRepresentation':
+                def __getitem__(self, i: int) -> 'SubtypeLayerDto':
                     return super().__getitem__(i)
             
             
-            class availableSubtypeIds(
-                schemas.ListSchema
+            class externalSignatureConfigId(
+                schemas.StrBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneStrMixin
             ):
             
             
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[None, str, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'availableSubtypeIds':
+                ) -> 'externalSignatureConfigId':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
+        
+            @staticmethod
+            def externalSignatureConfig() -> typing.Type['ExternalSignatureConfigRepresentation']:
+                return ExternalSignatureConfigRepresentation
             
             
-            class availableSubtypes(
-                schemas.ListSchema
+            class creationPermittedDeskIds(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
                     
-                    @staticmethod
-                    def items() -> typing.Type['TypologyRepresentation']:
-                        return TypologyRepresentation
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['TypologyRepresentation'], typing.List['TypologyRepresentation']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'availableSubtypes':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'TypologyRepresentation':
-                    return super().__getitem__(i)
-            
-            
-            class supervisorIds(
-                schemas.ListSchema
-            ):
-            
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
             
-                class MetaOapg:
-                    items = schemas.StrSchema
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'supervisorIds':
+                ) -> 'creationPermittedDeskIds':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            
             
-            class supervisors(
-                schemas.ListSchema
+            class creationPermittedDesks(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['UserRepresentation']:
-                        return UserRepresentation
+                    def items() -> typing.Type['DeskRepresentation']:
+                        return DeskRepresentation
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'supervisors':
+                ) -> 'creationPermittedDesks':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'UserRepresentation':
-                    return super().__getitem__(i)
             
-            
-            class delegationManagerIds(
-                schemas.ListSchema
+            class filterableByDeskIds(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
-                    items = schemas.StrSchema
+                    
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'delegationManagerIds':
+                ) -> 'filterableByDeskIds':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            
             
-            class delegationManagers(
-                schemas.ListSchema
+            class filterableByDesks(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['UserRepresentation']:
-                        return UserRepresentation
+                    def items() -> typing.Type['DeskRepresentation']:
+                        return DeskRepresentation
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'delegationManagers':
+                ) -> 'filterableByDesks':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
-            
-                def __getitem__(self, i: int) -> 'UserRepresentation':
-                    return super().__getitem__(i)
+            maxMainDocuments = schemas.Int32Schema
+            multiDocuments = schemas.BoolSchema
+            annexeIncluded = schemas.BoolSchema
+            digitalSignatureMandatory = schemas.BoolSchema
+            readingMandatory = schemas.BoolSchema
+            sealAutomatic = schemas.BoolSchema
             __annotations__ = {
                 "name": name,
-                "shortName": shortName,
-                "ownerIds": ownerIds,
                 "id": id,
-                "tenantId": tenantId,
                 "description": description,
-                "folderCreationAllowed": folderCreationAllowed,
-                "actionAllowed": actionAllowed,
-                "archivingAllowed": archivingAllowed,
-                "chainAllowed": chainAllowed,
-                "parentDeskId": parentDeskId,
-                "parentDesk": parentDesk,
-                "owners": owners,
-                "associatedDeskIds": associatedDeskIds,
-                "associatedDesks": associatedDesks,
-                "filterableMetadataIds": filterableMetadataIds,
-                "filterableMetadata": filterableMetadata,
-                "filterableSubtypeIds": filterableSubtypeIds,
-                "filterableSubtypes": filterableSubtypes,
-                "availableSubtypeIds": availableSubtypeIds,
-                "availableSubtypes": availableSubtypes,
-                "supervisorIds": supervisorIds,
-                "supervisors": supervisors,
-                "delegationManagerIds": delegationManagerIds,
-                "delegationManagers": delegationManagers,
+                "creationWorkflowId": creationWorkflowId,
+                "validationWorkflowId": validationWorkflowId,
+                "workflowSelectionScript": workflowSelectionScript,
+                "annotationsAllowed": annotationsAllowed,
+                "externalSignatureAutomatic": externalSignatureAutomatic,
+                "secureMailServerId": secureMailServerId,
+                "sealCertificateId": sealCertificateId,
+                "subtypeMetadataList": subtypeMetadataList,
+                "subtypeLayers": subtypeLayers,
+                "externalSignatureConfigId": externalSignatureConfigId,
+                "externalSignatureConfig": externalSignatureConfig,
+                "creationPermittedDeskIds": creationPermittedDeskIds,
+                "creationPermittedDesks": creationPermittedDesks,
+                "filterableByDeskIds": filterableByDeskIds,
+                "filterableByDesks": filterableByDesks,
+                "maxMainDocuments": maxMainDocuments,
+                "multiDocuments": multiDocuments,
+                "annexeIncluded": annexeIncluded,
+                "digitalSignatureMandatory": digitalSignatureMandatory,
+                "readingMandatory": readingMandatory,
+                "sealAutomatic": sealAutomatic,
             }
     
-    ownerIds: MetaOapg.properties.ownerIds
     name: MetaOapg.properties.name
-    shortName: MetaOapg.properties.shortName
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["shortName"]) -> MetaOapg.properties.shortName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tenantId"]) -> MetaOapg.properties.tenantId: ...
+    def __getitem__(self, name: typing_extensions.Literal["creationWorkflowId"]) -> MetaOapg.properties.creationWorkflowId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["validationWorkflowId"]) -> MetaOapg.properties.validationWorkflowId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["folderCreationAllowed"]) -> MetaOapg.properties.folderCreationAllowed: ...
+    def __getitem__(self, name: typing_extensions.Literal["workflowSelectionScript"]) -> MetaOapg.properties.workflowSelectionScript: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["actionAllowed"]) -> MetaOapg.properties.actionAllowed: ...
+    def __getitem__(self, name: typing_extensions.Literal["annotationsAllowed"]) -> MetaOapg.properties.annotationsAllowed: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["archivingAllowed"]) -> MetaOapg.properties.archivingAllowed: ...
+    def __getitem__(self, name: typing_extensions.Literal["externalSignatureAutomatic"]) -> MetaOapg.properties.externalSignatureAutomatic: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["chainAllowed"]) -> MetaOapg.properties.chainAllowed: ...
+    def __getitem__(self, name: typing_extensions.Literal["secureMailServerId"]) -> MetaOapg.properties.secureMailServerId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["parentDeskId"]) -> MetaOapg.properties.parentDeskId: ...
+    def __getitem__(self, name: typing_extensions.Literal["sealCertificateId"]) -> MetaOapg.properties.sealCertificateId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["parentDesk"]) -> 'DeskRepresentation': ...
+    def __getitem__(self, name: typing_extensions.Literal["subtypeMetadataList"]) -> MetaOapg.properties.subtypeMetadataList: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["owners"]) -> MetaOapg.properties.owners: ...
+    def __getitem__(self, name: typing_extensions.Literal["subtypeLayers"]) -> MetaOapg.properties.subtypeLayers: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["associatedDeskIds"]) -> MetaOapg.properties.associatedDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> MetaOapg.properties.externalSignatureConfigId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["associatedDesks"]) -> MetaOapg.properties.associatedDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> 'ExternalSignatureConfigRepresentation': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableMetadataIds"]) -> MetaOapg.properties.filterableMetadataIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> MetaOapg.properties.creationPermittedDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableMetadata"]) -> MetaOapg.properties.filterableMetadata: ...
+    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDesks"]) -> MetaOapg.properties.creationPermittedDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableSubtypeIds"]) -> MetaOapg.properties.filterableSubtypeIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> MetaOapg.properties.filterableByDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableSubtypes"]) -> MetaOapg.properties.filterableSubtypes: ...
+    def __getitem__(self, name: typing_extensions.Literal["filterableByDesks"]) -> MetaOapg.properties.filterableByDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["availableSubtypeIds"]) -> MetaOapg.properties.availableSubtypeIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["maxMainDocuments"]) -> MetaOapg.properties.maxMainDocuments: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["availableSubtypes"]) -> MetaOapg.properties.availableSubtypes: ...
+    def __getitem__(self, name: typing_extensions.Literal["multiDocuments"]) -> MetaOapg.properties.multiDocuments: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["supervisorIds"]) -> MetaOapg.properties.supervisorIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["annexeIncluded"]) -> MetaOapg.properties.annexeIncluded: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["supervisors"]) -> MetaOapg.properties.supervisors: ...
+    def __getitem__(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> MetaOapg.properties.digitalSignatureMandatory: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["delegationManagerIds"]) -> MetaOapg.properties.delegationManagerIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["readingMandatory"]) -> MetaOapg.properties.readingMandatory: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["delegationManagers"]) -> MetaOapg.properties.delegationManagers: ...
+    def __getitem__(self, name: typing_extensions.Literal["sealAutomatic"]) -> MetaOapg.properties.sealAutomatic: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "ownerIds", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "filterableSubtypeIds", "filterableSubtypes", "availableSubtypeIds", "availableSubtypes", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["shortName"]) -> MetaOapg.properties.shortName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tenantId"]) -> typing.Union[MetaOapg.properties.tenantId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["creationWorkflowId"]) -> typing.Union[MetaOapg.properties.creationWorkflowId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["validationWorkflowId"]) -> typing.Union[MetaOapg.properties.validationWorkflowId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["folderCreationAllowed"]) -> typing.Union[MetaOapg.properties.folderCreationAllowed, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["workflowSelectionScript"]) -> typing.Union[MetaOapg.properties.workflowSelectionScript, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["actionAllowed"]) -> typing.Union[MetaOapg.properties.actionAllowed, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["annotationsAllowed"]) -> typing.Union[MetaOapg.properties.annotationsAllowed, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["archivingAllowed"]) -> typing.Union[MetaOapg.properties.archivingAllowed, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureAutomatic"]) -> typing.Union[MetaOapg.properties.externalSignatureAutomatic, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["chainAllowed"]) -> typing.Union[MetaOapg.properties.chainAllowed, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["secureMailServerId"]) -> typing.Union[MetaOapg.properties.secureMailServerId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["parentDeskId"]) -> typing.Union[MetaOapg.properties.parentDeskId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sealCertificateId"]) -> typing.Union[MetaOapg.properties.sealCertificateId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["parentDesk"]) -> typing.Union['DeskRepresentation', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["subtypeMetadataList"]) -> typing.Union[MetaOapg.properties.subtypeMetadataList, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["owners"]) -> typing.Union[MetaOapg.properties.owners, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["subtypeLayers"]) -> typing.Union[MetaOapg.properties.subtypeLayers, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["associatedDeskIds"]) -> typing.Union[MetaOapg.properties.associatedDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> typing.Union[MetaOapg.properties.externalSignatureConfigId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["associatedDesks"]) -> typing.Union[MetaOapg.properties.associatedDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableMetadataIds"]) -> typing.Union[MetaOapg.properties.filterableMetadataIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> typing.Union[MetaOapg.properties.creationPermittedDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableMetadata"]) -> typing.Union[MetaOapg.properties.filterableMetadata, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDesks"]) -> typing.Union[MetaOapg.properties.creationPermittedDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableSubtypeIds"]) -> typing.Union[MetaOapg.properties.filterableSubtypeIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> typing.Union[MetaOapg.properties.filterableByDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableSubtypes"]) -> typing.Union[MetaOapg.properties.filterableSubtypes, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDesks"]) -> typing.Union[MetaOapg.properties.filterableByDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["availableSubtypeIds"]) -> typing.Union[MetaOapg.properties.availableSubtypeIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["maxMainDocuments"]) -> typing.Union[MetaOapg.properties.maxMainDocuments, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["availableSubtypes"]) -> typing.Union[MetaOapg.properties.availableSubtypes, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["multiDocuments"]) -> typing.Union[MetaOapg.properties.multiDocuments, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["supervisorIds"]) -> typing.Union[MetaOapg.properties.supervisorIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["annexeIncluded"]) -> typing.Union[MetaOapg.properties.annexeIncluded, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["supervisors"]) -> typing.Union[MetaOapg.properties.supervisors, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> typing.Union[MetaOapg.properties.digitalSignatureMandatory, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagerIds"]) -> typing.Union[MetaOapg.properties.delegationManagerIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["readingMandatory"]) -> typing.Union[MetaOapg.properties.readingMandatory, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagers"]) -> typing.Union[MetaOapg.properties.delegationManagers, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["sealAutomatic"]) -> typing.Union[MetaOapg.properties.sealAutomatic, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "ownerIds", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "filterableSubtypeIds", "filterableSubtypes", "availableSubtypeIds", "availableSubtypes", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        ownerIds: typing.Union[MetaOapg.properties.ownerIds, list, tuple, ],
         name: typing.Union[MetaOapg.properties.name, str, ],
-        shortName: typing.Union[MetaOapg.properties.shortName, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        tenantId: typing.Union[MetaOapg.properties.tenantId, str, schemas.Unset] = schemas.unset,
         description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        folderCreationAllowed: typing.Union[MetaOapg.properties.folderCreationAllowed, bool, schemas.Unset] = schemas.unset,
-        actionAllowed: typing.Union[MetaOapg.properties.actionAllowed, bool, schemas.Unset] = schemas.unset,
-        archivingAllowed: typing.Union[MetaOapg.properties.archivingAllowed, bool, schemas.Unset] = schemas.unset,
-        chainAllowed: typing.Union[MetaOapg.properties.chainAllowed, bool, schemas.Unset] = schemas.unset,
-        parentDeskId: typing.Union[MetaOapg.properties.parentDeskId, str, schemas.Unset] = schemas.unset,
-        parentDesk: typing.Union['DeskRepresentation', schemas.Unset] = schemas.unset,
-        owners: typing.Union[MetaOapg.properties.owners, list, tuple, schemas.Unset] = schemas.unset,
-        associatedDeskIds: typing.Union[MetaOapg.properties.associatedDeskIds, list, tuple, schemas.Unset] = schemas.unset,
-        associatedDesks: typing.Union[MetaOapg.properties.associatedDesks, list, tuple, schemas.Unset] = schemas.unset,
-        filterableMetadataIds: typing.Union[MetaOapg.properties.filterableMetadataIds, list, tuple, schemas.Unset] = schemas.unset,
-        filterableMetadata: typing.Union[MetaOapg.properties.filterableMetadata, list, tuple, schemas.Unset] = schemas.unset,
-        filterableSubtypeIds: typing.Union[MetaOapg.properties.filterableSubtypeIds, list, tuple, schemas.Unset] = schemas.unset,
-        filterableSubtypes: typing.Union[MetaOapg.properties.filterableSubtypes, list, tuple, schemas.Unset] = schemas.unset,
-        availableSubtypeIds: typing.Union[MetaOapg.properties.availableSubtypeIds, list, tuple, schemas.Unset] = schemas.unset,
-        availableSubtypes: typing.Union[MetaOapg.properties.availableSubtypes, list, tuple, schemas.Unset] = schemas.unset,
-        supervisorIds: typing.Union[MetaOapg.properties.supervisorIds, list, tuple, schemas.Unset] = schemas.unset,
-        supervisors: typing.Union[MetaOapg.properties.supervisors, list, tuple, schemas.Unset] = schemas.unset,
-        delegationManagerIds: typing.Union[MetaOapg.properties.delegationManagerIds, list, tuple, schemas.Unset] = schemas.unset,
-        delegationManagers: typing.Union[MetaOapg.properties.delegationManagers, list, tuple, schemas.Unset] = schemas.unset,
+        creationWorkflowId: typing.Union[MetaOapg.properties.creationWorkflowId, None, str, schemas.Unset] = schemas.unset,
+        validationWorkflowId: typing.Union[MetaOapg.properties.validationWorkflowId, str, schemas.Unset] = schemas.unset,
+        workflowSelectionScript: typing.Union[MetaOapg.properties.workflowSelectionScript, None, str, schemas.Unset] = schemas.unset,
+        annotationsAllowed: typing.Union[MetaOapg.properties.annotationsAllowed, bool, schemas.Unset] = schemas.unset,
+        externalSignatureAutomatic: typing.Union[MetaOapg.properties.externalSignatureAutomatic, bool, schemas.Unset] = schemas.unset,
+        secureMailServerId: typing.Union[MetaOapg.properties.secureMailServerId, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        sealCertificateId: typing.Union[MetaOapg.properties.sealCertificateId, None, str, schemas.Unset] = schemas.unset,
+        subtypeMetadataList: typing.Union[MetaOapg.properties.subtypeMetadataList, list, tuple, schemas.Unset] = schemas.unset,
+        subtypeLayers: typing.Union[MetaOapg.properties.subtypeLayers, list, tuple, schemas.Unset] = schemas.unset,
+        externalSignatureConfigId: typing.Union[MetaOapg.properties.externalSignatureConfigId, None, str, schemas.Unset] = schemas.unset,
+        externalSignatureConfig: typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset] = schemas.unset,
+        creationPermittedDeskIds: typing.Union[MetaOapg.properties.creationPermittedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        creationPermittedDesks: typing.Union[MetaOapg.properties.creationPermittedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        filterableByDeskIds: typing.Union[MetaOapg.properties.filterableByDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        filterableByDesks: typing.Union[MetaOapg.properties.filterableByDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        maxMainDocuments: typing.Union[MetaOapg.properties.maxMainDocuments, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        multiDocuments: typing.Union[MetaOapg.properties.multiDocuments, bool, schemas.Unset] = schemas.unset,
+        annexeIncluded: typing.Union[MetaOapg.properties.annexeIncluded, bool, schemas.Unset] = schemas.unset,
+        digitalSignatureMandatory: typing.Union[MetaOapg.properties.digitalSignatureMandatory, bool, schemas.Unset] = schemas.unset,
+        readingMandatory: typing.Union[MetaOapg.properties.readingMandatory, bool, schemas.Unset] = schemas.unset,
+        sealAutomatic: typing.Union[MetaOapg.properties.sealAutomatic, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'DeskDto':
+    ) -> 'SubtypeDto':
         return super().__new__(
             cls,
             *_args,
-            ownerIds=ownerIds,
             name=name,
-            shortName=shortName,
             id=id,
-            tenantId=tenantId,
             description=description,
-            folderCreationAllowed=folderCreationAllowed,
-            actionAllowed=actionAllowed,
-            archivingAllowed=archivingAllowed,
-            chainAllowed=chainAllowed,
-            parentDeskId=parentDeskId,
-            parentDesk=parentDesk,
-            owners=owners,
-            associatedDeskIds=associatedDeskIds,
-            associatedDesks=associatedDesks,
-            filterableMetadataIds=filterableMetadataIds,
-            filterableMetadata=filterableMetadata,
-            filterableSubtypeIds=filterableSubtypeIds,
-            filterableSubtypes=filterableSubtypes,
-            availableSubtypeIds=availableSubtypeIds,
-            availableSubtypes=availableSubtypes,
-            supervisorIds=supervisorIds,
-            supervisors=supervisors,
-            delegationManagerIds=delegationManagerIds,
-            delegationManagers=delegationManagers,
+            creationWorkflowId=creationWorkflowId,
+            validationWorkflowId=validationWorkflowId,
+            workflowSelectionScript=workflowSelectionScript,
+            annotationsAllowed=annotationsAllowed,
+            externalSignatureAutomatic=externalSignatureAutomatic,
+            secureMailServerId=secureMailServerId,
+            sealCertificateId=sealCertificateId,
+            subtypeMetadataList=subtypeMetadataList,
+            subtypeLayers=subtypeLayers,
+            externalSignatureConfigId=externalSignatureConfigId,
+            externalSignatureConfig=externalSignatureConfig,
+            creationPermittedDeskIds=creationPermittedDeskIds,
+            creationPermittedDesks=creationPermittedDesks,
+            filterableByDeskIds=filterableByDeskIds,
+            filterableByDesks=filterableByDesks,
+            maxMainDocuments=maxMainDocuments,
+            multiDocuments=multiDocuments,
+            annexeIncluded=annexeIncluded,
+            digitalSignatureMandatory=digitalSignatureMandatory,
+            readingMandatory=readingMandatory,
+            sealAutomatic=sealAutomatic,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
-from iparapheur_provisioning.model.metadata_representation import MetadataRepresentation
-from iparapheur_provisioning.model.typology_representation import TypologyRepresentation
-from iparapheur_provisioning.model.user_representation import UserRepresentation
+from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
+from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
+from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/desk_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/error_response.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/external_signature_config_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/external_signature_provider.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/folder_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/internal_metadata.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/layer_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/layer_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/metadata_type.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_desk_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_desk_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'DeskRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "numberOfElements": numberOfElements,
-                "pageable": pageable,
                 "first": first,
                 "last": last,
+                "numberOfElements": numberOfElements,
+                "pageable": pageable,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
+        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageDeskRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            numberOfElements=numberOfElements,
-            pageable=pageable,
             first=first,
             last=last,
+            numberOfElements=numberOfElements,
+            pageable=pageable,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
 from iparapheur_provisioning.model.pageable_object import PageableObject
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_subtype_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_subtype_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'SubtypeRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "numberOfElements": numberOfElements,
-                "pageable": pageable,
                 "first": first,
                 "last": last,
+                "numberOfElements": numberOfElements,
+                "pageable": pageable,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
+        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageSubtypeRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            numberOfElements=numberOfElements,
-            pageable=pageable,
             first=first,
             last=last,
+            numberOfElements=numberOfElements,
+            pageable=pageable,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_type_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_type_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'TypeRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "numberOfElements": numberOfElements,
-                "pageable": pageable,
                 "first": first,
                 "last": last,
+                "numberOfElements": numberOfElements,
+                "pageable": pageable,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
+        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageTypeRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            numberOfElements=numberOfElements,
-            pageable=pageable,
             first=first,
             last=last,
+            numberOfElements=numberOfElements,
+            pageable=pageable,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/page_user_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/page_user_representation.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,33 +67,33 @@
                 def __getitem__(self, i: int) -> 'UserRepresentation':
                     return super().__getitem__(i)
             number = schemas.Int32Schema
         
             @staticmethod
             def sort() -> typing.Type['SortObject']:
                 return SortObject
+            first = schemas.BoolSchema
+            last = schemas.BoolSchema
             numberOfElements = schemas.Int32Schema
         
             @staticmethod
             def pageable() -> typing.Type['PageableObject']:
                 return PageableObject
-            first = schemas.BoolSchema
-            last = schemas.BoolSchema
             empty = schemas.BoolSchema
             __annotations__ = {
                 "totalElements": totalElements,
                 "totalPages": totalPages,
                 "size": size,
                 "content": content,
                 "number": number,
                 "sort": sort,
-                "numberOfElements": numberOfElements,
-                "pageable": pageable,
                 "first": first,
                 "last": last,
+                "numberOfElements": numberOfElements,
+                "pageable": pageable,
                 "empty": empty,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["totalElements"]) -> MetaOapg.properties.totalElements: ...
     
     @typing.overload
@@ -108,32 +108,32 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["number"]) -> MetaOapg.properties.number: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["sort"]) -> 'SortObject': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
+    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
+    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["first"]) -> MetaOapg.properties.first: ...
+    def __getitem__(self, name: typing_extensions.Literal["numberOfElements"]) -> MetaOapg.properties.numberOfElements: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["last"]) -> MetaOapg.properties.last: ...
+    def __getitem__(self, name: typing_extensions.Literal["pageable"]) -> 'PageableObject': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["empty"]) -> MetaOapg.properties.empty: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["totalElements"]) -> typing.Union[MetaOapg.properties.totalElements, schemas.Unset]: ...
     
@@ -149,65 +149,65 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["number"]) -> typing.Union[MetaOapg.properties.number, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["sort"]) -> typing.Union['SortObject', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["first"]) -> typing.Union[MetaOapg.properties.first, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["numberOfElements"]) -> typing.Union[MetaOapg.properties.numberOfElements, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["last"]) -> typing.Union[MetaOapg.properties.last, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["pageable"]) -> typing.Union['PageableObject', schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["empty"]) -> typing.Union[MetaOapg.properties.empty, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "numberOfElements", "pageable", "first", "last", "empty", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["totalElements", "totalPages", "size", "content", "number", "sort", "first", "last", "numberOfElements", "pageable", "empty", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         totalElements: typing.Union[MetaOapg.properties.totalElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         totalPages: typing.Union[MetaOapg.properties.totalPages, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         content: typing.Union[MetaOapg.properties.content, list, tuple, schemas.Unset] = schemas.unset,
         number: typing.Union[MetaOapg.properties.number, decimal.Decimal, int, schemas.Unset] = schemas.unset,
         sort: typing.Union['SortObject', schemas.Unset] = schemas.unset,
-        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         first: typing.Union[MetaOapg.properties.first, bool, schemas.Unset] = schemas.unset,
         last: typing.Union[MetaOapg.properties.last, bool, schemas.Unset] = schemas.unset,
+        numberOfElements: typing.Union[MetaOapg.properties.numberOfElements, decimal.Decimal, int, schemas.Unset] = schemas.unset,
+        pageable: typing.Union['PageableObject', schemas.Unset] = schemas.unset,
         empty: typing.Union[MetaOapg.properties.empty, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'PageUserRepresentation':
         return super().__new__(
             cls,
             *_args,
             totalElements=totalElements,
             totalPages=totalPages,
             size=size,
             content=content,
             number=number,
             sort=sort,
-            numberOfElements=numberOfElements,
-            pageable=pageable,
             first=first,
             last=last,
+            numberOfElements=numberOfElements,
+            pageable=pageable,
             empty=empty,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.pageable_object import PageableObject
 from iparapheur_provisioning.model.sort_object import SortObject
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/pageable_object.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/pdf_signature_position.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/signature_format.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/signature_protocol.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/sort_object.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_dto.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,226 +20,271 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class SubtypeDto(
+class UserDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
+
+    Every field is mandatory
     """
 
 
     class MetaOapg:
         required = {
-            "name",
+            "firstName",
+            "lastName",
+            "privilege",
+            "userName",
+            "email",
         }
         
         class properties:
             
             
-            class name(
+            class userName(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 255
-                    min_length = 2
-                    regex=[{
-                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
-                    }]
-            id = schemas.StrSchema
+                    max_length = 128
+                    min_length = 1
             
             
-            class description(
+            class firstName(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 255
-                    min_length = 3
+                    max_length = 128
+                    min_length = 0
             
             
-            class creationWorkflowId(
-                schemas.StrBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneStrMixin
+            class lastName(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 128
+                    min_length = 0
+            email = schemas.StrSchema
+        
+            @staticmethod
+            def privilege() -> typing.Type['UserPrivilege']:
+                return UserPrivilege
+            id = schemas.StrSchema
+            isLdapSynchronized = schemas.BoolSchema
+            
+            
+            class associatedTenants(
+                schemas.ListSchema
             ):
             
             
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['TenantRepresentation']:
+                        return TenantRepresentation
+            
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, str, ],
+                    _arg: typing.Union[typing.Tuple['TenantRepresentation'], typing.List['TenantRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'creationWorkflowId':
+                ) -> 'associatedTenants':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
-            validationWorkflowId = schemas.StrSchema
             
+                def __getitem__(self, i: int) -> 'TenantRepresentation':
+                    return super().__getitem__(i)
             
-            class workflowSelectionScript(
-                schemas.StrBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneStrMixin
+            
+            class associatedTenantIds(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 65535
-                    min_length = 0
-            
+                    items = schemas.StrSchema
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, str, ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'workflowSelectionScript':
+                ) -> 'associatedTenantIds':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
-            annotationsAllowed = schemas.BoolSchema
-            externalSignatureAutomatic = schemas.BoolSchema
             
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
             
-            class secureMailServerId(
-                schemas.Int64Base,
-                schemas.IntBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneDecimalMixin
+            
+            class administeredTenants(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    format = 'int64'
-            
+                    
+                    @staticmethod
+                    def items() -> typing.Type['TenantRepresentation']:
+                        return TenantRepresentation
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, decimal.Decimal, int, ],
+                    _arg: typing.Union[typing.Tuple['TenantRepresentation'], typing.List['TenantRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'secureMailServerId':
+                ) -> 'administeredTenants':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> 'TenantRepresentation':
+                    return super().__getitem__(i)
             
-            class sealCertificateId(
-                schemas.StrBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneStrMixin
+            
+            class administeredTenantIds(
+                schemas.ListSchema
             ):
             
             
+                class MetaOapg:
+                    items = schemas.StrSchema
+            
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, str, ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'sealCertificateId':
+                ) -> 'administeredTenantIds':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
             
-            class subtypeMetadataList(
-                schemas.ListSchema
+            
+            class administeredDesks(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['SubtypeMetadataDto']:
-                        return SubtypeMetadataDto
+                    def items() -> typing.Type['DeskRepresentation']:
+                        return DeskRepresentation
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['SubtypeMetadataDto'], typing.List['SubtypeMetadataDto']],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'subtypeMetadataList':
+                ) -> 'administeredDesks':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SubtypeMetadataDto':
-                    return super().__getitem__(i)
-            
             
-            class subtypeLayers(
-                schemas.ListSchema
+            class administeredDeskIds(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
             ):
             
             
                 class MetaOapg:
                     
-                    @staticmethod
-                    def items() -> typing.Type['SubtypeLayerDto']:
-                        return SubtypeLayerDto
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
+            
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['SubtypeLayerDto'], typing.List['SubtypeLayerDto']],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'subtypeLayers':
+                ) -> 'administeredDeskIds':
                     return super().__new__(
                         cls,
-                        _arg,
+                        *_args,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'SubtypeLayerDto':
-                    return super().__getitem__(i)
-            
             
-            class externalSignatureConfigId(
-                schemas.StrBase,
+            class associatedDesks(
+                schemas.ListBase,
                 schemas.NoneBase,
                 schemas.Schema,
-                schemas.NoneStrMixin
+                schemas.NoneTupleMixin
             ):
             
             
+                class MetaOapg:
+                    
+                    @staticmethod
+                    def items() -> typing.Type['DeskRepresentation']:
+                        return DeskRepresentation
+            
+            
                 def __new__(
                     cls,
-                    *_args: typing.Union[None, str, ],
+                    *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'externalSignatureConfigId':
+                ) -> 'associatedDesks':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
-        
-            @staticmethod
-            def externalSignatureConfig() -> typing.Type['ExternalSignatureConfigRepresentation']:
-                return ExternalSignatureConfigRepresentation
             
             
-            class creationPermittedDeskIds(
+            class associatedDeskIds(
                 schemas.ListBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneTupleMixin
             ):
             
             
@@ -266,23 +311,23 @@
                             )
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'creationPermittedDeskIds':
+                ) -> 'associatedDeskIds':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
             
             
-            class creationPermittedDesks(
+            class supervisedDesks(
                 schemas.ListBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneTupleMixin
             ):
             
             
@@ -293,23 +338,23 @@
                         return DeskRepresentation
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'creationPermittedDesks':
+                ) -> 'supervisedDesks':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
             
             
-            class filterableByDeskIds(
+            class supervisedDeskIds(
                 schemas.ListBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneTupleMixin
             ):
             
             
@@ -336,23 +381,23 @@
                             )
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'filterableByDeskIds':
+                ) -> 'supervisedDeskIds':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
             
             
-            class filterableByDesks(
+            class delegationManagedDesks(
                 schemas.ListBase,
                 schemas.NoneBase,
                 schemas.Schema,
                 schemas.NoneTupleMixin
             ):
             
             
@@ -363,272 +408,306 @@
                         return DeskRepresentation
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[list, tuple, None, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'filterableByDesks':
+                ) -> 'delegationManagedDesks':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                    )
+            
+            
+            class delegationManagedDeskIds(
+                schemas.ListBase,
+                schemas.NoneBase,
+                schemas.Schema,
+                schemas.NoneTupleMixin
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    
+                    class items(
+                        schemas.StrBase,
+                        schemas.NoneBase,
+                        schemas.Schema,
+                        schemas.NoneStrMixin
+                    ):
+                    
+                    
+                        def __new__(
+                            cls,
+                            *_args: typing.Union[None, str, ],
+                            _configuration: typing.Optional[schemas.Configuration] = None,
+                        ) -> 'items':
+                            return super().__new__(
+                                cls,
+                                *_args,
+                                _configuration=_configuration,
+                            )
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[list, tuple, None, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                ) -> 'delegationManagedDeskIds':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                     )
-            maxMainDocuments = schemas.Int32Schema
-            multiDocuments = schemas.BoolSchema
-            annexeIncluded = schemas.BoolSchema
-            digitalSignatureMandatory = schemas.BoolSchema
-            readingMandatory = schemas.BoolSchema
-            sealAutomatic = schemas.BoolSchema
+            
+            
+            class complementaryField(
+                schemas.StrSchema
+            ):
+            
+            
+                class MetaOapg:
+                    max_length = 255
+                    min_length = 0
+            resetPasswordRequired = schemas.BoolSchema
+            password = schemas.StrSchema
             __annotations__ = {
-                "name": name,
+                "userName": userName,
+                "firstName": firstName,
+                "lastName": lastName,
+                "email": email,
+                "privilege": privilege,
                 "id": id,
-                "description": description,
-                "creationWorkflowId": creationWorkflowId,
-                "validationWorkflowId": validationWorkflowId,
-                "workflowSelectionScript": workflowSelectionScript,
-                "annotationsAllowed": annotationsAllowed,
-                "externalSignatureAutomatic": externalSignatureAutomatic,
-                "secureMailServerId": secureMailServerId,
-                "sealCertificateId": sealCertificateId,
-                "subtypeMetadataList": subtypeMetadataList,
-                "subtypeLayers": subtypeLayers,
-                "externalSignatureConfigId": externalSignatureConfigId,
-                "externalSignatureConfig": externalSignatureConfig,
-                "creationPermittedDeskIds": creationPermittedDeskIds,
-                "creationPermittedDesks": creationPermittedDesks,
-                "filterableByDeskIds": filterableByDeskIds,
-                "filterableByDesks": filterableByDesks,
-                "maxMainDocuments": maxMainDocuments,
-                "multiDocuments": multiDocuments,
-                "annexeIncluded": annexeIncluded,
-                "digitalSignatureMandatory": digitalSignatureMandatory,
-                "readingMandatory": readingMandatory,
-                "sealAutomatic": sealAutomatic,
+                "isLdapSynchronized": isLdapSynchronized,
+                "associatedTenants": associatedTenants,
+                "associatedTenantIds": associatedTenantIds,
+                "administeredTenants": administeredTenants,
+                "administeredTenantIds": administeredTenantIds,
+                "administeredDesks": administeredDesks,
+                "administeredDeskIds": administeredDeskIds,
+                "associatedDesks": associatedDesks,
+                "associatedDeskIds": associatedDeskIds,
+                "supervisedDesks": supervisedDesks,
+                "supervisedDeskIds": supervisedDeskIds,
+                "delegationManagedDesks": delegationManagedDesks,
+                "delegationManagedDeskIds": delegationManagedDeskIds,
+                "complementaryField": complementaryField,
+                "resetPasswordRequired": resetPasswordRequired,
+                "password": password,
             }
     
-    name: MetaOapg.properties.name
+    firstName: MetaOapg.properties.firstName
+    lastName: MetaOapg.properties.lastName
+    privilege: 'UserPrivilege'
+    userName: MetaOapg.properties.userName
+    email: MetaOapg.properties.email
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
+    def __getitem__(self, name: typing_extensions.Literal["userName"]) -> MetaOapg.properties.userName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["firstName"]) -> MetaOapg.properties.firstName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
+    def __getitem__(self, name: typing_extensions.Literal["lastName"]) -> MetaOapg.properties.lastName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["creationWorkflowId"]) -> MetaOapg.properties.creationWorkflowId: ...
+    def __getitem__(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["validationWorkflowId"]) -> MetaOapg.properties.validationWorkflowId: ...
+    def __getitem__(self, name: typing_extensions.Literal["privilege"]) -> 'UserPrivilege': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["workflowSelectionScript"]) -> MetaOapg.properties.workflowSelectionScript: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["annotationsAllowed"]) -> MetaOapg.properties.annotationsAllowed: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["externalSignatureAutomatic"]) -> MetaOapg.properties.externalSignatureAutomatic: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["secureMailServerId"]) -> MetaOapg.properties.secureMailServerId: ...
+    def __getitem__(self, name: typing_extensions.Literal["isLdapSynchronized"]) -> MetaOapg.properties.isLdapSynchronized: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sealCertificateId"]) -> MetaOapg.properties.sealCertificateId: ...
+    def __getitem__(self, name: typing_extensions.Literal["associatedTenants"]) -> MetaOapg.properties.associatedTenants: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["subtypeMetadataList"]) -> MetaOapg.properties.subtypeMetadataList: ...
+    def __getitem__(self, name: typing_extensions.Literal["associatedTenantIds"]) -> MetaOapg.properties.associatedTenantIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["subtypeLayers"]) -> MetaOapg.properties.subtypeLayers: ...
+    def __getitem__(self, name: typing_extensions.Literal["administeredTenants"]) -> MetaOapg.properties.administeredTenants: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> MetaOapg.properties.externalSignatureConfigId: ...
+    def __getitem__(self, name: typing_extensions.Literal["administeredTenantIds"]) -> MetaOapg.properties.administeredTenantIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> 'ExternalSignatureConfigRepresentation': ...
+    def __getitem__(self, name: typing_extensions.Literal["administeredDesks"]) -> MetaOapg.properties.administeredDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> MetaOapg.properties.creationPermittedDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["administeredDeskIds"]) -> MetaOapg.properties.administeredDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["creationPermittedDesks"]) -> MetaOapg.properties.creationPermittedDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["associatedDesks"]) -> MetaOapg.properties.associatedDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> MetaOapg.properties.filterableByDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["associatedDeskIds"]) -> MetaOapg.properties.associatedDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["filterableByDesks"]) -> MetaOapg.properties.filterableByDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["supervisedDesks"]) -> MetaOapg.properties.supervisedDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["maxMainDocuments"]) -> MetaOapg.properties.maxMainDocuments: ...
+    def __getitem__(self, name: typing_extensions.Literal["supervisedDeskIds"]) -> MetaOapg.properties.supervisedDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["multiDocuments"]) -> MetaOapg.properties.multiDocuments: ...
+    def __getitem__(self, name: typing_extensions.Literal["delegationManagedDesks"]) -> MetaOapg.properties.delegationManagedDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["annexeIncluded"]) -> MetaOapg.properties.annexeIncluded: ...
+    def __getitem__(self, name: typing_extensions.Literal["delegationManagedDeskIds"]) -> MetaOapg.properties.delegationManagedDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> MetaOapg.properties.digitalSignatureMandatory: ...
+    def __getitem__(self, name: typing_extensions.Literal["complementaryField"]) -> MetaOapg.properties.complementaryField: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["readingMandatory"]) -> MetaOapg.properties.readingMandatory: ...
+    def __getitem__(self, name: typing_extensions.Literal["resetPasswordRequired"]) -> MetaOapg.properties.resetPasswordRequired: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["sealAutomatic"]) -> MetaOapg.properties.sealAutomatic: ...
+    def __getitem__(self, name: typing_extensions.Literal["password"]) -> MetaOapg.properties.password: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["userName", "firstName", "lastName", "email", "privilege", "id", "isLdapSynchronized", "associatedTenants", "associatedTenantIds", "administeredTenants", "administeredTenantIds", "administeredDesks", "administeredDeskIds", "associatedDesks", "associatedDeskIds", "supervisedDesks", "supervisedDeskIds", "delegationManagedDesks", "delegationManagedDeskIds", "complementaryField", "resetPasswordRequired", "password", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["userName"]) -> MetaOapg.properties.userName: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["firstName"]) -> MetaOapg.properties.firstName: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["creationWorkflowId"]) -> typing.Union[MetaOapg.properties.creationWorkflowId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["lastName"]) -> MetaOapg.properties.lastName: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["validationWorkflowId"]) -> typing.Union[MetaOapg.properties.validationWorkflowId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["workflowSelectionScript"]) -> typing.Union[MetaOapg.properties.workflowSelectionScript, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["privilege"]) -> 'UserPrivilege': ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["annotationsAllowed"]) -> typing.Union[MetaOapg.properties.annotationsAllowed, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureAutomatic"]) -> typing.Union[MetaOapg.properties.externalSignatureAutomatic, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["secureMailServerId"]) -> typing.Union[MetaOapg.properties.secureMailServerId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["isLdapSynchronized"]) -> typing.Union[MetaOapg.properties.isLdapSynchronized, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sealCertificateId"]) -> typing.Union[MetaOapg.properties.sealCertificateId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["associatedTenants"]) -> typing.Union[MetaOapg.properties.associatedTenants, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["subtypeMetadataList"]) -> typing.Union[MetaOapg.properties.subtypeMetadataList, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["associatedTenantIds"]) -> typing.Union[MetaOapg.properties.associatedTenantIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["subtypeLayers"]) -> typing.Union[MetaOapg.properties.subtypeLayers, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["administeredTenants"]) -> typing.Union[MetaOapg.properties.administeredTenants, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfigId"]) -> typing.Union[MetaOapg.properties.externalSignatureConfigId, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["administeredTenantIds"]) -> typing.Union[MetaOapg.properties.administeredTenantIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["externalSignatureConfig"]) -> typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["administeredDesks"]) -> typing.Union[MetaOapg.properties.administeredDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDeskIds"]) -> typing.Union[MetaOapg.properties.creationPermittedDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["administeredDeskIds"]) -> typing.Union[MetaOapg.properties.administeredDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["creationPermittedDesks"]) -> typing.Union[MetaOapg.properties.creationPermittedDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["associatedDesks"]) -> typing.Union[MetaOapg.properties.associatedDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDeskIds"]) -> typing.Union[MetaOapg.properties.filterableByDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["associatedDeskIds"]) -> typing.Union[MetaOapg.properties.associatedDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["filterableByDesks"]) -> typing.Union[MetaOapg.properties.filterableByDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["supervisedDesks"]) -> typing.Union[MetaOapg.properties.supervisedDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["maxMainDocuments"]) -> typing.Union[MetaOapg.properties.maxMainDocuments, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["supervisedDeskIds"]) -> typing.Union[MetaOapg.properties.supervisedDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["multiDocuments"]) -> typing.Union[MetaOapg.properties.multiDocuments, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagedDesks"]) -> typing.Union[MetaOapg.properties.delegationManagedDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["annexeIncluded"]) -> typing.Union[MetaOapg.properties.annexeIncluded, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagedDeskIds"]) -> typing.Union[MetaOapg.properties.delegationManagedDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["digitalSignatureMandatory"]) -> typing.Union[MetaOapg.properties.digitalSignatureMandatory, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["complementaryField"]) -> typing.Union[MetaOapg.properties.complementaryField, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["readingMandatory"]) -> typing.Union[MetaOapg.properties.readingMandatory, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["resetPasswordRequired"]) -> typing.Union[MetaOapg.properties.resetPasswordRequired, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["sealAutomatic"]) -> typing.Union[MetaOapg.properties.sealAutomatic, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["password"]) -> typing.Union[MetaOapg.properties.password, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "description", "creationWorkflowId", "validationWorkflowId", "workflowSelectionScript", "annotationsAllowed", "externalSignatureAutomatic", "secureMailServerId", "sealCertificateId", "subtypeMetadataList", "subtypeLayers", "externalSignatureConfigId", "externalSignatureConfig", "creationPermittedDeskIds", "creationPermittedDesks", "filterableByDeskIds", "filterableByDesks", "maxMainDocuments", "multiDocuments", "annexeIncluded", "digitalSignatureMandatory", "readingMandatory", "sealAutomatic", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["userName", "firstName", "lastName", "email", "privilege", "id", "isLdapSynchronized", "associatedTenants", "associatedTenantIds", "administeredTenants", "administeredTenantIds", "administeredDesks", "administeredDeskIds", "associatedDesks", "associatedDeskIds", "supervisedDesks", "supervisedDeskIds", "delegationManagedDesks", "delegationManagedDeskIds", "complementaryField", "resetPasswordRequired", "password", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
+        firstName: typing.Union[MetaOapg.properties.firstName, str, ],
+        lastName: typing.Union[MetaOapg.properties.lastName, str, ],
+        privilege: 'UserPrivilege',
+        userName: typing.Union[MetaOapg.properties.userName, str, ],
+        email: typing.Union[MetaOapg.properties.email, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
-        creationWorkflowId: typing.Union[MetaOapg.properties.creationWorkflowId, None, str, schemas.Unset] = schemas.unset,
-        validationWorkflowId: typing.Union[MetaOapg.properties.validationWorkflowId, str, schemas.Unset] = schemas.unset,
-        workflowSelectionScript: typing.Union[MetaOapg.properties.workflowSelectionScript, None, str, schemas.Unset] = schemas.unset,
-        annotationsAllowed: typing.Union[MetaOapg.properties.annotationsAllowed, bool, schemas.Unset] = schemas.unset,
-        externalSignatureAutomatic: typing.Union[MetaOapg.properties.externalSignatureAutomatic, bool, schemas.Unset] = schemas.unset,
-        secureMailServerId: typing.Union[MetaOapg.properties.secureMailServerId, None, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        sealCertificateId: typing.Union[MetaOapg.properties.sealCertificateId, None, str, schemas.Unset] = schemas.unset,
-        subtypeMetadataList: typing.Union[MetaOapg.properties.subtypeMetadataList, list, tuple, schemas.Unset] = schemas.unset,
-        subtypeLayers: typing.Union[MetaOapg.properties.subtypeLayers, list, tuple, schemas.Unset] = schemas.unset,
-        externalSignatureConfigId: typing.Union[MetaOapg.properties.externalSignatureConfigId, None, str, schemas.Unset] = schemas.unset,
-        externalSignatureConfig: typing.Union['ExternalSignatureConfigRepresentation', schemas.Unset] = schemas.unset,
-        creationPermittedDeskIds: typing.Union[MetaOapg.properties.creationPermittedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
-        creationPermittedDesks: typing.Union[MetaOapg.properties.creationPermittedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
-        filterableByDeskIds: typing.Union[MetaOapg.properties.filterableByDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
-        filterableByDesks: typing.Union[MetaOapg.properties.filterableByDesks, list, tuple, None, schemas.Unset] = schemas.unset,
-        maxMainDocuments: typing.Union[MetaOapg.properties.maxMainDocuments, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        multiDocuments: typing.Union[MetaOapg.properties.multiDocuments, bool, schemas.Unset] = schemas.unset,
-        annexeIncluded: typing.Union[MetaOapg.properties.annexeIncluded, bool, schemas.Unset] = schemas.unset,
-        digitalSignatureMandatory: typing.Union[MetaOapg.properties.digitalSignatureMandatory, bool, schemas.Unset] = schemas.unset,
-        readingMandatory: typing.Union[MetaOapg.properties.readingMandatory, bool, schemas.Unset] = schemas.unset,
-        sealAutomatic: typing.Union[MetaOapg.properties.sealAutomatic, bool, schemas.Unset] = schemas.unset,
+        isLdapSynchronized: typing.Union[MetaOapg.properties.isLdapSynchronized, bool, schemas.Unset] = schemas.unset,
+        associatedTenants: typing.Union[MetaOapg.properties.associatedTenants, list, tuple, schemas.Unset] = schemas.unset,
+        associatedTenantIds: typing.Union[MetaOapg.properties.associatedTenantIds, list, tuple, schemas.Unset] = schemas.unset,
+        administeredTenants: typing.Union[MetaOapg.properties.administeredTenants, list, tuple, schemas.Unset] = schemas.unset,
+        administeredTenantIds: typing.Union[MetaOapg.properties.administeredTenantIds, list, tuple, schemas.Unset] = schemas.unset,
+        administeredDesks: typing.Union[MetaOapg.properties.administeredDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        administeredDeskIds: typing.Union[MetaOapg.properties.administeredDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        associatedDesks: typing.Union[MetaOapg.properties.associatedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        associatedDeskIds: typing.Union[MetaOapg.properties.associatedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        supervisedDesks: typing.Union[MetaOapg.properties.supervisedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        supervisedDeskIds: typing.Union[MetaOapg.properties.supervisedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        delegationManagedDesks: typing.Union[MetaOapg.properties.delegationManagedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
+        delegationManagedDeskIds: typing.Union[MetaOapg.properties.delegationManagedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
+        complementaryField: typing.Union[MetaOapg.properties.complementaryField, str, schemas.Unset] = schemas.unset,
+        resetPasswordRequired: typing.Union[MetaOapg.properties.resetPasswordRequired, bool, schemas.Unset] = schemas.unset,
+        password: typing.Union[MetaOapg.properties.password, str, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SubtypeDto':
+    ) -> 'UserDto':
         return super().__new__(
             cls,
             *_args,
-            name=name,
+            firstName=firstName,
+            lastName=lastName,
+            privilege=privilege,
+            userName=userName,
+            email=email,
             id=id,
-            description=description,
-            creationWorkflowId=creationWorkflowId,
-            validationWorkflowId=validationWorkflowId,
-            workflowSelectionScript=workflowSelectionScript,
-            annotationsAllowed=annotationsAllowed,
-            externalSignatureAutomatic=externalSignatureAutomatic,
-            secureMailServerId=secureMailServerId,
-            sealCertificateId=sealCertificateId,
-            subtypeMetadataList=subtypeMetadataList,
-            subtypeLayers=subtypeLayers,
-            externalSignatureConfigId=externalSignatureConfigId,
-            externalSignatureConfig=externalSignatureConfig,
-            creationPermittedDeskIds=creationPermittedDeskIds,
-            creationPermittedDesks=creationPermittedDesks,
-            filterableByDeskIds=filterableByDeskIds,
-            filterableByDesks=filterableByDesks,
-            maxMainDocuments=maxMainDocuments,
-            multiDocuments=multiDocuments,
-            annexeIncluded=annexeIncluded,
-            digitalSignatureMandatory=digitalSignatureMandatory,
-            readingMandatory=readingMandatory,
-            sealAutomatic=sealAutomatic,
+            isLdapSynchronized=isLdapSynchronized,
+            associatedTenants=associatedTenants,
+            associatedTenantIds=associatedTenantIds,
+            administeredTenants=administeredTenants,
+            administeredTenantIds=administeredTenantIds,
+            administeredDesks=administeredDesks,
+            administeredDeskIds=administeredDeskIds,
+            associatedDesks=associatedDesks,
+            associatedDeskIds=associatedDeskIds,
+            supervisedDesks=supervisedDesks,
+            supervisedDeskIds=supervisedDeskIds,
+            delegationManagedDesks=delegationManagedDesks,
+            delegationManagedDeskIds=delegationManagedDeskIds,
+            complementaryField=complementaryField,
+            resetPasswordRequired=resetPasswordRequired,
+            password=password,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
-from iparapheur_provisioning.model.external_signature_config_representation import ExternalSignatureConfigRepresentation
-from iparapheur_provisioning.model.subtype_layer_dto import SubtypeLayerDto
-from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
+from iparapheur_provisioning.model.tenant_representation import TenantRepresentation
+from iparapheur_provisioning.model.user_privilege import UserPrivilege
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_layer_association.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_layer_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/subtype_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/tenant_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/tenant_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/tenant_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/type_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/type_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/typology_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_dto.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/desk_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,694 +20,536 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from iparapheur_provisioning import schemas  # noqa: F401
 
 
-class UserDto(
+class DeskDto(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
-    Every field is mandatory
+    body
     """
 
 
     class MetaOapg:
         required = {
-            "firstName",
-            "lastName",
-            "privilege",
-            "userName",
-            "email",
+            "ownerIds",
+            "name",
+            "shortName",
         }
         
         class properties:
             
             
-            class userName(
+            class name(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 128
-                    min_length = 1
-            
-            
-            class firstName(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 128
-                    min_length = 0
+                    max_length = 255
+                    min_length = 2
+                    regex=[{
+                        'pattern': r'^[^\r\n ]+$',  # noqa: E501
+                    }]
             
             
-            class lastName(
+            class shortName(
                 schemas.StrSchema
             ):
             
             
                 class MetaOapg:
-                    max_length = 128
-                    min_length = 0
-            email = schemas.StrSchema
-        
-            @staticmethod
-            def privilege() -> typing.Type['UserPrivilege']:
-                return UserPrivilege
-            id = schemas.StrSchema
-            isLdapSynchronized = schemas.BoolSchema
-            
-            
-            class associatedTenants(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['TenantRepresentation']:
-                        return TenantRepresentation
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['TenantRepresentation'], typing.List['TenantRepresentation']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'associatedTenants':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'TenantRepresentation':
-                    return super().__getitem__(i)
+                    max_length = 255
+                    min_length = 2
             
             
-            class associatedTenantIds(
+            class ownerIds(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
+                    max_items = 256
+                    min_items = 0
                     items = schemas.StrSchema
             
                 def __new__(
                     cls,
                     _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'associatedTenantIds':
+                ) -> 'ownerIds':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
+            id = schemas.StrSchema
+            tenantId = schemas.StrSchema
+            description = schemas.StrSchema
+            folderCreationAllowed = schemas.BoolSchema
+            actionAllowed = schemas.BoolSchema
+            archivingAllowed = schemas.BoolSchema
+            chainAllowed = schemas.BoolSchema
+            parentDeskId = schemas.StrSchema
+        
+            @staticmethod
+            def parentDesk() -> typing.Type['DeskRepresentation']:
+                return DeskRepresentation
             
             
-            class administeredTenants(
+            class owners(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['TenantRepresentation']:
-                        return TenantRepresentation
+                    def items() -> typing.Type['UserRepresentation']:
+                        return UserRepresentation
             
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['TenantRepresentation'], typing.List['TenantRepresentation']],
+                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'administeredTenants':
+                ) -> 'owners':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
-                def __getitem__(self, i: int) -> 'TenantRepresentation':
+                def __getitem__(self, i: int) -> 'UserRepresentation':
                     return super().__getitem__(i)
             
             
-            class administeredTenantIds(
+            class associatedDeskIds(
                 schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     items = schemas.StrSchema
             
                 def __new__(
                     cls,
                     _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'administeredTenantIds':
+                ) -> 'associatedDeskIds':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
             
                 def __getitem__(self, i: int) -> MetaOapg.items:
                     return super().__getitem__(i)
             
             
-            class administeredDesks(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class associatedDesks(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
                     def items() -> typing.Type['DeskRepresentation']:
                         return DeskRepresentation
             
-            
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple['DeskRepresentation'], typing.List['DeskRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'administeredDesks':
+                ) -> 'associatedDesks':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> 'DeskRepresentation':
+                    return super().__getitem__(i)
+            
             
-            class administeredDeskIds(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class filterableMetadataIds(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    
-                    
-                    class items(
-                        schemas.StrBase,
-                        schemas.NoneBase,
-                        schemas.Schema,
-                        schemas.NoneStrMixin
-                    ):
-                    
-                    
-                        def __new__(
-                            cls,
-                            *_args: typing.Union[None, str, ],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'items':
-                            return super().__new__(
-                                cls,
-                                *_args,
-                                _configuration=_configuration,
-                            )
-            
+                    items = schemas.StrSchema
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'administeredDeskIds':
+                ) -> 'filterableMetadataIds':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+            
             
-            class associatedDesks(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class filterableMetadata(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['DeskRepresentation']:
-                        return DeskRepresentation
-            
+                    def items() -> typing.Type['MetadataRepresentation']:
+                        return MetadataRepresentation
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple['MetadataRepresentation'], typing.List['MetadataRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'associatedDesks':
+                ) -> 'filterableMetadata':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> 'MetadataRepresentation':
+                    return super().__getitem__(i)
+            
             
-            class associatedDeskIds(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class supervisorIds(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    
-                    
-                    class items(
-                        schemas.StrBase,
-                        schemas.NoneBase,
-                        schemas.Schema,
-                        schemas.NoneStrMixin
-                    ):
-                    
-                    
-                        def __new__(
-                            cls,
-                            *_args: typing.Union[None, str, ],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'items':
-                            return super().__new__(
-                                cls,
-                                *_args,
-                                _configuration=_configuration,
-                            )
-            
+                    items = schemas.StrSchema
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'associatedDeskIds':
+                ) -> 'supervisorIds':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+            
             
-            class supervisedDesks(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class supervisors(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
                     @staticmethod
-                    def items() -> typing.Type['DeskRepresentation']:
-                        return DeskRepresentation
-            
+                    def items() -> typing.Type['UserRepresentation']:
+                        return UserRepresentation
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'supervisedDesks':
+                ) -> 'supervisors':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
-            
-            class supervisedDeskIds(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    
-                    class items(
-                        schemas.StrBase,
-                        schemas.NoneBase,
-                        schemas.Schema,
-                        schemas.NoneStrMixin
-                    ):
-                    
-                    
-                        def __new__(
-                            cls,
-                            *_args: typing.Union[None, str, ],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'items':
-                            return super().__new__(
-                                cls,
-                                *_args,
-                                _configuration=_configuration,
-                            )
-            
-            
-                def __new__(
-                    cls,
-                    *_args: typing.Union[list, tuple, None, ],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'supervisedDeskIds':
-                    return super().__new__(
-                        cls,
-                        *_args,
-                        _configuration=_configuration,
-                    )
+                def __getitem__(self, i: int) -> 'UserRepresentation':
+                    return super().__getitem__(i)
             
             
-            class delegationManagedDesks(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class delegationManagerIds(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['DeskRepresentation']:
-                        return DeskRepresentation
-            
+                    items = schemas.StrSchema
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'delegationManagedDesks':
+                ) -> 'delegationManagerIds':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
+                def __getitem__(self, i: int) -> MetaOapg.items:
+                    return super().__getitem__(i)
+            
             
-            class delegationManagedDeskIds(
-                schemas.ListBase,
-                schemas.NoneBase,
-                schemas.Schema,
-                schemas.NoneTupleMixin
+            class delegationManagers(
+                schemas.ListSchema
             ):
             
             
                 class MetaOapg:
                     
-                    
-                    class items(
-                        schemas.StrBase,
-                        schemas.NoneBase,
-                        schemas.Schema,
-                        schemas.NoneStrMixin
-                    ):
-                    
-                    
-                        def __new__(
-                            cls,
-                            *_args: typing.Union[None, str, ],
-                            _configuration: typing.Optional[schemas.Configuration] = None,
-                        ) -> 'items':
-                            return super().__new__(
-                                cls,
-                                *_args,
-                                _configuration=_configuration,
-                            )
-            
+                    @staticmethod
+                    def items() -> typing.Type['UserRepresentation']:
+                        return UserRepresentation
             
                 def __new__(
                     cls,
-                    *_args: typing.Union[list, tuple, None, ],
+                    _arg: typing.Union[typing.Tuple['UserRepresentation'], typing.List['UserRepresentation']],
                     _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'delegationManagedDeskIds':
+                ) -> 'delegationManagers':
                     return super().__new__(
                         cls,
-                        *_args,
+                        _arg,
                         _configuration=_configuration,
                     )
             
-            
-            class complementaryField(
-                schemas.StrSchema
-            ):
-            
-            
-                class MetaOapg:
-                    max_length = 255
-                    min_length = 0
-            resetPasswordRequired = schemas.BoolSchema
-            password = schemas.StrSchema
+                def __getitem__(self, i: int) -> 'UserRepresentation':
+                    return super().__getitem__(i)
             __annotations__ = {
-                "userName": userName,
-                "firstName": firstName,
-                "lastName": lastName,
-                "email": email,
-                "privilege": privilege,
+                "name": name,
+                "shortName": shortName,
+                "ownerIds": ownerIds,
                 "id": id,
-                "isLdapSynchronized": isLdapSynchronized,
-                "associatedTenants": associatedTenants,
-                "associatedTenantIds": associatedTenantIds,
-                "administeredTenants": administeredTenants,
-                "administeredTenantIds": administeredTenantIds,
-                "administeredDesks": administeredDesks,
-                "administeredDeskIds": administeredDeskIds,
-                "associatedDesks": associatedDesks,
+                "tenantId": tenantId,
+                "description": description,
+                "folderCreationAllowed": folderCreationAllowed,
+                "actionAllowed": actionAllowed,
+                "archivingAllowed": archivingAllowed,
+                "chainAllowed": chainAllowed,
+                "parentDeskId": parentDeskId,
+                "parentDesk": parentDesk,
+                "owners": owners,
                 "associatedDeskIds": associatedDeskIds,
-                "supervisedDesks": supervisedDesks,
-                "supervisedDeskIds": supervisedDeskIds,
-                "delegationManagedDesks": delegationManagedDesks,
-                "delegationManagedDeskIds": delegationManagedDeskIds,
-                "complementaryField": complementaryField,
-                "resetPasswordRequired": resetPasswordRequired,
-                "password": password,
+                "associatedDesks": associatedDesks,
+                "filterableMetadataIds": filterableMetadataIds,
+                "filterableMetadata": filterableMetadata,
+                "supervisorIds": supervisorIds,
+                "supervisors": supervisors,
+                "delegationManagerIds": delegationManagerIds,
+                "delegationManagers": delegationManagers,
             }
     
-    firstName: MetaOapg.properties.firstName
-    lastName: MetaOapg.properties.lastName
-    privilege: 'UserPrivilege'
-    userName: MetaOapg.properties.userName
-    email: MetaOapg.properties.email
+    ownerIds: MetaOapg.properties.ownerIds
+    name: MetaOapg.properties.name
+    shortName: MetaOapg.properties.shortName
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["userName"]) -> MetaOapg.properties.userName: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["firstName"]) -> MetaOapg.properties.firstName: ...
+    def __getitem__(self, name: typing_extensions.Literal["shortName"]) -> MetaOapg.properties.shortName: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["lastName"]) -> MetaOapg.properties.lastName: ...
+    def __getitem__(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["privilege"]) -> 'UserPrivilege': ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
+    def __getitem__(self, name: typing_extensions.Literal["tenantId"]) -> MetaOapg.properties.tenantId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["isLdapSynchronized"]) -> MetaOapg.properties.isLdapSynchronized: ...
+    def __getitem__(self, name: typing_extensions.Literal["description"]) -> MetaOapg.properties.description: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["associatedTenants"]) -> MetaOapg.properties.associatedTenants: ...
+    def __getitem__(self, name: typing_extensions.Literal["folderCreationAllowed"]) -> MetaOapg.properties.folderCreationAllowed: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["associatedTenantIds"]) -> MetaOapg.properties.associatedTenantIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["actionAllowed"]) -> MetaOapg.properties.actionAllowed: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["administeredTenants"]) -> MetaOapg.properties.administeredTenants: ...
+    def __getitem__(self, name: typing_extensions.Literal["archivingAllowed"]) -> MetaOapg.properties.archivingAllowed: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["administeredTenantIds"]) -> MetaOapg.properties.administeredTenantIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["chainAllowed"]) -> MetaOapg.properties.chainAllowed: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["administeredDesks"]) -> MetaOapg.properties.administeredDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["parentDeskId"]) -> MetaOapg.properties.parentDeskId: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["administeredDeskIds"]) -> MetaOapg.properties.administeredDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["parentDesk"]) -> 'DeskRepresentation': ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["associatedDesks"]) -> MetaOapg.properties.associatedDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["owners"]) -> MetaOapg.properties.owners: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["associatedDeskIds"]) -> MetaOapg.properties.associatedDeskIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["supervisedDesks"]) -> MetaOapg.properties.supervisedDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["associatedDesks"]) -> MetaOapg.properties.associatedDesks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["supervisedDeskIds"]) -> MetaOapg.properties.supervisedDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["filterableMetadataIds"]) -> MetaOapg.properties.filterableMetadataIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["delegationManagedDesks"]) -> MetaOapg.properties.delegationManagedDesks: ...
+    def __getitem__(self, name: typing_extensions.Literal["filterableMetadata"]) -> MetaOapg.properties.filterableMetadata: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["delegationManagedDeskIds"]) -> MetaOapg.properties.delegationManagedDeskIds: ...
+    def __getitem__(self, name: typing_extensions.Literal["supervisorIds"]) -> MetaOapg.properties.supervisorIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["complementaryField"]) -> MetaOapg.properties.complementaryField: ...
+    def __getitem__(self, name: typing_extensions.Literal["supervisors"]) -> MetaOapg.properties.supervisors: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["resetPasswordRequired"]) -> MetaOapg.properties.resetPasswordRequired: ...
+    def __getitem__(self, name: typing_extensions.Literal["delegationManagerIds"]) -> MetaOapg.properties.delegationManagerIds: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["password"]) -> MetaOapg.properties.password: ...
+    def __getitem__(self, name: typing_extensions.Literal["delegationManagers"]) -> MetaOapg.properties.delegationManagers: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["userName", "firstName", "lastName", "email", "privilege", "id", "isLdapSynchronized", "associatedTenants", "associatedTenantIds", "administeredTenants", "administeredTenantIds", "administeredDesks", "administeredDeskIds", "associatedDesks", "associatedDeskIds", "supervisedDesks", "supervisedDeskIds", "delegationManagedDesks", "delegationManagedDeskIds", "complementaryField", "resetPasswordRequired", "password", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "ownerIds", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["userName"]) -> MetaOapg.properties.userName: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["firstName"]) -> MetaOapg.properties.firstName: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["shortName"]) -> MetaOapg.properties.shortName: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["lastName"]) -> MetaOapg.properties.lastName: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ownerIds"]) -> MetaOapg.properties.ownerIds: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["privilege"]) -> 'UserPrivilege': ...
+    def get_item_oapg(self, name: typing_extensions.Literal["tenantId"]) -> typing.Union[MetaOapg.properties.tenantId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> typing.Union[MetaOapg.properties.id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["description"]) -> typing.Union[MetaOapg.properties.description, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["isLdapSynchronized"]) -> typing.Union[MetaOapg.properties.isLdapSynchronized, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["folderCreationAllowed"]) -> typing.Union[MetaOapg.properties.folderCreationAllowed, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["associatedTenants"]) -> typing.Union[MetaOapg.properties.associatedTenants, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["actionAllowed"]) -> typing.Union[MetaOapg.properties.actionAllowed, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["associatedTenantIds"]) -> typing.Union[MetaOapg.properties.associatedTenantIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["archivingAllowed"]) -> typing.Union[MetaOapg.properties.archivingAllowed, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["administeredTenants"]) -> typing.Union[MetaOapg.properties.administeredTenants, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["chainAllowed"]) -> typing.Union[MetaOapg.properties.chainAllowed, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["administeredTenantIds"]) -> typing.Union[MetaOapg.properties.administeredTenantIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["parentDeskId"]) -> typing.Union[MetaOapg.properties.parentDeskId, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["administeredDesks"]) -> typing.Union[MetaOapg.properties.administeredDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["parentDesk"]) -> typing.Union['DeskRepresentation', schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["administeredDeskIds"]) -> typing.Union[MetaOapg.properties.administeredDeskIds, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["associatedDesks"]) -> typing.Union[MetaOapg.properties.associatedDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["owners"]) -> typing.Union[MetaOapg.properties.owners, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["associatedDeskIds"]) -> typing.Union[MetaOapg.properties.associatedDeskIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["supervisedDesks"]) -> typing.Union[MetaOapg.properties.supervisedDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["associatedDesks"]) -> typing.Union[MetaOapg.properties.associatedDesks, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["supervisedDeskIds"]) -> typing.Union[MetaOapg.properties.supervisedDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["filterableMetadataIds"]) -> typing.Union[MetaOapg.properties.filterableMetadataIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagedDesks"]) -> typing.Union[MetaOapg.properties.delegationManagedDesks, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["filterableMetadata"]) -> typing.Union[MetaOapg.properties.filterableMetadata, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagedDeskIds"]) -> typing.Union[MetaOapg.properties.delegationManagedDeskIds, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["supervisorIds"]) -> typing.Union[MetaOapg.properties.supervisorIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["complementaryField"]) -> typing.Union[MetaOapg.properties.complementaryField, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["supervisors"]) -> typing.Union[MetaOapg.properties.supervisors, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["resetPasswordRequired"]) -> typing.Union[MetaOapg.properties.resetPasswordRequired, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagerIds"]) -> typing.Union[MetaOapg.properties.delegationManagerIds, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["password"]) -> typing.Union[MetaOapg.properties.password, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["delegationManagers"]) -> typing.Union[MetaOapg.properties.delegationManagers, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["userName", "firstName", "lastName", "email", "privilege", "id", "isLdapSynchronized", "associatedTenants", "associatedTenantIds", "administeredTenants", "administeredTenantIds", "administeredDesks", "administeredDeskIds", "associatedDesks", "associatedDeskIds", "supervisedDesks", "supervisedDeskIds", "delegationManagedDesks", "delegationManagedDeskIds", "complementaryField", "resetPasswordRequired", "password", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "shortName", "ownerIds", "id", "tenantId", "description", "folderCreationAllowed", "actionAllowed", "archivingAllowed", "chainAllowed", "parentDeskId", "parentDesk", "owners", "associatedDeskIds", "associatedDesks", "filterableMetadataIds", "filterableMetadata", "supervisorIds", "supervisors", "delegationManagerIds", "delegationManagers", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        firstName: typing.Union[MetaOapg.properties.firstName, str, ],
-        lastName: typing.Union[MetaOapg.properties.lastName, str, ],
-        privilege: 'UserPrivilege',
-        userName: typing.Union[MetaOapg.properties.userName, str, ],
-        email: typing.Union[MetaOapg.properties.email, str, ],
+        ownerIds: typing.Union[MetaOapg.properties.ownerIds, list, tuple, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        shortName: typing.Union[MetaOapg.properties.shortName, str, ],
         id: typing.Union[MetaOapg.properties.id, str, schemas.Unset] = schemas.unset,
-        isLdapSynchronized: typing.Union[MetaOapg.properties.isLdapSynchronized, bool, schemas.Unset] = schemas.unset,
-        associatedTenants: typing.Union[MetaOapg.properties.associatedTenants, list, tuple, schemas.Unset] = schemas.unset,
-        associatedTenantIds: typing.Union[MetaOapg.properties.associatedTenantIds, list, tuple, schemas.Unset] = schemas.unset,
-        administeredTenants: typing.Union[MetaOapg.properties.administeredTenants, list, tuple, schemas.Unset] = schemas.unset,
-        administeredTenantIds: typing.Union[MetaOapg.properties.administeredTenantIds, list, tuple, schemas.Unset] = schemas.unset,
-        administeredDesks: typing.Union[MetaOapg.properties.administeredDesks, list, tuple, None, schemas.Unset] = schemas.unset,
-        administeredDeskIds: typing.Union[MetaOapg.properties.administeredDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
-        associatedDesks: typing.Union[MetaOapg.properties.associatedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
-        associatedDeskIds: typing.Union[MetaOapg.properties.associatedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
-        supervisedDesks: typing.Union[MetaOapg.properties.supervisedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
-        supervisedDeskIds: typing.Union[MetaOapg.properties.supervisedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
-        delegationManagedDesks: typing.Union[MetaOapg.properties.delegationManagedDesks, list, tuple, None, schemas.Unset] = schemas.unset,
-        delegationManagedDeskIds: typing.Union[MetaOapg.properties.delegationManagedDeskIds, list, tuple, None, schemas.Unset] = schemas.unset,
-        complementaryField: typing.Union[MetaOapg.properties.complementaryField, str, schemas.Unset] = schemas.unset,
-        resetPasswordRequired: typing.Union[MetaOapg.properties.resetPasswordRequired, bool, schemas.Unset] = schemas.unset,
-        password: typing.Union[MetaOapg.properties.password, str, schemas.Unset] = schemas.unset,
+        tenantId: typing.Union[MetaOapg.properties.tenantId, str, schemas.Unset] = schemas.unset,
+        description: typing.Union[MetaOapg.properties.description, str, schemas.Unset] = schemas.unset,
+        folderCreationAllowed: typing.Union[MetaOapg.properties.folderCreationAllowed, bool, schemas.Unset] = schemas.unset,
+        actionAllowed: typing.Union[MetaOapg.properties.actionAllowed, bool, schemas.Unset] = schemas.unset,
+        archivingAllowed: typing.Union[MetaOapg.properties.archivingAllowed, bool, schemas.Unset] = schemas.unset,
+        chainAllowed: typing.Union[MetaOapg.properties.chainAllowed, bool, schemas.Unset] = schemas.unset,
+        parentDeskId: typing.Union[MetaOapg.properties.parentDeskId, str, schemas.Unset] = schemas.unset,
+        parentDesk: typing.Union['DeskRepresentation', schemas.Unset] = schemas.unset,
+        owners: typing.Union[MetaOapg.properties.owners, list, tuple, schemas.Unset] = schemas.unset,
+        associatedDeskIds: typing.Union[MetaOapg.properties.associatedDeskIds, list, tuple, schemas.Unset] = schemas.unset,
+        associatedDesks: typing.Union[MetaOapg.properties.associatedDesks, list, tuple, schemas.Unset] = schemas.unset,
+        filterableMetadataIds: typing.Union[MetaOapg.properties.filterableMetadataIds, list, tuple, schemas.Unset] = schemas.unset,
+        filterableMetadata: typing.Union[MetaOapg.properties.filterableMetadata, list, tuple, schemas.Unset] = schemas.unset,
+        supervisorIds: typing.Union[MetaOapg.properties.supervisorIds, list, tuple, schemas.Unset] = schemas.unset,
+        supervisors: typing.Union[MetaOapg.properties.supervisors, list, tuple, schemas.Unset] = schemas.unset,
+        delegationManagerIds: typing.Union[MetaOapg.properties.delegationManagerIds, list, tuple, schemas.Unset] = schemas.unset,
+        delegationManagers: typing.Union[MetaOapg.properties.delegationManagers, list, tuple, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'UserDto':
+    ) -> 'DeskDto':
         return super().__new__(
             cls,
             *_args,
-            firstName=firstName,
-            lastName=lastName,
-            privilege=privilege,
-            userName=userName,
-            email=email,
+            ownerIds=ownerIds,
+            name=name,
+            shortName=shortName,
             id=id,
-            isLdapSynchronized=isLdapSynchronized,
-            associatedTenants=associatedTenants,
-            associatedTenantIds=associatedTenantIds,
-            administeredTenants=administeredTenants,
-            administeredTenantIds=administeredTenantIds,
-            administeredDesks=administeredDesks,
-            administeredDeskIds=administeredDeskIds,
-            associatedDesks=associatedDesks,
+            tenantId=tenantId,
+            description=description,
+            folderCreationAllowed=folderCreationAllowed,
+            actionAllowed=actionAllowed,
+            archivingAllowed=archivingAllowed,
+            chainAllowed=chainAllowed,
+            parentDeskId=parentDeskId,
+            parentDesk=parentDesk,
+            owners=owners,
             associatedDeskIds=associatedDeskIds,
-            supervisedDesks=supervisedDesks,
-            supervisedDeskIds=supervisedDeskIds,
-            delegationManagedDesks=delegationManagedDesks,
-            delegationManagedDeskIds=delegationManagedDeskIds,
-            complementaryField=complementaryField,
-            resetPasswordRequired=resetPasswordRequired,
-            password=password,
+            associatedDesks=associatedDesks,
+            filterableMetadataIds=filterableMetadataIds,
+            filterableMetadata=filterableMetadata,
+            supervisorIds=supervisorIds,
+            supervisors=supervisors,
+            delegationManagerIds=delegationManagerIds,
+            delegationManagers=delegationManagers,
             _configuration=_configuration,
             **kwargs,
         )
 
 from iparapheur_provisioning.model.desk_representation import DeskRepresentation
-from iparapheur_provisioning.model.tenant_representation import TenantRepresentation
-from iparapheur_provisioning.model.user_privilege import UserPrivilege
+from iparapheur_provisioning.model.metadata_representation import MetadataRepresentation
+from iparapheur_provisioning.model.user_representation import UserRepresentation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_privilege.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_representation.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/user_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/model/workflow_definition_sort_by.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/model/workflow_definition_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/models/__init__.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,13 @@
 from iparapheur_provisioning.model.subtype_metadata_dto import SubtypeMetadataDto
 from iparapheur_provisioning.model.subtype_representation import SubtypeRepresentation
 from iparapheur_provisioning.model.tenant_dto import TenantDto
 from iparapheur_provisioning.model.tenant_representation import TenantRepresentation
 from iparapheur_provisioning.model.tenant_sort_by import TenantSortBy
 from iparapheur_provisioning.model.type_dto import TypeDto
 from iparapheur_provisioning.model.type_representation import TypeRepresentation
-from iparapheur_provisioning.model.typology_representation import TypologyRepresentation
 from iparapheur_provisioning.model.typology_sort_by import TypologySortBy
 from iparapheur_provisioning.model.user_dto import UserDto
 from iparapheur_provisioning.model.user_privilege import UserPrivilege
 from iparapheur_provisioning.model.user_representation import UserRepresentation
 from iparapheur_provisioning.model.user_sort_by import UserSortBy
 from iparapheur_provisioning.model.workflow_definition_sort_by import WorkflowDefinitionSortBy
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/__init__.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,69 +40,69 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
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
 SchemaFor201ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -136,17 +136,17 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '201': _response_for_201,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/delete.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -54,31 +54,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
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
-    '403': _response_for_403,
+    '404': _response_for_404,
     '204': _response_for_204,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,31 +55,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -93,57 +93,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -123,58 +123,58 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TenantDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TenantDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,69 +143,69 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
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
 SchemaFor200ResponseBodyApplicationJson = PageDeskRepresentation
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -220,17 +220,17 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -104,50 +104,50 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = DeskDto
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
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
 SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor409(api_client.ApiResponse):
@@ -181,18 +181,18 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '201': _response_for_201,
-    '404': _response_for_404,
     '409': _response_for_409,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,31 +62,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
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
-    '403': _response_for_403,
+    '404': _response_for_404,
     '204': _response_for_204,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,31 +63,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=DeskIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -101,57 +101,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -112,50 +112,50 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = DeskDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = DeskDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor409(api_client.ApiResponse):
@@ -189,18 +189,18 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
     '409': _response_for_409,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,31 +135,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -173,57 +173,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageTypeRepresentation
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type/post.py`

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
 SchemaFor201ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -162,16 +162,16 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '201': _response_for_201,
     '409': _response_for_409,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,31 +62,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
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
-    '403': _response_for_403,
+    '404': _response_for_404,
     '204': _response_for_204,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -63,31 +63,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -101,57 +101,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -112,57 +112,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = TypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = TypeDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -143,31 +143,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -181,57 +181,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageSubtypeRepresentation
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -74,31 +74,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -112,50 +112,50 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor201ResponseBodyApplicationJson = SubtypeDto
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
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor201ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor201(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor201ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_201 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor201,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor201ResponseBodyApplicationJson),
     },
 )
 SchemaFor409ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor409(api_client.ApiResponse):
@@ -189,18 +189,18 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '201': _response_for_201,
-    '404': _response_for_404,
     '409': _response_for_409,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -70,31 +70,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
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
-    '403': _response_for_403,
+    '404': _response_for_404,
     '204': _response_for_204,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -71,31 +71,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=SubtypeIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -109,57 +109,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = SubtypeDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -82,31 +82,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
 SchemaFor204ResponseBodyApplicationJson = SubtypeDto
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
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
@@ -178,18 +178,18 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '204': _response_for_204,
     '401': _response_for_401,
-    '404': _response_for_404,
+    '403': _response_for_403,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -151,31 +151,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=TenantIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -208,58 +208,58 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user/post.py`

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
 SchemaFor201ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
 class ApiResponseFor201(api_client.ApiResponse):
@@ -162,16 +162,16 @@
     response_cls=ApiResponseFor507,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor507ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '401': _response_for_401,
+    '403': _response_for_403,
     '201': _response_for_201,
     '409': _response_for_409,
     '507': _response_for_507,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,44 +62,44 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor403(api_client.ApiResponse):
+class ApiResponseFor204(api_client.ApiResponse):
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
+_response_for_204 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor204,
 )
+SchemaFor406ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor204(api_client.ApiResponse):
+class ApiResponseFor406(api_client.ApiResponse):
     response: urllib3.HTTPResponse
-    body: schemas.Unset = schemas.unset
+    body: typing.Union[
+        SchemaFor406ResponseBodyApplicationJson,
+    ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_204 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor204,
+_response_for_406 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor406,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor406ResponseBodyApplicationJson),
+    },
 )
 SchemaFor401ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
 class ApiResponseFor401(api_client.ApiResponse):
     response: urllib3.HTTPResponse
@@ -112,38 +112,38 @@
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
 _status_code_to_response = {
-    '403': _response_for_403,
     '204': _response_for_204,
-    '401': _response_for_401,
     '406': _response_for_406,
+    '401': _response_for_401,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -63,31 +63,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -101,57 +101,57 @@
 _response_for_401 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor401,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor401ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_tenant_tenant_id_user_user_id/put.py`

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
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
-    '401': _response_for_401,
+    '404': _response_for_404,
     '406': _response_for_406,
+    '401': _response_for_401,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -117,69 +117,69 @@
     style=api_client.ParameterStyle.FORM,
     schema=SearchTermSchema,
     explode=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
+SchemaFor400ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor401(api_client.ApiResponse):
+class ApiResponseFor400(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor401ResponseBodyApplicationJson,
+        SchemaFor400ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_401 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor401,
+_response_for_400 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor401ResponseBodyApplicationJson),
+            schema=SchemaFor400ResponseBodyApplicationJson),
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
 SchemaFor200ResponseBodyApplicationJson = PageUserRepresentation
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
@@ -194,17 +194,17 @@
     response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '200': _response_for_200,
 }
 _all_accept_content_types = (
     'application/json',
 )
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/delete.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -54,33 +54,14 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
-SchemaFor403ResponseBodyApplicationJson = ErrorResponse
-
-
-@dataclass
-class ApiResponseFor403(api_client.ApiResponse):
-    response: urllib3.HTTPResponse
-    body: typing.Union[
-        SchemaFor403ResponseBodyApplicationJson,
-    ]
-    headers: schemas.Unset = schemas.unset
-
-
-_response_for_403 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor403,
-    content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor403ResponseBodyApplicationJson),
-    },
-)
 
 
 @dataclass
 class ApiResponseFor204(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: schemas.Unset = schemas.unset
     headers: schemas.Unset = schemas.unset
@@ -123,19 +104,38 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
+
+
+@dataclass
+class ApiResponseFor403(api_client.ApiResponse):
+    response: urllib3.HTTPResponse
+    body: typing.Union[
+        SchemaFor403ResponseBodyApplicationJson,
+    ]
+    headers: schemas.Unset = schemas.unset
+
+
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
+    content={
+        'application/json': api_client.MediaType(
+            schema=SchemaFor403ResponseBodyApplicationJson),
+    },
+)
 _status_code_to_response = {
-    '403': _response_for_403,
     '204': _response_for_204,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/get.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,31 +55,31 @@
     style=api_client.ParameterStyle.SIMPLE,
     schema=UserIdSchema,
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -112,58 +112,58 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/paths/api_provisioning_v1_admin_user_user_id/put.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,31 +66,31 @@
             schema=SchemaForRequestBodyApplicationJson),
     },
     required=True,
 )
 _auth = [
     'spring_oauth',
 ]
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
@@ -123,58 +123,58 @@
 _response_for_400 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor400,
     content={
         'application/json': api_client.MediaType(
             schema=SchemaFor400ResponseBodyApplicationJson),
     },
 )
-SchemaFor200ResponseBodyApplicationJson = UserDto
+SchemaFor403ResponseBodyApplicationJson = ErrorResponse
 
 
 @dataclass
-class ApiResponseFor200(api_client.ApiResponse):
+class ApiResponseFor403(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor200ResponseBodyApplicationJson,
+        SchemaFor403ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_200 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor200,
+_response_for_403 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor403,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+            schema=SchemaFor403ResponseBodyApplicationJson),
     },
 )
-SchemaFor404ResponseBodyApplicationJson = ErrorResponse
+SchemaFor200ResponseBodyApplicationJson = UserDto
 
 
 @dataclass
-class ApiResponseFor404(api_client.ApiResponse):
+class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
-        SchemaFor404ResponseBodyApplicationJson,
+        SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
-_response_for_404 = api_client.OpenApiResponse(
-    response_cls=ApiResponseFor404,
+_response_for_200 = api_client.OpenApiResponse(
+    response_cls=ApiResponseFor200,
     content={
         'application/json': api_client.MediaType(
-            schema=SchemaFor404ResponseBodyApplicationJson),
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 _status_code_to_response = {
-    '403': _response_for_403,
+    '404': _response_for_404,
     '401': _response_for_401,
     '400': _response_for_400,
+    '403': _response_for_403,
     '200': _response_for_200,
-    '404': _response_for_404,
 }
 _all_accept_content_types = (
     'application/json',
 )
 
 
 class BaseApi(api_client.Api):
```

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/rest.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/rest.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning/schemas.py` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning/schemas.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/iparapheur_provisioning.egg-info/SOURCES.txt` & `iparapheur-provisioning-1.6.6/iparapheur_provisioning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 iparapheur_provisioning/model/subtype_metadata_dto.py
 iparapheur_provisioning/model/subtype_representation.py
 iparapheur_provisioning/model/tenant_dto.py
 iparapheur_provisioning/model/tenant_representation.py
 iparapheur_provisioning/model/tenant_sort_by.py
 iparapheur_provisioning/model/type_dto.py
 iparapheur_provisioning/model/type_representation.py
-iparapheur_provisioning/model/typology_representation.py
 iparapheur_provisioning/model/typology_sort_by.py
 iparapheur_provisioning/model/user_dto.py
 iparapheur_provisioning/model/user_privilege.py
 iparapheur_provisioning/model/user_representation.py
 iparapheur_provisioning/model/user_sort_by.py
 iparapheur_provisioning/model/workflow_definition_sort_by.py
 iparapheur_provisioning/models/__init__.py
@@ -152,15 +151,14 @@
 test/test_models/test_subtype_metadata_dto.py
 test/test_models/test_subtype_representation.py
 test/test_models/test_tenant_dto.py
 test/test_models/test_tenant_representation.py
 test/test_models/test_tenant_sort_by.py
 test/test_models/test_type_dto.py
 test/test_models/test_type_representation.py
-test/test_models/test_typology_representation.py
 test/test_models/test_typology_sort_by.py
 test/test_models/test_user_dto.py
 test/test_models/test_user_privilege.py
 test/test_models/test_user_representation.py
 test/test_models/test_user_sort_by.py
 test/test_models/test_workflow_definition_sort_by.py
 test/test_paths/__init__.py
```

### Comparing `iparapheur-provisioning-1.6.5/setup.py` & `iparapheur-provisioning-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "iparapheur-provisioning"
-VERSION = "1.6.5"
+VERSION = "1.6.6"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_delegation_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_delegation_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_desk_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_desk_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_desk_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_error_response.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_error_response.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_external_signature_config_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_external_signature_config_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_config_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_external_signature_provider.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_external_signature_provider.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_folder_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_folder_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_internal_metadata.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_internal_metadata.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_layer_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_layer_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_layer_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_layer_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_metadata_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_metadata_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_metadata_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_metadata_type.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_metadata_type.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_page_desk_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_page_desk_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_page_subtype_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_page_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_page_type_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_page_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_page_user_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_page_user_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_pageable_object.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_pageable_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_pdf_signature_position.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_pdf_signature_position.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_seal_certificate_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_seal_certificate_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_signature_format.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_signature_format.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_signature_protocol.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_signature_protocol.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_sort_object.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_sort_object.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_subtype_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_subtype_layer_association.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_association.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_subtype_layer_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_layer_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_subtype_metadata_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_metadata_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_subtype_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_subtype_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_tenant_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_tenant_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_tenant_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_tenant_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_tenant_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_tenant_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_type_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_type_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_type_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_type_representation.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_typology_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_user_representation.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.typology_representation import TypologyRepresentation
+from iparapheur_provisioning.model.user_representation import UserRepresentation
 from iparapheur_provisioning import configuration
 
 
-class TestTypologyRepresentation(unittest.TestCase):
-    """TypologyRepresentation unit test stubs"""
+class TestUserRepresentation(unittest.TestCase):
+    """UserRepresentation unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_typology_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_typology_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_user_dto.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_user_dto.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_user_privilege.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_user_privilege.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_user_representation.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_workflow_definition_sort_by.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     Contact: iparapheur@libriciel.coop
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
 import iparapheur_provisioning
-from iparapheur_provisioning.model.user_representation import UserRepresentation
+from iparapheur_provisioning.model.workflow_definition_sort_by import WorkflowDefinitionSortBy
 from iparapheur_provisioning import configuration
 
 
-class TestUserRepresentation(unittest.TestCase):
-    """UserRepresentation unit test stubs"""
+class TestWorkflowDefinitionSortBy(unittest.TestCase):
+    """WorkflowDefinitionSortBy unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_models/test_user_sort_by.py` & `iparapheur-provisioning-1.6.6/test/test_models/test_user_sort_by.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/__init__.py` & `iparapheur-provisioning-1.6.6/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant/test_post.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_delete.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py`

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
 
-    response_status = 403
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_put.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py`

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
 
-    response_status = 403
-
-
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py`

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
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py`

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
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_desk_desk_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyType(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyType unit test stubs
-        List types  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
+        Edit a type  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type/test_post.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_get.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id/test_put.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id import put  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdTypologyTypeTypeId unit test stubs
-        Edit a type  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
+        Create a new user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
+        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 401
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_get.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype/test_post.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_delete.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_typology_type_type_id_subtype_subtype_id/test_put.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_get.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user/test_post.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id/test_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user import post  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUser(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminTenantTenantId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUser unit test stubs
-        Create a new user  # noqa: E501
+    ApiProvisioningV1AdminTenantTenantId unit test stubs
+        Get a full tenant description  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = post.ApiForpost(api_client=used_api_client)  # noqa: E501
+        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
-
-
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,13 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
-
-
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_tenant_tenant_id_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
-class TestApiProvisioningV1AdminTenantTenantIdUserUserId(ApiTestMixin, unittest.TestCase):
+class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
-    ApiProvisioningV1AdminTenantTenantIdUserUserId unit test stubs
-        Get a full user description  # noqa: E501
+    ApiProvisioningV1AdminUserUserId unit test stubs
+        Get a full user representation  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_tenant_tenant_id_user_user_id/test_put.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
 
 
 
 
 
 
 if __name__ == '__main__':
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user/test_get.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,14 @@
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
         self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 401
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_put.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,34 +8,36 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import put  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminUserUserId unit test stubs
-        Delete a user  # noqa: E501
+        Edit a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
+        self.api = put.ApiForput(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
+    response_status = 404
+
+
 
 
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `iparapheur-provisioning-1.6.5/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_get.py` & `iparapheur-provisioning-1.6.6/test/test_paths/test_api_provisioning_v1_admin_user_user_id/test_delete.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
 import iparapheur_provisioning
-from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import get  # noqa: E501
+from iparapheur_provisioning.paths.api_provisioning_v1_admin_user_user_id import delete  # noqa: E501
 from iparapheur_provisioning import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestApiProvisioningV1AdminUserUserId(ApiTestMixin, unittest.TestCase):
     """
     ApiProvisioningV1AdminUserUserId unit test stubs
-        Get a full user representation  # noqa: E501
+        Delete a user  # noqa: E501
     """
     _configuration = configuration.Configuration()
 
     def setUp(self):
         used_api_client = api_client.ApiClient(configuration=self._configuration)
-        self.api = get.ApiForget(api_client=used_api_client)  # noqa: E501
+        self.api = delete.ApiFordelete(api_client=used_api_client)  # noqa: E501
 
     def tearDown(self):
         pass
 
-    response_status = 403
-
-
+    response_status = 204
+    response_body = ''
 
 
 if __name__ == '__main__':
     unittest.main()
```

