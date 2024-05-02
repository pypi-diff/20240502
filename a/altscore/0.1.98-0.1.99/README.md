# Comparing `tmp/altscore-0.1.98.tar.gz` & `tmp/altscore-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altscore-0.1.98.tar", last modified: Wed Apr  3 22:25:17 2024, max compression
+gzip compressed data, was "altscore-0.1.99.tar", last modified: Wed Apr  3 23:26:42 2024, max compression
```

## Comparing `altscore-0.1.98.tar` & `altscore-0.1.99.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.080859 altscore-0.1.98/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 22:25:04.000000 altscore-0.1.98/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 22:25:17.080859 altscore-0.1.98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 22:25:04.000000 altscore-0.1.98/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 22:25:17.080859 altscore-0.1.98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-03 22:25:04.000000 altscore-0.1.98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.064859 altscore-0.1.98/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/altdata/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/altdata/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/altdata/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/model/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/model/common_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/model/data_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/altdata/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/altdata/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/altdata/utils/dataframes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/borrower_central/
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.068859 altscore-0.1.98/src/altscore/borrower_central/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/borrower_central/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/automations.py
--rw-r--r--   0 runner    (1001) docker     (127)    45781 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/borrower.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/borrower_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/data_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/executions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/form_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/identities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/borrower_central/model/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/integrations/sat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/otp_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/points_of_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/policy_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/risk_ratings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/stages.py
--rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/store_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/store_secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/store_sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/model/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/borrower_central/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/borrower_central/schemas/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/schemas/evaluators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/borrower_central/schemas/executions/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/schemas/executions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/borrower_central/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/cms/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/cms/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/cms/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/credit_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/debts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/dpas.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/model/partners.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/cms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/common/http_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/macros/
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/macros/validate_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 22:25:04.000000 altscore-0.1.98/src/altscore/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 22:25:17.076859 altscore-0.1.98/src/altscore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 22:25:17.000000 altscore-0.1.98/src/altscore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 22:25:17.000000 altscore-0.1.98/src/altscore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 22:25:17.000000 altscore-0.1.98/src/altscore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 22:25:17.000000 altscore-0.1.98/src/altscore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 22:25:17.000000 altscore-0.1.98/src/altscore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.367269 altscore-0.1.99/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-03 23:26:38.000000 altscore-0.1.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 23:26:42.367269 altscore-0.1.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 23:26:38.000000 altscore-0.1.99/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:26:42.367269 altscore-0.1.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-03 23:26:38.000000 altscore-0.1.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.351269 altscore-0.1.99/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.355269 altscore-0.1.99/src/altscore/
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.355269 altscore-0.1.99/src/altscore/altdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.359269 altscore-0.1.99/src/altscore/altdata/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.359269 altscore-0.1.99/src/altscore/altdata/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13002 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/model/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/model/common_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/model/data_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.359269 altscore-0.1.99/src/altscore/altdata/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.359269 altscore-0.1.99/src/altscore/altdata/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/altdata/utils/dataframes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.359269 altscore-0.1.99/src/altscore/borrower_central/
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.359269 altscore-0.1.99/src/altscore/borrower_central/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/borrower_central/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/automations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48278 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/borrower.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/borrower_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/data_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13219 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/executions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/form_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/identities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/borrower_central/model/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/integrations/sat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/otp_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/points_of_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/policy_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/risk_ratings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/store_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/store_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/store_sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/model/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/borrower_central/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/borrower_central/schemas/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/schemas/evaluators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/borrower_central/schemas/executions/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/schemas/executions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/borrower_central/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/cms/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.363269 altscore-0.1.99/src/altscore/cms/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.367269 altscore-0.1.99/src/altscore/cms/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/credit_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9171 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/debts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11557 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/dpas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8700 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/model/partners.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/cms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.367269 altscore-0.1.99/src/altscore/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/common/http_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.367269 altscore-0.1.99/src/altscore/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/macros/validate_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.367269 altscore-0.1.99/src/altscore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 23:26:38.000000 altscore-0.1.99/src/altscore/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:26:42.367269 altscore-0.1.99/src/altscore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 23:26:42.000000 altscore-0.1.99/src/altscore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 23:26:42.000000 altscore-0.1.99/src/altscore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:26:42.000000 altscore-0.1.99/src/altscore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 23:26:42.000000 altscore-0.1.99/src/altscore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 23:26:42.000000 altscore-0.1.99/src/altscore.egg-info/top_level.txt
```

### Comparing `altscore-0.1.98/LICENSE` & `altscore-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/PKG-INFO` & `altscore-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore
-Version: 0.1.98
+Version: 0.1.99
 Summary: Python SDK for AltScore. It provides a simple interface to the AltScore API.
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore-0.1.98/setup.py` & `altscore-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 long_description = "Python SDK for AltScore"
 
 setup(
     name="altscore",
-    version="0.1.98",
+    version="0.1.99",
     description="Python SDK for AltScore. It provides a simple interface to the AltScore API.",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/altscore/altscore-python",
     author="AltScore",
```

### Comparing `altscore-0.1.98/src/altscore/__init__.py` & `altscore-0.1.99/src/altscore/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/altdata/__init__.py` & `altscore-0.1.99/src/altscore/altdata/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/altdata/model/batch.py` & `altscore-0.1.99/src/altscore/altdata/model/batch.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/altdata/model/data_request.py` & `altscore-0.1.99/src/altscore/altdata/model/data_request.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/__init__.py` & `altscore-0.1.99/src/altscore/borrower_central/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/helpers/__init__.py` & `altscore-0.1.99/src/altscore/borrower_central/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/addresses.py` & `altscore-0.1.99/src/altscore/borrower_central/model/addresses.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/attachments.py` & `altscore-0.1.99/src/altscore/borrower_central/model/attachments.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/authorizations.py` & `altscore-0.1.99/src/altscore/borrower_central/model/authorizations.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/automations.py` & `altscore-0.1.99/src/altscore/borrower_central/model/automations.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/borrower.py` & `altscore-0.1.99/src/altscore/borrower_central/model/borrower.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel, Field
-from typing import Optional, List
+from typing import Optional, List, Literal, Dict
 import httpx
 import asyncio
 
 from altscore.borrower_central.helpers import build_headers
 from altscore.borrower_central.model.identities import IdentitySync, IdentityAsync
 from altscore.borrower_central.model.documents import DocumentSync, DocumentAsync
 from altscore.borrower_central.model.addresses import AddressSync, AddressAsync
@@ -34,14 +34,32 @@
 
     class Config:
         populate_by_name = True
         allow_population_by_field_name = True
         allow_population_by_alias = True
 
 
+class BorrowerSummaryAPIDTO(BaseModel):
+    id: str = Field(alias="id")
+    persona: str = Field(alias="persona")
+    label: Optional[str] = Field(alias="label")
+    identities: Optional[List[Dict]] = Field(alias="identities", default=[])
+    points_of_contact: Optional[List[Dict]] = Field(alias="pointsOfContact", default=[])
+    tags: List[str] = Field(alias="tags", default=[])
+    stage: Optional[str] = Field(alias="stage", default=None)
+    risk_rating: Optional[str] = Field(alias="riskRating", default=None)
+    created_at: str = Field(alias="createdAt")
+    updated_at: Optional[str] = Field(alias="updatedAt")
+
+    class Config:
+        populate_by_name = True
+        allow_population_by_field_name = True
+        allow_population_by_alias = True
+
+
 class CreateBorrowerDTO(BaseModel):
     persona: str = Field(alias="persona")
     label: Optional[str] = Field(alias="label")
     tags: List[str] = Field(alias="tags", default=[])
 
     class Config:
         populate_by_name = True
@@ -324,14 +342,35 @@
             return [BorrowerAsync(
                 base_url=self.altscore_client._borrower_central_base_url,
                 header_builder=self.build_headers,
                 renew_token=self.renew_token,
                 data=BorrowerAPIDTO.parse_obj(e)
             ) for e in response.json()]
 
+    @retry_on_401_async
+    async def query_summary(self, by: Optional[Literal["self", "identity"]] = None, search: Optional[str] = None,
+                            **kwargs):
+        query_params = {
+            "by": by,
+            "search": search
+        }
+        for k, v in kwargs.items():
+            if v is not None:
+                query_params[convert_to_dash_case(k)] = v
+        query_params = clean_dict(query_params)
+        async with httpx.AsyncClient(base_url=self.altscore_client._borrower_central_base_url) as client:
+            response = await client.get(
+                f"/v1/borrowers-summary",
+                headers=self.build_headers(),
+                params=query_params,
+                timeout=30
+            )
+            raise_for_status_improved(response)
+            return [BorrowerSummaryAPIDTO.parse_obj(e) for e in response.json()]
+
 
 class BorrowersSyncModule:
 
     def __init__(self, altscore_client):
         self.altscore_client = altscore_client
 
     def renew_token(self):
@@ -437,14 +476,35 @@
             return [BorrowerSync(
                 base_url=self.altscore_client._borrower_central_base_url,
                 header_builder=self.build_headers,
                 renew_token=self.renew_token,
                 data=BorrowerAPIDTO.parse_obj(e)
             ) for e in response.json()]
 
+    @retry_on_401
+    def query_summary(self, by: Optional[Literal["self", "identity"]] = None, search: Optional[str] = None,
+                      **kwargs):
+        query_params = {
+            "by": by,
+            "search": search
+        }
+        for k, v in kwargs.items():
+            if v is not None:
+                query_params[convert_to_dash_case(k)] = v
+        query_params = clean_dict(query_params)
+        with httpx.Client(base_url=self.altscore_client._borrower_central_base_url) as client:
+            response = client.get(
+                f"/v1/borrowers-summary",
+                headers=self.build_headers(),
+                params=query_params,
+                timeout=30
+            )
+            raise_for_status_improved(response)
+            return [BorrowerSummaryAPIDTO.parse_obj(e) for e in response.json()]
+
 
 class BorrowerAsync(BorrowerBase):
     data: BorrowerAPIDTO
 
     def __init__(self, base_url, header_builder, renew_token, data: BorrowerAPIDTO):
         super().__init__(base_url)
         self._header_builder = header_builder
```

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/borrower_fields.py` & `altscore-0.1.99/src/altscore/borrower_central/model/borrower_fields.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/data_models.py` & `altscore-0.1.99/src/altscore/borrower_central/model/data_models.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/documents.py` & `altscore-0.1.99/src/altscore/borrower_central/model/documents.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/evaluators.py` & `altscore-0.1.99/src/altscore/borrower_central/model/evaluators.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/executions.py` & `altscore-0.1.99/src/altscore/borrower_central/model/executions.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/form_templates.py` & `altscore-0.1.99/src/altscore/borrower_central/model/form_templates.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/forms.py` & `altscore-0.1.99/src/altscore/borrower_central/model/forms.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/generics.py` & `altscore-0.1.99/src/altscore/borrower_central/model/generics.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/identities.py` & `altscore-0.1.99/src/altscore/borrower_central/model/identities.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/integrations/sat.py` & `altscore-0.1.99/src/altscore/borrower_central/model/integrations/sat.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/otp_templates.py` & `altscore-0.1.99/src/altscore/borrower_central/model/otp_templates.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/points_of_contact.py` & `altscore-0.1.99/src/altscore/borrower_central/model/points_of_contact.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/policy_alerts.py` & `altscore-0.1.99/src/altscore/borrower_central/model/policy_alerts.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/policy_rules.py` & `altscore-0.1.99/src/altscore/borrower_central/model/policy_rules.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/relationships.py` & `altscore-0.1.99/src/altscore/borrower_central/model/relationships.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/risk_ratings.py` & `altscore-0.1.99/src/altscore/borrower_central/model/risk_ratings.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/stages.py` & `altscore-0.1.99/src/altscore/borrower_central/model/stages.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/store_packages.py` & `altscore-0.1.99/src/altscore/borrower_central/model/store_packages.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/store_secrets.py` & `altscore-0.1.99/src/altscore/borrower_central/model/store_secrets.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/store_sources.py` & `altscore-0.1.99/src/altscore/borrower_central/model/store_sources.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/tools.py` & `altscore-0.1.99/src/altscore/borrower_central/model/tools.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/borrower_central/model/workflows.py` & `altscore-0.1.99/src/altscore/borrower_central/model/workflows.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/__init__.py` & `altscore-0.1.99/src/altscore/cms/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/helpers/__init__.py` & `altscore-0.1.99/src/altscore/cms/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/clients.py` & `altscore-0.1.99/src/altscore/cms/model/clients.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/common.py` & `altscore-0.1.99/src/altscore/cms/model/common.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/credit_account.py` & `altscore-0.1.99/src/altscore/cms/model/credit_account.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/debts.py` & `altscore-0.1.99/src/altscore/cms/model/debts.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/dpas.py` & `altscore-0.1.99/src/altscore/cms/model/dpas.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/generics.py` & `altscore-0.1.99/src/altscore/cms/model/generics.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/cms/model/partners.py` & `altscore-0.1.99/src/altscore/cms/model/partners.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/common/http_errors.py` & `altscore-0.1.99/src/altscore/common/http_errors.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/macros/__init__.py` & `altscore-0.1.99/src/altscore/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore/macros/validate_inputs.py` & `altscore-0.1.99/src/altscore/macros/validate_inputs.py`

 * *Files identical despite different names*

### Comparing `altscore-0.1.98/src/altscore.egg-info/PKG-INFO` & `altscore-0.1.99/src/altscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altscore
-Version: 0.1.98
+Version: 0.1.99
 Summary: Python SDK for AltScore. It provides a simple interface to the AltScore API.
 Home-page: https://github.com/altscore/altscore-python
 Author: AltScore
 Author-email: developers@altscore.ai
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `altscore-0.1.98/src/altscore.egg-info/SOURCES.txt` & `altscore-0.1.99/src/altscore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

