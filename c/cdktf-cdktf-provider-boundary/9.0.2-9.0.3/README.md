# Comparing `tmp/cdktf-cdktf-provider-boundary-9.0.2.tar.gz` & `tmp/cdktf-cdktf-provider-boundary-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-boundary-9.0.2.tar", last modified: Thu Feb 15 03:12:25 2024, max compression
+gzip compressed data, was "cdktf-cdktf-provider-boundary-9.0.3.tar", last modified: Thu May  2 03:13:09 2024, max compression
```

## Comparing `cdktf-cdktf-provider-boundary-9.0.2.tar` & `cdktf-cdktf-provider-boundary-9.0.3.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.164726 cdktf-cdktf-provider-boundary-9.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   258361 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@9.0.2.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account/
--rw-r--r--   0 runner    (1001) docker     (127)    29104 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_ldap/
--rw-r--r--   0 runner    (1001) docker     (127)    27017 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    26938 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_password/
--rw-r--r--   0 runner    (1001) docker     (127)    29838 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method/
--rw-r--r--   0 runner    (1001) docker     (127)    29599 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_ldap/
--rw-r--r--   0 runner    (1001) docker     (127)   102184 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_oidc/
--rw-r--r--   0 runner    (1001) docker     (127)    73441 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_password/
--rw-r--r--   0 runner    (1001) docker     (127)    30405 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_json/
--rw-r--r--   0 runner    (1001) docker     (127)    25361 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_library_vault/
--rw-r--r--   0 runner    (1001) docker     (127)    37587 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)    48754 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/
--rw-r--r--   0 runner    (1001) docker     (127)    31233 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_store_static/
--rw-r--r--   0 runner    (1001) docker     (127)    22654 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_store_vault/
--rw-r--r--   0 runner    (1001) docker     (127)    47646 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_username_password/
--rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_account/
--rw-r--r--   0 runner    (1001) docker     (127)    29726 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_auth_method/
--rw-r--r--   0 runner    (1001) docker     (127)    30062 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_auth_method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_group/
--rw-r--r--   0 runner    (1001) docker     (127)    29774 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_scope/
--rw-r--r--   0 runner    (1001) docker     (127)    19673 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_scope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_user/
--rw-r--r--   0 runner    (1001) docker     (127)    30301 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/group/
--rw-r--r--   0 runner    (1001) docker     (127)    24778 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host/
--rw-r--r--   0 runner    (1001) docker     (127)    26547 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    24276 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    47632 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.176725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog_static/
--rw-r--r--   0 runner    (1001) docker     (127)    22458 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set/
--rw-r--r--   0 runner    (1001) docker     (127)    26725 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    33841 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set_static/
--rw-r--r--   0 runner    (1001) docker     (127)    27304 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_static/
--rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/managed_group/
--rw-r--r--   0 runner    (1001) docker     (127)    24592 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/managed_group_ldap/
--rw-r--r--   0 runner    (1001) docker     (127)    25085 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/managed_group_ldap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/policy_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    36312 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/policy_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/provider/
--rw-r--r--   0 runner    (1001) docker     (127)    41210 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/role/
--rw-r--r--   0 runner    (1001) docker     (127)    33454 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/role/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/scope/
--rw-r--r--   0 runner    (1001) docker     (127)    34164 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/scope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/scope_policy_attachment/
--rw-r--r--   0 runner    (1001) docker     (127)    22547 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/scope_policy_attachment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/storage_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    43285 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/storage_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/target/
--rw-r--r--   0 runner    (1001) docker     (127)    62527 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/target/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/user/
--rw-r--r--   0 runner    (1001) docker     (127)    24702 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.180725 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/worker/
--rw-r--r--   0 runner    (1001) docker     (127)    26438 2024-02-15 03:12:10.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 03:12:25.172726 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-15 03:12:25.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-15 03:12:25.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 03:12:25.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-15 03:12:25.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-15 03:12:25.000000 cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16012 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.134004 cdktf-cdktf-provider-boundary-9.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/
+-rw-r--r--   0 runner    (1001) docker     (127)     6177 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   262867 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@9.0.3.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account/
+-rw-r--r--   0 runner    (1001) docker     (127)    29180 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)    27093 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    27014 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_password/
+-rw-r--r--   0 runner    (1001) docker     (127)    29914 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/alias_target/
+-rw-r--r--   0 runner    (1001) docker     (127)    32132 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/alias_target/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method/
+-rw-r--r--   0 runner    (1001) docker     (127)    29675 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)   102260 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)    73517 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_password/
+-rw-r--r--   0 runner    (1001) docker     (127)    30481 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_json/
+-rw-r--r--   0 runner    (1001) docker     (127)    25437 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_library_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)    37663 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)    48830 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/
+-rw-r--r--   0 runner    (1001) docker     (127)    31309 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_store_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_store_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)    47722 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_username_password/
+-rw-r--r--   0 runner    (1001) docker     (127)    28246 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_account/
+-rw-r--r--   0 runner    (1001) docker     (127)    29802 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_auth_method/
+-rw-r--r--   0 runner    (1001) docker     (127)    30138 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_auth_method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_group/
+-rw-r--r--   0 runner    (1001) docker     (127)    29850 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_scope/
+-rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_scope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_user/
+-rw-r--r--   0 runner    (1001) docker     (127)    30377 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/group/
+-rw-r--r--   0 runner    (1001) docker     (127)    24854 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host/
+-rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    24352 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    47708 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    22534 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set/
+-rw-r--r--   0 runner    (1001) docker     (127)    26801 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    33917 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.142004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    27380 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    27202 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/managed_group/
+-rw-r--r--   0 runner    (1001) docker     (127)    24668 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/managed_group_ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)    25161 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/managed_group_ldap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/policy_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    36388 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/policy_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)    41286 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/role/
+-rw-r--r--   0 runner    (1001) docker     (127)    33530 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/role/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/scope/
+-rw-r--r--   0 runner    (1001) docker     (127)    34240 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/scope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/scope_policy_attachment/
+-rw-r--r--   0 runner    (1001) docker     (127)    22623 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/scope_policy_attachment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/storage_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    43361 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/storage_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/target/
+-rw-r--r--   0 runner    (1001) docker     (127)    62603 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/target/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    24778 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.146004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)    26514 2024-05-02 03:12:58.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 03:13:09.138004 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-02 03:13:09.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-02 03:13:09.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 03:13:09.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 03:13:09.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 03:13:09.000000 cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/LICENSE` & `cdktf-cdktf-provider-boundary-9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/PKG-INFO` & `cdktf-cdktf-provider-boundary-9.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-boundary
-Version: 9.0.2
+Version: 9.0.3
 Summary: Prebuilt boundary Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-boundary.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-boundary.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.14
+# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.15
 
-This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-boundary](https://www.npmjs.com/package/@cdktf/provider-boundary).
 
@@ -81,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform boundary provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14)
+* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/README.md` & `cdktf-cdktf-provider-boundary-9.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.14
+# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.15
 
-This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-boundary](https://www.npmjs.com/package/@cdktf/provider-boundary).
 
@@ -58,15 +58,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform boundary provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14)
+* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/setup.py` & `cdktf-cdktf-provider-boundary-9.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-boundary",
-    "version": "9.0.2",
+    "version": "9.0.3",
     "description": "Prebuilt boundary Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-boundary.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -23,14 +23,15 @@
     "packages": [
         "cdktf_cdktf_provider_boundary",
         "cdktf_cdktf_provider_boundary._jsii",
         "cdktf_cdktf_provider_boundary.account",
         "cdktf_cdktf_provider_boundary.account_ldap",
         "cdktf_cdktf_provider_boundary.account_oidc",
         "cdktf_cdktf_provider_boundary.account_password",
+        "cdktf_cdktf_provider_boundary.alias_target",
         "cdktf_cdktf_provider_boundary.auth_method",
         "cdktf_cdktf_provider_boundary.auth_method_ldap",
         "cdktf_cdktf_provider_boundary.auth_method_oidc",
         "cdktf_cdktf_provider_boundary.auth_method_password",
         "cdktf_cdktf_provider_boundary.credential_json",
         "cdktf_cdktf_provider_boundary.credential_library_vault",
         "cdktf_cdktf_provider_boundary.credential_library_vault_ssh_certificate",
@@ -62,25 +63,25 @@
         "cdktf_cdktf_provider_boundary.storage_bucket",
         "cdktf_cdktf_provider_boundary.target",
         "cdktf_cdktf_provider_boundary.user",
         "cdktf_cdktf_provider_boundary.worker"
     ],
     "package_data": {
         "cdktf_cdktf_provider_boundary._jsii": [
-            "provider-boundary@9.0.2.jsii.tgz"
+            "provider-boundary@9.0.3.jsii.tgz"
         ],
         "cdktf_cdktf_provider_boundary": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "cdktf>=0.20.0, <0.21.0",
         "constructs>=10.3.0, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.97.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.14
+# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.15
 
-This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-boundary](https://www.npmjs.com/package/@cdktf/provider-boundary).
 
@@ -59,15 +59,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform boundary provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14)
+* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
@@ -89,14 +89,17 @@
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [CDKTF Repository Manager](https://github.com/cdktf/cdktf-repository-manager/).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -108,14 +111,15 @@
 from ._jsii import *
 
 __all__ = [
     "account",
     "account_ldap",
     "account_oidc",
     "account_password",
+    "alias_target",
     "auth_method",
     "auth_method_ldap",
     "auth_method_oidc",
     "auth_method_password",
     "credential_json",
     "credential_library_vault",
     "credential_library_vault_ssh_certificate",
@@ -153,14 +157,15 @@
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
 from . import account
 from . import account_ldap
 from . import account_oidc
 from . import account_password
+from . import alias_target
 from . import auth_method
 from . import auth_method_ldap
 from . import auth_method_oidc
 from . import auth_method_password
 from . import credential_json
 from . import credential_library_vault
 from . import credential_library_vault_ssh_certificate
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_account`
 
-Refer to the Terraform Registry for docs: [`boundary_account`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account).
+Refer to the Terraform Registry for docs: [`boundary_account`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Account(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.account.Account",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account boundary_account}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account boundary_account}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account boundary_account} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account boundary_account} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#auth_method_id Account#auth_method_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#type Account#type}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#description Account#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#login_name Account#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#name Account#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#password Account#password}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#auth_method_id Account#auth_method_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#type Account#type}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#description Account#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#login_name Account#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#name Account#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#password Account#password}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Account resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Account to import.
-        :param import_from_id: The id of the existing Account that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Account that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Account to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bae95451d77aa27e983cdbcf6bb9a9715e3db81a12b31bb4847eb9a0477972a8)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -289,20 +292,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#auth_method_id Account#auth_method_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#type Account#type}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#description Account#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#login_name Account#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#name Account#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#password Account#password}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#auth_method_id Account#auth_method_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#type Account#type}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#description Account#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#login_name Account#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#name Account#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#password Account#password}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9f3a78290e59f53f12897f7e509e444fe46777e5e9e4d9f11c486df5264a6d41)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -408,62 +411,62 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#auth_method_id Account#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#auth_method_id Account#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#type Account#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#type Account#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#description Account#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#description Account#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def login_name(self) -> typing.Optional[builtins.str]:
         '''The login name for this account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#login_name Account#login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#login_name Account#login_name}
         '''
         result = self._values.get("login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#name Account#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#name Account#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''The account password. Only set on create, changes will not be reflected when updating account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account#password Account#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account#password Account#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_account_ldap`
 
-Refer to the Terraform Registry for docs: [`boundary_account_ldap`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap).
+Refer to the Terraform Registry for docs: [`boundary_account_ldap`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AccountLdap(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.accountLdap.AccountLdap",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap boundary_account_ldap}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap boundary_account_ldap}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap boundary_account_ldap} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap boundary_account_ldap} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#auth_method_id AccountLdap#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#description AccountLdap#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#login_name AccountLdap#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#name AccountLdap#name}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#type AccountLdap#type}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#auth_method_id AccountLdap#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#description AccountLdap#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#login_name AccountLdap#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#name AccountLdap#name}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#type AccountLdap#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AccountLdap resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AccountLdap to import.
-        :param import_from_id: The id of the existing AccountLdap that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AccountLdap that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AccountLdap to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__644807deba63a391b5d27b024f808d27853883a0b01378c3aba6118f6aff0e7e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -267,19 +270,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#auth_method_id AccountLdap#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#description AccountLdap#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#login_name AccountLdap#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#name AccountLdap#name}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#type AccountLdap#type}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#auth_method_id AccountLdap#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#description AccountLdap#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#login_name AccountLdap#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#name AccountLdap#name}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#type AccountLdap#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7ad48467a86b3d536b27b672737de8b6bba7df4fd8a4faf4fe53bd5d2140c189)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -383,52 +386,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#auth_method_id AccountLdap#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#auth_method_id AccountLdap#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#description AccountLdap#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#description AccountLdap#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def login_name(self) -> typing.Optional[builtins.str]:
         '''The login name for this account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#login_name AccountLdap#login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#login_name AccountLdap#login_name}
         '''
         result = self._values.get("login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#name AccountLdap#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#name AccountLdap#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_ldap#type AccountLdap#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_ldap#type AccountLdap#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_account_oidc`
 
-Refer to the Terraform Registry for docs: [`boundary_account_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc).
+Refer to the Terraform Registry for docs: [`boundary_account_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AccountOidc(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.accountOidc.AccountOidc",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc boundary_account_oidc}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc boundary_account_oidc}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc boundary_account_oidc} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc boundary_account_oidc} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#description AccountOidc#description}
-        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#issuer AccountOidc#issuer}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#name AccountOidc#name}
-        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#subject AccountOidc#subject}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#description AccountOidc#description}
+        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#issuer AccountOidc#issuer}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#name AccountOidc#name}
+        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#subject AccountOidc#subject}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AccountOidc resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AccountOidc to import.
-        :param import_from_id: The id of the existing AccountOidc that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AccountOidc that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AccountOidc to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0dac2fd5eb0855dbdb90d1ba38e21f68a185590aa29265faf4470d5799a25db8)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -267,19 +270,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#description AccountOidc#description}
-        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#issuer AccountOidc#issuer}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#name AccountOidc#name}
-        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#subject AccountOidc#subject}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#description AccountOidc#description}
+        :param issuer: The OIDC issuer. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#issuer AccountOidc#issuer}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#name AccountOidc#name}
+        :param subject: The OIDC subject. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#subject AccountOidc#subject}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5a9f2ecb8fb73ab43552aa884097a49be5578a649f7b9437164ada5cd9d24ded)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -383,52 +386,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#auth_method_id AccountOidc#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#description AccountOidc#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#description AccountOidc#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def issuer(self) -> typing.Optional[builtins.str]:
         '''The OIDC issuer.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#issuer AccountOidc#issuer}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#issuer AccountOidc#issuer}
         '''
         result = self._values.get("issuer")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#name AccountOidc#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#name AccountOidc#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def subject(self) -> typing.Optional[builtins.str]:
         '''The OIDC subject.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_oidc#subject AccountOidc#subject}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_oidc#subject AccountOidc#subject}
         '''
         result = self._values.get("subject")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/account_password/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/account_password/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_account_password`
 
-Refer to the Terraform Registry for docs: [`boundary_account_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password).
+Refer to the Terraform Registry for docs: [`boundary_account_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AccountPassword(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.accountPassword.AccountPassword",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password boundary_account_password}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password boundary_account_password}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password boundary_account_password} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password boundary_account_password} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#description AccountPassword#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#login_name AccountPassword#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#name AccountPassword#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#password AccountPassword#password}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#type AccountPassword#type}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#description AccountPassword#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#login_name AccountPassword#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#name AccountPassword#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#password AccountPassword#password}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#type AccountPassword#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AccountPassword resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AccountPassword to import.
-        :param import_from_id: The id of the existing AccountPassword that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AccountPassword that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AccountPassword to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f85d3975f0ab303dfdd6568cb15fe99acf04b13ef3f2530128054f432be2f118)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -293,20 +296,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
-        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#description AccountPassword#description}
-        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#login_name AccountPassword#login_name}
-        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#name AccountPassword#name}
-        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#password AccountPassword#password}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#type AccountPassword#type}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
+        :param description: The account description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#description AccountPassword#description}
+        :param login_name: The login name for this account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#login_name AccountPassword#login_name}
+        :param name: The account name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#name AccountPassword#name}
+        :param password: The account password. Only set on create, changes will not be reflected when updating account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#password AccountPassword#password}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#type AccountPassword#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9b0bbd75ce8fded2755ce13d83166390b51916ecaf627f133149858f88c5f382)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -413,61 +416,61 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#auth_method_id AccountPassword#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The account description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#description AccountPassword#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#description AccountPassword#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def login_name(self) -> typing.Optional[builtins.str]:
         '''The login name for this account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#login_name AccountPassword#login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#login_name AccountPassword#login_name}
         '''
         result = self._values.get("login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The account name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#name AccountPassword#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#name AccountPassword#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password(self) -> typing.Optional[builtins.str]:
         '''The account password. Only set on create, changes will not be reflected when updating account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#password AccountPassword#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#password AccountPassword#password}
         '''
         result = self._values.get("password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/account_password#type AccountPassword#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/account_password#type AccountPassword#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_auth_method`
 
-Refer to the Terraform Registry for docs: [`boundary_auth_method`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method).
+Refer to the Terraform Registry for docs: [`boundary_auth_method`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AuthMethod(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethod.AuthMethod",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method boundary_auth_method}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method boundary_auth_method}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method boundary_auth_method} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method boundary_auth_method} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#scope_id AuthMethod#scope_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#type AuthMethod#type}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#description AuthMethod#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#name AuthMethod#name}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#scope_id AuthMethod#scope_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#type AuthMethod#type}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#description AuthMethod#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#name AuthMethod#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AuthMethod resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AuthMethod to import.
-        :param import_from_id: The id of the existing AuthMethod that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AuthMethod that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AuthMethod to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__af154914ff5ec5ec77cda9d39d6c0b72ea3361c534f5c66d363a9240b30c578b)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -289,20 +292,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#scope_id AuthMethod#scope_id}
-        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#type AuthMethod#type}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#description AuthMethod#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#name AuthMethod#name}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#scope_id AuthMethod#scope_id}
+        :param type: The resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#type AuthMethod#type}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#description AuthMethod#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#name AuthMethod#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1dbc89045cef41c40c62b2ae4f0b26d37995a7c431554876680e5a3612faa380)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -408,62 +411,62 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#scope_id AuthMethod#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#scope_id AuthMethod#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#type AuthMethod#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#type AuthMethod#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#description AuthMethod#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#description AuthMethod#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def min_login_name_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum login name length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#min_login_name_length AuthMethod#min_login_name_length}
         '''
         result = self._values.get("min_login_name_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def min_password_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum password length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#min_password_length AuthMethod#min_password_length}
         '''
         result = self._values.get("min_password_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method#name AuthMethod#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method#name AuthMethod#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_auth_method_ldap`
 
-Refer to the Terraform Registry for docs: [`boundary_auth_method_ldap`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap).
+Refer to the Terraform Registry for docs: [`boundary_auth_method_ldap`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AuthMethodLdap(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethodLdap.AuthMethodLdap",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap boundary_auth_method_ldap}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap boundary_auth_method_ldap}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -67,48 +70,48 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap boundary_auth_method_ldap} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap boundary_auth_method_ldap} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#scope_id AuthMethodLdap#scope_id}
-        :param account_attribute_maps: Account attribute maps fullname and email. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#account_attribute_maps AuthMethodLdap#account_attribute_maps}
-        :param anon_group_search: Use anon bind when performing LDAP group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#anon_group_search AuthMethodLdap#anon_group_search}
-        :param bind_dn: The distinguished name of entry to bind when performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_dn AuthMethodLdap#bind_dn}
-        :param bind_password: The password to use along with bind-dn performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_password AuthMethodLdap#bind_password}
-        :param bind_password_hmac: The HMAC of the bind password returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_password_hmac AuthMethodLdap#bind_password_hmac}
-        :param certificates: PEM-encoded X.509 CA certificate in ASN.1 DER form that can be used as a trust anchor when connecting to an LDAP server(optional). This may be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#certificates AuthMethodLdap#certificates}
-        :param client_certificate: PEM-encoded X.509 client certificate in ASN.1 DER form that can be used to authenticate against an LDAP server(optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate AuthMethodLdap#client_certificate}
-        :param client_certificate_key: PEM-encoded X.509 client certificate key in PKCS #8, ASN.1 DER form used with the client certificate (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate_key AuthMethodLdap#client_certificate_key}
-        :param client_certificate_key_hmac: The HMAC of the client certificate key returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate_key_hmac AuthMethodLdap#client_certificate_key_hmac}
-        :param dereference_aliases: Control how aliases are dereferenced when performing the search. Can be one of: NeverDerefAliases, DerefInSearching, DerefFindingBaseObj, and DerefAlways (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#dereference_aliases AuthMethodLdap#dereference_aliases}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#description AuthMethodLdap#description}
-        :param discover_dn: Use anon bind to discover the bind DN of a user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#discover_dn AuthMethodLdap#discover_dn}
-        :param enable_groups: Find the authenticated user's groups during authentication (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#enable_groups AuthMethodLdap#enable_groups}
-        :param group_attr: The attribute that enumerates a user's group membership from entries returned by a group search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_attr AuthMethodLdap#group_attr}
-        :param group_dn: The base DN under which to perform group search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_dn AuthMethodLdap#group_dn}
-        :param group_filter: A go template used to construct a LDAP group search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_filter AuthMethodLdap#group_filter}
-        :param insecure_tls: Skip the LDAP server SSL certificate validation (optional) - insecure and use with caution. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#insecure_tls AuthMethodLdap#insecure_tls}
-        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the the user will be automatically created when they login using an LDAP account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#is_primary_for_scope AuthMethodLdap#is_primary_for_scope}
-        :param maximum_page_size: MaximumPageSize specifies a maximum search result size to use when retrieving the authenticated user's groups (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#maximum_page_size AuthMethodLdap#maximum_page_size}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#name AuthMethodLdap#name}
-        :param start_tls: Issue StartTLS command after connecting (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#start_tls AuthMethodLdap#start_tls}
-        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Defaults to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#state AuthMethodLdap#state}
-        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#type AuthMethodLdap#type}
-        :param upn_domain: The userPrincipalDomain used to construct the UPN string for the authenticating user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#upn_domain AuthMethodLdap#upn_domain}
-        :param urls: The LDAP URLs that specify LDAP servers to connect to (required). May be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#urls AuthMethodLdap#urls}
-        :param user_attr: The attribute on user entry matching the username passed when authenticating (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_attr AuthMethodLdap#user_attr}
-        :param user_dn: The base DN under which to perform user search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_dn AuthMethodLdap#user_dn}
-        :param user_filter: A go template used to construct a LDAP user search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_filter AuthMethodLdap#user_filter}
-        :param use_token_groups: Use the Active Directory tokenGroups constructed attribute of the user to find the group memberships (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#use_token_groups AuthMethodLdap#use_token_groups}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#scope_id AuthMethodLdap#scope_id}
+        :param account_attribute_maps: Account attribute maps fullname and email. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#account_attribute_maps AuthMethodLdap#account_attribute_maps}
+        :param anon_group_search: Use anon bind when performing LDAP group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#anon_group_search AuthMethodLdap#anon_group_search}
+        :param bind_dn: The distinguished name of entry to bind when performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_dn AuthMethodLdap#bind_dn}
+        :param bind_password: The password to use along with bind-dn performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_password AuthMethodLdap#bind_password}
+        :param bind_password_hmac: The HMAC of the bind password returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_password_hmac AuthMethodLdap#bind_password_hmac}
+        :param certificates: PEM-encoded X.509 CA certificate in ASN.1 DER form that can be used as a trust anchor when connecting to an LDAP server(optional). This may be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#certificates AuthMethodLdap#certificates}
+        :param client_certificate: PEM-encoded X.509 client certificate in ASN.1 DER form that can be used to authenticate against an LDAP server(optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate AuthMethodLdap#client_certificate}
+        :param client_certificate_key: PEM-encoded X.509 client certificate key in PKCS #8, ASN.1 DER form used with the client certificate (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate_key AuthMethodLdap#client_certificate_key}
+        :param client_certificate_key_hmac: The HMAC of the client certificate key returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate_key_hmac AuthMethodLdap#client_certificate_key_hmac}
+        :param dereference_aliases: Control how aliases are dereferenced when performing the search. Can be one of: NeverDerefAliases, DerefInSearching, DerefFindingBaseObj, and DerefAlways (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#dereference_aliases AuthMethodLdap#dereference_aliases}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#description AuthMethodLdap#description}
+        :param discover_dn: Use anon bind to discover the bind DN of a user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#discover_dn AuthMethodLdap#discover_dn}
+        :param enable_groups: Find the authenticated user's groups during authentication (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#enable_groups AuthMethodLdap#enable_groups}
+        :param group_attr: The attribute that enumerates a user's group membership from entries returned by a group search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_attr AuthMethodLdap#group_attr}
+        :param group_dn: The base DN under which to perform group search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_dn AuthMethodLdap#group_dn}
+        :param group_filter: A go template used to construct a LDAP group search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_filter AuthMethodLdap#group_filter}
+        :param insecure_tls: Skip the LDAP server SSL certificate validation (optional) - insecure and use with caution. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#insecure_tls AuthMethodLdap#insecure_tls}
+        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the the user will be automatically created when they login using an LDAP account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#is_primary_for_scope AuthMethodLdap#is_primary_for_scope}
+        :param maximum_page_size: MaximumPageSize specifies a maximum search result size to use when retrieving the authenticated user's groups (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#maximum_page_size AuthMethodLdap#maximum_page_size}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#name AuthMethodLdap#name}
+        :param start_tls: Issue StartTLS command after connecting (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#start_tls AuthMethodLdap#start_tls}
+        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Defaults to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#state AuthMethodLdap#state}
+        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#type AuthMethodLdap#type}
+        :param upn_domain: The userPrincipalDomain used to construct the UPN string for the authenticating user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#upn_domain AuthMethodLdap#upn_domain}
+        :param urls: The LDAP URLs that specify LDAP servers to connect to (required). May be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#urls AuthMethodLdap#urls}
+        :param user_attr: The attribute on user entry matching the username passed when authenticating (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_attr AuthMethodLdap#user_attr}
+        :param user_dn: The base DN under which to perform user search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_dn AuthMethodLdap#user_dn}
+        :param user_filter: A go template used to construct a LDAP user search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_filter AuthMethodLdap#user_filter}
+        :param use_token_groups: Use the Active Directory tokenGroups constructed attribute of the user to find the group memberships (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#use_token_groups AuthMethodLdap#use_token_groups}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -168,15 +171,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AuthMethodLdap resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AuthMethodLdap to import.
-        :param import_from_id: The id of the existing AuthMethodLdap that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AuthMethodLdap that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AuthMethodLdap to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__db66f29195e83a62225dbcf5f20f7b5cd76cd2a0b42855af0532de7169c81b10)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -960,44 +963,44 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#scope_id AuthMethodLdap#scope_id}
-        :param account_attribute_maps: Account attribute maps fullname and email. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#account_attribute_maps AuthMethodLdap#account_attribute_maps}
-        :param anon_group_search: Use anon bind when performing LDAP group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#anon_group_search AuthMethodLdap#anon_group_search}
-        :param bind_dn: The distinguished name of entry to bind when performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_dn AuthMethodLdap#bind_dn}
-        :param bind_password: The password to use along with bind-dn performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_password AuthMethodLdap#bind_password}
-        :param bind_password_hmac: The HMAC of the bind password returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_password_hmac AuthMethodLdap#bind_password_hmac}
-        :param certificates: PEM-encoded X.509 CA certificate in ASN.1 DER form that can be used as a trust anchor when connecting to an LDAP server(optional). This may be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#certificates AuthMethodLdap#certificates}
-        :param client_certificate: PEM-encoded X.509 client certificate in ASN.1 DER form that can be used to authenticate against an LDAP server(optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate AuthMethodLdap#client_certificate}
-        :param client_certificate_key: PEM-encoded X.509 client certificate key in PKCS #8, ASN.1 DER form used with the client certificate (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate_key AuthMethodLdap#client_certificate_key}
-        :param client_certificate_key_hmac: The HMAC of the client certificate key returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate_key_hmac AuthMethodLdap#client_certificate_key_hmac}
-        :param dereference_aliases: Control how aliases are dereferenced when performing the search. Can be one of: NeverDerefAliases, DerefInSearching, DerefFindingBaseObj, and DerefAlways (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#dereference_aliases AuthMethodLdap#dereference_aliases}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#description AuthMethodLdap#description}
-        :param discover_dn: Use anon bind to discover the bind DN of a user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#discover_dn AuthMethodLdap#discover_dn}
-        :param enable_groups: Find the authenticated user's groups during authentication (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#enable_groups AuthMethodLdap#enable_groups}
-        :param group_attr: The attribute that enumerates a user's group membership from entries returned by a group search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_attr AuthMethodLdap#group_attr}
-        :param group_dn: The base DN under which to perform group search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_dn AuthMethodLdap#group_dn}
-        :param group_filter: A go template used to construct a LDAP group search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_filter AuthMethodLdap#group_filter}
-        :param insecure_tls: Skip the LDAP server SSL certificate validation (optional) - insecure and use with caution. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#insecure_tls AuthMethodLdap#insecure_tls}
-        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the the user will be automatically created when they login using an LDAP account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#is_primary_for_scope AuthMethodLdap#is_primary_for_scope}
-        :param maximum_page_size: MaximumPageSize specifies a maximum search result size to use when retrieving the authenticated user's groups (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#maximum_page_size AuthMethodLdap#maximum_page_size}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#name AuthMethodLdap#name}
-        :param start_tls: Issue StartTLS command after connecting (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#start_tls AuthMethodLdap#start_tls}
-        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Defaults to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#state AuthMethodLdap#state}
-        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#type AuthMethodLdap#type}
-        :param upn_domain: The userPrincipalDomain used to construct the UPN string for the authenticating user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#upn_domain AuthMethodLdap#upn_domain}
-        :param urls: The LDAP URLs that specify LDAP servers to connect to (required). May be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#urls AuthMethodLdap#urls}
-        :param user_attr: The attribute on user entry matching the username passed when authenticating (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_attr AuthMethodLdap#user_attr}
-        :param user_dn: The base DN under which to perform user search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_dn AuthMethodLdap#user_dn}
-        :param user_filter: A go template used to construct a LDAP user search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_filter AuthMethodLdap#user_filter}
-        :param use_token_groups: Use the Active Directory tokenGroups constructed attribute of the user to find the group memberships (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#use_token_groups AuthMethodLdap#use_token_groups}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#scope_id AuthMethodLdap#scope_id}
+        :param account_attribute_maps: Account attribute maps fullname and email. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#account_attribute_maps AuthMethodLdap#account_attribute_maps}
+        :param anon_group_search: Use anon bind when performing LDAP group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#anon_group_search AuthMethodLdap#anon_group_search}
+        :param bind_dn: The distinguished name of entry to bind when performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_dn AuthMethodLdap#bind_dn}
+        :param bind_password: The password to use along with bind-dn performing user and group searches (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_password AuthMethodLdap#bind_password}
+        :param bind_password_hmac: The HMAC of the bind password returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_password_hmac AuthMethodLdap#bind_password_hmac}
+        :param certificates: PEM-encoded X.509 CA certificate in ASN.1 DER form that can be used as a trust anchor when connecting to an LDAP server(optional). This may be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#certificates AuthMethodLdap#certificates}
+        :param client_certificate: PEM-encoded X.509 client certificate in ASN.1 DER form that can be used to authenticate against an LDAP server(optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate AuthMethodLdap#client_certificate}
+        :param client_certificate_key: PEM-encoded X.509 client certificate key in PKCS #8, ASN.1 DER form used with the client certificate (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate_key AuthMethodLdap#client_certificate_key}
+        :param client_certificate_key_hmac: The HMAC of the client certificate key returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate_key_hmac AuthMethodLdap#client_certificate_key_hmac}
+        :param dereference_aliases: Control how aliases are dereferenced when performing the search. Can be one of: NeverDerefAliases, DerefInSearching, DerefFindingBaseObj, and DerefAlways (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#dereference_aliases AuthMethodLdap#dereference_aliases}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#description AuthMethodLdap#description}
+        :param discover_dn: Use anon bind to discover the bind DN of a user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#discover_dn AuthMethodLdap#discover_dn}
+        :param enable_groups: Find the authenticated user's groups during authentication (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#enable_groups AuthMethodLdap#enable_groups}
+        :param group_attr: The attribute that enumerates a user's group membership from entries returned by a group search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_attr AuthMethodLdap#group_attr}
+        :param group_dn: The base DN under which to perform group search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_dn AuthMethodLdap#group_dn}
+        :param group_filter: A go template used to construct a LDAP group search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_filter AuthMethodLdap#group_filter}
+        :param insecure_tls: Skip the LDAP server SSL certificate validation (optional) - insecure and use with caution. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#insecure_tls AuthMethodLdap#insecure_tls}
+        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the the user will be automatically created when they login using an LDAP account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#is_primary_for_scope AuthMethodLdap#is_primary_for_scope}
+        :param maximum_page_size: MaximumPageSize specifies a maximum search result size to use when retrieving the authenticated user's groups (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#maximum_page_size AuthMethodLdap#maximum_page_size}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#name AuthMethodLdap#name}
+        :param start_tls: Issue StartTLS command after connecting (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#start_tls AuthMethodLdap#start_tls}
+        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Defaults to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#state AuthMethodLdap#state}
+        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#type AuthMethodLdap#type}
+        :param upn_domain: The userPrincipalDomain used to construct the UPN string for the authenticating user (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#upn_domain AuthMethodLdap#upn_domain}
+        :param urls: The LDAP URLs that specify LDAP servers to connect to (required). May be specified multiple times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#urls AuthMethodLdap#urls}
+        :param user_attr: The attribute on user entry matching the username passed when authenticating (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_attr AuthMethodLdap#user_attr}
+        :param user_dn: The base DN under which to perform user search (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_dn AuthMethodLdap#user_dn}
+        :param user_filter: A go template used to construct a LDAP user search filter (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_filter AuthMethodLdap#user_filter}
+        :param use_token_groups: Use the Active Directory tokenGroups constructed attribute of the user to find the group memberships (optional). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#use_token_groups AuthMethodLdap#use_token_groups}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7c3fa989bab318c9833759914b8a10299e3bf7eec840275545f2026b3766418d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -1176,293 +1179,293 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#scope_id AuthMethodLdap#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#scope_id AuthMethodLdap#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def account_attribute_maps(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Account attribute maps fullname and email.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#account_attribute_maps AuthMethodLdap#account_attribute_maps}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#account_attribute_maps AuthMethodLdap#account_attribute_maps}
         '''
         result = self._values.get("account_attribute_maps")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def anon_group_search(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use anon bind when performing LDAP group searches (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#anon_group_search AuthMethodLdap#anon_group_search}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#anon_group_search AuthMethodLdap#anon_group_search}
         '''
         result = self._values.get("anon_group_search")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def bind_dn(self) -> typing.Optional[builtins.str]:
         '''The distinguished name of entry to bind when performing user and group searches (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_dn AuthMethodLdap#bind_dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_dn AuthMethodLdap#bind_dn}
         '''
         result = self._values.get("bind_dn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def bind_password(self) -> typing.Optional[builtins.str]:
         '''The password to use along with bind-dn performing user and group searches (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_password AuthMethodLdap#bind_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_password AuthMethodLdap#bind_password}
         '''
         result = self._values.get("bind_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def bind_password_hmac(self) -> typing.Optional[builtins.str]:
         '''The HMAC of the bind password returned by the Boundary controller, which is used for comparison after initial setting of the value.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#bind_password_hmac AuthMethodLdap#bind_password_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#bind_password_hmac AuthMethodLdap#bind_password_hmac}
         '''
         result = self._values.get("bind_password_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def certificates(self) -> typing.Optional[typing.List[builtins.str]]:
         '''PEM-encoded X.509 CA certificate in ASN.1 DER form that can be used as a trust anchor when connecting to an LDAP server(optional).  This may be specified multiple times.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#certificates AuthMethodLdap#certificates}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#certificates AuthMethodLdap#certificates}
         '''
         result = self._values.get("certificates")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def client_certificate(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded X.509 client certificate in ASN.1 DER form that can be used to authenticate against an LDAP server(optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate AuthMethodLdap#client_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate AuthMethodLdap#client_certificate}
         '''
         result = self._values.get("client_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate_key(self) -> typing.Optional[builtins.str]:
         '''PEM-encoded X.509 client certificate key in PKCS #8, ASN.1 DER form used with the client certificate (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate_key AuthMethodLdap#client_certificate_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate_key AuthMethodLdap#client_certificate_key}
         '''
         result = self._values.get("client_certificate_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate_key_hmac(self) -> typing.Optional[builtins.str]:
         '''The HMAC of the client certificate key returned by the Boundary controller, which is used for comparison after initial setting of the value.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#client_certificate_key_hmac AuthMethodLdap#client_certificate_key_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#client_certificate_key_hmac AuthMethodLdap#client_certificate_key_hmac}
         '''
         result = self._values.get("client_certificate_key_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def dereference_aliases(self) -> typing.Optional[builtins.str]:
         '''Control how aliases are dereferenced when performing the search. Can be one of: NeverDerefAliases, DerefInSearching, DerefFindingBaseObj, and DerefAlways (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#dereference_aliases AuthMethodLdap#dereference_aliases}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#dereference_aliases AuthMethodLdap#dereference_aliases}
         '''
         result = self._values.get("dereference_aliases")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#description AuthMethodLdap#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#description AuthMethodLdap#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def discover_dn(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use anon bind to discover the bind DN of a user (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#discover_dn AuthMethodLdap#discover_dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#discover_dn AuthMethodLdap#discover_dn}
         '''
         result = self._values.get("discover_dn")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def enable_groups(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Find the authenticated user's groups during authentication (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#enable_groups AuthMethodLdap#enable_groups}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#enable_groups AuthMethodLdap#enable_groups}
         '''
         result = self._values.get("enable_groups")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def group_attr(self) -> typing.Optional[builtins.str]:
         '''The attribute that enumerates a user's group membership from entries returned by a group search (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_attr AuthMethodLdap#group_attr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_attr AuthMethodLdap#group_attr}
         '''
         result = self._values.get("group_attr")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def group_dn(self) -> typing.Optional[builtins.str]:
         '''The base DN under which to perform group search.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_dn AuthMethodLdap#group_dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_dn AuthMethodLdap#group_dn}
         '''
         result = self._values.get("group_dn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def group_filter(self) -> typing.Optional[builtins.str]:
         '''A go template used to construct a LDAP group search filter (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#group_filter AuthMethodLdap#group_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#group_filter AuthMethodLdap#group_filter}
         '''
         result = self._values.get("group_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def insecure_tls(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Skip the LDAP server SSL certificate validation (optional) - insecure and use with caution.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#insecure_tls AuthMethodLdap#insecure_tls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#insecure_tls AuthMethodLdap#insecure_tls}
         '''
         result = self._values.get("insecure_tls")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def is_primary_for_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, makes this auth method the primary auth method for the scope in which it resides.
 
         The primary auth method for a scope means the the user will be automatically created when they login using an LDAP account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#is_primary_for_scope AuthMethodLdap#is_primary_for_scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#is_primary_for_scope AuthMethodLdap#is_primary_for_scope}
         '''
         result = self._values.get("is_primary_for_scope")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def maximum_page_size(self) -> typing.Optional[jsii.Number]:
         '''MaximumPageSize specifies a maximum search result size to use when retrieving the authenticated user's groups (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#maximum_page_size AuthMethodLdap#maximum_page_size}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#maximum_page_size AuthMethodLdap#maximum_page_size}
         '''
         result = self._values.get("maximum_page_size")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#name AuthMethodLdap#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#name AuthMethodLdap#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def start_tls(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Issue StartTLS command after connecting (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#start_tls AuthMethodLdap#start_tls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#start_tls AuthMethodLdap#start_tls}
         '''
         result = self._values.get("start_tls")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def state(self) -> typing.Optional[builtins.str]:
         '''Can be one of 'inactive', 'active-private', or 'active-public'. Defaults to active-public.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#state AuthMethodLdap#state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#state AuthMethodLdap#state}
         '''
         result = self._values.get("state")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of auth method; hardcoded.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#type AuthMethodLdap#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#type AuthMethodLdap#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def upn_domain(self) -> typing.Optional[builtins.str]:
         '''The userPrincipalDomain used to construct the UPN string for the authenticating user (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#upn_domain AuthMethodLdap#upn_domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#upn_domain AuthMethodLdap#upn_domain}
         '''
         result = self._values.get("upn_domain")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def urls(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The LDAP URLs that specify LDAP servers to connect to (required).  May be specified multiple times.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#urls AuthMethodLdap#urls}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#urls AuthMethodLdap#urls}
         '''
         result = self._values.get("urls")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def user_attr(self) -> typing.Optional[builtins.str]:
         '''The attribute on user entry matching the username passed when authenticating (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_attr AuthMethodLdap#user_attr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_attr AuthMethodLdap#user_attr}
         '''
         result = self._values.get("user_attr")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def user_dn(self) -> typing.Optional[builtins.str]:
         '''The base DN under which to perform user search (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_dn AuthMethodLdap#user_dn}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_dn AuthMethodLdap#user_dn}
         '''
         result = self._values.get("user_dn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def user_filter(self) -> typing.Optional[builtins.str]:
         '''A go template used to construct a LDAP user search filter (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#user_filter AuthMethodLdap#user_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#user_filter AuthMethodLdap#user_filter}
         '''
         result = self._values.get("user_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def use_token_groups(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Use the Active Directory tokenGroups constructed attribute of the user to find the group memberships (optional).
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_ldap#use_token_groups AuthMethodLdap#use_token_groups}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_ldap#use_token_groups AuthMethodLdap#use_token_groups}
         '''
         result = self._values.get("use_token_groups")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_auth_method_oidc`
 
-Refer to the Terraform Registry for docs: [`boundary_auth_method_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc).
+Refer to the Terraform Registry for docs: [`boundary_auth_method_oidc`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AuthMethodOidc(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethodOidc.AuthMethodOidc",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc boundary_auth_method_oidc}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc boundary_auth_method_oidc}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -57,38 +60,38 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc boundary_auth_method_oidc} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc boundary_auth_method_oidc} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
-        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
-        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
-        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
-        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
-        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
-        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
-        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
-        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
-        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
-        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
-        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
-        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
-        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
-        :param prompts: The prompts passed to the identity provider to determine whether to prompt the end-user for reauthentication, account selection or consent. Please note the values passed are case-sensitive. The valid values are: ``none``, ``login``, ``consent`` and ``select_account``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#prompts AuthMethodOidc#prompts}
-        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
-        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
-        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
+        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
+        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
+        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
+        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
+        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
+        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
+        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
+        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
+        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
+        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
+        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
+        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
+        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
+        :param prompts: The prompts passed to the identity provider to determine whether to prompt the end-user for reauthentication, account selection or consent. Please note the values passed are case-sensitive. The valid values are: ``none``, ``login``, ``consent`` and ``select_account``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#prompts AuthMethodOidc#prompts}
+        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
+        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
+        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -138,15 +141,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AuthMethodOidc resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AuthMethodOidc to import.
-        :param import_from_id: The id of the existing AuthMethodOidc that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AuthMethodOidc that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AuthMethodOidc to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__94e1dc85b9a1a903a05d70f6b601adec7ec57de5fc5f6f0052932cffc417f3fe)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -671,34 +674,34 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
-        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
-        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
-        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
-        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
-        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
-        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
-        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
-        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
-        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
-        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
-        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
-        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
-        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
-        :param prompts: The prompts passed to the identity provider to determine whether to prompt the end-user for reauthentication, account selection or consent. Please note the values passed are case-sensitive. The valid values are: ``none``, ``login``, ``consent`` and ``select_account``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#prompts AuthMethodOidc#prompts}
-        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
-        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
-        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
+        :param account_claim_maps: Account claim maps for the to_claim of sub. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
+        :param allowed_audiences: Audiences for which the provider responses will be allowed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
+        :param api_url_prefix: The API prefix to use when generating callback URLs for the provider. Should be set to an address at which the provider can reach back to the controller. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
+        :param callback_url: The URL that should be provided to the IdP for callbacks. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
+        :param claims_scopes: Claims scopes. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
+        :param client_id: The client ID assigned to this auth method from the provider. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
+        :param client_secret: The secret key assigned to this auth method from the provider. Once set, only the hash will be kept and the original value can be removed from configuration. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
+        :param client_secret_hmac: The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
+        :param disable_discovered_config_validation: Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here. The validation is only performed at create or update time. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
+        :param idp_ca_certs: A list of CA certificates to trust when validating the IdP's token signatures. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
+        :param is_primary_for_scope: When true, makes this auth method the primary auth method for the scope in which it resides. The primary auth method for a scope means the user will be automatically created when they login using an OIDC account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
+        :param issuer: The issuer corresponding to the provider, which must match the issuer field in generated tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
+        :param max_age: The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again. A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
+        :param prompts: The prompts passed to the identity provider to determine whether to prompt the end-user for reauthentication, account selection or consent. Please note the values passed are case-sensitive. The valid values are: ``none``, ``login``, ``consent`` and ``select_account``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#prompts AuthMethodOidc#prompts}
+        :param signing_algorithms: Allowed signing algorithms for the provider's issued tokens. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
+        :param state: Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
+        :param type: The type of auth method; hardcoded. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__109748e397e8bf3db45cc8c8ef5e0c5cd569f2720acf7de41e15cd8807f5d1a5)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -847,203 +850,203 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#scope_id AuthMethodOidc#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def account_claim_maps(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Account claim maps for the to_claim of sub.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#account_claim_maps AuthMethodOidc#account_claim_maps}
         '''
         result = self._values.get("account_claim_maps")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def allowed_audiences(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Audiences for which the provider responses will be allowed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#allowed_audiences AuthMethodOidc#allowed_audiences}
         '''
         result = self._values.get("allowed_audiences")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def api_url_prefix(self) -> typing.Optional[builtins.str]:
         '''The API prefix to use when generating callback URLs for the provider.
 
         Should be set to an address at which the provider can reach back to the controller.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#api_url_prefix AuthMethodOidc#api_url_prefix}
         '''
         result = self._values.get("api_url_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def callback_url(self) -> typing.Optional[builtins.str]:
         '''The URL that should be provided to the IdP for callbacks.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#callback_url AuthMethodOidc#callback_url}
         '''
         result = self._values.get("callback_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def claims_scopes(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Claims scopes.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#claims_scopes AuthMethodOidc#claims_scopes}
         '''
         result = self._values.get("claims_scopes")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def client_id(self) -> typing.Optional[builtins.str]:
         '''The client ID assigned to this auth method from the provider.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_id AuthMethodOidc#client_id}
         '''
         result = self._values.get("client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_secret(self) -> typing.Optional[builtins.str]:
         '''The secret key assigned to this auth method from the provider.
 
         Once set, only the hash will be kept and the original value can be removed from configuration.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_secret AuthMethodOidc#client_secret}
         '''
         result = self._values.get("client_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_secret_hmac(self) -> typing.Optional[builtins.str]:
         '''The HMAC of the client secret returned by the Boundary controller, which is used for comparison after initial setting of the value.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#client_secret_hmac AuthMethodOidc#client_secret_hmac}
         '''
         result = self._values.get("client_secret_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#description AuthMethodOidc#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def disable_discovered_config_validation(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Disables validation logic ensuring that the OIDC provider's information from its discovery endpoint matches the information here.
 
         The validation is only performed at create or update time.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#disable_discovered_config_validation AuthMethodOidc#disable_discovered_config_validation}
         '''
         result = self._values.get("disable_discovered_config_validation")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def idp_ca_certs(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of CA certificates to trust when validating the IdP's token signatures.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#idp_ca_certs AuthMethodOidc#idp_ca_certs}
         '''
         result = self._values.get("idp_ca_certs")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def is_primary_for_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When true, makes this auth method the primary auth method for the scope in which it resides.
 
         The primary auth method for a scope means the user will be automatically created when they login using an OIDC account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#is_primary_for_scope AuthMethodOidc#is_primary_for_scope}
         '''
         result = self._values.get("is_primary_for_scope")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def issuer(self) -> typing.Optional[builtins.str]:
         '''The issuer corresponding to the provider, which must match the issuer field in generated tokens.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#issuer AuthMethodOidc#issuer}
         '''
         result = self._values.get("issuer")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def max_age(self) -> typing.Optional[jsii.Number]:
         '''The max age to provide to the provider, indicating how much time is allowed to have passed since the last authentication before the user is challenged again.
 
         A value of 0 sets an immediate requirement for all users to reauthenticate, and an unset maxAge results in a Terraform value of -1 and the default TTL of the chosen OIDC will be used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#max_age AuthMethodOidc#max_age}
         '''
         result = self._values.get("max_age")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#name AuthMethodOidc#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prompts(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The prompts passed to the identity provider to determine whether to prompt the end-user for reauthentication, account selection or consent.
 
         Please note the values passed are case-sensitive. The valid values are: ``none``, ``login``, ``consent`` and ``select_account``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#prompts AuthMethodOidc#prompts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#prompts AuthMethodOidc#prompts}
         '''
         result = self._values.get("prompts")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def signing_algorithms(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Allowed signing algorithms for the provider's issued tokens.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#signing_algorithms AuthMethodOidc#signing_algorithms}
         '''
         result = self._values.get("signing_algorithms")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def state(self) -> typing.Optional[builtins.str]:
         '''Can be one of 'inactive', 'active-private', or 'active-public'. Currently automatically set to active-public.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#state AuthMethodOidc#state}
         '''
         result = self._values.get("state")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of auth method; hardcoded.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_oidc#type AuthMethodOidc#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_auth_method_password`
 
-Refer to the Terraform Registry for docs: [`boundary_auth_method_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password).
+Refer to the Terraform Registry for docs: [`boundary_auth_method_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class AuthMethodPassword(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.authMethodPassword.AuthMethodPassword",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password boundary_auth_method_password}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password boundary_auth_method_password}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password boundary_auth_method_password} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password boundary_auth_method_password} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#description AuthMethodPassword#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#name AuthMethodPassword#name}
-        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#type AuthMethodPassword#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#description AuthMethodPassword#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#name AuthMethodPassword#name}
+        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#type AuthMethodPassword#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a AuthMethodPassword resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the AuthMethodPassword to import.
-        :param import_from_id: The id of the existing AuthMethodPassword that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing AuthMethodPassword that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the AuthMethodPassword to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce289c6f415ae9e22069f8b551ecb238fcd29e91679022f5435ae4c81c0c3b24)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -293,20 +296,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
-        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#description AuthMethodPassword#description}
-        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
-        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
-        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#name AuthMethodPassword#name}
-        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#type AuthMethodPassword#type}
+        :param scope_id: The scope ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
+        :param description: The auth method description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#description AuthMethodPassword#description}
+        :param min_login_name_length: The minimum login name length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
+        :param min_password_length: The minimum password length. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
+        :param name: The auth method name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#name AuthMethodPassword#name}
+        :param type: The resource type, hardcoded per resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#type AuthMethodPassword#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__af88e38a2d8da29c1ca22bf38935f935319c8c7e54482070ed6059cf1b1914ae)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -413,61 +416,61 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#scope_id AuthMethodPassword#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The auth method description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#description AuthMethodPassword#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#description AuthMethodPassword#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def min_login_name_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum login name length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#min_login_name_length AuthMethodPassword#min_login_name_length}
         '''
         result = self._values.get("min_login_name_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def min_password_length(self) -> typing.Optional[jsii.Number]:
         '''The minimum password length.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#min_password_length AuthMethodPassword#min_password_length}
         '''
         result = self._values.get("min_password_length")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The auth method name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#name AuthMethodPassword#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#name AuthMethodPassword#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The resource type, hardcoded per resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/auth_method_password#type AuthMethodPassword#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/auth_method_password#type AuthMethodPassword#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_json/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_json`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_json`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json).
+Refer to the Terraform Registry for docs: [`boundary_credential_json`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialJson(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialJson.CredentialJson",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json boundary_credential_json}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json boundary_credential_json}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json boundary_credential_json} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json boundary_credential_json} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
-        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#object CredentialJson#object}
-        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#description CredentialJson#description}
-        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#name CredentialJson#name}
+        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
+        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#object CredentialJson#object}
+        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#description CredentialJson#description}
+        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#name CredentialJson#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialJson resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialJson to import.
-        :param import_from_id: The id of the existing CredentialJson that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialJson that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialJson to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2fb52ad26743cb294c5f192053c91446bdfc658ec7bddcb62724402b98a8f171)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -242,18 +245,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
-        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#object CredentialJson#object}
-        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#description CredentialJson#description}
-        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#name CredentialJson#name}
+        :param credential_store_id: The credential store in which to save this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
+        :param object: The object for the this json credential. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#object CredentialJson#object}
+        :param description: The description of this json credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#description CredentialJson#description}
+        :param name: The name of this json credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#name CredentialJson#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__340d4278104f6afbd7bb239bf58cb0463b6ea62d015f46764886dc09702f25f7)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -353,46 +356,46 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The credential store in which to save this json credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#credential_store_id CredentialJson#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def object(self) -> builtins.str:
         '''The object for the this json credential.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#object CredentialJson#object}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#object CredentialJson#object}
         '''
         result = self._values.get("object")
         assert result is not None, "Required property 'object' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of this json credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#description CredentialJson#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#description CredentialJson#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of this json credential. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_json#name CredentialJson#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_json#name CredentialJson#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_library_vault`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_library_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault).
+Refer to the Terraform Registry for docs: [`boundary_credential_library_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialLibraryVault(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialLibraryVault.CredentialLibraryVault",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault boundary_credential_library_vault}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault boundary_credential_library_vault}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -45,26 +48,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault boundary_credential_library_vault} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault boundary_credential_library_vault} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
-        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
-        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
-        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
-        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
+        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
+        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
+        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
+        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -102,15 +105,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialLibraryVault resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialLibraryVault to import.
-        :param import_from_id: The id of the existing CredentialLibraryVault that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialLibraryVault that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialLibraryVault to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__548a9299fa73b6bffba1d98163168cbb8eb654f38a54e99e4d80161085c8bc49)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -348,22 +351,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
-        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
-        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
-        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
-        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
+        :param credential_mapping_overrides: The credential mapping override. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
+        :param credential_type: The type of credential the library generates. Cannot be updated on an existing resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
+        :param http_method: The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
+        :param http_request_body: The body of the HTTP request the library sends to Vault when requesting credentials. Only valid if ``http_method`` is set to ``POST``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__91de0f894b7ba615dddb6aca0eb531c0b3eb874ab7cf11ccd93bc0005f9d79fb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -475,84 +478,84 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The ID of the credential store that this library belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_store_id CredentialLibraryVault#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def path(self) -> builtins.str:
         '''The path in Vault to request credentials from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#path CredentialLibraryVault#path}
         '''
         result = self._values.get("path")
         assert result is not None, "Required property 'path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def credential_mapping_overrides(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''The credential mapping override.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_mapping_overrides CredentialLibraryVault#credential_mapping_overrides}
         '''
         result = self._values.get("credential_mapping_overrides")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def credential_type(self) -> typing.Optional[builtins.str]:
         '''The type of credential the library generates. Cannot be updated on an existing resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#credential_type CredentialLibraryVault#credential_type}
         '''
         result = self._values.get("credential_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#description CredentialLibraryVault#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def http_method(self) -> typing.Optional[builtins.str]:
         '''The HTTP method the library uses when requesting credentials from Vault. Defaults to 'GET'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#http_method CredentialLibraryVault#http_method}
         '''
         result = self._values.get("http_method")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def http_request_body(self) -> typing.Optional[builtins.str]:
         '''The body of the HTTP request the library sends to Vault when requesting credentials.
 
         Only valid if ``http_method`` is set to ``POST``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#http_request_body CredentialLibraryVault#http_request_body}
         '''
         result = self._values.get("http_request_body")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault#name CredentialLibraryVault#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_library_vault_ssh_certificate`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_library_vault_ssh_certificate`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate).
+Refer to the Terraform Registry for docs: [`boundary_credential_library_vault_ssh_certificate`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialLibraryVaultSshCertificate(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialLibraryVaultSshCertificate.CredentialLibraryVaultSshCertificate",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -49,30 +52,30 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate boundary_credential_library_vault_ssh_certificate} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
-        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
-        :param additional_valid_principals: Principals to be signed as "valid_principles" in addition to username. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#additional_valid_principals CredentialLibraryVaultSshCertificate#additional_valid_principals}
-        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
-        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
-        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
-        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
-        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
-        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
+        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
+        :param additional_valid_principals: Principals to be signed as "valid_principles" in addition to username. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#additional_valid_principals CredentialLibraryVaultSshCertificate#additional_valid_principals}
+        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
+        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
+        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
+        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
+        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
+        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -114,15 +117,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialLibraryVaultSshCertificate resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialLibraryVaultSshCertificate to import.
-        :param import_from_id: The id of the existing CredentialLibraryVaultSshCertificate that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialLibraryVaultSshCertificate that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialLibraryVaultSshCertificate to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7190fe129cf76728c675704972f411f78fd326b467bff93be73661374f92bf19)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -452,26 +455,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
-        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
-        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
-        :param additional_valid_principals: Principals to be signed as "valid_principles" in addition to username. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#additional_valid_principals CredentialLibraryVaultSshCertificate#additional_valid_principals}
-        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
-        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
-        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
-        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
-        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
-        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
-        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
-        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
+        :param credential_store_id: The ID of the credential store that this library belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
+        :param path: The path in Vault to request credentials from. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
+        :param username: The username to use with the certificate returned by the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
+        :param additional_valid_principals: Principals to be signed as "valid_principles" in addition to username. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#additional_valid_principals CredentialLibraryVaultSshCertificate#additional_valid_principals}
+        :param critical_options: Specifies a map of the critical options that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
+        :param description: The Vault credential library description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
+        :param extensions: Specifies a map of the extensions that the certificate should be signed for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
+        :param key_bits: Specifies the number of bits to use for the generated keys. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
+        :param key_id: Specifies the key id a certificate should have. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
+        :param key_type: Specifies the desired key type; must be ed25519, ecdsa, or rsa. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
+        :param name: The Vault credential library name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
+        :param ttl: Specifies the requested time to live for a certificate returned from the library. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__07a8dcdd30946ca78931edfad9b73c37ebdc6bbf6b64db6c12efef586c5bdaeb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -594,119 +597,119 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The ID of the credential store that this library belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#credential_store_id CredentialLibraryVaultSshCertificate#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def path(self) -> builtins.str:
         '''The path in Vault to request credentials from.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#path CredentialLibraryVaultSshCertificate#path}
         '''
         result = self._values.get("path")
         assert result is not None, "Required property 'path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username to use with the certificate returned by the library.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#username CredentialLibraryVaultSshCertificate#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def additional_valid_principals(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Principals to be signed as "valid_principles" in addition to username.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#additional_valid_principals CredentialLibraryVaultSshCertificate#additional_valid_principals}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#additional_valid_principals CredentialLibraryVaultSshCertificate#additional_valid_principals}
         '''
         result = self._values.get("additional_valid_principals")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def critical_options(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Specifies a map of the critical options that the certificate should be signed for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#critical_options CredentialLibraryVaultSshCertificate#critical_options}
         '''
         result = self._values.get("critical_options")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#description CredentialLibraryVaultSshCertificate#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def extensions(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''Specifies a map of the extensions that the certificate should be signed for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#extensions CredentialLibraryVaultSshCertificate#extensions}
         '''
         result = self._values.get("extensions")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def key_bits(self) -> typing.Optional[jsii.Number]:
         '''Specifies the number of bits to use for the generated keys.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_bits CredentialLibraryVaultSshCertificate#key_bits}
         '''
         result = self._values.get("key_bits")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def key_id(self) -> typing.Optional[builtins.str]:
         '''Specifies the key id a certificate should have.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_id CredentialLibraryVaultSshCertificate#key_id}
         '''
         result = self._values.get("key_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def key_type(self) -> typing.Optional[builtins.str]:
         '''Specifies the desired key type; must be ed25519, ecdsa, or rsa.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#key_type CredentialLibraryVaultSshCertificate#key_type}
         '''
         result = self._values.get("key_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The Vault credential library name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#name CredentialLibraryVaultSshCertificate#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[builtins.str]:
         '''Specifies the requested time to live for a certificate returned from the library.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_library_vault_ssh_certificate#ttl CredentialLibraryVaultSshCertificate#ttl}
         '''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_ssh_private_key/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_ssh_private_key`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_ssh_private_key`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key).
+Refer to the Terraform Registry for docs: [`boundary_credential_ssh_private_key`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialSshPrivateKey(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialSshPrivateKey.CredentialSshPrivateKey",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key boundary_credential_ssh_private_key} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
-        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
-        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
-        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
-        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
-        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
+        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
+        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
+        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
+        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
+        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
+        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialSshPrivateKey resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialSshPrivateKey to import.
-        :param import_from_id: The id of the existing CredentialSshPrivateKey that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialSshPrivateKey that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialSshPrivateKey to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6c8135fb4fafe6386cb377d4533cc3b77c029eb2186d0fb82596cfcebcf45b0e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -295,20 +298,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
-        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
-        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
-        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
-        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
-        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
+        :param credential_store_id: ID of the credential store this credential belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
+        :param private_key: The private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
+        :param username: The username associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
+        :param description: The description of the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
+        :param name: The name of the credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
+        :param private_key_passphrase: The passphrase of the private key associated with the credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__30a5df1330fa363ae15ceeafc3730ab842c6721e89ade7fcc4b7d65e0db69db4)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -413,63 +416,63 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''ID of the credential store this credential belongs to.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#credential_store_id CredentialSshPrivateKey#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def private_key(self) -> builtins.str:
         '''The private key associated with the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#private_key CredentialSshPrivateKey#private_key}
         '''
         result = self._values.get("private_key")
         assert result is not None, "Required property 'private_key' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username associated with the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#username CredentialSshPrivateKey#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#description CredentialSshPrivateKey#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of the credential. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#name CredentialSshPrivateKey#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def private_key_passphrase(self) -> typing.Optional[builtins.str]:
         '''The passphrase of the private key associated with the credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_ssh_private_key#private_key_passphrase CredentialSshPrivateKey#private_key_passphrase}
         '''
         result = self._values.get("private_key_passphrase")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_store_static/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_store_static`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_store_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static).
+Refer to the Terraform Registry for docs: [`boundary_credential_store_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialStoreStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialStoreStatic.CredentialStoreStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static boundary_credential_store_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static boundary_credential_store_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -40,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static boundary_credential_store_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static boundary_credential_store_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
-        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#description CredentialStoreStatic#description}
-        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#name CredentialStoreStatic#name}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
+        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#description CredentialStoreStatic#description}
+        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#name CredentialStoreStatic#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialStoreStatic resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialStoreStatic to import.
-        :param import_from_id: The id of the existing CredentialStoreStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialStoreStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialStoreStatic to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9d8f200a73a6f7e8a2d804af52f906e0c207fcf9b437bfa9d91daf3f3f279140)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -215,17 +218,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
-        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#description CredentialStoreStatic#description}
-        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#name CredentialStoreStatic#name}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
+        :param description: The static credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#description CredentialStoreStatic#description}
+        :param name: The static credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#name CredentialStoreStatic#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9199286378c9cad7567fbfde5ad647f35cde57753384ceb6f5f8980c1bcd491a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -323,34 +326,34 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope for this credential store.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#scope_id CredentialStoreStatic#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The static credential store description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#description CredentialStoreStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#description CredentialStoreStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The static credential store name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_static#name CredentialStoreStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_static#name CredentialStoreStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_store_vault/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_store_vault`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_store_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault).
+Refer to the Terraform Registry for docs: [`boundary_credential_store_vault`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialStoreVault(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialStoreVault.CredentialStoreVault",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault boundary_credential_store_vault}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault boundary_credential_store_vault}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         address: builtins.str,
@@ -49,30 +52,30 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault boundary_credential_store_vault} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault boundary_credential_store_vault} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#address CredentialStoreVault#address}
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
-        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#token CredentialStoreVault#token}
-        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
-        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
-        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
-        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#description CredentialStoreVault#description}
-        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#name CredentialStoreVault#name}
-        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
-        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
-        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
-        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
+        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#address CredentialStoreVault#address}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
+        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#token CredentialStoreVault#token}
+        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
+        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
+        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
+        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#description CredentialStoreVault#description}
+        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#name CredentialStoreVault#name}
+        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
+        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
+        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
+        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -114,15 +117,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialStoreVault resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialStoreVault to import.
-        :param import_from_id: The id of the existing CredentialStoreVault that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialStoreVault that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialStoreVault to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__546027ed0247ecf2e63b0a6cc254c1d69c7864f806533cc0f612f18ecff8a1a7)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -458,26 +461,26 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#address CredentialStoreVault#address}
-        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
-        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#token CredentialStoreVault#token}
-        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
-        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
-        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
-        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#description CredentialStoreVault#description}
-        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#name CredentialStoreVault#name}
-        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
-        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
-        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
-        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
+        :param address: The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#address CredentialStoreVault#address}
+        :param scope_id: The scope for this credential store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
+        :param token: A token used for accessing Vault. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#token CredentialStoreVault#token}
+        :param ca_cert: A PEM-encoded CA certificate to verify the Vault server's TLS certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
+        :param client_certificate: A PEM-encoded client certificate to use for TLS authentication to the Vault server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
+        :param client_certificate_key: A PEM-encoded private key matching the client certificate from 'client_certificate'. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
+        :param description: The Vault credential store description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#description CredentialStoreVault#description}
+        :param name: The Vault credential store name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#name CredentialStoreVault#name}
+        :param namespace: The namespace within Vault to use. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
+        :param tls_server_name: Name to use as the SNI host when connecting to Vault via TLS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
+        :param tls_skip_verify: Whether or not to skip TLS verification. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
+        :param worker_filter: HCP Only. A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__98b4ccd3b8d782228826e5520d5bbf05d295e8cc284d74dbfbe4630aaff8c9ef)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -600,121 +603,121 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def address(self) -> builtins.str:
         '''The address to Vault server. This should be a complete URL such as 'https://127.0.0.1:8200'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#address CredentialStoreVault#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#address CredentialStoreVault#address}
         '''
         result = self._values.get("address")
         assert result is not None, "Required property 'address' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope for this credential store.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#scope_id CredentialStoreVault#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def token(self) -> builtins.str:
         '''A token used for accessing Vault.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#token CredentialStoreVault#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#token CredentialStoreVault#token}
         '''
         result = self._values.get("token")
         assert result is not None, "Required property 'token' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ca_cert(self) -> typing.Optional[builtins.str]:
         '''A PEM-encoded CA certificate to verify the Vault server's TLS certificate.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#ca_cert CredentialStoreVault#ca_cert}
         '''
         result = self._values.get("ca_cert")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate(self) -> typing.Optional[builtins.str]:
         '''A PEM-encoded client certificate to use for TLS authentication to the Vault server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#client_certificate CredentialStoreVault#client_certificate}
         '''
         result = self._values.get("client_certificate")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def client_certificate_key(self) -> typing.Optional[builtins.str]:
         '''A PEM-encoded private key matching the client certificate from 'client_certificate'.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#client_certificate_key CredentialStoreVault#client_certificate_key}
         '''
         result = self._values.get("client_certificate_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The Vault credential store description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#description CredentialStoreVault#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#description CredentialStoreVault#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The Vault credential store name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#name CredentialStoreVault#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#name CredentialStoreVault#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def namespace(self) -> typing.Optional[builtins.str]:
         '''The namespace within Vault to use.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#namespace CredentialStoreVault#namespace}
         '''
         result = self._values.get("namespace")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tls_server_name(self) -> typing.Optional[builtins.str]:
         '''Name to use as the SNI host when connecting to Vault via TLS.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#tls_server_name CredentialStoreVault#tls_server_name}
         '''
         result = self._values.get("tls_server_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tls_skip_verify(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not to skip TLS verification.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#tls_skip_verify CredentialStoreVault#tls_skip_verify}
         '''
         result = self._values.get("tls_skip_verify")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def worker_filter(self) -> typing.Optional[builtins.str]:
         '''HCP Only.
 
         A filter used to control which PKI workers can handle Vault requests. This allows the use of private Vault instances with Boundary.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_store_vault#worker_filter CredentialStoreVault#worker_filter}
         '''
         result = self._values.get("worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/credential_username_password/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_credential_username_password`
 
-Refer to the Terraform Registry for docs: [`boundary_credential_username_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password).
+Refer to the Terraform Registry for docs: [`boundary_credential_username_password`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class CredentialUsernamePassword(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.credentialUsernamePassword.CredentialUsernamePassword",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password boundary_credential_username_password}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password boundary_credential_username_password}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         credential_store_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password boundary_credential_username_password} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password boundary_credential_username_password} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
-        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
-        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
-        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
-        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
+        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
+        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
+        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
+        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
+        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a CredentialUsernamePassword resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the CredentialUsernamePassword to import.
-        :param import_from_id: The id of the existing CredentialUsernamePassword that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing CredentialUsernamePassword that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the CredentialUsernamePassword to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__163f882e49d01fe747fa216c6b5bf7644b50ab8c13ac0210ac86f9f6202e6032)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -264,19 +267,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
-        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
-        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
-        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
-        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
+        :param credential_store_id: The credential store in which to save this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
+        :param password: The password of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
+        :param username: The username of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
+        :param description: The description of this username/password credential. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
+        :param name: The name of this username/password credential. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ffd92fc256fbcf6b17cc68b6fbac14f8859e600b946cff80399bbbf4c2cc960d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -378,54 +381,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def credential_store_id(self) -> builtins.str:
         '''The credential store in which to save this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#credential_store_id CredentialUsernamePassword#credential_store_id}
         '''
         result = self._values.get("credential_store_id")
         assert result is not None, "Required property 'credential_store_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def password(self) -> builtins.str:
         '''The password of this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#password CredentialUsernamePassword#password}
         '''
         result = self._values.get("password")
         assert result is not None, "Required property 'password' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def username(self) -> builtins.str:
         '''The username of this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#username CredentialUsernamePassword#username}
         '''
         result = self._values.get("username")
         assert result is not None, "Required property 'username' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description of this username/password credential.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#description CredentialUsernamePassword#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name of this username/password credential. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/credential_username_password#name CredentialUsernamePassword#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_account/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_boundary_account`
 
-Refer to the Terraform Registry for docs: [`data_boundary_account`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account).
+Refer to the Terraform Registry for docs: [`data_boundary_account`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataBoundaryAccount(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.dataBoundaryAccount.DataBoundaryAccount",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account boundary_account}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account boundary_account}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account boundary_account} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account boundary_account} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The auth method ID that will be queried for the account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#auth_method_id DataBoundaryAccount#auth_method_id}
-        :param name: The name of the account to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#name DataBoundaryAccount#name}
+        :param auth_method_id: The auth method ID that will be queried for the account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#auth_method_id DataBoundaryAccount#auth_method_id}
+        :param name: The name of the account to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#name DataBoundaryAccount#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataBoundaryAccount resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataBoundaryAccount to import.
-        :param import_from_id: The id of the existing DataBoundaryAccount that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataBoundaryAccount that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataBoundaryAccount to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cba50c1ca7a0edcd622c611be1b522ec46c0ccce9635d1c05ce44ab670bc43cd)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -200,16 +203,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The auth method ID that will be queried for the account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#auth_method_id DataBoundaryAccount#auth_method_id}
-        :param name: The name of the account to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#name DataBoundaryAccount#name}
+        :param auth_method_id: The auth method ID that will be queried for the account. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#auth_method_id DataBoundaryAccount#auth_method_id}
+        :param name: The name of the account to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#name DataBoundaryAccount#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bd62977769ee2acd0d9a3ca9947603072506d12e1dba635272bd81224e9fe87e)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -303,25 +306,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The auth method ID that will be queried for the account.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#auth_method_id DataBoundaryAccount#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#auth_method_id DataBoundaryAccount#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the account to retrieve.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/account#name DataBoundaryAccount#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/account#name DataBoundaryAccount#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_auth_method/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_auth_method/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_boundary_auth_method`
 
-Refer to the Terraform Registry for docs: [`data_boundary_auth_method`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method).
+Refer to the Terraform Registry for docs: [`data_boundary_auth_method`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataBoundaryAuthMethod(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.dataBoundaryAuthMethod.DataBoundaryAuthMethod",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method boundary_auth_method}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method boundary_auth_method}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method boundary_auth_method} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method boundary_auth_method} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the auth method to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#name DataBoundaryAuthMethod#name}
-        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#scope_id DataBoundaryAuthMethod#scope_id}
+        :param name: The name of the auth method to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#name DataBoundaryAuthMethod#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#scope_id DataBoundaryAuthMethod#scope_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataBoundaryAuthMethod resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataBoundaryAuthMethod to import.
-        :param import_from_id: The id of the existing DataBoundaryAuthMethod that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataBoundaryAuthMethod that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataBoundaryAuthMethod to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6d8a333db2abc24cc7a87bf1aa03a762e72b5ca3189c0a5a2b81b9095295bf35)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -204,16 +207,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the auth method to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#name DataBoundaryAuthMethod#name}
-        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#scope_id DataBoundaryAuthMethod#scope_id}
+        :param name: The name of the auth method to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#name DataBoundaryAuthMethod#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#scope_id DataBoundaryAuthMethod#scope_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5125dc1c4a610f9e62f31de05de210d87018ebf15a5e83d30ae72a3340aa1dee)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -308,25 +311,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the auth method to retrieve.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#name DataBoundaryAuthMethod#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#name DataBoundaryAuthMethod#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope ID in which the resource is created. Defaults ``global`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/auth_method#scope_id DataBoundaryAuthMethod#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/auth_method#scope_id DataBoundaryAuthMethod#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_group/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_group/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_boundary_group`
 
-Refer to the Terraform Registry for docs: [`data_boundary_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group).
+Refer to the Terraform Registry for docs: [`data_boundary_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataBoundaryGroup(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.dataBoundaryGroup.DataBoundaryGroup",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group boundary_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group boundary_group}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group boundary_group} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group boundary_group} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the group to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#name DataBoundaryGroup#name}
-        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#scope_id DataBoundaryGroup#scope_id}
+        :param name: The name of the group to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#name DataBoundaryGroup#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#scope_id DataBoundaryGroup#scope_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataBoundaryGroup resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataBoundaryGroup to import.
-        :param import_from_id: The id of the existing DataBoundaryGroup that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataBoundaryGroup that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataBoundaryGroup to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__98d5a283f3d13650da3fe5c4c9928154450dd3a2f7b5a4b0c61ffc5071e3d88c)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -204,16 +207,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the group to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#name DataBoundaryGroup#name}
-        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#scope_id DataBoundaryGroup#scope_id}
+        :param name: The name of the group to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#name DataBoundaryGroup#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#scope_id DataBoundaryGroup#scope_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d6a7df795b972257d8b9592c96ba518824144ee6d891c74395a84ba541998505)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -308,25 +311,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the group to retrieve.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#name DataBoundaryGroup#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#name DataBoundaryGroup#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope ID in which the resource is created. Defaults ``global`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/group#scope_id DataBoundaryGroup#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/group#scope_id DataBoundaryGroup#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_scope/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_scope/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_boundary_scope`
 
-Refer to the Terraform Registry for docs: [`data_boundary_scope`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope).
+Refer to the Terraform Registry for docs: [`data_boundary_scope`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataBoundaryScope(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.dataBoundaryScope.DataBoundaryScope",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope boundary_scope}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope boundary_scope}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope boundary_scope} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope boundary_scope} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The name of the scope to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#name DataBoundaryScope#name}
-        :param scope_id: The parent scope ID that will be queried for the scope. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#scope_id DataBoundaryScope#scope_id}
+        :param name: The name of the scope to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#name DataBoundaryScope#name}
+        :param scope_id: The parent scope ID that will be queried for the scope. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#scope_id DataBoundaryScope#scope_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataBoundaryScope resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataBoundaryScope to import.
-        :param import_from_id: The id of the existing DataBoundaryScope that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataBoundaryScope that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataBoundaryScope to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1f2c4f994e9ca133907a4704e6ba918981023395d994aad8bc40917fdea64c1d)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -190,16 +193,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The name of the scope to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#name DataBoundaryScope#name}
-        :param scope_id: The parent scope ID that will be queried for the scope. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#scope_id DataBoundaryScope#scope_id}
+        :param name: The name of the scope to retrieve. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#name DataBoundaryScope#name}
+        :param scope_id: The parent scope ID that will be queried for the scope. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#scope_id DataBoundaryScope#scope_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8b83ed9432504335a7e66e3c2780e2e27683f89eea1381795bf55b297dfef0d6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -293,25 +296,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the scope to retrieve.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#name DataBoundaryScope#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#name DataBoundaryScope#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The parent scope ID that will be queried for the scope.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/scope#scope_id DataBoundaryScope#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/scope#scope_id DataBoundaryScope#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/data_boundary_user/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/data_boundary_user/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `data_boundary_user`
 
-Refer to the Terraform Registry for docs: [`data_boundary_user`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user).
+Refer to the Terraform Registry for docs: [`data_boundary_user`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class DataBoundaryUser(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.dataBoundaryUser.DataBoundaryUser",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user boundary_user}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user boundary_user}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
@@ -39,20 +42,20 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user boundary_user} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user boundary_user} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: The username to search for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#name DataBoundaryUser#name}
-        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#scope_id DataBoundaryUser#scope_id}
+        :param name: The username to search for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#name DataBoundaryUser#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#scope_id DataBoundaryUser#scope_id}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -84,15 +87,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a DataBoundaryUser resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the DataBoundaryUser to import.
-        :param import_from_id: The id of the existing DataBoundaryUser that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing DataBoundaryUser that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the DataBoundaryUser to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__26a84b3236f26f235f6c4a27960bcbc838a7c28e16dd375ba59bcc409863bd45)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -219,16 +222,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: The username to search for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#name DataBoundaryUser#name}
-        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#scope_id DataBoundaryUser#scope_id}
+        :param name: The username to search for. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#name DataBoundaryUser#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults ``global`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#scope_id DataBoundaryUser#scope_id}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__92b063b01212bcf75733ad868209425bb0a717be8f2d41772fa03e7c2539db17)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -323,25 +326,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The username to search for.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#name DataBoundaryUser#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#name DataBoundaryUser#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope ID in which the resource is created. Defaults ``global`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/data-sources/user#scope_id DataBoundaryUser#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/data-sources/user#scope_id DataBoundaryUser#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/group/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/group/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_group`
 
-Refer to the Terraform Registry for docs: [`boundary_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group).
+Refer to the Terraform Registry for docs: [`boundary_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Group(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.group.Group",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group boundary_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group boundary_group}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group boundary_group} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group boundary_group} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#scope_id Group#scope_id}
-        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#description Group#description}
-        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#member_ids Group#member_ids}
-        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#name Group#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#scope_id Group#scope_id}
+        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#description Group#description}
+        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#member_ids Group#member_ids}
+        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#name Group#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Group resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Group to import.
-        :param import_from_id: The id of the existing Group that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Group that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Group to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__28d146e9d72a176eed6ba0aeeffbc45f7f1516f7521e978a39e71ea6f41e8726)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -241,18 +244,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#scope_id Group#scope_id}
-        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#description Group#description}
-        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#member_ids Group#member_ids}
-        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#name Group#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#scope_id Group#scope_id}
+        :param description: The group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#description Group#description}
+        :param member_ids: Resource IDs for group members, these are most likely boundary users. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#member_ids Group#member_ids}
+        :param name: The group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#name Group#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4db7560a2c3e5e1eedd9ad833302c92daa20a64a18b6ee019a618c9566a07e3d)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -353,43 +356,43 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#scope_id Group#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#scope_id Group#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The group description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#description Group#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#description Group#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def member_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Resource IDs for group members, these are most likely boundary users.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#member_ids Group#member_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#member_ids Group#member_ids}
         '''
         result = self._values.get("member_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The group name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/group#name Group#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/group#name Group#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host`
 
-Refer to the Terraform Registry for docs: [`boundary_host`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host).
+Refer to the Terraform Registry for docs: [`boundary_host`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Host(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.host.Host",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host boundary_host}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host boundary_host}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host boundary_host} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host boundary_host} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#host_catalog_id Host#host_catalog_id}.
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#type Host#type}
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#address Host#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#description Host#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#name Host#name}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#host_catalog_id Host#host_catalog_id}.
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#type Host#type}
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#address Host#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#description Host#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#name Host#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Host resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Host to import.
-        :param import_from_id: The id of the existing Host that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Host that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Host to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__30026118af1d820a4d423327fc2b1f9fc4532e5c0345fd39019d0e28cb80a4ca)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -263,19 +266,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#host_catalog_id Host#host_catalog_id}.
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#type Host#type}
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#address Host#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#description Host#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#name Host#name}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#host_catalog_id Host#host_catalog_id}.
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#type Host#type}
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#address Host#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#description Host#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#name Host#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ebe99a87ead3c0ce0b9de7f0dc233a854652e290cf41e96b1c672f05484d1724)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -376,52 +379,52 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#host_catalog_id Host#host_catalog_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#host_catalog_id Host#host_catalog_id}.'''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of host.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#type Host#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#type Host#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address(self) -> typing.Optional[builtins.str]:
         '''The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#address Host#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#address Host#address}
         '''
         result = self._values.get("address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#description Host#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#description Host#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host#name Host#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host#name Host#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_catalog`
 
-Refer to the Terraform Registry for docs: [`boundary_host_catalog`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog).
+Refer to the Terraform Registry for docs: [`boundary_host_catalog`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostCatalog(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostCatalog.HostCatalog",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog boundary_host_catalog}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog boundary_host_catalog}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog boundary_host_catalog} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog boundary_host_catalog} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
-        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#type HostCatalog#type}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#description HostCatalog#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#name HostCatalog#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
+        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#type HostCatalog#type}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#description HostCatalog#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#name HostCatalog#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostCatalog resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostCatalog to import.
-        :param import_from_id: The id of the existing HostCatalog that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostCatalog that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostCatalog to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__332a7500e1179bb543e2ca33ce1555c59a50bf707898136d938e61e975a89187)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -237,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
-        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#type HostCatalog#type}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#description HostCatalog#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#name HostCatalog#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
+        :param type: The host catalog type. Only ``static`` is supported. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#type HostCatalog#type}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#description HostCatalog#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#name HostCatalog#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__221287db26b11bf22cb1c1861301eb80b842c76934da2dfbe1504d9975a77502)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,44 +351,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#scope_id HostCatalog#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The host catalog type. Only ``static`` is supported.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#type HostCatalog#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#type HostCatalog#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host catalog description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#description HostCatalog#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#description HostCatalog#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host catalog name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog#name HostCatalog#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog#name HostCatalog#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog_plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_catalog_plugin`
 
-Refer to the Terraform Registry for docs: [`boundary_host_catalog_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin).
+Refer to the Terraform Registry for docs: [`boundary_host_catalog_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostCatalogPlugin(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostCatalogPlugin.HostCatalogPlugin",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin boundary_host_catalog_plugin}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin boundary_host_catalog_plugin}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -48,29 +51,29 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin boundary_host_catalog_plugin} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin boundary_host_catalog_plugin} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
-        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
-        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
-        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
-        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
-        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
-        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
-        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
-        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
+        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
+        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
+        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
+        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
+        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
+        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
+        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
+        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -111,15 +114,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostCatalogPlugin resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostCatalogPlugin to import.
-        :param import_from_id: The id of the existing HostCatalogPlugin that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostCatalogPlugin that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostCatalogPlugin to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__95837711a9d37693822ce433a569f49201b360d048ac88c70ef2ff9553850488)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -425,25 +428,25 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
-        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
-        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
-        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
-        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
-        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
-        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
-        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
-        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
+        :param attributes_json: The attributes for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
+        :param internal_force_update: Internal only. Used to force update so that we can always check the value of secrets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
+        :param internal_hmac_used_for_secrets_config_hmac: Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
+        :param internal_secrets_config_hmac: Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
+        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
+        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
+        :param secrets_hmac: The HMAC'd secrets value returned from the server. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
+        :param secrets_json: The secrets for the host catalog. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__352355fe94a5287d3aa37ee520dadb07588b2f1dd967fdfb5d4b31e89e6ad83a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -565,112 +568,112 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#scope_id HostCatalogPlugin#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attributes_json(self) -> typing.Optional[builtins.str]:
         '''The attributes for the host catalog.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host catalog.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#attributes_json HostCatalogPlugin#attributes_json}
         '''
         result = self._values.get("attributes_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host catalog description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#description HostCatalogPlugin#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def internal_force_update(self) -> typing.Optional[builtins.str]:
         '''Internal only. Used to force update so that we can always check the value of secrets.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_force_update HostCatalogPlugin#internal_force_update}
         '''
         result = self._values.get("internal_force_update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def internal_hmac_used_for_secrets_config_hmac(
         self,
     ) -> typing.Optional[builtins.str]:
         '''Internal only. The Boundary-provided HMAC used to calculate the current value of the HMAC'd config. Used for drift detection.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_hmac_used_for_secrets_config_hmac HostCatalogPlugin#internal_hmac_used_for_secrets_config_hmac}
         '''
         result = self._values.get("internal_hmac_used_for_secrets_config_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def internal_secrets_config_hmac(self) -> typing.Optional[builtins.str]:
         '''Internal only. HMAC of (serverSecretsHmac + config secrets). Used for proper secrets handling.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#internal_secrets_config_hmac HostCatalogPlugin#internal_secrets_config_hmac}
         '''
         result = self._values.get("internal_secrets_config_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host catalog name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#name HostCatalogPlugin#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the plugin that should back the resource. This or plugin_name must be defined.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#plugin_id HostCatalogPlugin#plugin_id}
         '''
         result = self._values.get("plugin_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_name(self) -> typing.Optional[builtins.str]:
         '''The name of the plugin that should back the resource. This or plugin_id must be defined.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#plugin_name HostCatalogPlugin#plugin_name}
         '''
         result = self._values.get("plugin_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secrets_hmac(self) -> typing.Optional[builtins.str]:
         '''The HMAC'd secrets value returned from the server.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#secrets_hmac HostCatalogPlugin#secrets_hmac}
         '''
         result = self._values.get("secrets_hmac")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secrets_json(self) -> typing.Optional[builtins.str]:
         '''The secrets for the host catalog.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the host catalog; this allows injecting secrets for one call, then removing them for storage.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_plugin#secrets_json HostCatalogPlugin#secrets_json}
         '''
         result = self._values.get("secrets_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_catalog_static/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_catalog_static`
 
-Refer to the Terraform Registry for docs: [`boundary_host_catalog_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static).
+Refer to the Terraform Registry for docs: [`boundary_host_catalog_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostCatalogStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostCatalogStatic.HostCatalogStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static boundary_host_catalog_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static boundary_host_catalog_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -40,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static boundary_host_catalog_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static boundary_host_catalog_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#description HostCatalogStatic#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#name HostCatalogStatic#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#description HostCatalogStatic#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#name HostCatalogStatic#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostCatalogStatic resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostCatalogStatic to import.
-        :param import_from_id: The id of the existing HostCatalogStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostCatalogStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostCatalogStatic to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__be0558996bf377c13a87c0677689679366cf94d1a03365b2f86f268d104ea215)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -215,17 +218,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
-        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#description HostCatalogStatic#description}
-        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#name HostCatalogStatic#name}
+        :param scope_id: The scope ID in which the resource is created. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
+        :param description: The host catalog description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#description HostCatalogStatic#description}
+        :param name: The host catalog name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#name HostCatalogStatic#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b9383c014a702a29d2bd6b4cb2cb8ffbdb1a1941e41b5c6c21399d435f4054ea)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -323,34 +326,34 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#scope_id HostCatalogStatic#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host catalog description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#description HostCatalogStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#description HostCatalogStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host catalog name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_catalog_static#name HostCatalogStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_catalog_static#name HostCatalogStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_set`
 
-Refer to the Terraform Registry for docs: [`boundary_host_set`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set).
+Refer to the Terraform Registry for docs: [`boundary_host_set`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostSet(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostSet.HostSet",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set boundary_host_set}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set boundary_host_set}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set boundary_host_set} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set boundary_host_set} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#type HostSet#type}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#description HostSet#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#host_ids HostSet#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#name HostSet#name}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#type HostSet#type}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#description HostSet#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#host_ids HostSet#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#name HostSet#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostSet resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostSet to import.
-        :param import_from_id: The id of the existing HostSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostSet that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostSet to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f0eb22a4a41a2ee76a91a258d3e87aef115d02a862349696a5072e5c7eac7291)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -263,19 +266,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#type HostSet#type}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#description HostSet#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#host_ids HostSet#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#name HostSet#name}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#type HostSet#type}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#description HostSet#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#host_ids HostSet#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#name HostSet#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4f0f7249da202193b7621aef5791ff05b5a4977c2a6ddd1052028d3fd7cdea2f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -378,53 +381,53 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
         '''The catalog for the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#host_catalog_id HostSet#host_catalog_id}
         '''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The type of host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#type HostSet#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#type HostSet#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host set description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#description HostSet#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#description HostSet#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of host IDs contained in this set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#host_ids HostSet#host_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#host_ids HostSet#host_ids}
         '''
         result = self._values.get("host_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host set name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set#name HostSet#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set#name HostSet#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set_plugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_set_plugin`
 
-Refer to the Terraform Registry for docs: [`boundary_host_set_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin).
+Refer to the Terraform Registry for docs: [`boundary_host_set_plugin`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostSetPlugin(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostSetPlugin.HostSetPlugin",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin boundary_host_set_plugin}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin boundary_host_set_plugin}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -44,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin boundary_host_set_plugin} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin boundary_host_set_plugin} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
-        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#description HostSetPlugin#description}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#name HostSetPlugin#name}
-        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
-        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#type HostSetPlugin#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
+        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#description HostSetPlugin#description}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#name HostSetPlugin#name}
+        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
+        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#type HostSetPlugin#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostSetPlugin resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostSetPlugin to import.
-        :param import_from_id: The id of the existing HostSetPlugin that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostSetPlugin that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostSetPlugin to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__161470354e3e5c1395bd92dba7c68acbffa7fea9ff3c1b3d8824e24f51284376)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -319,21 +322,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
-        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#description HostSetPlugin#description}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#name HostSetPlugin#name}
-        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
-        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#type HostSetPlugin#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
+        :param attributes_json: The attributes for the host set. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#description HostSetPlugin#description}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#name HostSetPlugin#name}
+        :param preferred_endpoints: The ordered list of preferred endpoints. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
+        :param sync_interval_seconds: The value to set for the sync interval seconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#type HostSetPlugin#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__118767d2d06e32bb053df9ba5727e72bfc2f7350f582cb3475bfc3b827e174f3)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -443,72 +446,72 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
         '''The catalog for the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#host_catalog_id HostSetPlugin#host_catalog_id}
         '''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attributes_json(self) -> typing.Optional[builtins.str]:
         '''The attributes for the host set.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#attributes_json HostSetPlugin#attributes_json}
         '''
         result = self._values.get("attributes_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host set description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#description HostSetPlugin#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#description HostSetPlugin#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host set name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#name HostSetPlugin#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#name HostSetPlugin#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def preferred_endpoints(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The ordered list of preferred endpoints.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#preferred_endpoints HostSetPlugin#preferred_endpoints}
         '''
         result = self._values.get("preferred_endpoints")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def sync_interval_seconds(self) -> typing.Optional[jsii.Number]:
         '''The value to set for the sync interval seconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#sync_interval_seconds HostSetPlugin#sync_interval_seconds}
         '''
         result = self._values.get("sync_interval_seconds")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_plugin#type HostSetPlugin#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_plugin#type HostSetPlugin#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_set_static/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_set_static`
 
-Refer to the Terraform Registry for docs: [`boundary_host_set_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static).
+Refer to the Terraform Registry for docs: [`boundary_host_set_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostSetStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostSetStatic.HostSetStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static boundary_host_set_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static boundary_host_set_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static boundary_host_set_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static boundary_host_set_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#description HostSetStatic#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#name HostSetStatic#name}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#type HostSetStatic#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#description HostSetStatic#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#name HostSetStatic#name}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#type HostSetStatic#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostSetStatic resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostSetStatic to import.
-        :param import_from_id: The id of the existing HostSetStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostSetStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostSetStatic to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1c01207c66c23a76c83fb9d4e62e9fde4065a37edce7781120fd828d42649cc6)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -267,19 +270,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
-        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#description HostSetStatic#description}
-        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
-        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#name HostSetStatic#name}
-        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#type HostSetStatic#type}
+        :param host_catalog_id: The catalog for the host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
+        :param description: The host set description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#description HostSetStatic#description}
+        :param host_ids: The list of host IDs contained in this set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
+        :param name: The host set name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#name HostSetStatic#name}
+        :param type: The type of host set. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#type HostSetStatic#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5e378da7fa60e1ab50df3e685f2e8b19f77831f1ea60d61b9137fa43f412a047)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -383,52 +386,52 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
         '''The catalog for the host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#host_catalog_id HostSetStatic#host_catalog_id}
         '''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host set description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#description HostSetStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#description HostSetStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def host_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''The list of host IDs contained in this set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#host_ids HostSetStatic#host_ids}
         '''
         result = self._values.get("host_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host set name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#name HostSetStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#name HostSetStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of host set.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_set_static#type HostSetStatic#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_set_static#type HostSetStatic#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/host_static/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/host_static/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_host_static`
 
-Refer to the Terraform Registry for docs: [`boundary_host_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static).
+Refer to the Terraform Registry for docs: [`boundary_host_static`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class HostStatic(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.hostStatic.HostStatic",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static boundary_host_static}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static boundary_host_static}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         host_catalog_id: builtins.str,
@@ -42,23 +45,23 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static boundary_host_static} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static boundary_host_static} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#address HostStatic#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#description HostStatic#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#name HostStatic#name}
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#type HostStatic#type}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#address HostStatic#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#description HostStatic#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#name HostStatic#name}
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#type HostStatic#type}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a HostStatic resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the HostStatic to import.
-        :param import_from_id: The id of the existing HostStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing HostStatic that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the HostStatic to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bee2de0fc55f652fc37d20d83ce9d67cffa512c051a2cf443ca38f08fceb6def)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -267,19 +270,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
-        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#address HostStatic#address}
-        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#description HostStatic#description}
-        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#name HostStatic#name}
-        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#type HostStatic#type}
+        :param host_catalog_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.
+        :param address: The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#address HostStatic#address}
+        :param description: The host description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#description HostStatic#description}
+        :param name: The host name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#name HostStatic#name}
+        :param type: The type of host. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#type HostStatic#type}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__eeda198263353c7d24b1fe17ba6fe23a0aa061206aff004195ac1d8a9bc85ecb)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -381,51 +384,51 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def host_catalog_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#host_catalog_id HostStatic#host_catalog_id}.'''
         result = self._values.get("host_catalog_id")
         assert result is not None, "Required property 'host_catalog_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address(self) -> typing.Optional[builtins.str]:
         '''The static address of the host resource as ``<IP>`` (note: port assignment occurs in the target resource definition, do not add :port here) or a domain name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#address HostStatic#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#address HostStatic#address}
         '''
         result = self._values.get("address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The host description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#description HostStatic#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#description HostStatic#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The host name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#name HostStatic#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#name HostStatic#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def type(self) -> typing.Optional[builtins.str]:
         '''The type of host.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/host_static#type HostStatic#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/host_static#type HostStatic#type}
         '''
         result = self._values.get("type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/managed_group/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_managed_group`
 
-Refer to the Terraform Registry for docs: [`boundary_managed_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group).
+Refer to the Terraform Registry for docs: [`boundary_managed_group`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class ManagedGroup(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.managedGroup.ManagedGroup",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group boundary_managed_group}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group boundary_managed_group}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group boundary_managed_group} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group boundary_managed_group} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
-        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#filter ManagedGroup#filter}
-        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#description ManagedGroup#description}
-        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#name ManagedGroup#name}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
+        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#filter ManagedGroup#filter}
+        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#description ManagedGroup#description}
+        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#name ManagedGroup#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a ManagedGroup resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the ManagedGroup to import.
-        :param import_from_id: The id of the existing ManagedGroup that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing ManagedGroup that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the ManagedGroup to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d12c41523f6e6de30ade168140bed99978638b8d99421dc85f0cc084210076e3)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -237,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
-        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#filter ManagedGroup#filter}
-        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#description ManagedGroup#description}
-        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#name ManagedGroup#name}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
+        :param filter: Boolean expression to filter the workers for this managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#filter ManagedGroup#filter}
+        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#description ManagedGroup#description}
+        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#name ManagedGroup#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__08f9b5aef6a5e8658e96841aaa7e0bc8f0561fd9010c936a6943512913fd8fcc)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,44 +351,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#auth_method_id ManagedGroup#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def filter(self) -> builtins.str:
         '''Boolean expression to filter the workers for this managed group.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#filter ManagedGroup#filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#filter ManagedGroup#filter}
         '''
         result = self._values.get("filter")
         assert result is not None, "Required property 'filter' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The managed group description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#description ManagedGroup#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#description ManagedGroup#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The managed group name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group#name ManagedGroup#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group#name ManagedGroup#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/managed_group_ldap/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/managed_group_ldap/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_managed_group_ldap`
 
-Refer to the Terraform Registry for docs: [`boundary_managed_group_ldap`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap).
+Refer to the Terraform Registry for docs: [`boundary_managed_group_ldap`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class ManagedGroupLdap(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.managedGroupLdap.ManagedGroupLdap",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap boundary_managed_group_ldap}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap boundary_managed_group_ldap}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auth_method_id: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap boundary_managed_group_ldap} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap boundary_managed_group_ldap} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#auth_method_id ManagedGroupLdap#auth_method_id}
-        :param group_names: The list of groups that make up the managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#group_names ManagedGroupLdap#group_names}
-        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#description ManagedGroupLdap#description}
-        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#name ManagedGroupLdap#name}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#auth_method_id ManagedGroupLdap#auth_method_id}
+        :param group_names: The list of groups that make up the managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#group_names ManagedGroupLdap#group_names}
+        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#description ManagedGroupLdap#description}
+        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#name ManagedGroupLdap#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a ManagedGroupLdap resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the ManagedGroupLdap to import.
-        :param import_from_id: The id of the existing ManagedGroupLdap that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing ManagedGroupLdap that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the ManagedGroupLdap to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e95915e83523438f0e97f04c3759a4f6c221f9d7485f5615f00ba2c5d093e226)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -237,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#auth_method_id ManagedGroupLdap#auth_method_id}
-        :param group_names: The list of groups that make up the managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#group_names ManagedGroupLdap#group_names}
-        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#description ManagedGroupLdap#description}
-        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#name ManagedGroupLdap#name}
+        :param auth_method_id: The resource ID for the auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#auth_method_id ManagedGroupLdap#auth_method_id}
+        :param group_names: The list of groups that make up the managed group. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#group_names ManagedGroupLdap#group_names}
+        :param description: The managed group description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#description ManagedGroupLdap#description}
+        :param name: The managed group name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#name ManagedGroupLdap#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__38ff0e52598734bc5e511851e69ffde32a5b98fa90103af9369298af1dfacaad)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -348,44 +351,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auth_method_id(self) -> builtins.str:
         '''The resource ID for the auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#auth_method_id ManagedGroupLdap#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#auth_method_id ManagedGroupLdap#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         assert result is not None, "Required property 'auth_method_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def group_names(self) -> typing.List[builtins.str]:
         '''The list of groups that make up the managed group.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#group_names ManagedGroupLdap#group_names}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#group_names ManagedGroupLdap#group_names}
         '''
         result = self._values.get("group_names")
         assert result is not None, "Required property 'group_names' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The managed group description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#description ManagedGroupLdap#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#description ManagedGroupLdap#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The managed group name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/managed_group_ldap#name ManagedGroupLdap#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/managed_group_ldap#name ManagedGroupLdap#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/policy_storage/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/policy_storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_policy_storage`
 
-Refer to the Terraform Registry for docs: [`boundary_policy_storage`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage).
+Refer to the Terraform Registry for docs: [`boundary_policy_storage`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class PolicyStorage(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.policyStorage.PolicyStorage",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage boundary_policy_storage}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage boundary_policy_storage}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -44,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage boundary_policy_storage} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage boundary_policy_storage} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#scope_id PolicyStorage#scope_id}
-        :param delete_after_days: The number of days after which a session recording will be automatically deleted. Defaults to 0: never automatically delete. However, delete_after_days and retain_for_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#delete_after_days PolicyStorage#delete_after_days}
-        :param delete_after_overridable: Whether or not the associated delete_after_days value can be overridden by org scopes. Note: if the associated delete_after_days value is 0, overridable is ignored Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#delete_after_overridable PolicyStorage#delete_after_overridable}
-        :param description: The policy description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#description PolicyStorage#description}
-        :param name: The policy name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#name PolicyStorage#name}
-        :param retain_for_days: The number of days a session recording is required to be stored. Defaults to 0: allow deletions at any time. However, retain_for_days and delete_after_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#retain_for_days PolicyStorage#retain_for_days}
-        :param retain_for_overridable: Whether or not the associated retain_for_days value can be overridden by org scopes. Note: if the associated retain_for_days value is 0, overridable is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#retain_for_overridable PolicyStorage#retain_for_overridable}
+        :param scope_id: The scope for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#scope_id PolicyStorage#scope_id}
+        :param delete_after_days: The number of days after which a session recording will be automatically deleted. Defaults to 0: never automatically delete. However, delete_after_days and retain_for_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#delete_after_days PolicyStorage#delete_after_days}
+        :param delete_after_overridable: Whether or not the associated delete_after_days value can be overridden by org scopes. Note: if the associated delete_after_days value is 0, overridable is ignored Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#delete_after_overridable PolicyStorage#delete_after_overridable}
+        :param description: The policy description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#description PolicyStorage#description}
+        :param name: The policy name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#name PolicyStorage#name}
+        :param retain_for_days: The number of days a session recording is required to be stored. Defaults to 0: allow deletions at any time. However, retain_for_days and delete_after_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#retain_for_days PolicyStorage#retain_for_days}
+        :param retain_for_overridable: Whether or not the associated retain_for_days value can be overridden by org scopes. Note: if the associated retain_for_days value is 0, overridable is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#retain_for_overridable PolicyStorage#retain_for_overridable}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a PolicyStorage resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the PolicyStorage to import.
-        :param import_from_id: The id of the existing PolicyStorage that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing PolicyStorage that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the PolicyStorage to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__71c75bf8f3147c7fb5aa36d7e82817096180aeaa7b44abe9fcb2252525ce97ff)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -333,21 +336,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#scope_id PolicyStorage#scope_id}
-        :param delete_after_days: The number of days after which a session recording will be automatically deleted. Defaults to 0: never automatically delete. However, delete_after_days and retain_for_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#delete_after_days PolicyStorage#delete_after_days}
-        :param delete_after_overridable: Whether or not the associated delete_after_days value can be overridden by org scopes. Note: if the associated delete_after_days value is 0, overridable is ignored Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#delete_after_overridable PolicyStorage#delete_after_overridable}
-        :param description: The policy description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#description PolicyStorage#description}
-        :param name: The policy name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#name PolicyStorage#name}
-        :param retain_for_days: The number of days a session recording is required to be stored. Defaults to 0: allow deletions at any time. However, retain_for_days and delete_after_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#retain_for_days PolicyStorage#retain_for_days}
-        :param retain_for_overridable: Whether or not the associated retain_for_days value can be overridden by org scopes. Note: if the associated retain_for_days value is 0, overridable is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#retain_for_overridable PolicyStorage#retain_for_overridable}
+        :param scope_id: The scope for this policy. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#scope_id PolicyStorage#scope_id}
+        :param delete_after_days: The number of days after which a session recording will be automatically deleted. Defaults to 0: never automatically delete. However, delete_after_days and retain_for_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#delete_after_days PolicyStorage#delete_after_days}
+        :param delete_after_overridable: Whether or not the associated delete_after_days value can be overridden by org scopes. Note: if the associated delete_after_days value is 0, overridable is ignored Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#delete_after_overridable PolicyStorage#delete_after_overridable}
+        :param description: The policy description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#description PolicyStorage#description}
+        :param name: The policy name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#name PolicyStorage#name}
+        :param retain_for_days: The number of days a session recording is required to be stored. Defaults to 0: allow deletions at any time. However, retain_for_days and delete_after_days cannot both be 0. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#retain_for_days PolicyStorage#retain_for_days}
+        :param retain_for_overridable: Whether or not the associated retain_for_days value can be overridden by org scopes. Note: if the associated retain_for_days value is 0, overridable is ignored. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#retain_for_overridable PolicyStorage#retain_for_overridable}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__519301c29b552d4e0821e56bbdacfda01b364f1414a77b8290d03dc707029bc0)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -457,82 +460,82 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope for this policy.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#scope_id PolicyStorage#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#scope_id PolicyStorage#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def delete_after_days(self) -> typing.Optional[jsii.Number]:
         '''The number of days after which a session recording will be automatically deleted.
 
         Defaults to 0: never automatically delete. However, delete_after_days and retain_for_days cannot both be 0.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#delete_after_days PolicyStorage#delete_after_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#delete_after_days PolicyStorage#delete_after_days}
         '''
         result = self._values.get("delete_after_days")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def delete_after_overridable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not the associated delete_after_days value can be overridden by org scopes.
 
         Note: if the associated delete_after_days value is 0, overridable is ignored
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#delete_after_overridable PolicyStorage#delete_after_overridable}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#delete_after_overridable PolicyStorage#delete_after_overridable}
         '''
         result = self._values.get("delete_after_overridable")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The policy description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#description PolicyStorage#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#description PolicyStorage#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The policy name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#name PolicyStorage#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#name PolicyStorage#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def retain_for_days(self) -> typing.Optional[jsii.Number]:
         '''The number of days a session recording is required to be stored.
 
         Defaults to 0: allow deletions at any time. However, retain_for_days and delete_after_days cannot both be 0.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#retain_for_days PolicyStorage#retain_for_days}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#retain_for_days PolicyStorage#retain_for_days}
         '''
         result = self._values.get("retain_for_days")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def retain_for_overridable(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Whether or not the associated retain_for_days value can be overridden by org scopes.
 
         Note: if the associated retain_for_days value is 0, overridable is ignored.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/policy_storage#retain_for_overridable PolicyStorage#retain_for_overridable}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/policy_storage#retain_for_overridable PolicyStorage#retain_for_overridable}
         '''
         result = self._values.get("retain_for_overridable")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/provider/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/provider/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `provider`
 
-Refer to the Terraform Registry for docs: [`boundary`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs).
+Refer to the Terraform Registry for docs: [`boundary`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class BoundaryProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.provider.BoundaryProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs boundary}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs boundary}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         addr: builtins.str,
@@ -42,30 +45,30 @@
         password_auth_method_password: typing.Optional[builtins.str] = None,
         plugin_execution_dir: typing.Optional[builtins.str] = None,
         recovery_kms_hcl: typing.Optional[builtins.str] = None,
         scope_id: typing.Optional[builtins.str] = None,
         tls_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs boundary} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs boundary} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#addr BoundaryProvider#addr}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#alias BoundaryProvider#alias}
-        :param auth_method_id: The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_id BoundaryProvider#auth_method_id}
-        :param auth_method_login_name: The auth method login name for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
-        :param auth_method_password: The auth method password for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_password BoundaryProvider#auth_method_password}
-        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
-        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
-        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
-        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
-        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#scope_id BoundaryProvider#scope_id}
-        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#tls_insecure BoundaryProvider#tls_insecure}
-        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#token BoundaryProvider#token}
+        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#addr BoundaryProvider#addr}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#alias BoundaryProvider#alias}
+        :param auth_method_id: The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_id BoundaryProvider#auth_method_id}
+        :param auth_method_login_name: The auth method login name for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
+        :param auth_method_password: The auth method password for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_password BoundaryProvider#auth_method_password}
+        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
+        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
+        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
+        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
+        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#scope_id BoundaryProvider#scope_id}
+        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#tls_insecure BoundaryProvider#tls_insecure}
+        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#token BoundaryProvider#token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ce45866643ede5c3f23dda6c62ba4515b4bf12276ac23bc01292aac21f883d15)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = BoundaryProviderConfig(
             addr=addr,
@@ -93,15 +96,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a BoundaryProvider resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the BoundaryProvider to import.
-        :param import_from_id: The id of the existing BoundaryProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing BoundaryProvider that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the BoundaryProvider to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cc778755ea1ae165d642a9c02e4af74bc984663a807c91b55f9c54706b655068)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -415,26 +418,26 @@
         plugin_execution_dir: typing.Optional[builtins.str] = None,
         recovery_kms_hcl: typing.Optional[builtins.str] = None,
         scope_id: typing.Optional[builtins.str] = None,
         tls_insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#addr BoundaryProvider#addr}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#alias BoundaryProvider#alias}
-        :param auth_method_id: The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_id BoundaryProvider#auth_method_id}
-        :param auth_method_login_name: The auth method login name for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
-        :param auth_method_password: The auth method password for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_password BoundaryProvider#auth_method_password}
-        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
-        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
-        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
-        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
-        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#scope_id BoundaryProvider#scope_id}
-        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#tls_insecure BoundaryProvider#tls_insecure}
-        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#token BoundaryProvider#token}
+        :param addr: The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#addr BoundaryProvider#addr}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#alias BoundaryProvider#alias}
+        :param auth_method_id: The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_id BoundaryProvider#auth_method_id}
+        :param auth_method_login_name: The auth method login name for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
+        :param auth_method_password: The auth method password for password-style or ldap-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_password BoundaryProvider#auth_method_password}
+        :param password_auth_method_login_name: The auth method login name for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
+        :param password_auth_method_password: The auth method password for password-style auth methods. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
+        :param plugin_execution_dir: Specifies a directory that the Boundary provider can use to write and execute its built-in plugins. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
+        :param recovery_kms_hcl: Can be a heredoc string or a path on disk. If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
+        :param scope_id: The scope ID for the default auth method. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#scope_id BoundaryProvider#scope_id}
+        :param tls_insecure: When set to true, does not validate the Boundary API endpoint certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#tls_insecure BoundaryProvider#tls_insecure}
+        :param token: The Boundary token to use, as a string or path on disk containing just the string. If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#token BoundaryProvider#token}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1eb8f2baf8fdc05f14b99407eb26d4ce7c1d5cfdffa21ca1c28275218ffd85f4)
             check_type(argname="argument addr", value=addr, expected_type=type_hints["addr"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument auth_method_id", value=auth_method_id, expected_type=type_hints["auth_method_id"])
             check_type(argname="argument auth_method_login_name", value=auth_method_login_name, expected_type=type_hints["auth_method_login_name"])
@@ -472,121 +475,121 @@
         if token is not None:
             self._values["token"] = token
 
     @builtins.property
     def addr(self) -> builtins.str:
         '''The base url of the Boundary API, e.g. "http://127.0.0.1:9200". If not set, it will be read from the "BOUNDARY_ADDR" env var.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#addr BoundaryProvider#addr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#addr BoundaryProvider#addr}
         '''
         result = self._values.get("addr")
         assert result is not None, "Required property 'addr' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#alias BoundaryProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#alias BoundaryProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def auth_method_id(self) -> typing.Optional[builtins.str]:
         '''The auth method ID e.g. ampw_1234567890. If not set, the default auth method for the given scope ID will be used.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_id BoundaryProvider#auth_method_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_id BoundaryProvider#auth_method_id}
         '''
         result = self._values.get("auth_method_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def auth_method_login_name(self) -> typing.Optional[builtins.str]:
         '''The auth method login name for password-style or ldap-style auth methods.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_login_name BoundaryProvider#auth_method_login_name}
         '''
         result = self._values.get("auth_method_login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def auth_method_password(self) -> typing.Optional[builtins.str]:
         '''The auth method password for password-style or ldap-style auth methods.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#auth_method_password BoundaryProvider#auth_method_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#auth_method_password BoundaryProvider#auth_method_password}
         '''
         result = self._values.get("auth_method_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password_auth_method_login_name(self) -> typing.Optional[builtins.str]:
         '''The auth method login name for password-style auth methods.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#password_auth_method_login_name BoundaryProvider#password_auth_method_login_name}
         '''
         result = self._values.get("password_auth_method_login_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def password_auth_method_password(self) -> typing.Optional[builtins.str]:
         '''The auth method password for password-style auth methods.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#password_auth_method_password BoundaryProvider#password_auth_method_password}
         '''
         result = self._values.get("password_auth_method_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_execution_dir(self) -> typing.Optional[builtins.str]:
         '''Specifies a directory that the Boundary provider can use to write and execute its built-in plugins.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#plugin_execution_dir BoundaryProvider#plugin_execution_dir}
         '''
         result = self._values.get("plugin_execution_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def recovery_kms_hcl(self) -> typing.Optional[builtins.str]:
         '''Can be a heredoc string or a path on disk.
 
         If set, the string/file will be parsed as HCL and used with the recovery KMS mechanism. While this is set, it will override any other authentication information; the KMS mechanism will always be used. See Boundary's KMS docs for examples: https://boundaryproject.io/docs/configuration/kms
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#recovery_kms_hcl BoundaryProvider#recovery_kms_hcl}
         '''
         result = self._values.get("recovery_kms_hcl")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope ID for the default auth method.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#scope_id BoundaryProvider#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#scope_id BoundaryProvider#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tls_insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''When set to true, does not validate the Boundary API endpoint certificate.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#tls_insecure BoundaryProvider#tls_insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#tls_insecure BoundaryProvider#tls_insecure}
         '''
         result = self._values.get("tls_insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''The Boundary token to use, as a string or path on disk containing just the string.
 
         If set, the token read here will be used in place of authenticating with the auth method specified in "auth_method_id", although the recovery KMS mechanism will still override this. Can also be set with the BOUNDARY_TOKEN environment variable.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs#token BoundaryProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs#token BoundaryProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/role/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/role/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_role`
 
-Refer to the Terraform Registry for docs: [`boundary_role`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role).
+Refer to the Terraform Registry for docs: [`boundary_role`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Role(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.role.Role",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role boundary_role}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role boundary_role}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -44,25 +47,25 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role boundary_role} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role boundary_role} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#scope_id Role#scope_id}
-        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#description Role#description}
-        :param grant_scope_id: For Boundary 0.15+, use ``grant_scope_ids`` instead. The scope for which the grants in the role should apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_scope_id Role#grant_scope_id}
-        :param grant_scope_ids: A list of scopes for which the grants in this role should apply, which can include the special values "this", "children", or "descendants". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_scope_ids Role#grant_scope_ids}
-        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_strings Role#grant_strings}
-        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#name Role#name}
-        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#principal_ids Role#principal_ids}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#scope_id Role#scope_id}
+        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#description Role#description}
+        :param grant_scope_id: For Boundary 0.15+, use ``grant_scope_ids`` instead. The scope for which the grants in the role should apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_scope_id Role#grant_scope_id}
+        :param grant_scope_ids: A list of scopes for which the grants in this role should apply, which can include the special values "this", "children", or "descendants". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_scope_ids Role#grant_scope_ids}
+        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_strings Role#grant_strings}
+        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#name Role#name}
+        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#principal_ids Role#principal_ids}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -99,15 +102,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Role resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Role to import.
-        :param import_from_id: The id of the existing Role that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Role that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Role to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b5c683e68dbd71e31d5596c636eae54ebc34bd93cb94c5d1ec99e11da96c3544)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -319,21 +322,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#scope_id Role#scope_id}
-        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#description Role#description}
-        :param grant_scope_id: For Boundary 0.15+, use ``grant_scope_ids`` instead. The scope for which the grants in the role should apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_scope_id Role#grant_scope_id}
-        :param grant_scope_ids: A list of scopes for which the grants in this role should apply, which can include the special values "this", "children", or "descendants". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_scope_ids Role#grant_scope_ids}
-        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_strings Role#grant_strings}
-        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#name Role#name}
-        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#principal_ids Role#principal_ids}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#scope_id Role#scope_id}
+        :param description: The role description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#description Role#description}
+        :param grant_scope_id: For Boundary 0.15+, use ``grant_scope_ids`` instead. The scope for which the grants in the role should apply. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_scope_id Role#grant_scope_id}
+        :param grant_scope_ids: A list of scopes for which the grants in this role should apply, which can include the special values "this", "children", or "descendants". Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_scope_ids Role#grant_scope_ids}
+        :param grant_strings: A list of stringified grants for the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_strings Role#grant_strings}
+        :param name: The role name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#name Role#name}
+        :param principal_ids: A list of principal (user or group) IDs to add as principals on the role. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#principal_ids Role#principal_ids}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a0d9a550fe5793affacbae0f009d3344df6182595218cea1c9b59021276c36f2)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -443,70 +446,70 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#scope_id Role#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#scope_id Role#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The role description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#description Role#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#description Role#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grant_scope_id(self) -> typing.Optional[builtins.str]:
         '''For Boundary 0.15+, use ``grant_scope_ids`` instead. The scope for which the grants in the role should apply.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_scope_id Role#grant_scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_scope_id Role#grant_scope_id}
         '''
         result = self._values.get("grant_scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def grant_scope_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of scopes for which the grants in this role should apply, which can include the special values "this", "children", or "descendants".
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_scope_ids Role#grant_scope_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_scope_ids Role#grant_scope_ids}
         '''
         result = self._values.get("grant_scope_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def grant_strings(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of stringified grants for the role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#grant_strings Role#grant_strings}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#grant_strings Role#grant_strings}
         '''
         result = self._values.get("grant_strings")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The role name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#name Role#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#name Role#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def principal_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of principal (user or group) IDs to add as principals on the role.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/role#principal_ids Role#principal_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/role#principal_ids Role#principal_ids}
         '''
         result = self._values.get("principal_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/scope/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/scope/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_scope`
 
-Refer to the Terraform Registry for docs: [`boundary_scope`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope).
+Refer to the Terraform Registry for docs: [`boundary_scope`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Scope(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.scope.Scope",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope boundary_scope}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope boundary_scope}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -43,24 +46,24 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope boundary_scope} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope boundary_scope} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#scope_id Scope#scope_id}
-        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
-        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
-        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#description Scope#description}
-        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#global_scope Scope#global_scope}
-        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#name Scope#name}
+        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#scope_id Scope#scope_id}
+        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
+        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
+        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#description Scope#description}
+        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#global_scope Scope#global_scope}
+        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#name Scope#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -96,15 +99,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Scope resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Scope to import.
-        :param import_from_id: The id of the existing Scope that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Scope that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Scope to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5eca9561e580a7f605f91ccd275d530deaf312d4289825953c195adf1f22dcdc)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -312,20 +315,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#scope_id Scope#scope_id}
-        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
-        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
-        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#description Scope#description}
-        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#global_scope Scope#global_scope}
-        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#name Scope#name}
+        :param scope_id: The scope ID containing the sub scope resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#scope_id Scope#scope_id}
+        :param auto_create_admin_role: If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
+        :param auto_create_default_role: Only relevant when creating an org scope. If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
+        :param description: The scope description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#description Scope#description}
+        :param global_scope: Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#global_scope Scope#global_scope}
+        :param name: The scope name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#name Scope#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e623dbf4353f12f9cc9aff6267dbb8619be6780c3fa9407450c3f5986ce9a4c6)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -432,71 +435,71 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID containing the sub scope resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#scope_id Scope#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#scope_id Scope#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def auto_create_admin_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives permissions to manage the scope to the provider's user.
 
         Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#auto_create_admin_role Scope#auto_create_admin_role}
         '''
         result = self._values.get("auto_create_admin_role")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def auto_create_default_role(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Only relevant when creating an org scope.
 
         If set, when a new scope is created, the provider will not disable the functionality that automatically creates a role in the new scope and gives listing of scopes and auth methods and the ability to authenticate to the anonymous user. Marking this true makes for simpler HCL but results in role resources that are unmanaged by Terraform.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#auto_create_default_role Scope#auto_create_default_role}
         '''
         result = self._values.get("auto_create_default_role")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The scope description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#description Scope#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#description Scope#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def global_scope(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Indicates that the scope containing this value is the global scope, which triggers some specialized behavior to allow it to be imported and managed.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#global_scope Scope#global_scope}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#global_scope Scope#global_scope}
         '''
         result = self._values.get("global_scope")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The scope name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope#name Scope#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope#name Scope#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/scope_policy_attachment/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/scope_policy_attachment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_scope_policy_attachment`
 
-Refer to the Terraform Registry for docs: [`boundary_scope_policy_attachment`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment).
+Refer to the Terraform Registry for docs: [`boundary_scope_policy_attachment`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class ScopePolicyAttachment(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.scopePolicyAttachment.ScopePolicyAttachment",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment boundary_scope_policy_attachment}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment boundary_scope_policy_attachment}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         policy_id: builtins.str,
@@ -40,21 +43,21 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment boundary_scope_policy_attachment} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment boundary_scope_policy_attachment} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param policy_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#policy_id ScopePolicyAttachment#policy_id}.
-        :param scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#scope_id ScopePolicyAttachment#scope_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#id ScopePolicyAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#policy_id ScopePolicyAttachment#policy_id}.
+        :param scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#scope_id ScopePolicyAttachment#scope_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#id ScopePolicyAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -87,15 +90,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a ScopePolicyAttachment resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the ScopePolicyAttachment to import.
-        :param import_from_id: The id of the existing ScopePolicyAttachment that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing ScopePolicyAttachment that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the ScopePolicyAttachment to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__1e7bbfa6ca8ada0566dda02ed3185554f8c9f8e27a238ee203480ba2f1e10fcb)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -206,17 +209,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param policy_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#policy_id ScopePolicyAttachment#policy_id}.
-        :param scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#scope_id ScopePolicyAttachment#scope_id}.
-        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#id ScopePolicyAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param policy_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#policy_id ScopePolicyAttachment#policy_id}.
+        :param scope_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#scope_id ScopePolicyAttachment#scope_id}.
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#id ScopePolicyAttachment#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f3ac9d0881c6cb3b925967140322d338c30fbcfb7db2f8cbdcc45936ed1e7b92)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -311,29 +314,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def policy_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#policy_id ScopePolicyAttachment#policy_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#policy_id ScopePolicyAttachment#policy_id}.'''
         result = self._values.get("policy_id")
         assert result is not None, "Required property 'policy_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#scope_id ScopePolicyAttachment#scope_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#scope_id ScopePolicyAttachment#scope_id}.'''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/scope_policy_attachment#id ScopePolicyAttachment#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/scope_policy_attachment#id ScopePolicyAttachment#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/storage_bucket/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/storage_bucket/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_storage_bucket`
 
-Refer to the Terraform Registry for docs: [`boundary_storage_bucket`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket).
+Refer to the Terraform Registry for docs: [`boundary_storage_bucket`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class StorageBucket(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.storageBucket.StorageBucket",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket boundary_storage_bucket}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket boundary_storage_bucket}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         bucket_name: builtins.str,
@@ -47,28 +50,28 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket boundary_storage_bucket} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket boundary_storage_bucket} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param bucket_name: The name of the bucket within the external object store service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#bucket_name StorageBucket#bucket_name}
-        :param scope_id: The scope for this storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#scope_id StorageBucket#scope_id}
-        :param worker_filter: Filters to the worker(s) that can handle requests for this storage bucket. The filter must match an existing worker in order to create a storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#worker_filter StorageBucket#worker_filter}
-        :param attributes_json: The attributes for the storage bucket. The "region" attribute field is required when creating an AWS storage bucket. Values are either encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#attributes_json StorageBucket#attributes_json}
-        :param bucket_prefix: The prefix used to organize the data held within the external object store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#bucket_prefix StorageBucket#bucket_prefix}
-        :param description: The storage bucket description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#description StorageBucket#description}
-        :param name: The storage bucket name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#name StorageBucket#name}
-        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#plugin_id StorageBucket#plugin_id}
-        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#plugin_name StorageBucket#plugin_name}
-        :param secrets_json: The secrets for the storage bucket. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the storage bucket; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#secrets_json StorageBucket#secrets_json}
+        :param bucket_name: The name of the bucket within the external object store service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#bucket_name StorageBucket#bucket_name}
+        :param scope_id: The scope for this storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#scope_id StorageBucket#scope_id}
+        :param worker_filter: Filters to the worker(s) that can handle requests for this storage bucket. The filter must match an existing worker in order to create a storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#worker_filter StorageBucket#worker_filter}
+        :param attributes_json: The attributes for the storage bucket. The "region" attribute field is required when creating an AWS storage bucket. Values are either encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#attributes_json StorageBucket#attributes_json}
+        :param bucket_prefix: The prefix used to organize the data held within the external object store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#bucket_prefix StorageBucket#bucket_prefix}
+        :param description: The storage bucket description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#description StorageBucket#description}
+        :param name: The storage bucket name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#name StorageBucket#name}
+        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#plugin_id StorageBucket#plugin_id}
+        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#plugin_name StorageBucket#plugin_name}
+        :param secrets_json: The secrets for the storage bucket. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the storage bucket; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#secrets_json StorageBucket#secrets_json}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -108,15 +111,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a StorageBucket resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the StorageBucket to import.
-        :param import_from_id: The id of the existing StorageBucket that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing StorageBucket that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the StorageBucket to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a521dcf964a12fb144fc9fbef855bbe75f36ef4ff78e8929bcb445fd5785408e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -409,24 +412,24 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param bucket_name: The name of the bucket within the external object store service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#bucket_name StorageBucket#bucket_name}
-        :param scope_id: The scope for this storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#scope_id StorageBucket#scope_id}
-        :param worker_filter: Filters to the worker(s) that can handle requests for this storage bucket. The filter must match an existing worker in order to create a storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#worker_filter StorageBucket#worker_filter}
-        :param attributes_json: The attributes for the storage bucket. The "region" attribute field is required when creating an AWS storage bucket. Values are either encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#attributes_json StorageBucket#attributes_json}
-        :param bucket_prefix: The prefix used to organize the data held within the external object store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#bucket_prefix StorageBucket#bucket_prefix}
-        :param description: The storage bucket description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#description StorageBucket#description}
-        :param name: The storage bucket name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#name StorageBucket#name}
-        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#plugin_id StorageBucket#plugin_id}
-        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#plugin_name StorageBucket#plugin_name}
-        :param secrets_json: The secrets for the storage bucket. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the storage bucket; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#secrets_json StorageBucket#secrets_json}
+        :param bucket_name: The name of the bucket within the external object store service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#bucket_name StorageBucket#bucket_name}
+        :param scope_id: The scope for this storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#scope_id StorageBucket#scope_id}
+        :param worker_filter: Filters to the worker(s) that can handle requests for this storage bucket. The filter must match an existing worker in order to create a storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#worker_filter StorageBucket#worker_filter}
+        :param attributes_json: The attributes for the storage bucket. The "region" attribute field is required when creating an AWS storage bucket. Values are either encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the storage bucket. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#attributes_json StorageBucket#attributes_json}
+        :param bucket_prefix: The prefix used to organize the data held within the external object store. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#bucket_prefix StorageBucket#bucket_prefix}
+        :param description: The storage bucket description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#description StorageBucket#description}
+        :param name: The storage bucket name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#name StorageBucket#name}
+        :param plugin_id: The ID of the plugin that should back the resource. This or plugin_name must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#plugin_id StorageBucket#plugin_id}
+        :param plugin_name: The name of the plugin that should back the resource. This or plugin_id must be defined. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#plugin_name StorageBucket#plugin_name}
+        :param secrets_json: The secrets for the storage bucket. Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the storage bucket; this allows injecting secrets for one call, then removing them for storage. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#secrets_json StorageBucket#secrets_json}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a020f1e42b21ae062f173ab01eff0f31c45b607286cb95c086da3cb32293966f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -543,105 +546,105 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def bucket_name(self) -> builtins.str:
         '''The name of the bucket within the external object store service.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#bucket_name StorageBucket#bucket_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#bucket_name StorageBucket#bucket_name}
         '''
         result = self._values.get("bucket_name")
         assert result is not None, "Required property 'bucket_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope for this storage bucket.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#scope_id StorageBucket#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#scope_id StorageBucket#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def worker_filter(self) -> builtins.str:
         '''Filters to the worker(s) that can handle requests for this storage bucket.
 
         The filter must match an existing worker in order to create a storage bucket.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#worker_filter StorageBucket#worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#worker_filter StorageBucket#worker_filter}
         '''
         result = self._values.get("worker_filter")
         assert result is not None, "Required property 'worker_filter' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def attributes_json(self) -> typing.Optional[builtins.str]:
         '''The attributes for the storage bucket.
 
         The "region" attribute field is required when creating an AWS storage bucket. Values are either encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" or remove the block to clear all attributes in the storage bucket.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#attributes_json StorageBucket#attributes_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#attributes_json StorageBucket#attributes_json}
         '''
         result = self._values.get("attributes_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def bucket_prefix(self) -> typing.Optional[builtins.str]:
         '''The prefix used to organize the data held within the external object store.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#bucket_prefix StorageBucket#bucket_prefix}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#bucket_prefix StorageBucket#bucket_prefix}
         '''
         result = self._values.get("bucket_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The storage bucket description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#description StorageBucket#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#description StorageBucket#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The storage bucket name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#name StorageBucket#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#name StorageBucket#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_id(self) -> typing.Optional[builtins.str]:
         '''The ID of the plugin that should back the resource. This or plugin_name must be defined.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#plugin_id StorageBucket#plugin_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#plugin_id StorageBucket#plugin_id}
         '''
         result = self._values.get("plugin_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plugin_name(self) -> typing.Optional[builtins.str]:
         '''The name of the plugin that should back the resource. This or plugin_id must be defined.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#plugin_name StorageBucket#plugin_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#plugin_name StorageBucket#plugin_name}
         '''
         result = self._values.get("plugin_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def secrets_json(self) -> typing.Optional[builtins.str]:
         '''The secrets for the storage bucket.
 
         Either values encoded with the "jsonencode" function, pre-escaped JSON string, or a file:// or env:// path. Set to a string "null" to clear any existing values. NOTE: Unlike "attributes_json", removing this block will NOT clear secrets from the storage bucket; this allows injecting secrets for one call, then removing them for storage.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/storage_bucket#secrets_json StorageBucket#secrets_json}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/storage_bucket#secrets_json StorageBucket#secrets_json}
         '''
         result = self._values.get("secrets_json")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/target/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/target/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_target`
 
-Refer to the Terraform Registry for docs: [`boundary_target`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target).
+Refer to the Terraform Registry for docs: [`boundary_target`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Target(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.target.Target",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target boundary_target}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target boundary_target}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -54,35 +57,35 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target boundary_target} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target boundary_target} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#scope_id Target#scope_id}
-        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#type Target#type}
-        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#address Target#address}
-        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
-        :param default_client_port: The default client port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#default_client_port Target#default_client_port}
-        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#default_port Target#default_port}
-        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#description Target#description}
-        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
-        :param enable_session_recording: HCP/Ent Only. Enable sessions recording for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#enable_session_recording Target#enable_session_recording}
-        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#host_source_ids Target#host_source_ids}
-        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
-        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
-        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#name Target#name}
-        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#session_connection_limit Target#session_connection_limit}.
-        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#session_max_seconds Target#session_max_seconds}.
-        :param storage_bucket_id: HCP/Ent Only. Storage bucket for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#storage_bucket_id Target#storage_bucket_id}
-        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#worker_filter Target#worker_filter}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#scope_id Target#scope_id}
+        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#type Target#type}
+        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#address Target#address}
+        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
+        :param default_client_port: The default client port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#default_client_port Target#default_client_port}
+        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#default_port Target#default_port}
+        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#description Target#description}
+        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
+        :param enable_session_recording: HCP/Ent Only. Enable sessions recording for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#enable_session_recording Target#enable_session_recording}
+        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#host_source_ids Target#host_source_ids}
+        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
+        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
+        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#name Target#name}
+        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#session_connection_limit Target#session_connection_limit}.
+        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#session_max_seconds Target#session_max_seconds}.
+        :param storage_bucket_id: HCP/Ent Only. Storage bucket for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#storage_bucket_id Target#storage_bucket_id}
+        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#worker_filter Target#worker_filter}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -129,15 +132,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Target resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Target to import.
-        :param import_from_id: The id of the existing Target that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Target that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Target to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__848349402aba15585e0db3e16fd2861e09eb262ee77830ae06b98f91da57f28e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -589,31 +592,31 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#scope_id Target#scope_id}
-        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#type Target#type}
-        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#address Target#address}
-        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
-        :param default_client_port: The default client port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#default_client_port Target#default_client_port}
-        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#default_port Target#default_port}
-        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#description Target#description}
-        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
-        :param enable_session_recording: HCP/Ent Only. Enable sessions recording for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#enable_session_recording Target#enable_session_recording}
-        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#host_source_ids Target#host_source_ids}
-        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
-        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
-        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#name Target#name}
-        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#session_connection_limit Target#session_connection_limit}.
-        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#session_max_seconds Target#session_max_seconds}.
-        :param storage_bucket_id: HCP/Ent Only. Storage bucket for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#storage_bucket_id Target#storage_bucket_id}
-        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#worker_filter Target#worker_filter}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#scope_id Target#scope_id}
+        :param type: The target resource type. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#type Target#type}
+        :param address: Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#address Target#address}
+        :param brokered_credential_source_ids: A list of brokered credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
+        :param default_client_port: The default client port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#default_client_port Target#default_client_port}
+        :param default_port: The default port for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#default_port Target#default_port}
+        :param description: The target description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#description Target#description}
+        :param egress_worker_filter: Boolean expression to filter the workers used to access this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
+        :param enable_session_recording: HCP/Ent Only. Enable sessions recording for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#enable_session_recording Target#enable_session_recording}
+        :param host_source_ids: A list of host source ID's. Cannot be used alongside address. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#host_source_ids Target#host_source_ids}
+        :param ingress_worker_filter: HCP Only. Boolean expression to filter the workers a user will connect to when initiating a session against this target Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
+        :param injected_application_credential_source_ids: A list of injected application credential source ID's. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
+        :param name: The target name. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#name Target#name}
+        :param session_connection_limit: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#session_connection_limit Target#session_connection_limit}.
+        :param session_max_seconds: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#session_max_seconds Target#session_max_seconds}.
+        :param storage_bucket_id: HCP/Ent Only. Storage bucket for this target. Only applicable for SSH targets. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#storage_bucket_id Target#storage_bucket_id}
+        :param worker_filter: Boolean expression to filter the workers for this target. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#worker_filter Target#worker_filter}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b3790b32773af6299bc7839606b6164e1bada068e491dd6db09b0641a30f5e25)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -752,163 +755,163 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#scope_id Target#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#scope_id Target#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
         '''The target resource type.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#type Target#type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#type Target#type}
         '''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def address(self) -> typing.Optional[builtins.str]:
         '''Optionally, a valid network address to connect to for this target. Cannot be used alongside host_source_ids.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#address Target#address}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#address Target#address}
         '''
         result = self._values.get("address")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def brokered_credential_source_ids(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of brokered credential source ID's.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#brokered_credential_source_ids Target#brokered_credential_source_ids}
         '''
         result = self._values.get("brokered_credential_source_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def default_client_port(self) -> typing.Optional[jsii.Number]:
         '''The default client port for this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#default_client_port Target#default_client_port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#default_client_port Target#default_client_port}
         '''
         result = self._values.get("default_client_port")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def default_port(self) -> typing.Optional[jsii.Number]:
         '''The default port for this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#default_port Target#default_port}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#default_port Target#default_port}
         '''
         result = self._values.get("default_port")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The target description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#description Target#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#description Target#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def egress_worker_filter(self) -> typing.Optional[builtins.str]:
         '''Boolean expression to filter the workers used to access this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#egress_worker_filter Target#egress_worker_filter}
         '''
         result = self._values.get("egress_worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def enable_session_recording(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''HCP/Ent Only. Enable sessions recording for this target. Only applicable for SSH targets.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#enable_session_recording Target#enable_session_recording}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#enable_session_recording Target#enable_session_recording}
         '''
         result = self._values.get("enable_session_recording")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def host_source_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of host source ID's. Cannot be used alongside address.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#host_source_ids Target#host_source_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#host_source_ids Target#host_source_ids}
         '''
         result = self._values.get("host_source_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def ingress_worker_filter(self) -> typing.Optional[builtins.str]:
         '''HCP Only.
 
         Boolean expression to filter the workers a user will connect to when initiating a session against this target
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#ingress_worker_filter Target#ingress_worker_filter}
         '''
         result = self._values.get("ingress_worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def injected_application_credential_source_ids(
         self,
     ) -> typing.Optional[typing.List[builtins.str]]:
         '''A list of injected application credential source ID's.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#injected_application_credential_source_ids Target#injected_application_credential_source_ids}
         '''
         result = self._values.get("injected_application_credential_source_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The target name. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#name Target#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#name Target#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def session_connection_limit(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#session_connection_limit Target#session_connection_limit}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#session_connection_limit Target#session_connection_limit}.'''
         result = self._values.get("session_connection_limit")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def session_max_seconds(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#session_max_seconds Target#session_max_seconds}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#session_max_seconds Target#session_max_seconds}.'''
         result = self._values.get("session_max_seconds")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def storage_bucket_id(self) -> typing.Optional[builtins.str]:
         '''HCP/Ent Only. Storage bucket for this target. Only applicable for SSH targets.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#storage_bucket_id Target#storage_bucket_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#storage_bucket_id Target#storage_bucket_id}
         '''
         result = self._values.get("storage_bucket_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def worker_filter(self) -> typing.Optional[builtins.str]:
         '''Boolean expression to filter the workers for this target.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/target#worker_filter Target#worker_filter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/target#worker_filter Target#worker_filter}
         '''
         result = self._values.get("worker_filter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/user/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/user/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_user`
 
-Refer to the Terraform Registry for docs: [`boundary_user`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user).
+Refer to the Terraform Registry for docs: [`boundary_user`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class User(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.user.User",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user boundary_user}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user boundary_user}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         scope_id: builtins.str,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user boundary_user} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user boundary_user} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#scope_id User#scope_id}
-        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#account_ids User#account_ids}
-        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#description User#description}
-        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#name User#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#scope_id User#scope_id}
+        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#account_ids User#account_ids}
+        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#description User#description}
+        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#name User#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a User resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the User to import.
-        :param import_from_id: The id of the existing User that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing User that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the User to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__65fa3904df9a714b8504155c17383757207c67f39fc032928db5b6eb153cdbf9)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -241,18 +244,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#scope_id User#scope_id}
-        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#account_ids User#account_ids}
-        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#description User#description}
-        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#name User#name}
+        :param scope_id: The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#scope_id User#scope_id}
+        :param account_ids: Account ID's to associate with this user resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#account_ids User#account_ids}
+        :param description: The user description. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#description User#description}
+        :param name: The username. Defaults to the resource name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#name User#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e5abd1b3d9322f90ebf0dff710e71ef2c316c6fb92dd740ef40f6a4d5bb5f496)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -353,43 +356,43 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def scope_id(self) -> builtins.str:
         '''The scope ID in which the resource is created. Defaults to the provider's ``default_scope`` if unset.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#scope_id User#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#scope_id User#scope_id}
         '''
         result = self._values.get("scope_id")
         assert result is not None, "Required property 'scope_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def account_ids(self) -> typing.Optional[typing.List[builtins.str]]:
         '''Account ID's to associate with this user resource.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#account_ids User#account_ids}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#account_ids User#account_ids}
         '''
         result = self._values.get("account_ids")
         return typing.cast(typing.Optional[typing.List[builtins.str]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The user description.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#description User#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#description User#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The username. Defaults to the resource name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/user#name User#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/user#name User#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary/worker/__init__.py` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary/worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 '''
 # `boundary_worker`
 
-Refer to the Terraform Registry for docs: [`boundary_worker`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker).
+Refer to the Terraform Registry for docs: [`boundary_worker`](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker).
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -22,15 +25,15 @@
 
 
 class Worker(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-boundary.worker.Worker",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker boundary_worker}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker boundary_worker}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         description: typing.Optional[builtins.str] = None,
@@ -41,22 +44,22 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker boundary_worker} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker boundary_worker} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#description Worker#description}
-        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#name Worker#name}
-        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#scope_id Worker#scope_id}
-        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
+        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#description Worker#description}
+        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#name Worker#name}
+        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#scope_id Worker#scope_id}
+        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,15 +93,15 @@
         import_from_id: builtins.str,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     ) -> _cdktf_9a9027ec.ImportableResource:
         '''Generates CDKTF code for importing a Worker resource upon running "cdktf plan ".
 
         :param scope: The scope in which to define this construct.
         :param import_to_id: The construct id used in the generated config for the Worker to import.
-        :param import_from_id: The id of the existing Worker that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#import import section} in the documentation of this resource for the id to use
+        :param import_from_id: The id of the existing Worker that should be imported. Refer to the {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#import import section} in the documentation of this resource for the id to use
         :param provider: ? Optional instance of the provider where the Worker to import is found.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dc5e02070615c4f09a0d80fe8a87861c6c904ad2c3783d8bcdb49a50db9e1b95)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument import_to_id", value=import_to_id, expected_type=type_hints["import_to_id"])
             check_type(argname="argument import_from_id", value=import_from_id, expected_type=type_hints["import_from_id"])
@@ -265,18 +268,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#description Worker#description}
-        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#name Worker#name}
-        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#scope_id Worker#scope_id}
-        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
+        :param description: The description for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#description Worker#description}
+        :param name: The name for the worker. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#name Worker#name}
+        :param scope_id: The scope for the worker. Defaults to ``global``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#scope_id Worker#scope_id}
+        :param worker_generated_auth_token: The worker authentication token required to register the worker for the worker-led authentication flow. Leaving this blank will result in a controller generated token. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__87814f62730dab1883e5e4cb04d8df44dd248528f40ec027645b1ad9f9de86b1)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -377,44 +380,44 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''The description for the worker.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#description Worker#description}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#description Worker#description}
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def name(self) -> typing.Optional[builtins.str]:
         '''The name for the worker.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#name Worker#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#name Worker#name}
         '''
         result = self._values.get("name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def scope_id(self) -> typing.Optional[builtins.str]:
         '''The scope for the worker. Defaults to ``global``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#scope_id Worker#scope_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#scope_id Worker#scope_id}
         '''
         result = self._values.get("scope_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def worker_generated_auth_token(self) -> typing.Optional[builtins.str]:
         '''The worker authentication token required to register the worker for the worker-led authentication flow.
 
         Leaving this blank will result in a controller generated token.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs/resources/worker#worker_generated_auth_token Worker#worker_generated_auth_token}
         '''
         result = self._values.get("worker_generated_auth_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-boundary
-Version: 9.0.2
+Version: 9.0.3
 Summary: Prebuilt boundary Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-boundary.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-boundary.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -17,17 +17,17 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.14
+# CDKTF prebuilt bindings for hashicorp/boundary provider version 1.1.15
 
-This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14/docs) bindings for [CDK for Terraform](https://cdk.tf).
+This repo builds and publishes the [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15/docs) bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
 The npm package is available at [https://www.npmjs.com/package/@cdktf/provider-boundary](https://www.npmjs.com/package/@cdktf/provider-boundary).
 
@@ -81,15 +81,15 @@
 ## Versioning
 
 This project is explicitly not tracking the Terraform boundary provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by [generating the provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [CDK for Terraform](https://cdk.tf)
-* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.14)
+* [Terraform boundary provider](https://registry.terraform.io/providers/hashicorp/boundary/1.1.15)
 * [Terraform Engine](https://terraform.io)
 
 If there are breaking changes (backward incompatible) in any of the above, the major version of this project will be bumped.
 
 ## Features / Issues / Bugs
 
 Please report bugs and issues to the [CDK for Terraform](https://cdk.tf) project:
```

### Comparing `cdktf-cdktf-provider-boundary-9.0.2/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-boundary-9.0.3/src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 src/cdktf_cdktf_provider_boundary/py.typed
 src/cdktf_cdktf_provider_boundary.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_boundary.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_boundary.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_boundary.egg-info/requires.txt
 src/cdktf_cdktf_provider_boundary.egg-info/top_level.txt
 src/cdktf_cdktf_provider_boundary/_jsii/__init__.py
-src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@9.0.2.jsii.tgz
+src/cdktf_cdktf_provider_boundary/_jsii/provider-boundary@9.0.3.jsii.tgz
 src/cdktf_cdktf_provider_boundary/account/__init__.py
 src/cdktf_cdktf_provider_boundary/account_ldap/__init__.py
 src/cdktf_cdktf_provider_boundary/account_oidc/__init__.py
 src/cdktf_cdktf_provider_boundary/account_password/__init__.py
+src/cdktf_cdktf_provider_boundary/alias_target/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method_ldap/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method_oidc/__init__.py
 src/cdktf_cdktf_provider_boundary/auth_method_password/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_json/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_library_vault/__init__.py
 src/cdktf_cdktf_provider_boundary/credential_library_vault_ssh_certificate/__init__.py
```

