# Comparing `tmp/odoo-configurator-3.4.6.tar.gz` & `tmp/odoo_configurator-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-configurator-3.4.6.tar", last modified: Fri Apr 12 15:14:52 2024, max compression
+gzip compressed data, was "odoo_configurator-3.4.7.tar", last modified: Thu May  2 08:25:41 2024, max compression
```

## Comparing `odoo-configurator-3.4.6.tar` & `odoo_configurator-3.4.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.374180 odoo-configurator-3.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22346 2024-04-12 15:14:52.374180 odoo-configurator-3.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/logo_scalizer.png
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:14:52.374180 odoo-configurator-3.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.362180 odoo-configurator-3.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.366180 odoo-configurator-3.4.6/src/odoo_configurator/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.370180 odoo-configurator-3.4.6/src/odoo_configurator/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7008 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/account.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5415 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/call.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2914 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      293 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12070 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/datas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14343 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/import_configurator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2238 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/imports.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1487 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/mattermost.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5425 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/modules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/roles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/system_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/translations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/users.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/apps/website.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/bitwarden.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8708 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/configurator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8695 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/import_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3495 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/keepass.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9622 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/odoo_configurator/odoo_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.374180 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22346 2024-04-12 15:14:52.000000 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-12 15:14:52.000000 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:14:52.000000 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 15:14:52.000000 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 15:14:52.000000 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 15:14:52.000000 odoo-configurator-3.4.6/src/odoo_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.374180 odoo-configurator-3.4.6/src/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/0_base.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:14:52.374180 odoo-configurator-3.4.6/src/templates/14.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/14.0/0_base.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/1_base_auto_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/1_base_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_account.yml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_account_14.yml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_account_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_crm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_expense.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_ged.yml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_hr.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_maintenance.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_marketing.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_mrp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_purchase.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_sale.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_sale_subscription.yml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_sign.yml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/src/templates/2_base_website.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-04-12 15:14:47.000000 odoo-configurator-3.4.6/start_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.648463 odoo_configurator-3.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22346 2024-05-02 08:25:41.648463 odoo_configurator-3.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/logo_scalizer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:25:41.648463 odoo_configurator-3.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.636463 odoo_configurator-3.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.640463 odoo_configurator-3.4.7/src/odoo_configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.644463 odoo_configurator-3.4.7/src/odoo_configurator/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7008 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5415 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/call.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2914 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      293 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12070 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/datas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14343 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/import_configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2238 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1487 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/mattermost.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5425 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/system_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/users.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/apps/website.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2121 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/bitwarden.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8708 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8695 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/import_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3495 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/keepass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9622 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/odoo_configurator/odoo_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.648463 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22346 2024-05-02 08:25:41.000000 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-02 08:25:41.000000 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:25:41.000000 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 08:25:41.000000 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-02 08:25:41.000000 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 08:25:41.000000 odoo_configurator-3.4.7/src/odoo_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.648463 odoo_configurator-3.4.7/src/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/0_base.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:25:41.648463 odoo_configurator-3.4.7/src/templates/14.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/14.0/0_base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/1_base_auto_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/1_base_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_account.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_account_14.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_account_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_crm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_expense.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_ged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_hr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_maintenance.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_marketing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_mrp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_purchase.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_sale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_sale_subscription.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_sign.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/src/templates/2_base_website.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-05-02 08:25:32.000000 odoo_configurator-3.4.7/start_config.py
```

### Comparing `odoo-configurator-3.4.6/LICENSE` & `odoo_configurator-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/PKG-INFO` & `odoo_configurator-3.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.4.6
+Version: 3.4.7
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `odoo-configurator-3.4.6/README.md` & `odoo_configurator-3.4.7/README.md`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/logo_scalizer.png` & `odoo_configurator-3.4.7/logo_scalizer.png`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/pyproject.toml` & `odoo_configurator-3.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "odoo-configurator"
-version = "3.4.6"
+version = "3.4.7"
 description = "Configure and update Odoo database with YAML files"
 readme = "README.md"
 authors = [{ name = "Michel Perrocheau", email = "myrrkel@gmail.com" },
 { name = "David Halgand", email = "david@scalizer.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
```

### Comparing `odoo-configurator-3.4.6/requirements.txt` & `odoo_configurator-3.4.7/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,10 +60,10 @@
     # via beautifulsoup4
 unidecode==1.3.6
     # via odoo-configurator (pyproject.toml)
 urllib3==2.0.3
     # via
     #   odoo-configurator (pyproject.toml)
     #   requests
-s6r_bitwarden_cli==1.0.5
+s6r_bitwarden_cli==1.0.6
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/__main__.py` & `odoo_configurator-3.4.7/src/odoo_configurator/__main__.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/account.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/account.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/base.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/base.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/call.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/call.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/config.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/config.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/datas.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/datas.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/defaults.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/defaults.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/import_configurator.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/import_configurator.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/imports.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/imports.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/mattermost.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/mattermost.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/modules.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/modules.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/roles.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/roles.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/system_parameter.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/system_parameter.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/translations.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/translations.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/users.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/users.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/apps/website.py` & `odoo_configurator-3.4.7/src/odoo_configurator/apps/website.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/configurator.py` & `odoo_configurator-3.4.7/src/odoo_configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/import_manager.py` & `odoo_configurator-3.4.7/src/odoo_configurator/import_manager.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/keepass.py` & `odoo_configurator-3.4.7/src/odoo_configurator/keepass.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator/odoo_connection.py` & `odoo_configurator-3.4.7/src/odoo_configurator/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator.egg-info/PKG-INFO` & `odoo_configurator-3.4.7/src/odoo_configurator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.4.6
+Version: 3.4.7
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `odoo-configurator-3.4.6/src/odoo_configurator.egg-info/SOURCES.txt` & `odoo_configurator-3.4.7/src/odoo_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/templates/1_base_auto_entreprise.yml` & `odoo_configurator-3.4.7/src/templates/1_base_auto_entreprise.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/templates/2_base_account.yml` & `odoo_configurator-3.4.7/src/templates/2_base_account.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/templates/2_base_account_14.yml` & `odoo_configurator-3.4.7/src/templates/2_base_account_14.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.6/src/templates/2_base_sale.yml` & `odoo_configurator-3.4.7/src/templates/2_base_sale.yml`

 * *Files identical despite different names*

