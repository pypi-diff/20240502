# Comparing `tmp/OpenFisca-Country-Template-6.0.3.tar.gz` & `tmp/openfisca_country_template-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Country-Template-6.0.3.tar", last modified: Fri Sep 15 15:48:18 2023, max compression
+gzip compressed data, was "openfisca_country_template-7.0.0.tar", last modified: Thu May  2 07:44:18 2024, max compression
```

## Comparing `OpenFisca-Country-Template-6.0.3.tar` & `openfisca_country_template-7.0.0.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.167523 OpenFisca-Country-Template-6.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    34519 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2023-09-15 15:48:18.000000 OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-09-15 15:48:18.000000 OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 15:48:18.000000 OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-09-15 15:48:18.000000 OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-09-15 15:48:18.000000 OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10386 2023-09-15 15:48:18.167523 OpenFisca-Country-Template-6.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.155522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/index.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/parenting_allowance/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/general/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/general/age_of_majority.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/general/age_of_retirement.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/taxes/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/taxes/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      403 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.159522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/add_dynamic_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/add_new_tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/flat_social_security_contribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/modify_social_security_taxation.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/removal_basic_income.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.163522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/situation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/situation_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/situation_examples/couple.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/situation_examples/housing.json
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/situation_examples/single.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.163522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/age.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/basic_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/disposable_income.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/housing_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/housing_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/income_tax.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.163522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/reforms/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/reforms/add_new_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.163522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/situations/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/situations/income_tax.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/situations/parenting_allowance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/social_security_contribution.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 15:48:18.163522 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/benefits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/demographics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/income.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-09-15 15:48:18.167523 OpenFisca-Country-Template-6.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2023-09-15 15:47:53.000000 OpenFisca-Country-Template-6.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34519 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8421 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.296840 openfisca_country_template-7.0.0/openfisca_country_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.296840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/index.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/general/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/general/age_of_majority.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/general/age_of_retirement.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/income_tax_rate.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_dynamic_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_new_tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/reforms/removal_basic_income.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/couple.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/housing.json
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/single.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/age.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/basic_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/disposable_income.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/housing_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/housing_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/income_tax.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.300840 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/add_dynamic_variable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/income_tax.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/tests/social_security_contribution.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/openfisca_country_template/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/benefits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/demographics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/income.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/openfisca_country_template/variables/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 07:44:18.000000 openfisca_country_template-7.0.0/openfisca_country_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-02 07:44:02.000000 openfisca_country_template-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 07:44:18.304840 openfisca_country_template-7.0.0/setup.cfg
```

### Comparing `OpenFisca-Country-Template-6.0.3/LICENSE` & `openfisca_country_template-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/PKG-INFO` & `openfisca_country_template-7.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,56 @@
 Metadata-Version: 2.1
-Name: OpenFisca-Country-Template
-Version: 6.0.3
-Summary: OpenFisca tax and benefit system for Country-Template
-Home-page: https://github.com/openfisca/country-template
-Author: OpenFisca Team
-Author-email: contact@openfisca.org
-License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
-Keywords: benefit microsimulation social tax
+Name: openfisca-country_template
+Version: 7.0.0
+Summary: OpenFisca Rules as Code model for Country-Template.
+Project-URL: Homepage, https://github.com/openfisca/country-template
+Project-URL: Repository, https://github.com/openfisca/country-template
+Project-URL: Documentation, https://openfisca.org/doc
+Project-URL: Issues, https://github.com/openfisca/country-template/issues
+Project-URL: Changelog, https://github.com/openfisca/country-template/blob/main/CHANGELOG.md
+Keywords: microsimulation,tax,benefit,rac,rules-as-code
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openfisca-core[web-api]<42.0.0,>=41.0.0
 Provides-Extra: dev
-Requires-Dist: autopep8<3.0,>=2.0.2; extra == "dev"
-Requires-Dist: flake8<7.0,>=6.0.0; extra == "dev"
-Requires-Dist: flake8-bugbear<24.0,>=23.3.23; extra == "dev"
-Requires-Dist: flake8-builtins<3.0,>=2.1.0; extra == "dev"
-Requires-Dist: flake8-coding<2.0,>=1.3.2; extra == "dev"
-Requires-Dist: flake8-commas<3.0,>=2.1.0; extra == "dev"
-Requires-Dist: flake8-comprehensions<4.0,>=3.11.1; extra == "dev"
-Requires-Dist: flake8-docstrings<2.0,>=1.7.0; extra == "dev"
-Requires-Dist: flake8-import-order<0.19.0,>=0.18.2; extra == "dev"
-Requires-Dist: flake8-print<6.0,>=5.0.0; extra == "dev"
-Requires-Dist: flake8-quotes<4.0,>=3.3.2; extra == "dev"
-Requires-Dist: flake8-simplify<0.20.0,>=0.19.3; extra == "dev"
-Requires-Dist: flake8-use-fstring<2,>=1.4; extra == "dev"
-Requires-Dist: importlib-metadata<7.0,>=6.1.0; extra == "dev"
-Requires-Dist: pycodestyle<3.0,>=2.10.0; extra == "dev"
-Requires-Dist: pylint<3.0,>=2.17.1; extra == "dev"
+Requires-Dist: autopep8>=2.0.4; extra == "dev"
+Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: isort>=5.13.2; extra == "dev"
+Requires-Dist: pylint>=3.1.0; extra == "dev"
+Requires-Dist: pyupgrade>=3.15.1; extra == "dev"
+Requires-Dist: yamllint>=1.35.1; extra == "dev"
 
 # OpenFisca Country-Template
 
 This repository helps you quickly bootstrap and use your own OpenFisca country package.
 
 **You should NOT fork it but [download a copy](https://github.com/openfisca/country-template/archive/master.zip) of it** and follow the bootstrapping instructions below.
 
 > Otherwise, you will have to clean up all tags when you deploy your own country package.
 
-
 ## Bootstrapping your Country Package
 
-This set of instructions will create your own copy of this boilerplate directory and customise it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
+This set of instructions **only needs to be followed once** and will create your own copy of this boilerplate directory, customising it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
 
 1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
 
-2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-france`.
-
-3. Set up the two following variables and execute the `bootstrap.sh` script to initialise the git repository and replace all references to `openfisca_country_template` with references to your new country package in the code base:
+2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-new_zealand` or `openfisca-france`.
 
-```sh
-export COUNTRY_NAME=France  # set the name of your country here; you should keep all capitals, and replace any spaces in the name by underscores
-export REPOSITORY_URL=https://github.com/YOUR_ORGANISATION/OpenFisca-$COUNTRY_NAME  # set here the URL of the repository you created in step 2.
-./bootstrap.sh
-```
+3. Execute the `bootstrap.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package. 
+   - To execute the script run `bash bootstrap.sh` from the command line. _Note: this script can only run on Unix systems, but OpenFisca and the resulting package will work on Windows too._
+   - After the `bootstrap.sh` has run both it and these instructions are removed.
 
-4. Push your changes to your git host:
-
-```sh
-git push origin master
-```
-
-That's it, you're all set!
+4. Follow the instructions in the new repository's README.md.
 
 ## Writing the Legislation
 
 The country whose law is modelled here has a very simple tax and benefit system.
 
 - It has a flat rate tax whose rates increase every year.
 - On the first of December, 2015, it introduced a basic income for all its citizens of age who have no income.
@@ -101,16 +80,16 @@
 In order to limit dependencies conflicts, we recommend using a [virtual environment](https://www.python.org/dev/peps/pep-0405/) with [venv](https://docs.python.org/3/library/venv.html).
 
 - A [venv](https://docs.python.org/3/library/venv.html) is a project specific environment created to suit the needs of the project you are working on.
 
 To create a virtual environment, launch a terminal on your computer, `cd` into your directory and follow these instructions:
 
 ```sh
-python3 -m venv openfisca # create a new venv called “openfisca”
-source openfisca/bin/activate # activate the venv
+python3 -m venv .venv # create a new virtual environment in the “.venv” folder, which will contain all dependencies
+source .venv/bin/activate # activate the venv
 ```
 
 You can now operate in the venv you just created.
 
 You can deactivate that venv at any time with `deactivate`.
 
 :tada: You are now ready to install this OpenFisca Country Package!
@@ -138,25 +117,25 @@
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Install the Country Package:
 
 ```sh
-pip install openfisca_country_template
+pip install openfisca-country_template
 ```
 
 :warning: Please beware that installing the Country Package with `pip` is dependent on its maintainers publishing said package.
 
 :tada: This OpenFisca Country Package is now installed and ready!
 
 #### Next Steps
 
 - To learn how to use OpenFisca, follow our [tutorials](https://openfisca.org/doc/).
-- To serve this Country Package, serve the [OpenFisca web API](#serve-your-country-package-with-the-openFisca-web-api).
+- To serve this Country Package, serve the [OpenFisca Web API](#serve-your-country-package-with-the-openFisca-web-api).
 
 Depending on what you want to do with OpenFisca, you may want to install yet other packages in your venv:
 - To install extensions or write on top of this Country Package, head to the [Extensions documentation](https://openfisca.org/doc/contribute/extensions.html).
 - To plot simulation results, try [matplotlib](http://matplotlib.org/).
 - To manage data, check out [pandas](http://pandas.pydata.org/).
 
 ### B. Advanced Installation (Git Clone)
@@ -173,24 +152,21 @@
 
 Inside your venv, check the prerequisites:
 
 ```sh
 python --version  # should print "Python 3.9.xx".
 ```
 
-```sh
-pip --version  # should print at least 9.0.
-# if not, run "pip install --upgrade pip"
-```
 Clone this Country Package on your machine:
 
 ```sh
-git clone https://github.com/openfisca/openfisca-country-template.git
-cd openfisca-country-template
-pip install --editable .[dev]
+git clone https://example.com/repository.git
+cd repository_folder
+pip install --upgrade pip build twine
+pip install --editable .[dev] --upgrade
 ```
 
 You can make sure that everything is working by running the provided tests with `make test`.
 
 > [Learn more about tests](https://openfisca.org/doc/coding-the-legislation/writing_yaml_tests.html)
 
 :tada: This OpenFisca Country Package is now installed and ready!
@@ -203,15 +179,15 @@
 ## Serve this Country Package with the OpenFisca Web API
 
 If you are considering building a web application, you can use the packaged OpenFisca Web API with your Country Package.
 
 To serve the Openfisca Web API locally, run:
 
 ```sh
-openfisca serve --port 5000
+openfisca serve --port 5000 --country-package openfisca_country_template
 ```
 
 Or use the quick-start Make command:
 
 ```
 make serve-local
 ```
@@ -226,14 +202,12 @@
 
 This endpoint returns the [Open API specification](https://www.openapis.org/) of your API.
 
 :tada: This OpenFisca Country Package is now served by the OpenFisca Web API! To learn more, go to the [OpenFisca Web API documentation](https://openfisca.org/doc/openfisca-web-api/index.html).
 
 You can test your new Web API by sending it example JSON data located in the `situation_examples` folder.
 
-Substitute your package's country name for `openfisca_country_template` below:
-
 ```sh
 curl -X POST -H "Content-Type: application/json" \
   -d @./openfisca_country_template/situation_examples/couple.json \
   http://localhost:5000/calculate
 ```
```

### Comparing `OpenFisca-Country-Template-6.0.3/OpenFisca_Country_Template.egg-info/SOURCES.txt` & `openfisca_country_template-7.0.0/openfisca_country_template.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
-setup.cfg
-setup.py
-OpenFisca_Country_Template.egg-info/PKG-INFO
-OpenFisca_Country_Template.egg-info/SOURCES.txt
-OpenFisca_Country_Template.egg-info/dependency_links.txt
-OpenFisca_Country_Template.egg-info/requires.txt
-OpenFisca_Country_Template.egg-info/top_level.txt
+pyproject.toml
 openfisca_country_template/__init__.py
 openfisca_country_template/entities.py
+openfisca_country_template.egg-info/PKG-INFO
+openfisca_country_template.egg-info/SOURCES.txt
+openfisca_country_template.egg-info/dependency_links.txt
+openfisca_country_template.egg-info/requires.txt
+openfisca_country_template.egg-info/top_level.txt
 openfisca_country_template/parameters/benefits/basic_income.yaml
 openfisca_country_template/parameters/benefits/housing_allowance.yaml
 openfisca_country_template/parameters/benefits/index.yaml
 openfisca_country_template/parameters/benefits/parenting_allowance/amount.yaml
 openfisca_country_template/parameters/benefits/parenting_allowance/income_threshold.yaml
 openfisca_country_template/parameters/general/age_of_majority.yaml
 openfisca_country_template/parameters/general/age_of_retirement.yaml
```

### Comparing `OpenFisca-Country-Template-6.0.3/PKG-INFO` & `openfisca_country_template-7.0.0/openfisca_country_template.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,56 @@
 Metadata-Version: 2.1
-Name: OpenFisca-Country-Template
-Version: 6.0.3
-Summary: OpenFisca tax and benefit system for Country-Template
-Home-page: https://github.com/openfisca/country-template
-Author: OpenFisca Team
-Author-email: contact@openfisca.org
-License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
-Keywords: benefit microsimulation social tax
+Name: openfisca-country_template
+Version: 7.0.0
+Summary: OpenFisca Rules as Code model for Country-Template.
+Project-URL: Homepage, https://github.com/openfisca/country-template
+Project-URL: Repository, https://github.com/openfisca/country-template
+Project-URL: Documentation, https://openfisca.org/doc
+Project-URL: Issues, https://github.com/openfisca/country-template/issues
+Project-URL: Changelog, https://github.com/openfisca/country-template/blob/main/CHANGELOG.md
+Keywords: microsimulation,tax,benefit,rac,rules-as-code
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openfisca-core[web-api]<42.0.0,>=41.0.0
 Provides-Extra: dev
-Requires-Dist: autopep8<3.0,>=2.0.2; extra == "dev"
-Requires-Dist: flake8<7.0,>=6.0.0; extra == "dev"
-Requires-Dist: flake8-bugbear<24.0,>=23.3.23; extra == "dev"
-Requires-Dist: flake8-builtins<3.0,>=2.1.0; extra == "dev"
-Requires-Dist: flake8-coding<2.0,>=1.3.2; extra == "dev"
-Requires-Dist: flake8-commas<3.0,>=2.1.0; extra == "dev"
-Requires-Dist: flake8-comprehensions<4.0,>=3.11.1; extra == "dev"
-Requires-Dist: flake8-docstrings<2.0,>=1.7.0; extra == "dev"
-Requires-Dist: flake8-import-order<0.19.0,>=0.18.2; extra == "dev"
-Requires-Dist: flake8-print<6.0,>=5.0.0; extra == "dev"
-Requires-Dist: flake8-quotes<4.0,>=3.3.2; extra == "dev"
-Requires-Dist: flake8-simplify<0.20.0,>=0.19.3; extra == "dev"
-Requires-Dist: flake8-use-fstring<2,>=1.4; extra == "dev"
-Requires-Dist: importlib-metadata<7.0,>=6.1.0; extra == "dev"
-Requires-Dist: pycodestyle<3.0,>=2.10.0; extra == "dev"
-Requires-Dist: pylint<3.0,>=2.17.1; extra == "dev"
+Requires-Dist: autopep8>=2.0.4; extra == "dev"
+Requires-Dist: flake8>=7.0.0; extra == "dev"
+Requires-Dist: isort>=5.13.2; extra == "dev"
+Requires-Dist: pylint>=3.1.0; extra == "dev"
+Requires-Dist: pyupgrade>=3.15.1; extra == "dev"
+Requires-Dist: yamllint>=1.35.1; extra == "dev"
 
 # OpenFisca Country-Template
 
 This repository helps you quickly bootstrap and use your own OpenFisca country package.
 
 **You should NOT fork it but [download a copy](https://github.com/openfisca/country-template/archive/master.zip) of it** and follow the bootstrapping instructions below.
 
 > Otherwise, you will have to clean up all tags when you deploy your own country package.
 
-
 ## Bootstrapping your Country Package
 
-This set of instructions will create your own copy of this boilerplate directory and customise it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
+This set of instructions **only needs to be followed once** and will create your own copy of this boilerplate directory, customising it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
 
 1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
 
-2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-france`.
-
-3. Set up the two following variables and execute the `bootstrap.sh` script to initialise the git repository and replace all references to `openfisca_country_template` with references to your new country package in the code base:
+2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-new_zealand` or `openfisca-france`.
 
-```sh
-export COUNTRY_NAME=France  # set the name of your country here; you should keep all capitals, and replace any spaces in the name by underscores
-export REPOSITORY_URL=https://github.com/YOUR_ORGANISATION/OpenFisca-$COUNTRY_NAME  # set here the URL of the repository you created in step 2.
-./bootstrap.sh
-```
+3. Execute the `bootstrap.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package. 
+   - To execute the script run `bash bootstrap.sh` from the command line. _Note: this script can only run on Unix systems, but OpenFisca and the resulting package will work on Windows too._
+   - After the `bootstrap.sh` has run both it and these instructions are removed.
 
-4. Push your changes to your git host:
-
-```sh
-git push origin master
-```
-
-That's it, you're all set!
+4. Follow the instructions in the new repository's README.md.
 
 ## Writing the Legislation
 
 The country whose law is modelled here has a very simple tax and benefit system.
 
 - It has a flat rate tax whose rates increase every year.
 - On the first of December, 2015, it introduced a basic income for all its citizens of age who have no income.
@@ -101,16 +80,16 @@
 In order to limit dependencies conflicts, we recommend using a [virtual environment](https://www.python.org/dev/peps/pep-0405/) with [venv](https://docs.python.org/3/library/venv.html).
 
 - A [venv](https://docs.python.org/3/library/venv.html) is a project specific environment created to suit the needs of the project you are working on.
 
 To create a virtual environment, launch a terminal on your computer, `cd` into your directory and follow these instructions:
 
 ```sh
-python3 -m venv openfisca # create a new venv called “openfisca”
-source openfisca/bin/activate # activate the venv
+python3 -m venv .venv # create a new virtual environment in the “.venv” folder, which will contain all dependencies
+source .venv/bin/activate # activate the venv
 ```
 
 You can now operate in the venv you just created.
 
 You can deactivate that venv at any time with `deactivate`.
 
 :tada: You are now ready to install this OpenFisca Country Package!
@@ -138,25 +117,25 @@
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Install the Country Package:
 
 ```sh
-pip install openfisca_country_template
+pip install openfisca-country_template
 ```
 
 :warning: Please beware that installing the Country Package with `pip` is dependent on its maintainers publishing said package.
 
 :tada: This OpenFisca Country Package is now installed and ready!
 
 #### Next Steps
 
 - To learn how to use OpenFisca, follow our [tutorials](https://openfisca.org/doc/).
-- To serve this Country Package, serve the [OpenFisca web API](#serve-your-country-package-with-the-openFisca-web-api).
+- To serve this Country Package, serve the [OpenFisca Web API](#serve-your-country-package-with-the-openFisca-web-api).
 
 Depending on what you want to do with OpenFisca, you may want to install yet other packages in your venv:
 - To install extensions or write on top of this Country Package, head to the [Extensions documentation](https://openfisca.org/doc/contribute/extensions.html).
 - To plot simulation results, try [matplotlib](http://matplotlib.org/).
 - To manage data, check out [pandas](http://pandas.pydata.org/).
 
 ### B. Advanced Installation (Git Clone)
@@ -173,24 +152,21 @@
 
 Inside your venv, check the prerequisites:
 
 ```sh
 python --version  # should print "Python 3.9.xx".
 ```
 
-```sh
-pip --version  # should print at least 9.0.
-# if not, run "pip install --upgrade pip"
-```
 Clone this Country Package on your machine:
 
 ```sh
-git clone https://github.com/openfisca/openfisca-country-template.git
-cd openfisca-country-template
-pip install --editable .[dev]
+git clone https://example.com/repository.git
+cd repository_folder
+pip install --upgrade pip build twine
+pip install --editable .[dev] --upgrade
 ```
 
 You can make sure that everything is working by running the provided tests with `make test`.
 
 > [Learn more about tests](https://openfisca.org/doc/coding-the-legislation/writing_yaml_tests.html)
 
 :tada: This OpenFisca Country Package is now installed and ready!
@@ -203,15 +179,15 @@
 ## Serve this Country Package with the OpenFisca Web API
 
 If you are considering building a web application, you can use the packaged OpenFisca Web API with your Country Package.
 
 To serve the Openfisca Web API locally, run:
 
 ```sh
-openfisca serve --port 5000
+openfisca serve --port 5000 --country-package openfisca_country_template
 ```
 
 Or use the quick-start Make command:
 
 ```
 make serve-local
 ```
@@ -226,14 +202,12 @@
 
 This endpoint returns the [Open API specification](https://www.openapis.org/) of your API.
 
 :tada: This OpenFisca Country Package is now served by the OpenFisca Web API! To learn more, go to the [OpenFisca Web API documentation](https://openfisca.org/doc/openfisca-web-api/index.html).
 
 You can test your new Web API by sending it example JSON data located in the `situation_examples` folder.
 
-Substitute your package's country name for `openfisca_country_template` below:
-
 ```sh
 curl -X POST -H "Content-Type: application/json" \
   -d @./openfisca_country_template/situation_examples/couple.json \
   http://localhost:5000/calculate
 ```
```

### Comparing `OpenFisca-Country-Template-6.0.3/README.md` & `openfisca_country_template-7.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,38 +2,27 @@
 
 This repository helps you quickly bootstrap and use your own OpenFisca country package.
 
 **You should NOT fork it but [download a copy](https://github.com/openfisca/country-template/archive/master.zip) of it** and follow the bootstrapping instructions below.
 
 > Otherwise, you will have to clean up all tags when you deploy your own country package.
 
-
 ## Bootstrapping your Country Package
 
-This set of instructions will create your own copy of this boilerplate directory and customise it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
+This set of instructions **only needs to be followed once** and will create your own copy of this boilerplate directory, customising it to the country you want to work on. You will need to have [Git](https://git-scm.com) installed.
 
 1. [Download a copy](https://github.com/openfisca/country-template/archive/master.zip) of this repository, unzip it and `cd` into it in a Terminal window.
 
-2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-france`.
-
-3. Set up the two following variables and execute the `bootstrap.sh` script to initialise the git repository and replace all references to `openfisca_country_template` with references to your new country package in the code base:
+2. Create a new repository on your favourite git host (Github, Bitbucket, GitLab, etc) with the name openfisca-your_country_name. For example, `openfisca-new_zealand` or `openfisca-france`.
 
-```sh
-export COUNTRY_NAME=France  # set the name of your country here; you should keep all capitals, and replace any spaces in the name by underscores
-export REPOSITORY_URL=https://github.com/YOUR_ORGANISATION/OpenFisca-$COUNTRY_NAME  # set here the URL of the repository you created in step 2.
-./bootstrap.sh
-```
+3. Execute the `bootstrap.sh` script to initialise the git repository. This performs numerous tasks including replacing all references to `openfisca-country_template` with references to the new country package. 
+   - To execute the script run `bash bootstrap.sh` from the command line. _Note: this script can only run on Unix systems, but OpenFisca and the resulting package will work on Windows too._
+   - After the `bootstrap.sh` has run both it and these instructions are removed.
 
-4. Push your changes to your git host:
-
-```sh
-git push origin master
-```
-
-That's it, you're all set!
+4. Follow the instructions in the new repository's README.md.
 
 ## Writing the Legislation
 
 The country whose law is modelled here has a very simple tax and benefit system.
 
 - It has a flat rate tax whose rates increase every year.
 - On the first of December, 2015, it introduced a basic income for all its citizens of age who have no income.
@@ -63,16 +52,16 @@
 In order to limit dependencies conflicts, we recommend using a [virtual environment](https://www.python.org/dev/peps/pep-0405/) with [venv](https://docs.python.org/3/library/venv.html).
 
 - A [venv](https://docs.python.org/3/library/venv.html) is a project specific environment created to suit the needs of the project you are working on.
 
 To create a virtual environment, launch a terminal on your computer, `cd` into your directory and follow these instructions:
 
 ```sh
-python3 -m venv openfisca # create a new venv called “openfisca”
-source openfisca/bin/activate # activate the venv
+python3 -m venv .venv # create a new virtual environment in the “.venv” folder, which will contain all dependencies
+source .venv/bin/activate # activate the venv
 ```
 
 You can now operate in the venv you just created.
 
 You can deactivate that venv at any time with `deactivate`.
 
 :tada: You are now ready to install this OpenFisca Country Package!
@@ -100,25 +89,25 @@
 ```sh
 pip --version  # should print at least 9.0.
 # if not, run "pip install --upgrade pip"
 ```
 Install the Country Package:
 
 ```sh
-pip install openfisca_country_template
+pip install openfisca-country_template
 ```
 
 :warning: Please beware that installing the Country Package with `pip` is dependent on its maintainers publishing said package.
 
 :tada: This OpenFisca Country Package is now installed and ready!
 
 #### Next Steps
 
 - To learn how to use OpenFisca, follow our [tutorials](https://openfisca.org/doc/).
-- To serve this Country Package, serve the [OpenFisca web API](#serve-your-country-package-with-the-openFisca-web-api).
+- To serve this Country Package, serve the [OpenFisca Web API](#serve-your-country-package-with-the-openFisca-web-api).
 
 Depending on what you want to do with OpenFisca, you may want to install yet other packages in your venv:
 - To install extensions or write on top of this Country Package, head to the [Extensions documentation](https://openfisca.org/doc/contribute/extensions.html).
 - To plot simulation results, try [matplotlib](http://matplotlib.org/).
 - To manage data, check out [pandas](http://pandas.pydata.org/).
 
 ### B. Advanced Installation (Git Clone)
@@ -135,24 +124,21 @@
 
 Inside your venv, check the prerequisites:
 
 ```sh
 python --version  # should print "Python 3.9.xx".
 ```
 
-```sh
-pip --version  # should print at least 9.0.
-# if not, run "pip install --upgrade pip"
-```
 Clone this Country Package on your machine:
 
 ```sh
-git clone https://github.com/openfisca/openfisca-country-template.git
-cd openfisca-country-template
-pip install --editable .[dev]
+git clone https://example.com/repository.git
+cd repository_folder
+pip install --upgrade pip build twine
+pip install --editable .[dev] --upgrade
 ```
 
 You can make sure that everything is working by running the provided tests with `make test`.
 
 > [Learn more about tests](https://openfisca.org/doc/coding-the-legislation/writing_yaml_tests.html)
 
 :tada: This OpenFisca Country Package is now installed and ready!
@@ -165,15 +151,15 @@
 ## Serve this Country Package with the OpenFisca Web API
 
 If you are considering building a web application, you can use the packaged OpenFisca Web API with your Country Package.
 
 To serve the Openfisca Web API locally, run:
 
 ```sh
-openfisca serve --port 5000
+openfisca serve --port 5000 --country-package openfisca_country_template
 ```
 
 Or use the quick-start Make command:
 
 ```
 make serve-local
 ```
@@ -188,14 +174,12 @@
 
 This endpoint returns the [Open API specification](https://www.openapis.org/) of your API.
 
 :tada: This OpenFisca Country Package is now served by the OpenFisca Web API! To learn more, go to the [OpenFisca Web API documentation](https://openfisca.org/doc/openfisca-web-api/index.html).
 
 You can test your new Web API by sending it example JSON data located in the `situation_examples` folder.
 
-Substitute your package's country name for `openfisca_country_template` below:
-
 ```sh
 curl -X POST -H "Content-Type: application/json" \
   -d @./openfisca_country_template/situation_examples/couple.json \
   http://localhost:5000/calculate
 ```
```

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/__init__.py` & `openfisca_country_template-7.0.0/openfisca_country_template/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/entities.py` & `openfisca_country_template-7.0.0/openfisca_country_template/entities.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/parameters/taxes/social_security_contribution.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/parameters/taxes/social_security_contribution.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/add_dynamic_variable.py` & `openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_dynamic_variable.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/add_new_tax.py` & `openfisca_country_template-7.0.0/openfisca_country_template/reforms/add_new_tax.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/flat_social_security_contribution.py` & `openfisca_country_template-7.0.0/openfisca_country_template/reforms/flat_social_security_contribution.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/modify_social_security_taxation.py` & `openfisca_country_template-7.0.0/openfisca_country_template/reforms/modify_social_security_taxation.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/reforms/removal_basic_income.py` & `openfisca_country_template-7.0.0/openfisca_country_template/reforms/removal_basic_income.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/situation_examples/couple.json` & `openfisca_country_template-7.0.0/openfisca_country_template/situation_examples/couple.json`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/age.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/age.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/basic_income.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/basic_income.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/disposable_income.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/disposable_income.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/housing_tax.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/housing_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/reforms/add_new_tax.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/add_new_tax.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/reforms/modify_social_security_taxation.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/situations/income_tax.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/income_tax.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
       children: [ Michael ]
       accommodation_size: 100
       housing_occupancy_status: tenant
     persons:
       Alicia:
         birth: 1961-01-15
         salary:
-         2017-01: 2400
+          2017-01: 2400
       Michael:
         birth: 2002-01-15
         salary:
-         2016: 0
+          2016: 0
   output:
     persons:
       Alicia:
         income_tax: 360
       Michael:
         income_tax: 0
     household:
```

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/situations/parenting_allowance.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/situations/parenting_allowance.yaml`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/tests/social_security_contribution.yaml` & `openfisca_country_template-7.0.0/openfisca_country_template/tests/social_security_contribution.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Test files describe situations and their expected outcomes
 # We can run this test on our command line using `openfisca-run-test social_security_contribution.yaml`
 
 - name: Person earning 2000 in 2013-01
   period: 2013-01
   input:
     salary: 2000
```

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/benefits.py` & `openfisca_country_template-7.0.0/openfisca_country_template/variables/benefits.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/demographics.py` & `openfisca_country_template-7.0.0/openfisca_country_template/variables/demographics.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 
 from datetime import date
 
 # Import from numpy the operations you need to apply on OpenFisca's population vectors
 # Import from openfisca-core the Python objects used to code the legislation in OpenFisca
 from numpy import where
+
 from openfisca_core.periods import ETERNITY, MONTH
 from openfisca_core.variables import Variable
 
 # Import the Entities specifically defined for this tax and benefit system
 from openfisca_country_template.entities import Person
```

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/housing.py` & `openfisca_country_template-7.0.0/openfisca_country_template/variables/housing.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/income.py` & `openfisca_country_template-7.0.0/openfisca_country_template/variables/income.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/stats.py` & `openfisca_country_template-7.0.0/openfisca_country_template/variables/stats.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Country-Template-6.0.3/openfisca_country_template/variables/taxes.py` & `openfisca_country_template-7.0.0/openfisca_country_template/variables/taxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 See https://openfisca.org/doc/key-concepts/variables.html
 """
 
 # Import from numpy the operations you need to apply on OpenFisca's population vectors
 # Import from openfisca-core the Python objects used to code the legislation in OpenFisca
 from numpy import maximum as max_
+
 from openfisca_core.periods import MONTH, YEAR
 from openfisca_core.variables import Variable
 
 # Import the Entities specifically defined for this tax and benefit system
 from openfisca_country_template.entities import Household, Person
```

