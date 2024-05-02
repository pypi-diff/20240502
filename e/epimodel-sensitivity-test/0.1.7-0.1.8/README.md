# Comparing `tmp/epimodel_sensitivity_test-0.1.7.tar.gz` & `tmp/epimodel_sensitivity_test-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epimodel_sensitivity_test-0.1.7.tar", last modified: Tue Apr 30 16:59:44 2024, max compression
+gzip compressed data, was "epimodel_sensitivity_test-0.1.8.tar", last modified: Thu May  2 13:28:21 2024, max compression
```

## Comparing `epimodel_sensitivity_test-0.1.7.tar` & `epimodel_sensitivity_test-0.1.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.586039 epimodel_sensitivity_test-0.1.7/
--rw-rw-rw-   0        0        0     2153 2024-04-30 16:59:44.585039 epimodel_sensitivity_test-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.441342 epimodel_sensitivity_test-0.1.7/data/
--rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/data/age_distribution.xls
--rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/data/contact_matrices.xls
--rw-rw-rw-   0        0        0     3079 2024-04-28 22:03:14.000000 epimodel_sensitivity_test-0.1.7/data/model_parameters.json
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.465349 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/
--rw-rw-rw-   0        0        0     2153 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2423 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 16:59:44.000000 epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.468349 epimodel_sensitivity_test-0.1.7/examples/
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.474351 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.479353 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/
--rw-rw-rw-   0        0        0      840 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      569 2024-04-30 14:26:59.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0     1003 2024-04-30 14:43:33.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
--rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/simulation_seihr.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.491365 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.496357 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/
--rw-rw-rw-   0        0        0      543 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/model_struct.json
--rw-rw-rw-   0        0        0      372 2024-04-30 14:17:47.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/sampling_config.json
--rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/model_seir.py
--rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/sampler_seir.py
--rw-rw-rw-   0        0        0      739 2024-04-30 14:11:55.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/seir_no_ag_main.py
--rw-rw-rw-   0        0        0     1187 2024-04-30 14:15:47.000000 epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/simulation_seir.py
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.506488 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.511541 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/
--rw-rw-rw-   0        0        0     1961 2024-04-30 14:35:59.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0      452 2024-04-30 14:08:09.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/contact_main.py
--rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sampler_contact.py
--rw-rw-rw-   0        0        0     3159 2024-04-30 14:37:54.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sensitivity_model_contact.py
--rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/simulation_contact.py
--rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.7/examples/test.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.515605 epimodel_sensitivity_test-0.1.7/examples/utils/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/utils/__init__.py
--rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/utils/dataloader_16_ag.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.528936 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.535029 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/
--rw-rw-rw-   0        0        0     1569 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/model_struct.json
--rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/sampling_config.json
--rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sampler_vaccinated.py
--rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
--rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/simulation_vacc.py
--rw-rw-rw-   0        0        0      439 2024-04-30 13:55:41.000000 epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/vaccinated_main.py
--rw-rw-rw-   0        0        0       42 2024-04-30 16:59:44.586039 epimodel_sensitivity_test-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-04-30 16:59:34.000000 epimodel_sensitivity_test-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.544028 epimodel_sensitivity_test-0.1.7/src/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/src/__init__.py
--rw-rw-rw-   0        0        0      517 2024-04-29 08:05:11.000000 epimodel_sensitivity_test-0.1.7/src/dataloader.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.556032 epimodel_sensitivity_test-0.1.7/src/model/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/src/model/__init__.py
--rw-rw-rw-   0        0        0     1239 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/model/epidemic_model.py
--rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.7/src/model/matrix_generator.py
--rw-rw-rw-   0        0        0     4466 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/model/model_base.py
--rw-rw-rw-   0        0        0     4742 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/model/r0.py
--rw-rw-rw-   0        0        0     8110 2024-04-28 16:26:24.000000 epimodel_sensitivity_test-0.1.7/src/plotter.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.566035 epimodel_sensitivity_test-0.1.7/src/sensitivity/
--rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/__init__.py
--rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/prcc.py
--rw-rw-rw-   0        0        0     4661 2024-04-30 14:26:59.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/sampler_base.py
--rw-rw-rw-   0        0        0     4988 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/sensitivity_model_base.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.573035 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/
--rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/__init__.py
--rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/output_generator.py
--rw-rw-rw-   0        0        0     1606 2024-04-30 14:36:56.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/r0calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:59:44.582039 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/
--rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/__init__.py
--rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/final_size_calc.py
--rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/peak_calc.py
--rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/target_calc_base.py
--rw-rw-rw-   0        0        0     8430 2024-04-30 14:36:31.000000 epimodel_sensitivity_test-0.1.7/src/simulation_base.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.461729 epimodel_sensitivity_test-0.1.8/
+-rw-rw-rw-   0        0        0     2153 2024-05-02 13:28:21.460730 epimodel_sensitivity_test-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1698 2024-04-05 10:47:20.000000 epimodel_sensitivity_test-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.119040 epimodel_sensitivity_test-0.1.8/data/
+-rw-rw-rw-   0        0        0     6144 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.8/data/age_distribution.xls
+-rw-rw-rw-   0        0        0    26112 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.8/data/contact_matrices.xls
+-rw-rw-rw-   0        0        0     3079 2024-04-28 22:03:14.000000 epimodel_sensitivity_test-0.1.8/data/model_parameters.json
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.154174 epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/
+-rw-rw-rw-   0        0        0     2153 2024-05-02 13:28:20.000000 epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2423 2024-05-02 13:28:21.000000 epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 13:28:20.000000 epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-02 13:28:20.000000 epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 13:28:20.000000 epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.158179 epimodel_sensitivity_test-0.1.8/examples/
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.178194 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.182184 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/configs/
+-rw-rw-rw-   0        0        0      840 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      569 2024-04-30 14:26:59.000000 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0     1003 2024-04-30 14:43:33.000000 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/seihr_2_ag_main.py
+-rw-rw-rw-   0        0        0     1694 2024-04-27 18:48:18.000000 epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/simulation_seihr.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.199278 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.202286 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/configs/
+-rw-rw-rw-   0        0        0      543 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/configs/model_struct.json
+-rw-rw-rw-   0        0        0      372 2024-04-30 14:17:47.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      344 2024-04-12 11:39:01.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/model_seir.py
+-rw-rw-rw-   0        0        0      332 2024-04-08 13:30:52.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/sampler_seir.py
+-rw-rw-rw-   0        0        0      777 2024-05-02 12:13:14.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/seir_no_ag_main.py
+-rw-rw-rw-   0        0        0     1187 2024-04-30 14:15:47.000000 epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/simulation_seir.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.243300 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.246292 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1961 2024-04-30 14:35:59.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      428 2024-04-05 22:30:36.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0      452 2024-04-30 14:08:09.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/contact_main.py
+-rw-rw-rw-   0        0        0      572 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/sampler_contact.py
+-rw-rw-rw-   0        0        0     3159 2024-04-30 14:37:54.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/sensitivity_model_contact.py
+-rw-rw-rw-   0        0        0     3820 2024-04-11 14:42:43.000000 epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/simulation_contact.py
+-rw-rw-rw-   0        0        0      398 2024-04-08 21:01:30.000000 epimodel_sensitivity_test-0.1.8/examples/test.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.260299 epimodel_sensitivity_test-0.1.8/examples/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/utils/__init__.py
+-rw-rw-rw-   0        0        0     3456 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/utils/dataloader_16_ag.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.322309 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.328311 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/configs/
+-rw-rw-rw-   0        0        0     1569 2024-04-30 14:35:58.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/configs/model_struct.json
+-rw-rw-rw-   0        0        0      414 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/configs/sampling_config.json
+-rw-rw-rw-   0        0        0     2771 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/sampler_vaccinated.py
+-rw-rw-rw-   0        0        0     1112 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py
+-rw-rw-rw-   0        0        0     3666 2024-04-08 20:55:46.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/simulation_vacc.py
+-rw-rw-rw-   0        0        0      439 2024-04-30 13:55:41.000000 epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/vaccinated_main.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 13:28:21.462727 epimodel_sensitivity_test-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-05-02 13:27:47.000000 epimodel_sensitivity_test-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.346316 epimodel_sensitivity_test-0.1.8/src/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.8/src/__init__.py
+-rw-rw-rw-   0        0        0      517 2024-04-29 08:05:11.000000 epimodel_sensitivity_test-0.1.8/src/dataloader.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.377323 epimodel_sensitivity_test-0.1.8/src/model/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.8/src/model/__init__.py
+-rw-rw-rw-   0        0        0     1239 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.8/src/model/epidemic_model.py
+-rw-rw-rw-   0        0        0    10445 2024-04-28 12:30:58.000000 epimodel_sensitivity_test-0.1.8/src/model/matrix_generator.py
+-rw-rw-rw-   0        0        0     4476 2024-05-02 12:11:59.000000 epimodel_sensitivity_test-0.1.8/src/model/model_base.py
+-rw-rw-rw-   0        0        0     4742 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.8/src/model/r0.py
+-rw-rw-rw-   0        0        0     8655 2024-05-02 12:08:05.000000 epimodel_sensitivity_test-0.1.8/src/plotter.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.401327 epimodel_sensitivity_test-0.1.8/src/sensitivity/
+-rw-rw-rw-   0        0        0        0 2023-12-03 10:59:34.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/__init__.py
+-rw-rw-rw-   0        0        0     1137 2024-04-04 14:22:44.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/prcc.py
+-rw-rw-rw-   0        0        0     4661 2024-04-30 14:26:59.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/sampler_base.py
+-rw-rw-rw-   0        0        0     4988 2024-04-30 14:32:48.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/sensitivity_model_base.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.428334 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/
+-rw-rw-rw-   0        0        0        0 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-08 13:26:57.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/output_generator.py
+-rw-rw-rw-   0        0        0     1606 2024-04-30 14:36:56.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/r0calculator.py
+drwxrwxrwx   0        0        0        0 2024-05-02 13:28:21.457727 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/
+-rw-rw-rw-   0        0        0        0 2024-04-07 15:24:44.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-04-28 11:42:55.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/final_size_calc.py
+-rw-rw-rw-   0        0        0      923 2024-04-07 15:33:11.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/peak_calc.py
+-rw-rw-rw-   0        0        0     3373 2024-04-04 20:44:27.000000 epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/target_calc_base.py
+-rw-rw-rw-   0        0        0     8430 2024-04-30 14:36:31.000000 epimodel_sensitivity_test-0.1.8/src/simulation_base.py
```

### Comparing `epimodel_sensitivity_test-0.1.7/PKG-INFO` & `epimodel_sensitivity_test-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel_sensitivity_test
-Version: 0.1.7
+Version: 0.1.8
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.7/README.md` & `epimodel_sensitivity_test-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/data/age_distribution.xls` & `epimodel_sensitivity_test-0.1.8/data/age_distribution.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/data/contact_matrices.xls` & `epimodel_sensitivity_test-0.1.8/data/contact_matrices.xls`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/data/model_parameters.json` & `epimodel_sensitivity_test-0.1.8/data/model_parameters.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/PKG-INFO` & `epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epimodel-sensitivity-test
-Version: 0.1.7
+Version: 0.1.8
 Summary: Efficient sensitivity analysis and evaluation of epidemiological models
 Home-page: https://github.com/KKol21/epimodel_sensitivity
 Author: Kolos Kovács
 Author-email: kovkol21@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `epimodel_sensitivity_test-0.1.7/epimodel_sensitivity_test.egg-info/SOURCES.txt` & `epimodel_sensitivity_test-0.1.8/epimodel_sensitivity_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/configs/sampling_config.json` & `epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/configs/sampling_config.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/seihr_2_ag_main.py` & `epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/seihr_2_ag_main.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIHR_2_age_groups/simulation_seihr.py` & `epimodel_sensitivity_test-0.1.8/examples/SEIHR_2_age_groups/simulation_seihr.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/seir_no_ag_main.py` & `epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/seir_no_ag_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 from examples.SEIR_no_age_groups.simulation_seir import SimulationSEIR
 
 
 def main():
     params = {"gamma": 0.2, "alpha": 0.3}
     contact_data = torch.tensor(1)
-    age_data = torch.tensor(10000)
+    age_data = torch.tensor([10000])
     data = SimpleNamespace(**{"params": params,
                               "cm": contact_data,
                               "age_data": age_data,
                               "n_age": 1,
                               "device": "cpu"})
 
     sim = SimulationSEIR(data)
     sim.model.visualize_transmission_graph()
+    sim.model.get_initial_values()
     sim.run_sampling()
     sim.calculate_all_prcc()
     sim.calculate_all_p_values()
     sim.plot_all_prcc()
 
 
 if __name__ == "__main__":
```

### Comparing `epimodel_sensitivity_test-0.1.7/examples/SEIR_no_age_groups/simulation_seir.py` & `epimodel_sensitivity_test-0.1.8/examples/SEIR_no_age_groups/simulation_seir.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sampler_contact.py` & `epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/sampler_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/sensitivity_model_contact.py` & `epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/sensitivity_model_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/contact_sensitivity/simulation_contact.py` & `epimodel_sensitivity_test-0.1.8/examples/contact_sensitivity/simulation_contact.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/utils/dataloader_16_ag.py` & `epimodel_sensitivity_test-0.1.8/examples/utils/dataloader_16_ag.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/configs/model_struct.json` & `epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/configs/model_struct.json`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sampler_vaccinated.py` & `epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/sampler_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py` & `epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/sensitivity_model_vaccinated.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/examples/vaccinated_sensitivity/simulation_vacc.py` & `epimodel_sensitivity_test-0.1.8/examples/vaccinated_sensitivity/simulation_vacc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/setup.py` & `epimodel_sensitivity_test-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='epimodel_sensitivity_test',
-    version='0.1.7',
+    version='0.1.8',
     author='Kolos Kovács',
     author_email='kovkol21@gmail.com',
     description='Efficient sensitivity analysis and evaluation of epidemiological models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KKol21/epimodel_sensitivity',
     packages=find_packages(),
```

### Comparing `epimodel_sensitivity_test-0.1.7/src/dataloader.py` & `epimodel_sensitivity_test-0.1.8/src/dataloader.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/model/epidemic_model.py` & `epimodel_sensitivity_test-0.1.8/src/model/epidemic_model.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/model/matrix_generator.py` & `epimodel_sensitivity_test-0.1.8/src/model/matrix_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/model/model_base.py` & `epimodel_sensitivity_test-0.1.8/src/model/model_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
             None
         """
         self.data = data
         self.state_data = model_struct["state_data"]
         self.trans_data = model_struct["trans_data"]
         self.tms_rules = model_struct["tms_rules"]
 
-        self.n_age = data.n_age
         self.population = data.age_data.flatten()
+        self.n_age = len(self.population)
         self.compartments = self.get_compartments()
         self.n_comp = len(self.compartments)
         self.ps = data.params
         self.device = data.device
 
         self.c_idx = {comp: idx for idx, comp in enumerate(self.compartments)}
         self.n_eq = self.n_age * self.n_comp
```

### Comparing `epimodel_sensitivity_test-0.1.7/src/model/r0.py` & `epimodel_sensitivity_test-0.1.8/src/model/r0.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/plotter.py` & `epimodel_sensitivity_test-0.1.8/src/plotter.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,20 +12,32 @@
 
 def visualize_transmission_graph(state_data, trans_data, tms_rules):
     plt.figure(figsize=(10, 8))
     G = nx.DiGraph()
 
     # Add nodes
     def get_node_label(node):
-        if n_substates := state_data[node].get("n_substates"):
+        if n_substates := state_data[node].get("n_substates", 1) > 1:
             return f"{node}$^{{{n_substates}}}$"
         return node
 
+    def get_node_color(node):
+        node_type =  state_data[node].get("type", "basic")
+        if node_type == "susceptible":
+            return "green"
+        if node_type == "infected":
+            return "red"
+        if node_type == "recovered":
+            return "blue"
+        if node_type == "dead":
+            return "gray"
+        return "orange"
+
     for node, data in state_data.items():
-        G.add_node(get_node_label(node))
+        G.add_node(get_node_label(node), color=get_node_color(node))
 
     # Add edges from transitions
     def get_edge_label(trans):
         if trans.get("distr"):
             distr_muls = \
                 [distr
                  if distr[-1] != "_"
@@ -58,15 +70,21 @@
 
     if len(state_data) > 4:
         pos = nx.kamada_kawai_layout(G)
         pos = nx.arf_layout(G, pos=pos)
     else:
         pos = nx.circular_layout(G)
     #pos = nx.multipartite_layout(G)  #requires manual partitioning
-    nx.draw(G, pos, with_labels=True, node_size=500, node_color="skyblue", font_size=10, arrowsize=10)
+    node_colors = [node[1]['color'] for node in G.nodes(data=True)]
+    nx.draw(G, pos,
+            with_labels=True,
+            node_size=500,
+            node_color=node_colors,
+            font_size=12,
+            arrowsize=10)
 
     # Draw full edges with labels
     labels = nx.get_edge_attributes(G, 'param')
     nx.draw_networkx_edge_labels(G, pos, edge_labels=labels, font_size=7)
 
     # Draw dashed edges and label
     dashed_edge_labels = {(edge[0], edge[1]): edge[2] for edge in tms_edges}
```

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/prcc.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/prcc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/sampler_base.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/sampler_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/sensitivity_model_base.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/sensitivity_model_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/output_generator.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/output_generator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/r0calculator.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/r0calculator.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/final_size_calc.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/final_size_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/peak_calc.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/peak_calc.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/sensitivity/target_calc/sol_based/target_calc_base.py` & `epimodel_sensitivity_test-0.1.8/src/sensitivity/target_calc/sol_based/target_calc_base.py`

 * *Files identical despite different names*

### Comparing `epimodel_sensitivity_test-0.1.7/src/simulation_base.py` & `epimodel_sensitivity_test-0.1.8/src/simulation_base.py`

 * *Files identical despite different names*

