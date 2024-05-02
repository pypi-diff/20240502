# Comparing `tmp/pyphetools-0.9.83.tar.gz` & `tmp/pyphetools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.9.83.tar", last modified: Thu May  2 16:26:44 2024, max compression
+gzip compressed data, was "pyphetools-0.9.9.tar", last modified: Wed Dec  6 13:56:54 2023, max compression
```

## Comparing `pyphetools-0.9.83.tar` & `pyphetools-0.9.9.tar`

### file list

```diff
@@ -1,136 +1,103 @@
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.526045 pyphetools-0.9.83/
--rw-r--r--   0 robin      (501) staff       (20)     1079 2024-04-18 06:00:31.000000 pyphetools-0.9.83/LICENSE
--rw-r--r--   0 robin      (501) staff       (20)       39 2024-04-18 06:00:31.000000 pyphetools-0.9.83/MANIFEST.in
--rw-r--r--   0 robin      (501) staff       (20)     3559 2024-05-02 16:26:44.525792 pyphetools-0.9.83/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)      788 2024-04-18 06:00:31.000000 pyphetools-0.9.83/README.md
--rw-r--r--   0 robin      (501) staff       (20)     2204 2024-04-18 06:00:31.000000 pyphetools-0.9.83/pyproject.toml
--rw-r--r--   0 robin      (501) staff       (20)       38 2024-05-02 16:26:44.526103 pyphetools-0.9.83/setup.cfg
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.497321 pyphetools-0.9.83/src/
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.498552 pyphetools-0.9.83/src/pyphetools/
--rw-r--r--   0 robin      (501) staff       (20)      208 2024-05-02 16:26:10.000000 pyphetools-0.9.83/src/pyphetools/__init__.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.509450 pyphetools-0.9.83/src/pyphetools/creation/
--rw-r--r--   0 robin      (501) staff       (20)     2360 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)     1905 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/abstract_encoder.py
--rw-r--r--   0 robin      (501) staff       (20)    11658 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/age_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     3249 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/age_isoformater.py
--rw-r--r--   0 robin      (501) staff       (20)     1690 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/age_of_death_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)      117 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/allelic_requirement.py
--rw-r--r--   0 robin      (501) staff       (20)    23862 2024-04-23 07:50:42.000000 pyphetools-0.9.83/src/pyphetools/creation/case_template_encoder.py
--rw-r--r--   0 robin      (501) staff       (20)      577 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/citation.py
--rw-r--r--   0 robin      (501) staff       (20)    12186 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/cohort_encoder.py
--rw-r--r--   0 robin      (501) staff       (20)     1538 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     2831 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/constant_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)      311 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/constants.py
--rw-r--r--   0 robin      (501) staff       (20)     5501 2024-04-28 05:24:31.000000 pyphetools-0.9.83/src/pyphetools/creation/create_template.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.509701 pyphetools-0.9.83/src/pyphetools/creation/data/
--rw-r--r--   0 robin      (501) staff       (20)     4063 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/data/thresholds.tsv
--rw-r--r--   0 robin      (501) staff       (20)     1053 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/disease.py
--rw-r--r--   0 robin      (501) staff       (20)     1170 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/disease_id_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     5897 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/hgvs_variant.py
--rw-r--r--   0 robin      (501) staff       (20)    11097 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/hp_term.py
--rw-r--r--   0 robin      (501) staff       (20)     1981 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/hpo_cr.py
--rw-r--r--   0 robin      (501) staff       (20)    12852 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/hpo_exact_cr.py
--rw-r--r--   0 robin      (501) staff       (20)     3551 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/hpo_parser.py
--rw-r--r--   0 robin      (501) staff       (20)    14923 2024-05-02 16:22:58.000000 pyphetools-0.9.83/src/pyphetools/creation/import_template.py
--rw-r--r--   0 robin      (501) staff       (20)    21152 2024-04-29 06:05:59.000000 pyphetools-0.9.83/src/pyphetools/creation/individual.py
--rw-r--r--   0 robin      (501) staff       (20)     9204 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/metadata.py
--rw-r--r--   0 robin      (501) staff       (20)     8453 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/option_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)    12588 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/pyphetools_age.py
--rw-r--r--   0 robin      (501) staff       (20)     5770 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/scm_generator.py
--rw-r--r--   0 robin      (501) staff       (20)     3346 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/sex_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     3961 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/simple_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     9179 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/structural_variant.py
--rw-r--r--   0 robin      (501) staff       (20)     1437 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/thresholded_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)    16940 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/thresholder.py
--rw-r--r--   0 robin      (501) staff       (20)     1841 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/variant.py
--rw-r--r--   0 robin      (501) staff       (20)     4897 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/variant_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)    17109 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/variant_manager.py
--rw-r--r--   0 robin      (501) staff       (20)     4122 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/creation/variant_validator.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.510144 pyphetools-0.9.83/src/pyphetools/pp/
--rw-r--r--   0 robin      (501) staff       (20)      231 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)      510 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/_api.py
--rw-r--r--   0 robin      (501) staff       (20)     5115 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/_timestamp.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.510932 pyphetools-0.9.83/src/pyphetools/pp/parse/
--rw-r--r--   0 robin      (501) staff       (20)      571 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)     7493 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/_io.py
--rw-r--r--   0 robin      (501) staff       (20)     3827 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/_pb.py
--rw-r--r--   0 robin      (501) staff       (20)     3123 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/_test_util.py
--rw-r--r--   0 robin      (501) staff       (20)     4034 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/_util.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.511247 pyphetools-0.9.83/src/pyphetools/pp/parse/json/
--rw-r--r--   0 robin      (501) staff       (20)      196 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/json/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)     3061 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/parse/json/_json.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.515273 pyphetools-0.9.83/src/pyphetools/pp/v202/
--rw-r--r--   0 robin      (501) staff       (20)     2004 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)    25795 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_base.py
--rw-r--r--   0 robin      (501) staff       (20)    17708 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_biosample.py
--rw-r--r--   0 robin      (501) staff       (20)     6956 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_disease.py
--rw-r--r--   0 robin      (501) staff       (20)     4506 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_gene_descriptor.py
--rw-r--r--   0 robin      (501) staff       (20)    14116 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_individual.py
--rw-r--r--   0 robin      (501) staff       (20)    18647 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_interpretation.py
--rw-r--r--   0 robin      (501) staff       (20)    17258 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_measurement.py
--rw-r--r--   0 robin      (501) staff       (20)    25682 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_medical_action.py
--rw-r--r--   0 robin      (501) staff       (20)    12638 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_meta_data.py
--rw-r--r--   0 robin      (501) staff       (20)     7863 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_phenopackets.py
--rw-r--r--   0 robin      (501) staff       (20)     6571 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_phenotypic_feature.py
--rw-r--r--   0 robin      (501) staff       (20)      461 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_test_individual.py
--rw-r--r--   0 robin      (501) staff       (20)    20487 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/pp/v202/_vrsatile.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.516745 pyphetools-0.9.83/src/pyphetools/validation/
--rw-r--r--   0 robin      (501) staff       (20)      421 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/validation/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)     2586 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/validation/cohort_validator.py
--rw-r--r--   0 robin      (501) staff       (20)     7798 2024-04-27 11:38:00.000000 pyphetools-0.9.83/src/pyphetools/validation/content_validator.py
--rw-r--r--   0 robin      (501) staff       (20)    12601 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/validation/ontology_qc.py
--rw-r--r--   0 robin      (501) staff       (20)      267 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/validation/phenopacket_validator.py
--rw-r--r--   0 robin      (501) staff       (20)     3170 2024-04-27 10:51:49.000000 pyphetools-0.9.83/src/pyphetools/validation/validated_individual.py
--rw-r--r--   0 robin      (501) staff       (20)    10618 2024-04-27 10:43:24.000000 pyphetools-0.9.83/src/pyphetools/validation/validation_result.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.520125 pyphetools-0.9.83/src/pyphetools/visualization/
--rw-r--r--   0 robin      (501) staff       (20)      566 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/__init__.py
--rw-r--r--   0 robin      (501) staff       (20)     1660 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/counted_hpo_term.py
--rw-r--r--   0 robin      (501) staff       (20)     7040 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/detailed_suppl_table.py
--rw-r--r--   0 robin      (501) staff       (20)     5693 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/focus_count_table.py
--rw-r--r--   0 robin      (501) staff       (20)     2980 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/hpo_category.py
--rw-r--r--   0 robin      (501) staff       (20)    15131 2024-04-29 08:47:00.000000 pyphetools-0.9.83/src/pyphetools/visualization/hpoa_table_creator.py
--rw-r--r--   0 robin      (501) staff       (20)     1366 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/html_table_generator.py
--rw-r--r--   0 robin      (501) staff       (20)     8656 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/individual_table.py
--rw-r--r--   0 robin      (501) staff       (20)     4878 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/onset_calculator.py
--rw-r--r--   0 robin      (501) staff       (20)     3509 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/phenopacket_charts.py
--rw-r--r--   0 robin      (501) staff       (20)     2346 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/phenopacket_ingestor.py
--rw-r--r--   0 robin      (501) staff       (20)     9636 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/phenopacket_table.py
--rw-r--r--   0 robin      (501) staff       (20)     9487 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/qc_visualizer.py
--rw-r--r--   0 robin      (501) staff       (20)     3339 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/simple_age.py
--rw-r--r--   0 robin      (501) staff       (20)     7477 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/simple_patient.py
--rw-r--r--   0 robin      (501) staff       (20)     5823 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/simple_variant.py
--rw-r--r--   0 robin      (501) staff       (20)      569 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/term_count.py
--rw-r--r--   0 robin      (501) staff       (20)     1806 2024-04-18 06:00:31.000000 pyphetools-0.9.83/src/pyphetools/visualization/variant_visualizer.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.524970 pyphetools-0.9.83/src/pyphetools.egg-info/
--rw-r--r--   0 robin      (501) staff       (20)     3559 2024-05-02 16:26:44.000000 pyphetools-0.9.83/src/pyphetools.egg-info/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)     4588 2024-05-02 16:26:44.000000 pyphetools-0.9.83/src/pyphetools.egg-info/SOURCES.txt
--rw-r--r--   0 robin      (501) staff       (20)        1 2024-05-02 16:26:44.000000 pyphetools-0.9.83/src/pyphetools.egg-info/dependency_links.txt
--rw-r--r--   0 robin      (501) staff       (20)        1 2024-04-23 07:45:33.000000 pyphetools-0.9.83/src/pyphetools.egg-info/not-zip-safe
--rw-r--r--   0 robin      (501) staff       (20)      302 2024-05-02 16:26:44.000000 pyphetools-0.9.83/src/pyphetools.egg-info/requires.txt
--rw-r--r--   0 robin      (501) staff       (20)       11 2024-05-02 16:26:44.000000 pyphetools-0.9.83/src/pyphetools.egg-info/top_level.txt
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2024-05-02 16:26:44.523583 pyphetools-0.9.83/test/
--rw-r--r--   0 robin      (501) staff       (20)     5234 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_age_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     2000 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_age_isoformater.py
--rw-r--r--   0 robin      (501) staff       (20)     3379 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_assume_excluded.py
--rw-r--r--   0 robin      (501) staff       (20)     4462 2024-04-27 11:40:32.000000 pyphetools-0.9.83/test/test_cohort_validator.py
--rw-r--r--   0 robin      (501) staff       (20)     1193 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_constant_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)      901 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_disease.py
--rw-r--r--   0 robin      (501) staff       (20)     3214 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_hp_term.py
--rw-r--r--   0 robin      (501) staff       (20)      921 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_hpo_category.py
--rw-r--r--   0 robin      (501) staff       (20)     6683 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_hpo_cr.py
--rw-r--r--   0 robin      (501) staff       (20)      835 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_hpo_parser.py
--rw-r--r--   0 robin      (501) staff       (20)     2057 2024-04-29 06:09:52.000000 pyphetools-0.9.83/test/test_individual.py
--rw-r--r--   0 robin      (501) staff       (20)     2745 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_metadata.py
--rw-r--r--   0 robin      (501) staff       (20)     5857 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_ontology_qc.py
--rw-r--r--   0 robin      (501) staff       (20)     7793 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_option_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)    10163 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_option_column_mapper2.py
--rw-r--r--   0 robin      (501) staff       (20)      844 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_phenopacket_table.py
--rw-r--r--   0 robin      (501) staff       (20)      914 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_pyphetools_age.py
--rw-r--r--   0 robin      (501) staff       (20)     2676 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_simple_age.py
--rw-r--r--   0 robin      (501) staff       (20)     1156 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_simple_variant.py
--rw-r--r--   0 robin      (501) staff       (20)     1474 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_structural_variant.py
--rw-r--r--   0 robin      (501) staff       (20)     2506 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_threshold_column_mapper.py
--rw-r--r--   0 robin      (501) staff       (20)     2696 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_thresholder.py
--rw-r--r--   0 robin      (501) staff       (20)     3566 2024-04-27 11:00:24.000000 pyphetools-0.9.83/test/test_validation_result.py
--rw-r--r--   0 robin      (501) staff       (20)     1391 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_variant.py
--rw-r--r--   0 robin      (501) staff       (20)     2160 2024-04-18 06:00:31.000000 pyphetools-0.9.83/test/test_vital_status.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.420699 pyphetools-0.9.9/
+-rw-r--r--   0 robinp   (904623974) 1088672553     1079 2023-01-08 15:20:15.000000 pyphetools-0.9.9/LICENSE
+-rw-r--r--   0 robinp   (904623974) 1088672553        0 2023-01-05 13:57:40.000000 pyphetools-0.9.9/MANIFEST.in
+-rw-r--r--   0 robinp   (904623974) 1088672553     3109 2023-12-06 13:56:54.420028 pyphetools-0.9.9/PKG-INFO
+-rw-r--r--   0 robinp   (904623974) 1088672553      791 2023-09-30 00:15:51.000000 pyphetools-0.9.9/README.md
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.017914 pyphetools-0.9.9/ppt_venv/
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.100066 pyphetools-0.9.9/ppt_venv/bin/
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      630 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2html.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      750 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2html4.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553     1118 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2html5.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      827 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2latex.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      635 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2man.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      800 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2odt.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553     1762 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      637 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      673 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2s5.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      907 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2xetex.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      638 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2xml.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      706 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rstpep2html.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.419213 pyphetools-0.9.9/pyphetools.egg-info/
+-rw-r--r--   0 robinp   (904623974) 1088672553     3109 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/PKG-INFO
+-rw-r--r--   0 robinp   (904623974) 1088672553     5557 2023-12-06 13:56:54.000000 pyphetools-0.9.9/pyphetools.egg-info/SOURCES.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/dependency_links.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-08-30 08:37:05.000000 pyphetools-0.9.9/pyphetools.egg-info/not-zip-safe
+-rw-r--r--   0 robinp   (904623974) 1088672553       81 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/requires.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553       71 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/top_level.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553     1833 2023-10-12 20:14:59.000000 pyphetools-0.9.9/pyproject.toml
+-rw-r--r--   0 robinp   (904623974) 1088672553       38 2023-12-06 13:56:54.420772 pyphetools-0.9.9/setup.cfg
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.019189 pyphetools-0.9.9/src/
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.337929 pyphetools-0.9.9/src/pyphetools/
+-rw-r--r--   0 robinp   (904623974) 1088672553      180 2023-12-06 13:56:07.000000 pyphetools-0.9.9/src/pyphetools/__init__.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.379289 pyphetools-0.9.9/src/pyphetools/creation/
+-rw-r--r--   0 robinp   (904623974) 1088672553     1871 2023-12-05 15:45:33.000000 pyphetools-0.9.9/src/pyphetools/creation/__init__.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1905 2023-12-02 13:48:44.000000 pyphetools-0.9.9/src/pyphetools/creation/abstract_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7296 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/creation/age_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3249 2023-10-25 06:40:55.000000 pyphetools-0.9.9/src/pyphetools/creation/age_isoformater.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      117 2023-11-16 08:39:03.000000 pyphetools-0.9.9/src/pyphetools/creation/allelic_requirement.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    12272 2023-11-27 12:05:13.000000 pyphetools-0.9.9/src/pyphetools/creation/case_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      577 2023-11-27 12:00:38.000000 pyphetools-0.9.9/src/pyphetools/creation/citation.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    10738 2023-12-02 13:37:26.000000 pyphetools-0.9.9/src/pyphetools/creation/cohort_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      679 2023-10-15 12:30:42.000000 pyphetools-0.9.9/src/pyphetools/creation/column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2401 2023-11-19 06:55:43.000000 pyphetools-0.9.9/src/pyphetools/creation/constant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      310 2023-11-16 08:22:53.000000 pyphetools-0.9.9/src/pyphetools/creation/constants.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      745 2023-11-13 14:50:53.000000 pyphetools-0.9.9/src/pyphetools/creation/disease.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1083 2023-10-16 07:36:08.000000 pyphetools-0.9.9/src/pyphetools/creation/disease_id_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5966 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/creation/hgvs_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    10732 2023-12-05 15:58:54.000000 pyphetools-0.9.9/src/pyphetools/creation/hp_term.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2228 2023-11-29 08:07:02.000000 pyphetools-0.9.9/src/pyphetools/creation/hpo_cr.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    11557 2023-11-29 09:06:11.000000 pyphetools-0.9.9/src/pyphetools/creation/hpo_exact_cr.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2875 2023-10-15 12:52:45.000000 pyphetools-0.9.9/src/pyphetools/creation/hpo_parser.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    16116 2023-12-05 15:58:54.000000 pyphetools-0.9.9/src/pyphetools/creation/individual.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9134 2023-12-03 14:38:15.000000 pyphetools-0.9.9/src/pyphetools/creation/metadata.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     8320 2023-12-06 13:02:45.000000 pyphetools-0.9.9/src/pyphetools/creation/mixed_cohort_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9130 2023-11-29 09:16:36.000000 pyphetools-0.9.9/src/pyphetools/creation/option_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2902 2023-10-15 13:02:16.000000 pyphetools-0.9.9/src/pyphetools/creation/sex_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     6567 2023-12-05 07:36:33.000000 pyphetools-0.9.9/src/pyphetools/creation/simple_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9179 2023-11-19 06:53:20.000000 pyphetools-0.9.9/src/pyphetools/creation/structural_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2949 2023-11-11 21:18:43.000000 pyphetools-0.9.9/src/pyphetools/creation/thresholded_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1841 2023-09-28 17:50:55.000000 pyphetools-0.9.9/src/pyphetools/creation/variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4902 2023-10-14 17:25:22.000000 pyphetools-0.9.9/src/pyphetools/creation/variant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4122 2023-12-06 12:56:24.000000 pyphetools-0.9.9/src/pyphetools/creation/variant_validator.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.386571 pyphetools-0.9.9/src/pyphetools/validation/
+-rw-r--r--   0 robinp   (904623974) 1088672553      421 2023-11-23 07:21:16.000000 pyphetools-0.9.9/src/pyphetools/validation/__init__.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2586 2023-12-02 13:38:25.000000 pyphetools-0.9.9/src/pyphetools/validation/cohort_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7274 2023-11-25 16:19:51.000000 pyphetools-0.9.9/src/pyphetools/validation/content_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9158 2023-12-05 07:42:45.000000 pyphetools-0.9.9/src/pyphetools/validation/ontology_qc.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      267 2023-10-25 07:05:50.000000 pyphetools-0.9.9/src/pyphetools/validation/phenopacket_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2735 2023-12-05 13:38:24.000000 pyphetools-0.9.9/src/pyphetools/validation/validated_individual.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    10081 2023-12-05 14:01:30.000000 pyphetools-0.9.9/src/pyphetools/validation/validation_result.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.393993 pyphetools-0.9.9/src/pyphetools/visualization/
+-rw-r--r--   0 robinp   (904623974) 1088672553      416 2023-11-14 11:38:23.000000 pyphetools-0.9.9/src/pyphetools/visualization/__init__.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7040 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/detailed_suppl_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5693 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/focus_count_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2980 2023-09-18 21:32:39.000000 pyphetools-0.9.9/src/pyphetools/visualization/hpo_category.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7303 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/hpoa_table_creator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1366 2023-11-20 07:10:51.000000 pyphetools-0.9.9/src/pyphetools/visualization/html_table_generator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1694 2023-11-19 06:46:01.000000 pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_ingestor.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9526 2023-12-02 12:27:50.000000 pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9620 2023-12-05 13:29:54.000000 pyphetools-0.9.9/src/pyphetools/visualization/qc_visualizer.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     6987 2023-11-19 09:19:38.000000 pyphetools-0.9.9/src/pyphetools/visualization/simple_patient.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5840 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/simple_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      569 2023-09-18 21:32:39.000000 pyphetools-0.9.9/src/pyphetools/visualization/term_count.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.418473 pyphetools-0.9.9/test/
+-rw-r--r--   0 robinp   (904623974) 1088672553     4766 2023-11-12 16:12:40.000000 pyphetools-0.9.9/test/test_age_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2003 2023-10-25 06:44:57.000000 pyphetools-0.9.9/test/test_age_isoformater.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3026 2023-11-14 10:48:33.000000 pyphetools-0.9.9/test/test_assume_excluded.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4522 2023-11-27 12:05:56.000000 pyphetools-0.9.9/test/test_case_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4075 2023-12-05 09:09:58.000000 pyphetools-0.9.9/test/test_cohort_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1160 2023-11-19 06:54:43.000000 pyphetools-0.9.9/test/test_constant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3879 2023-12-05 16:11:01.000000 pyphetools-0.9.9/test/test_hp_term.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      925 2023-09-18 21:32:39.000000 pyphetools-0.9.9/test/test_hpo_category.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     6687 2023-11-29 08:47:33.000000 pyphetools-0.9.9/test/test_hpo_cr.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      839 2023-09-18 00:23:19.000000 pyphetools-0.9.9/test/test_hpo_parser.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2749 2023-11-27 12:08:08.000000 pyphetools-0.9.9/test/test_metadata.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5355 2023-12-05 09:07:49.000000 pyphetools-0.9.9/test/test_ontology_qc.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7443 2023-11-19 07:48:16.000000 pyphetools-0.9.9/test/test_option_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9551 2023-11-29 09:12:50.000000 pyphetools-0.9.9/test/test_option_column_mapper2.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      848 2023-11-20 21:20:20.000000 pyphetools-0.9.9/test/test_phenopacket_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1164 2023-10-02 00:47:18.000000 pyphetools-0.9.9/test/test_simple_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1478 2023-11-19 06:41:10.000000 pyphetools-0.9.9/test/test_structural_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1860 2023-09-18 00:23:19.000000 pyphetools-0.9.9/test/test_threshold_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3229 2023-12-05 14:03:30.000000 pyphetools-0.9.9/test/test_validation_result.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1395 2023-11-12 16:02:14.000000 pyphetools-0.9.9/test/test_variant.py
```

### Comparing `pyphetools-0.9.83/LICENSE` & `pyphetools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/PKG-INFO` & `pyphetools-0.9.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.9.83
+Version: 0.9.9
 Summary: Generate and work with GA4GH phenopackets
-Author-email: Peter Robinson <peter.robinson@bih-charite.de>, Daniel Danis <daniel.gordon.danis@protonmail.com>
+Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,30 +32,24 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hpo-toolkit<0.6.0,>=0.5.0
-Requires-Dist: matplotlib<4.0,>=3.2.0
-Requires-Dist: pandas[excel]<3.0.0,>=2.0.0
-Requires-Dist: phenopackets>=2.0.2
-Requires-Dist: protobuf<4.0.0,>=3.15.0
-Requires-Dist: requests<3.0,>=2.25.0
+Requires-Dist: hpo-toolkit>=0.3.0
+Requires-Dist: openpyxl
+Requires-Dist: pandas
+Requires-Dist: phenopackets
+Requires-Dist: protobuf
+Requires-Dist: requests
 Provides-Extra: test
-Requires-Dist: pytest<8.0.0,>=7.0.0; extra == "test"
-Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]<10,>=9.5.10; extra == "docs"
-Requires-Dist: mkdocs-material-extensions<2.0,>=1.3; extra == "docs"
-Requires-Dist: mkdocstrings[python]<1.0,>=0.22; extra == "docs"
-Requires-Dist: pillow; extra == "docs"
-Requires-Dist: cairosvg; extra == "docs"
+Requires-Dist: pytest; extra == "test"
 
-[![CI](https://github.com/monarch-initiative/pyphetools/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
+[![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
 
 # pyphetools
 Python Phenopacket Tools
 
 This package currently is designed to test how to use the Python version of the phenopackets package together with pandas to create phenopackets from typical supplemental tables.
 
 Development goals include making builder code similar to the Java package to create valid phenopackets and to perform JSON Schema-based validation.
```

### Comparing `pyphetools-0.9.83/README.md` & `pyphetools-0.9.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![CI](https://github.com/monarch-initiative/pyphetools/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
+[![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
 
 # pyphetools
 Python Phenopacket Tools
 
 This package currently is designed to test how to use the Python version of the phenopackets package together with pandas to create phenopackets from typical supplemental tables.
 
 Development goals include making builder code similar to the Java package to create valid phenopackets and to perform JSON Schema-based validation.
```

### Comparing `pyphetools-0.9.83/pyproject.toml` & `pyphetools-0.9.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,78 +1,68 @@
 # pyproject.toml
 
 [build-system]
 requires = ["setuptools>=65.6.3", "wheel"]
 build-backend = "setuptools.build_meta"
 
+
+[tool.setuptools.packages.find]
+where = [".","src"]
+exclude = ["notebooks", "test"]
+
 [project]
 name = "pyphetools"
+# version in __init__
 requires-python = ">=3.8"
 description = "Generate and work with GA4GH phenopackets"
 readme = "README.md"
 authors = [
-    {name = "Peter Robinson", email="peter.robinson@bih-charite.de"},
-    {name = "Daniel Danis", email="daniel.gordon.danis@protonmail.com"},
-]
+    {name = "Peter Robinson", email="peter.robinson@jax.org"},
+     ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 keywords = [
     "Global Alliance for Genomics and Health",
     "GA4GH Phenopacket Schema",
     "Human Phenotype Ontology",
     "GA4GH",
     "HPO"]
-
-# version in __init__
-dynamic = ["version"]
-
 dependencies = [
-    "hpo-toolkit>=0.5.0,<0.6.0",
-    "matplotlib>=3.2.0,<4.0",
-    "pandas[excel]>=2.0.0,<3.0.0",  # We want to parse Excel files.
-    "phenopackets>=2.0.2",
-    "protobuf>=3.15.0,<4.0.0",
-    "requests>=2.25.0,<3.0",
+    "hpo-toolkit>=0.3.0",
+    "openpyxl",
+    "pandas",
+    "phenopackets",
+    "protobuf",
+    "requests"
 ]
-
+dynamic = ["version"]
 [project.optional-dependencies]
-test = ["pytest>=7.0.0,<8.0.0"]
-docs = [
-    'mkdocs-material[imaging]>=9.5.10,<10',
-    'mkdocs-material-extensions>=1.3,<2.0',
-    'mkdocstrings[python]>=0.22,<1.0',
-    'pillow',
-    'cairosvg',
-]
+test = ["pytest"]
 
 
 [project.urls]
 homepage = "https://github.com/monarch-initiative/pyphetools"
 repository = "https://github.com/monarch-initiative/pyphetools.git"
 documentation = "https://github.com/monarch-initiative/pyphetools"
 bugtracker = "https://github.com/monarch-initiative/pyphetools/issues"
 
 
+
+
 [tool.setuptools]
-package-dir = { "" = "src" }
+package-dir = { "" = "." }
 zip-safe = false
-
 [tool.setuptools.dynamic]
 version = { attr = "pyphetools.__version__" }
 
-
-# See MANIFEST.in for the list of the data files
-# being included in the package.
-
-
 [tool.yapf]
 blank_line_before_nested_class_or_def = true
 column_limit = 88
 
 [tool.pylint]
 max-line-length = 88
 disable = [
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/__init__.py` & `pyphetools-0.9.9/src/pyphetools/creation/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,40 @@
 from .age_column_mapper import AgeColumnMapper
 from .age_isoformater import AgeIsoFormater
-from .age_of_death_mapper import AgeOfDeathColumnMapper
 from .allelic_requirement import AllelicRequirement
-from .case_template_encoder import CaseTemplateEncoder
+from .case_encoder import CaseEncoder
 from .citation import Citation
 from .cohort_encoder import CohortEncoder
 from .column_mapper import ColumnMapper
 from .constant_column_mapper import ConstantColumnMapper
-from .create_template import TemplateCreator
 from .disease import Disease
 from .disease_id_column_mapper import DiseaseIdColumnMapper
 from .hgvs_variant import HgvsVariant
 from .hpo_cr import HpoConceptRecognizer
 from .hpo_exact_cr import HpoExactConceptRecognizer
 from .hpo_parser import HpoParser
 from .hp_term import HpTerm, HpTermBuilder
-from .import_template import TemplateImporter
 from .individual import Individual
 from .metadata import MetaData
+from .mixed_cohort_encoder import MixedCohortEncoder
 from .option_column_mapper import OptionColumnMapper
-from .pyphetools_age import PyPheToolsAge, IsoAge, HpoAge, GestationalAge, HPO_ONSET_TERMS
 from .sex_column_mapper import SexColumnMapper
-from .simple_column_mapper import SimpleColumnMapper
-from .scm_generator import SimpleColumnMapperGenerator
+from .simple_column_mapper import SimpleColumnMapper, SimpleColumnMapperGenerator
 from .structural_variant import StructuralVariant
 from .thresholded_column_mapper import ThresholdedColumnMapper
-from .thresholder import Thresholder
-from .variant import Variant
-from .variant_column_mapper import VariantColumnMapper
-from .variant_manager import VariantManager
 from .variant_validator import VariantValidator
-
+from .variant_column_mapper import VariantColumnMapper
+from .variant import Variant
 
 
 __all__ = [
     "AgeColumnMapper",
     "AgeIsoFormater",
-    "AgeOfDeathColumnMapper",
     "AllelicRequirement",
-    "CaseTemplateEncoder",
+    "CaseEncoder",
     "Citation",
     "CohortEncoder",
     "ColumnMapper",
     "ConstantColumnMapper",
     "ColumnMapper",
     "Disease",
     "DiseaseIdColumnMapper",
@@ -50,22 +42,18 @@
     "HpoConceptRecognizer",
     "HpoExactConceptRecognizer",
     "HpoParser",
     "HpTerm",
     "HpTermBuilder",
     "Individual",
     "MetaData",
+    "MixedCohortEncoder",
     "OptionColumnMapper",
-    "PyPheToolsAge", "IsoAge", "HpoAge", "GestationalAge", "HPO_ONSET_TERMS",
     "SexColumnMapper",
     "SimpleColumnMapper",
     "SimpleColumnMapperGenerator",
     "StructuralVariant",
-    "TemplateCreator",
-    "TemplateImporter",
     "ThresholdedColumnMapper",
-    "Thresholder",
-    "Variant",
-    "VariantColumnMapper",
-    "VariantManager",
     "VariantValidator",
+    "VariantColumnMapper",
+    "Variant"
 ]
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/abstract_encoder.py` & `pyphetools-0.9.9/src/pyphetools/creation/abstract_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/age_isoformater.py` & `pyphetools-0.9.9/src/pyphetools/creation/age_isoformater.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/citation.py` & `pyphetools-0.9.9/src/pyphetools/creation/citation.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.9.9/src/pyphetools/creation/cohort_encoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import pandas as pd
 from math import isnan
 from typing import Dict, List
 
 from .abstract_encoder import AbstractEncoder
 from .age_column_mapper import AgeColumnMapper
 from .citation import Citation
-from .column_mapper import ColumnMapper
 from .constants import Constants
 from .disease import Disease
 from .hpo_cr import HpoConceptRecognizer
 from .individual import Individual
-from .pyphetools_age import NoneAge
 from .sex_column_mapper import SexColumnMapper
 from .variant_column_mapper import VariantColumnMapper
 
 
 class CohortEncoder(AbstractEncoder):
     """Map a table of data to Individual/GA4GH Phenopacket Schema objects
 
@@ -24,95 +22,93 @@
 
     The column_mapper_d is a dictionary with key=column names, and value=Mapper objects. These mappers are responsible
     for mapping HPO terms. The agemapper and the sexmapper are specialized for the respective columns. The
     variant mapper is useful if there is a single variant column that is all HGVS or structural variants. In some
     cases, it is preferable to use the variant_dictionary, which has key=string (cell contents) and value=Hgvs or
     StructuralVariant object.
 
-    :param df: tabular data about a cohort
+    :param df: tabular data abotu a cohort
     :type df: pd.DataFrame
     :param hpo_cr: HpoConceptRecognizer for text mining
     :type hpo_cr: pyphetools.creation.HpoConceptRecognizer
-    :param column_mapper_list: list of ColumnMapper objects
-    :type column_mapper_list: List[pyphetools.creation.ColumnMapper]
+    :param column_mapper_d: Dictionary with key: Column name, value: ColumnMapper object
+    :type column_mapper_d: Dict[pyphetools.creation.ColumnMapper]
     :param individual_column_name: label of column with individual/proband/patient identifier
     :type individual_column_name: str
     :param metadata: GA4GH MetaData object
     :type metadata: PPkt.MetaData
-    :param age_of_onset_mapper:Mapper for the Age of onset column. Defaults to AgeColumnMapper.not_provided()
-    :type age_of_onset_mapper: pyphetools.creation.AgeColumnMapper
-    :param age_at_last_encounter_mapper:Mapper for the Age at last clinical encounter column. Defaults to AgeColumnMapper.not_provided()
-    :type age_at_last_encounter_mapper: pyphetools.creation.AgeColumnMapper
+    :param agemapper:Mapper for the Age column. Defaults to AgeColumnMapper.not_provided()
+    :type agemapper: pyphetools.creation.AgeColumnMapper
     :param sexmapper: Mapper for the Sex column. Defaults to SexColumnMapper.not_provided().
     :type sexmapper: pyphetools.creation.SexColumnMapper
     :param variant_mapper: column mapper for HGVS-encoded variant column.
     :type variant_mapper: pyphetools.creation.VariantColumnMapper
     :raises: ValueError - several of the input arguments are checked.
     """
 
     def __init__(self,
-                df:pd.DataFrame,
-                hpo_cr: HpoConceptRecognizer,
-                column_mapper_list:List[ColumnMapper],
-                individual_column_name:str,
+                df,
+                hpo_cr,
+                column_mapper_d,
+                individual_column_name,
                 metadata,
-                age_of_onset_mapper:AgeColumnMapper=AgeColumnMapper.not_provided(),
-                age_at_last_encounter_mapper:AgeColumnMapper=AgeColumnMapper.not_provided(),
-                sexmapper:SexColumnMapper=SexColumnMapper.not_provided(),
-                variant_mapper:VariantColumnMapper=None,
-                delimiter:str=None):
+                agemapper=AgeColumnMapper.not_provided(),
+                sexmapper=SexColumnMapper.not_provided(),
+                variant_mapper=None,
+                delimiter=None):
         """Constructor
         """
         super().__init__(metadata=metadata)
         if not isinstance(hpo_cr, HpoConceptRecognizer):
             raise ValueError(
                 "concept_recognizer argument must be HpoConceptRecognizer but was {type(concept_recognizer)}")
         self._hpo_concept_recognizer = hpo_cr
         if not isinstance(df, pd.DataFrame):
             raise ValueError(f"df argument must be pandas data frame but was {type(df)}")
-        if not isinstance(column_mapper_list, list):
-            raise ValueError(f"column_mapper_list argument must be a list but was {type(column_mapper_list)}")
+        if not isinstance(column_mapper_d, dict):
+            raise ValueError(f"column_mapper_d argument must be a dictionary but was {type(column_mapper_d)}")
         if not isinstance(individual_column_name, str):
             raise ValueError(f"individual_column_name argument must be a string but was {type(individual_column_name)}")
         if variant_mapper is not None and not isinstance(variant_mapper, VariantColumnMapper):
             raise ValueError(f"variant_mapper argument must be VariantColumnMapper but was {type(variant_mapper)}")
         self._df = df.astype(str)
-        self._column_mapper_list = column_mapper_list
+        self._column_mapper_d = column_mapper_d
         self._id_column_name = individual_column_name
-        self._age_of_onset_mapper = age_of_onset_mapper
-        self._age_at_last_encounter_mapper = age_at_last_encounter_mapper
+        self._age_mapper = agemapper
         self._sex_mapper = sexmapper
         self._disease = None
         self._variant_mapper = variant_mapper
         self._disease_dictionary = None
         self._delimiter = delimiter
+        ontology = hpo_cr.get_hpo_ontology()
+        if ontology is None:
+            raise ValueError("ontology cannot be None")
 
     def preview_dataframe(self):
         """
         Generate a dataframe with a preview of the parsed contents
 
         :returns: a DataFrame representing the cohort to check results
         :rtype: pd.DataFrame
         """
         df = self._df.reset_index()  # make sure indexes pair with number of rows
         individuals = []
-        age_column_name = self._age_of_onset_mapper.get_column_name()
+        age_column_name = self._age_mapper.get_column_name()
         sex_column_name = self._sex_mapper.get_column_name()
         for index, row in df.iterrows():
             individual_id = row[self._id_column_name]
             if age_column_name == Constants.NOT_PROVIDED:
                 age = Constants.NOT_PROVIDED
             else:
                 age_cell_contents = row[age_column_name]
                 age = self._age_mapper.map_cell(age_cell_contents)
             sex_cell_contents = row[sex_column_name]
             sex = self._sex_mapper.map_cell(sex_cell_contents)
             hpo_terms = []
-            for column_mapper in self.__column_mapper_list:
-                column_name = column_mapper.get_column_name()
+            for column_name, column_mapper in self._column_mapper_d.items():
                 cell_contents = row[column_name]
                 # Empty cells are often represented as float non-a-number by Pandas
                 if isinstance(cell_contents, float) and isnan(cell_contents):
                     continue
                 terms = column_mapper.map_cell(row[column_name])
                 hpo_terms.extend(terms)
             hpo_string = "\n".join([h.to_string() for h in hpo_terms])
@@ -139,60 +135,48 @@
 
         For tables with multiple different diseases, we provide a dictionary that has as key
         the string used in the original table and as value
         """
         self._disease_dictionary = disease_d
         self._disease = None
 
-
-    def _get_age(row:pd.Series, mapper:AgeColumnMapper):
-        import math
-        column_name = mapper.get_column_name()
-        if column_name == Constants.NOT_PROVIDED:
-            return NoneAge("na")
-        age_cell_contents = row[column_name]
-        if isinstance(age_cell_contents, float) and math.isnan(age_cell_contents):
-            return NoneAge("na")
-        try:
-            age = mapper.map_cell(age_cell_contents)
-        except Exception as ee:
-            print(f"Warning: Could not parse age {ee}. Setting age to \"not provided\"")
-            age = NoneAge("na")
-        return age
-
-
     def get_individuals(self) -> List[Individual]:
         """Get a list of all Individual objects in the cohort
 
         :returns: a list of all Individual objects in the cohort
         :rtype: List[Individual]
         """
-        # make sure indexes pair with number of rows, if needed
-        if not self._df.index.name in self._df.columns:
-            df = self._df.reset_index()
+        df = self._df.reset_index()  # make sure indexes pair with number of rows
         individuals = []
+        age_column_name = self._age_mapper.get_column_name()
         sex_column_name = self._sex_mapper.get_column_name()
         if self._variant_mapper is None:
             variant_colname = None
             genotype_colname = None
         else:
             variant_colname = self._variant_mapper.get_variant_column_name()
             genotype_colname = self._variant_mapper.get_genotype_colname()
         for index, row in df.iterrows():
             individual_id = row[self._id_column_name]
-            age_of_onset = CohortEncoder._get_age(row, self._age_of_onset_mapper)
-            age_last_encounter = CohortEncoder._get_age(row, self._age_at_last_encounter_mapper)
+            if age_column_name == Constants.NOT_PROVIDED:
+                age = Constants.NOT_PROVIDED
+            else:
+                age_cell_contents = row[age_column_name]
+                try:
+                    age = self._age_mapper.map_cell(age_cell_contents)
+                except Exception as ee:
+                    print(f"Warning: Could not parse age {ee}. Setting age to \"not provided\"")
+                    age = Constants.NOT_PROVIDED
             if sex_column_name == Constants.NOT_PROVIDED:
                 sex = self._sex_mapper.map_cell(Constants.NOT_PROVIDED)
             else:
                 sex_cell_contents = row[sex_column_name]
                 sex = self._sex_mapper.map_cell(sex_cell_contents)
             hpo_terms = []
-            for column_mapper in self._column_mapper_list:
-                column_name = column_mapper.get_column_name()
+            for column_name, column_mapper in self._column_mapper_d.items():
                 if column_name not in df.columns:
                     raise ValueError(f"Did not find column name '{column_name}' in dataframe -- check spelling!")
                 cell_contents = row[column_name]
                 # Empty cells are often represented as float non-a-number by Pandas
                 if isinstance(cell_contents, float) and isnan(cell_contents):
                     continue
                 terms = column_mapper.map_cell(cell_contents)
@@ -211,32 +195,24 @@
                 interpretation_list = []
             if self._disease_dictionary is not None and self._disease is None:
                 if individual_id not in self._disease_dictionary:
                     raise ValueError(f"Could not find disease link for {individual_id}")
                 disease = self._disease_dictionary.get(individual_id)
                 indi = Individual(individual_id=individual_id,
                                 sex=sex,
-                                age_of_onset=age_of_onset,
-                                age_at_last_encounter=age_last_encounter,
+                                age=age,
                                 hpo_terms=hpo_terms,
                                 citation=self._metadata.get_citation(),
                                 interpretation_list=interpretation_list,
                                 disease=disease)
             elif self._disease_dictionary is None and self._disease is not None:
                 indi = Individual(individual_id=individual_id,
                                 sex=sex,
-                                age_of_onset=age_of_onset,
-                                age_at_last_encounter=age_last_encounter,
+                                age=age,
                                 hpo_terms=hpo_terms,
                                 citation=self._metadata.get_citation(),
                                 interpretation_list=interpretation_list,
                                 disease=self._disease)
             else:
                 raise ValueError(f"Could not find disease data for '{individual_id}'")
             individuals.append(indi)
-        if self._age_of_onset_mapper.has_error():
-            print(self._age_of_onset_mapper.error_summary())
-        if self._age_at_last_encounter_mapper.has_error():
-            print(self._age_at_last_encounter_mapper.error_summary())
-        if self._sex_mapper.has_error():
-            print(self._sex_mapper.error_summary())
         return individuals
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/constant_column_mapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from typing import List
 import pandas as pd
-from collections import defaultdict
 from .column_mapper import ColumnMapper
 from .hp_term import HpTerm
 
 
 class ConstantColumnMapper(ColumnMapper):
     """Column mapper for cases in which all patients have an (optionally excluded) HPO term.
-    :param column_name: name of the column in the pandas DataFrame
-    :type column_name: str
+
     :param hpo_id: HPO  id, e.g., HP:0004321
     :type hpo_id: str
     :param hpo_label: Corresponding term label
     :type hpo_label: str
     :param term_list: list of lists with [label, hpo_id
     :type term_list: List[lst]
     :param excluded: if True, then all individuals had this feature explicitly excluded
     :type excluded: bool
     """
-    def __init__(self, column_name,  hpo_id=None, hpo_label=None, term_list=None, excluded:bool=False) -> None:
+    def __init__(self, hpo_id=None, hpo_label=None, term_list=None, excluded:bool=False) -> None:
 
-        super().__init__(column_name=column_name)
+        super().__init__()
         self._hpo_id = hpo_id
         if hpo_id is None and hpo_label is None and term_list is not None:
             self._hpo_terms = []
             for term in term_list:
                 if excluded:
                     hpoterm = HpTerm(label=term[0], hpo_id=term[1], observed=False)
                 else:
@@ -47,23 +45,16 @@
             cell_contents (str): not used, can be None or any other value
 
         Returns:
             List[HpTerm]: list of HPO terms
         """
         return self._hpo_terms
 
-    def preview_column(self, df:pd.DataFrame) -> pd.DataFrame:
-        if not isinstance(df, pd.DataFrame):
-            raise ValueError("df argument must be pandas DataFrame, but was {type(column)}")
-        mapping_counter = defaultdict(int)
-
+    def preview_column(self, column) -> pd.DataFrame:
+        if not isinstance(column, pd.Series):
+            raise ValueError("column argument must be pandas Series, but was {type(column)}")
         dlist = []
-        column = df[self._column_name]
         for _, value in column.items():
             display = ";".join(hpterm.display_value for hpterm in self._hpo_terms)
-            display = f"{value} -> {display}"
-            mapping_counter[display] +=1
-        for k, v in mapping_counter.items():
-            d = {"mapping": k, "count": str(v)}
-            dlist.append(d)
+            dlist.append(display)
         return pd.DataFrame(dlist)
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/disease.py` & `pyphetools-0.9.9/src/pyphetools/creation/disease.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     :param disease_id: a CURIE such as OMIM:600324
     :type disease_id: str
     :param disease_label: the name of the disease
     :type disease_label: str
     """
 
     def __init__(self, disease_id:str, disease_label):
-        if " " in disease_id:
-            raise ValueError(f"Malformed disease identifier with white space: \"{disease_id}\"")
-        if disease_label.startswith(" ") or disease_label.endswith(" "):
-            raise ValueError(f"Malformed disease label (starts/ends with whitespace): \"{disease_label}\"")
         self._id = disease_id
         self._label = disease_label
 
 
     @property
     def id(self):
         return self._id
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/disease_id_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/disease_id_column_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,13 @@
         """
         :param cell_contents: contents of a cell of the origiinal table
         :type cell_contents: str
         :returns: corresponding Disease object
         :rtype: Disease
         :raises: ValueError if the cell contents cannot be mapped
         """
-        disease_id = str(cell_contents) # sometime pandas give us an int or an object
-        if disease_id not in self._disease_id_dict:
-            raise ValueError(f"Could not map disease \"{cell_contents}\"")
+        if cell_contents not in self._disease_id_dict:
+            raise ValueError(f"Could not map disease {cell_contents}")
         return self._disease_id_dict.get(cell_contents)
 
     def get_column_name(self):
         return self._column_name
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/hgvs_variant.py` & `pyphetools-0.9.9/src/pyphetools/creation/hgvs_variant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import phenopackets
+import phenopackets 
 from .variant import Variant
 import string
 from typing import Dict
 import random
 
 ACCEPTABLE_GENOMES = {"GRCh37", "GRCh38", "hg19", "hg38"}
 
@@ -47,82 +47,82 @@
         self._transcript = transcript
         self._g_hgvs = g_hgvs
         self._genotype = None
         if variant_id is None:
             self._variant_id = "var_" + "".join(random.choices(string.ascii_letters, k=25))
         else:
             self._variant_id = variant_id
-
+        
     @property
     def assembly(self):
         return self._assembly
-
+        
     @property
     def chr(self):
         return self._chr
-
+        
     @property
     def position(self):
         return self._position
-
+        
     @property
     def ref(self):
         return self._ref
-
+        
     @property
     def alt(self):
         return self._alt
-
+    
     @property
     def genotype(self):
         return self._genotype
-
+          
     def __str__(self):
-        return f"{self._hgvs}({self._chr}:{self._position}{self._ref}>{self._alt})"
-
+        return f"{self._chr}:{self._position}{self._ref}>{self._alt}"
+    
     def to_string(self):
         return self.__str__()
-
+    
     def to_ga4gh_variant_interpretation(self, acmg=None):
         """For the new interface. Refactor client code to use this function, which has an unambiguous name
         """
         return self.to_ga4gh(acmg=acmg)
-
+    
     def to_ga4gh(self, acmg=None):
         """
         Transform this Variant object into a "variantInterpretation" message of the GA4GH Phenopacket schema
         """
         vdescriptor = phenopackets.VariationDescriptor()
         vdescriptor.id = self._variant_id
         if self._hgnc_id is not None and self._symbol is not None:
             vdescriptor.gene_context.value_id = self._hgnc_id
             vdescriptor.gene_context.symbol = self._symbol
         hgvs_expression = phenopackets.Expression()
         if self._hgvs is not None:
             hgvs_expression.syntax = "hgvs.c"
             hgvs_expression.value = self._hgvs
-            vdescriptor.expressions.append(hgvs_expression)
-        if self._g_hgvs is not None:
+            vdescriptor.expressions.append(hgvs_expression) 
+        if self._g_hgvs is not None: 
             hgvs_expression.syntax = "hgvs.g"
             hgvs_expression.value = self._g_hgvs
-            vdescriptor.expressions.append(hgvs_expression)
+            vdescriptor.expressions.append(hgvs_expression) 
         vdescriptor.molecule_context =  phenopackets.MoleculeContext.genomic
         if self._genotype is not None:
             if self._genotype == 'heterozygous':
                 vdescriptor.allelic_state.id = "GENO:0000135"
                 vdescriptor.allelic_state.label = "heterozygous"
             elif self._genotype == 'homozygous':
                 vdescriptor.allelic_state.id = "GENO:0000136"
-                vdescriptor.allelic_state.label = "homozygous"
+                vdescriptor.allelic_state.label = "homozygous" 
             elif self._genotype == 'hemizygous':
                 vdescriptor.allelic_state.id = "GENO:0000134"
-                vdescriptor.allelic_state.label = "hemizygous"
+                vdescriptor.allelic_state.label = "hemizygous" 
             else:
-                print(f"Did not recognize genotype {self._genotype}")
-        vinterpretation = phenopackets.VariantInterpretation()
+                print(f"Did not recognize genotype {self._genotype}")  
+        vinterpretation = phenopackets.VariantInterpretation() 
         if acmg is not None:
             if acmg.lower() == 'benign':
                 vinterpretation.acmgPathogenicityClassification = phenopackets.AcmgPathogenicityClassification.BENIGN
             elif acmg.lower == 'likely benign' or acmg.lower() == 'likely_benign':
                 vinterpretation.acmgPathogenicityClassification = phenopackets.AcmgPathogenicityClassification.LIKELY_BENIGN
             elif acmg.lower == 'uncertain significance' or acmg.lower() == 'uncertain_significance':
                 vinterpretation.acmgPathogenicityClassification = phenopackets.AcmgPathogenicityClassification.UNCERTAIN_SIGNIFICANCE
@@ -137,7 +137,8 @@
         vcf_record.chrom = self._chr
         vcf_record.pos = self._position
         vcf_record.ref = self._ref
         vcf_record.alt = self._alt
         vdescriptor.vcf_record.CopyFrom(vcf_record)
         vinterpretation.variation_descriptor.CopyFrom(vdescriptor)
         return vinterpretation
+
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/hp_term.py` & `pyphetools-0.9.9/src/pyphetools/creation/hp_term.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import phenopackets as PPKt
 from .constants import Constants
-from .pyphetools_age import HpoAge, IsoAge, NoneAge, PyPheToolsAge
 import hpotk
 
 class HpTerm:
     """
     Class to represent a phenotypic observation as an HPO term with optional modifiers
 
     :param hpo_id: a Human Phenotype Ontology (HPO) identifier such as HP:0001166
@@ -17,154 +16,155 @@
     :param measured: a boolean that indicates whether the HPO was measured (True) or not explicitly measured (False)
     :type measured: bool
     :param onset: an ISO8601 string representing the age of onset, optional
     :type onset: str
     :param resolution: an ISO8601 string representing the age of resolution, optional
     :type resolution: str
     """
-    def __init__(self, hpo_id:str, label:str, observed:bool=True, measured:bool=True, onset=NoneAge("na"), resolution=NoneAge("na")):
+    def __init__(self, hpo_id, label, observed=True, measured=True, onset=Constants.NOT_PROVIDED, onset_term=None, resolution=None):
         if hpo_id is None or len(hpo_id) == 0 or not hpo_id.startswith("HP"):
             raise ValueError(f"invalid id argument: '{hpo_id}'")
         if label is None or len(label) == 0:
             raise ValueError(f"invalid label argument: '{label}'")
         self._id = hpo_id
         self._label = label
         self._observed = observed
         self._measured = measured
-        if not isinstance(onset, PyPheToolsAge):
-            raise ValueError(f"onset argument must be PyPheToolsAge or subclass but was {type(onset)}")
-        self._onset = onset
-        self._resolution = resolution
+        if onset is None:
+            self._onset = Constants.NOT_PROVIDED
+        else:
+            self._onset = onset
+        self._onset_term = onset_term
+        if resolution is None:
+            self._resolution = Constants.NOT_PROVIDED
+        else:
+            self._resolution = resolution
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self._id == other._id and self._label == other._label and self._measured == other._measured and self._onset == other._onset and self._resolution == other._resolution
         else:
             return NotImplemented
 
     def __hash__(self):
         return hash((self._id, self._label, self._observed, self._measured, self._onset, self._resolution))
 
     @property
-    def id(self) -> str:
+    def id(self):
         """
         :returns: The HPO identifier, e.g., HP:0001166
         :rtype: str
         """
         return self._id
 
     @property
-    def label(self) -> str:
+    def label(self):
         """
         :returns: The HPO label, e.g., Arachnodactyly
         :rtype: str
         """
         return self._label
 
     @property
-    def observed(self) -> bool:
-        """
-        :returns: True if this feature was observed (i.e., present)
-        :rtype: bool
-        """
+    def observed(self):
         return self._observed
 
     @property
-    def measured(self) -> bool:
+    def measured(self):
         """
         :returns: True iff a measurement to assess this abnormality (HpTerm) was performed
         :rtype: bool
         """
         return self._measured
 
     @property
-    def onset(self) -> PyPheToolsAge:
+    def onset(self):
         """
-        :returns: A PyPheToolsAge object representing the age this abnormality first was observed
-        :rtype: PyPheToolsAge
+        :returns: iso8601 string representing the age this abnormality first was observed
+        :rtype: str, optional
         """
         return self._onset
 
-    def set_onset(self, onset:PyPheToolsAge) -> None:
-        if not isinstance(onset, PyPheToolsAge):
-            raise ValueError(f"argument of set_onset but be PyPheToolsAge but was {type(onset)}")
+    def set_onset(self, onset):
         self._onset = onset
 
+    @property
+    def onset_term(self):
+        return self._onset_term
 
     @property
-    def resolution(self) -> PyPheToolsAge:
+    def resolution(self):
         """
-        :returns: A PyPheToolsAge object representing the age this abnormality resolved
-        :rtype: PyPheToolsAge
+        :returns: iso8601 string representing the age this abnormality resolved
+        :rtype: str, optional
         """
         return self._resolution
 
     @property
-    def display_value(self) -> str:
+    def display_value(self):
         """
         :returns: One of three strings describing the status of the term: "not measured", "excluded", or "observed"
         :rtype: str
         """
         if not self._measured:
             return "not measured"
         if not self._observed:
             return "excluded"
         else:
             return "observed"
 
     @property
-    def hpo_term_and_id(self) -> str:
+    def hpo_term_and_id(self):
         """
         :returns: A string such as Arachnodactyly (HP:0001166) for display
         :rtype: str
         """
         return f"{self._label} ({self._id})"
 
-    def _term_and_id_with_onset(self) -> str:
-        if self._onset is not None and self._onset.is_valid():
-            return f"{self.hpo_term_and_id}: onset {self._onset.age_string}"
-        else:
-            return self.hpo_term_and_id
-
     def __str__(self) -> str:
         if not self._measured:
             return f"not measured: {self._label} ({self._id})"
         elif not self._observed:
-            return f"excluded: {self._term_and_id_with_onset()}"
+            return f"excluded: {self._label} ({self._id})"
         else:
-            return self._term_and_id_with_onset()
+            return f"{self._label} ({self._id})"
 
-    def to_string(self) -> str:
+    def to_string(self):
         return self.__str__()
 
-    def excluded(self) -> None:
+    def excluded(self):
         """
         Sets the current term to excluded (i.e., the abnormality was sought but explicitly ruled out clinically)
         """
         self._observed = False
 
-    def to_ga4gh_phenotypic_feature(self) -> PPKt.PhenotypicFeature:
+    def to_ga4gh_phenotypic_feature(self):
         """
         :returns: A GA4GH PhenotypcFeature corresponding to this HpTerm
         :rtype: phenopackets.PhenotypicFeature
         """
         pf = PPKt.PhenotypicFeature()
         pf.type.id = self._id
         pf.type.label = self._label
         if not self._observed:
             pf.excluded = True
-        if self._onset.is_valid():
-            pf.onset.CopyFrom(self._onset.to_ga4gh_time_element())
-        if self._resolution.is_valid():
-            pf.resolution.CopyFrom(self._resolution.to_ga4gh_time_element())
+        if self._onset != Constants.NOT_PROVIDED:
+            pf.onset.age.iso8601duration = self._onset
+        elif self.onset_term is not None:
+            oclass = PPKt.OntologyClass()
+            oclass.id = self._onset_term[1]
+            oclass.label = self._onset_term[0]
+            pf.onset.ontology_class.CopyFrom(oclass)
+        if self._resolution != Constants.NOT_PROVIDED:
+            pf.resolution.age.iso8601duration = self._resolution
         return pf
 
 
     @staticmethod
-    def term_list_to_dataframe(hpo_list) -> pd.DataFrame:
+    def term_list_to_dataframe(hpo_list):
         if not isinstance(hpo_list, list):
             raise ValueError(f"hpo_list argument must be a list but was {type(hpo_list)}")
         if len(hpo_list) > 0:
             hpo1 = hpo_list[0]
             if not isinstance(hpo1, HpTerm):
                 raise ValueError(f"hpo_list argument must consist of HpTerm objects but had {type(hpo1)}")
         if len(hpo_list) == 0:
@@ -172,15 +172,15 @@
         items = []
         for hp in hpo_list:
             d = { "id": hp.id, "label": hp.label, "observed":hp.observed, "measured": hp.measured }
             items.append(d)
         return pd.DataFrame(items)
 
     @staticmethod
-    def from_hpo_tk_term(hpotk_term:hpotk.Term) -> "HpTerm":
+    def from_hpo_tk_term(hpotk_term:hpotk.Term):
         """Create a pyphetools HpTerm object from an hpo-toolkit Term object
 
         :param hpotk_term: A term from the HPO toolkit
         :type hpotk_term: hpotk.Term
         :returns: The corresponding HpTerm object
         :rtype: HpTerm
         """
@@ -191,125 +191,126 @@
 
 class HpTermBuilder:
 
     def __init__(self, hpo_id:str, hpo_label:str):
         if not hpo_id.startswith("HP:"):
             raise ValueError(f"Malformed HPO id {hpo_id}")
         if not len(hpo_id) == 10:
+            length = len(hpo_id)
             raise ValueError(f"Malformed HPO id with length {len(hpo_id)}: {hpo_id}")
         self._hpo_id = hpo_id
         if hpo_label is None or len(hpo_label) < 3:
             raise ValueError(f"Malformed HPO label \"{hpo_label}\"")
         self._hpo_label = hpo_label
-        self._observed = True
-        self._measured = True
-        self._onset = NoneAge("na")
-        self._resolution = NoneAge("na")
+        self._observed=True
+        self._measured=True
+        self._onset=None
+        self._onsetTerm=None
 
     def excluded(self):
         self._observed = False
         return self
 
     def not_measured(self):
         self._measured = False
         return self
 
     def iso8601_onset(self, onset):
-        """Set the age with an iso8601 string
-        """
-        if not isinstance(onset, str):
-            raise ValueError(f"onset argument must be iso8601 string but was {type(onset)}")
-        self._onset = IsoAge.from_iso8601(onset)
+        self._onset = onset
         return self
 
     def embryonal_onset(self):
         """Onset of disease at up to 8 weeks following fertilization (corresponding to 10 weeks of gestation).
         """
-        self._onsetTerm = HpoAge("Embryonal onset") # HP:0011460
+        self._onsetTerm = ["Embryonal onset", "HP:0011460"]
         return self
 
     def fetal_onset(self):
         """Onset prior to birth but after 8 weeks of embryonic development (corresponding to a gestational age of 10 weeks).
         """
-        self._onset = HpoAge("Fetal onset") # HP:0011461
+        self._onsetTerm = ["Fetal onset", "HP:0011461"]
         return self
 
     def second_trimester_onset(self):
         """second trimester, which comprises the range of gestational ages from 14 0/7 weeks to 27 6/7 (inclusive)
         """
-        self._onset = HpoAge("Second trimester onset") # HP:0034198
+        self._onsetTerm = ["Second trimester onset", "HP:0034198"]
         return self
 
     def late_first_trimester_onset(self):
         """late first trimester during the early fetal period, which is defined as 11 0/7 to 13 6/7 weeks of gestation (inclusive).
         """
-        self._onset = HpoAge("Late first trimester onset") # HP:0034199
+        self._onsetTerm = ["Late first trimester onset", "HP:0034199"]
         return self
 
     def third_trimester_onset(self):
         """third trimester, which is defined as 28 weeks and zero days (28+0) of gestation and beyond.
         """
-        self._onset = HpoAge("Third trimester onset") # HP:0034197
+        self._onsetTerm = ["Third trimester onset", "HP:0034197"]
         return self
 
     def antenatal_onset(self):
         """onset prior to birth
         """
-        self._onset = HpoAge("Antenatal onset") # HP:0030674
+        self._onsetTerm = ["Antenatal onset", "HP:0030674"]
         return self
 
     def congenital_onset(self):
         """A phenotypic abnormality that is present at birth.
         """
-        self._onset = HpoAge("Congenital onset") # HP:0003577
+        self._onsetTerm = ["Congenital onset", "HP:0003577"]
         return self
 
     def neonatal_onset(self):
         """Onset of signs or symptoms of disease within the first 28 days of life.
         """
-        self._onset = HpoAge("Neonatal onset") # HP:0003623)
+        self._onsetTerm = ["Neonatal onset", "HP:0003623"]
         return self
 
 
     def infantile_onset(self):
         """Onset of signs or symptoms of disease between 28 days to one year of life.
         """
-        self._onset = HpoAge("Infantile onset") # HP:0003593
+        self._onsetTerm = ["Infantile onset", "HP:0003593"]
         return self
 
     def childhood_onset(self):
         """Onset of disease at the age of between 1 and 5 years.
         """
-        self._onset = HpoAge("Childhood onset") # HP:0011463
+        self._onsetTerm = ["Childhood onset", "HP:0011463"]
         return self
 
     def juvenile_onset(self):
         """Onset of signs or symptoms of disease between the age of 5 and 15 years.
         """
-        self._onset = HpoAge("Juvenile onset") # HP:0003621
+        self._onsetTerm = ["Juvenile onset", "HP:0003621"]
         return self
 
     def young_adult_onset(self):
         """Onset of disease at the age of between 16 and 40 years.
         """
-        self._onset = HpoAge("Young adult onset") # HP:0011462
+        self._onsetTerm = ["Young adult onset", "HP:0011462"]
         return self
 
     def middle_age_onset(self):
         """onset of symptoms at the age of 40 to 60 years.
         """
-        self._onset = HpoAge("Middle age onset") # HP:0003596
+        self._onsetTerm = ["Middle age onset", "HP:0003596"]
         return self
 
     def late_onset(self):
         """Onset of symptoms after the age of 60 years.
         """
-        self._onset = HpoAge("Late onset") # HP:0003584
+        self._onsetTerm = ["Late onset", "HP:0003584"]
         return self
 
     def build(self) -> HpTerm:
+        if self._onset is not None and self._onsetTerm is not None:
+            raise ValueError("Both onset and onsetTerm were set but only a maximum of one of them may be not None")
         return HpTerm(hpo_id=self._hpo_id,
                     label=self._hpo_label,
                     observed=self._observed,
                     measured=self._measured,
-                    onset=self._onset)
+                    onset=self._onset,
+                    onset_term=self._onsetTerm)
+
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/hpo_cr.py` & `pyphetools-0.9.9/src/pyphetools/creation/hpo_cr.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 
 class HpoConceptRecognizer(metaclass=abc.ABCMeta):
     """
     This abstract class acts as an interface for classes that implement parse_cell to perform HPO-based concept recognition.
     """
 
+    def __init__(self):
+        pass
+
     @abc.abstractmethod
     def parse_cell(self, cell_contents, custom_d=None) -> List[HpTerm]:
         """
         parse HPO Terms from the contents of a cell of the original table
 
         :param cell_contents: a cell of the original table
         :type cell_contents: str
@@ -56,7 +59,15 @@
 
     @abc.abstractmethod
     def initialize_simple_column_maps(self, column_name_to_hpo_label_map, observed, excluded, non_measured=None):
         """
         Create a dictionary of SimpleColumnMappers
         """
         pass
+
+    @abc.abstractmethod
+    def get_hpo_ontology(self):
+        """
+        :returns: a reference to the HPO-toolkit Ontology object for the HPO
+        :rtype: hpotk.MinimalOntology
+        """
+        pass
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.9.9/src/pyphetools/creation/hpo_exact_cr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import re
-import typing
-
-from collections import defaultdict
-
 import hpotk
 
 from .hpo_cr import HpoConceptRecognizer
 from .hp_term import HpTerm
 from .column_mapper import ColumnMapper
 from .simple_column_mapper import SimpleColumnMapper
 
+import re
+from typing import List, Union
+from collections import defaultdict
 
 
 class ConceptMatch:
     def __init__(self, term, start: int, end: int) -> None:
         self._hp_term = term
         self._start = start
         self._end = end
@@ -46,72 +44,27 @@
             return True
         elif self.end >= other.end >= self.start:
             return True
         else:
             return False
 
 
-def get_label_to_id_map(hpo: hpotk.Ontology) -> typing.Mapping[str, str]:
-    """
-    Create a map from a lower case version of HPO labels to the corresponding HPO id
-    only include terms that are descendants of PHENOTYPE_ROOT
-
-    :returns: a map from lower-case HPO term labels to HPO ids
-    """
-    label_to_id_d = {}
-    for term in hpo.terms:
-        hpo_id = term.identifier
-        if not hpo.graph.is_ancestor_of(hpotk.constants.hpo.base.PHENOTYPIC_ABNORMALITY, hpo_id):
-            continue
-        label_to_id_d[term.name.lower()] = hpo_id.value
-        # Add the labels of the synonyms
-        if term.synonyms is not None and len(term.synonyms) > 0:
-            for synonym in term.synonyms:
-                lc_syn = synonym.name.lower()
-                # only take synonyms with length at least 5 to avoid spurious matches
-                if len(lc_syn) > 4:
-                    label_to_id_d[lc_syn] = hpo_id.value
-
-    return label_to_id_d
-
-
-def get_id_to_label_map(hpo: hpotk.MinimalOntology) -> typing.Mapping[str, str]:
-    """
-    :returns: a map from HPO term ids to HPO labels
-    :rtype: Dict[str,str]
-    """
-    id_to_label_d = {}
-
-    for term in hpo.terms:
-        id_to_label_d[term.identifier.value] = term.name
-
-    return id_to_label_d
-
-
 class HpoExactConceptRecognizer(HpoConceptRecognizer):
-
-    @staticmethod
-    def from_hpo(hpo: hpotk.Ontology):
-        label_to_id = get_label_to_id_map(hpo)
-        id_to_primary_label = get_id_to_label_map(hpo)
-
-        return HpoExactConceptRecognizer(
-            label_to_id=label_to_id,
-            id_to_primary_label=id_to_primary_label,
-        )
-
-    def __init__(self, label_to_id, id_to_primary_label):
+    # self._label_to_id_d, self._id_to_primary_label
+    def __init__(self, label_to_id, id_to_primary_label, ontology:hpotk.Ontology=None):
+        super().__init__()
         if not isinstance(label_to_id, dict):
             raise ValueError("label_to_id_d argument must be dictionary")
         if not isinstance(id_to_primary_label, dict):
             raise ValueError("labels_to_primary_label_d argument must be dictionary")
         self._id_to_primary_label = id_to_primary_label
         self._label_to_id = label_to_id
+        self._ontology = ontology
 
-    def parse_cell(self, cell_contents, custom_d=None) -> typing.List[HpTerm]:
+    def parse_cell(self, cell_contents, custom_d=None) -> List[HpTerm]:
         """parse the contents of one table cell
 
         Args:
             cell_contents (str): description of patient phenotypes. Assumption is that if there are new lines, any given phenotype is on its own line
             custom_d (dict, optional): User-provided dictionary with mappings to HPO terms. Defaults to None.
         """
         if not isinstance(cell_contents, str):
@@ -124,15 +77,15 @@
         if custom_d is None:
             # initialize to empty dictionary if this argument is not passed
             # to avoid needed to check for None in other functions
             custom_d = defaultdict()
         return self._parse_contents(cell_text=cell_text, custom_d=custom_d)
 
 
-    def _get_exact_match_in_custom_d(self, cell_text, custom_d) -> typing.List[HpTerm]:
+    def _get_exact_match_in_custom_d(self, cell_text, custom_d) -> List[HpTerm]:
         """This method is called by _parse_contents if cell_text was present in custom_d
 
         If the match does not result in at least one HpTerm match, it is an error and the custom_d probably has an incorrect string
 
         :param cell_text: The text of a table cell
         :type cell_text: str
         :param custom_d: key - text in original table value-corresponding HPO label
@@ -154,15 +107,15 @@
             if hp_term is None:
                     raise ValueError(f"Could not get HpTerm from {label}")
             else:
                 results.append(hp_term)
         return results
 
 
-    def _find_text_within_custom_items(self, lc_chunk, custom_d) -> typing.List[HpTerm]:
+    def _find_text_within_custom_items(self, lc_chunk, custom_d) -> List[HpTerm]:
         hits = []
         # Note that chunk has been stripped of whitespace and lower-cased already
         for original_text, hpo_label in custom_d.items():
             lc_original = original_text.lower()
             startpos = lc_chunk.find(lc_original)
             if startpos < 0:
                 continue
@@ -172,15 +125,15 @@
                 hits.append(ConceptMatch(term=hp_term, start=startpos, end=endpos))
             elif isinstance(hpo_label, list):
                 for h in hpo_label:
                     hp_term = self.get_term_from_label(h)
                     hits.append(ConceptMatch(term=hp_term, start=startpos, end=endpos))
         return hits
 
-    def _find_hpo_term_in_lc_chunk(self, lc_chunk) -> typing.List[HpTerm]:
+    def _find_hpo_term_in_lc_chunk(self, lc_chunk) -> List[HpTerm]:
         hits = []
         for lower_case_hp_label, hpo_tid in self._label_to_id.items():
                 key = lower_case_hp_label.lower()
                 startpos = lc_chunk.find(key)
                 endpos = startpos + len(key) - 1
                 if startpos < 0:
                     continue
@@ -189,15 +142,15 @@
                 # Create a regex to enforce the match is at word boundary
                 BOUNDARY_REGEX = re.compile(r'\b%s\b' % key, re.I)
                 if BOUNDARY_REGEX.search(lc_chunk):
                     hp_term = self.get_term_from_id(hpo_id=hpo_tid)  # Get properly capitalized label
                     hits.append(ConceptMatch(term=hp_term, start=startpos, end=endpos))
         return hits
 
-    def _parse_contents(self, cell_text, custom_d) -> typing.List[HpTerm]:
+    def _parse_contents(self, cell_text, custom_d) -> List[HpTerm]:
         """Parse the contents of a cell for HPO terms
         Args:
             cell_text (str): The text of a table cell
             custom_d (dict): key - text in original table value-corresponding HPO label
         """
         if cell_text in custom_d:
             return self._get_exact_match_in_custom_d(cell_text=cell_text, custom_d=custom_d)
@@ -207,15 +160,15 @@
             lc_chunk = chunk.lower()
             hits_1 = self._find_text_within_custom_items(lc_chunk=lc_chunk, custom_d=custom_d)
             hits_2 = self._find_hpo_term_in_lc_chunk(lc_chunk=lc_chunk)
             hits_1.extend(hits_2)
             results.extend(self._get_non_overlapping_matches(hits=hits_1))
         return results
 
-    def parse_cell_for_exact_matches(self, cell_text, custom_d) -> typing.List[HpTerm]:
+    def parse_cell_for_exact_matches(self, cell_text, custom_d) -> List[HpTerm]:
         """
         Identify HPO Terms from the contents of a cell whose label exactly matches a string in the custom dictionary
 
         :param cell_contents: a cell of the original table
         :type cell_contents: str
         :param custom_d: a dictionary with keys for strings in the original table and their mappings to HPO labels
         :type custom_d: Dict[str,str]
@@ -226,15 +179,15 @@
         results = []
         for chunk in chunks:
             lc_chunk = chunk.lower()
             hits = self._find_text_within_custom_items(lc_chunk=lc_chunk, custom_d=custom_d)
             results.extend(self._get_non_overlapping_matches(hits=hits))
         return
 
-    def _get_non_overlapping_matches(self, hits:[typing.List[ConceptMatch]]) -> typing.List[HpTerm]:
+    def _get_non_overlapping_matches(self, hits:[List[ConceptMatch]]) -> List[HpTerm]:
         """The prupose of this method is to choose a list of non-overlapping matches
 
         Sometimes, we get multiple matches that partially overlap. We will greedily take the longest matches and discard overlaps.
 
         :param hits: list of ConceptMatch objects that encode HpTerm matches and their positions
         :type hits: List[ConceptMatch]
         :returns: a list of non-overlapping HtTerm objects (matches)
@@ -300,10 +253,17 @@
             if not isinstance(hpo_label_and_id, list):
                 raise ValueError(f"Expected {hpo_label_and_id} to be a two-item list with HPO label and id")
             hpo_label = hpo_label_and_id[0]
             expected_id = hpo_label_and_id[1]
             hp_term = self.get_term_from_label(hpo_label)
             if hp_term.id != expected_id:
                 raise ValueError(f"Got {hp_term.id} but was expecting {expected_id} for {hpo_label}")
-            mpr = SimpleColumnMapper(column_name=column_name, hpo_id=hp_term.id, hpo_label=hp_term.label, observed=observed, excluded=excluded)
+            mpr = SimpleColumnMapper(hpo_id=hp_term.id, hpo_label=hp_term.label, observed=observed, excluded=excluded)
             simple_mapper_d[column_name] = mpr
         return simple_mapper_d
+
+    def get_hpo_ontology(self):
+        """
+        :returns: a reference to the HPO-toolkit Ontology object for the HPO
+        :rtype: hpotk.MinimalOntology
+        """
+        return self._ontology
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/individual.py` & `pyphetools-0.9.9/src/pyphetools/creation/individual.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from google.protobuf.json_format import MessageToJson
 from .citation import Citation
 from .constants import Constants
 from .disease import Disease
 from .hp_term import HpTerm
 from .hgvs_variant import Variant
 from .metadata import MetaData, Resource
-from .pyphetools_age import PyPheToolsAge, NoneAge, IsoAge
-from ..pp.v202 import VitalStatus
+
 
 class Individual:
     """
     A class to represent one individual of the cohort
 
     :param individual_id: The individual identifier
     :type individual_id: str
@@ -31,49 +30,40 @@
     """
 
     def __init__(self,
                 individual_id:str,
                 hpo_terms:List[HpTerm]=None,
                 citation:Citation=None,
                 sex:str=Constants.NOT_PROVIDED,
-                age_of_onset:str=NoneAge("na"),
-                age_at_last_encounter:str=NoneAge("na"),
-                vital_status:VitalStatus=None,
+                age:str=Constants.NOT_PROVIDED,
                 interpretation_list:List[PPKt.VariantInterpretation]=None,
                 disease:Disease=None):
         """Constructor
         """
         if isinstance(individual_id, int):
             self._individual_id = str(individual_id)
         elif isinstance(individual_id, str):
             self._individual_id = individual_id
         else:
             raise ValueError(f"individual_id argument must be int or string but was {type(individual_id)}")
         if sex is None:
             self._sex = PPKt.Sex.UNKNOWN_SEX
         else:
             self._sex = sex
-        #if age_of_onset is None or isinstance(age_of_onset, str):
-        #    raise ValueError(f"age_of_onset argument must be PyPheToolsAge but was {type(age_of_onset)}")
-        self._age_of_onset = age_of_onset
-        #if age_at_last_encounter is None or isinstance(age_at_last_encounter, str):
-        #    raise ValueError(f"age_at_last_encounter argument must be PyPheToolsAge but was {type(age_of_onset)}")
-        self._age_at_last_encounter = age_at_last_encounter
-        self._vital_status = vital_status
+        self._age = age
         if hpo_terms is None:
             self._hpo_terms = list()
         else:
             self._hpo_terms = hpo_terms
         if interpretation_list is None:
             self._interpretation_list = list()
         else:
             self._interpretation_list = interpretation_list
         self._disease = disease
         self._citation = citation
-        self._vital_status = None
 
     @property
     def id(self):
         """
         :returns: the individual identifier
         :rtype: str
         """
@@ -87,44 +77,23 @@
         """
         return self._sex
 
     def set_sex(self, sex):
         self._sex = sex
 
     @property
-    def age_of_onset(self):
+    def age(self):
         """
-        :returns: an iso8601 representation of age or HPO term label
+        :returns: an iso8601 representation of age
         :rtype: str
         """
-        return self._age_of_onset
-
-    @property
-    def age_at_last_encounter(self):
-        """
-        :returns: an iso8601 representation of age or HPO term label
-        :rtype: str
-        """
-        return self._age_at_last_encounter
-
-    def set_age_of_onset(self, age):
-        """
-        :param age: iso8601 string or HPO onset label
-        :type age: str
-        """
-        if not isinstance(age, str):
-            raise ValueError(f"age argument must be a string but was {type(age)}")
-        self._age_of_onset = PyPheToolsAge.get_age(age)
+        return self._age
 
-    def set_age_at_last_encounter(self, age):
-        """
-        :param age: iso8601 string or HPO onset label
-        :type age: str
-        """
-        self._age_at_last_encounter = age
+    def set_age(self, iso_age):
+        self._age = iso_age
 
     @property
     def hpo_terms(self):
         """
         :returns: a list of observed and excluded HPO terms
         :rtype: List[pyphetools.creation.HpTerm]
         """
@@ -172,20 +141,14 @@
         CohortEncoder
 
         :param disease: the disease diagnosis for this individual
         :type disease: Disease
         """
         self._disease = disease
 
-    def disease_count(self):
-        if self._disease is None:
-            return 0
-        else:
-            return 1
-
     def set_hpo_terms(self, cleansed_hpo_terms:List[HpTerm]):
         """
         :param cleansed_hpo_terms: a list of HpTerm objects that has been cleansed by OntologyQC
         :type cleansed_hpo_terms: List[pyphetools.creation.HpTerm]
         """
         self._hpo_terms = cleansed_hpo_terms
 
@@ -196,126 +159,62 @@
     def set_citation(self, citation:Citation):
         """
         :param citation: Object with the title and PubMed identifier for the publication in which this individual was described (e.g. PMID:321..)
         :type citation: Citation
         """
         self._citation = citation
 
-    def set_vital_status(self, vstatus:VitalStatus):
-        if not isinstance(vstatus, VitalStatus):
-            raise ValueError(f"vstatus argument must be pyphetools.pp.v202.VitalStatus but was{type(vstatus)}")
-        self._vital_status = vstatus
-
     def get_phenopacket_id(self, phenopacket_id=None) -> str:
         """
         :returns: the Phenopacket identifier for this individual
         :rtype: str
         """
         if phenopacket_id is None:
             indi_id = self._individual_id.replace(" ", "_")
             if self._citation is not None:
                 pmid = self._citation.pmid.replace(":", "_")
                 ppkt_id = f"{pmid}_{indi_id}"
             else:
                 ppkt_id = indi_id
         else:
             ppkt_id = phenopacket_id
-        # strip non alphanumeric characters
-        ppkt_id = ''.join(e if e.isalnum()  else "_" for e in ppkt_id)
-        ppkt_id = ppkt_id.replace("__", "_")
-        if ppkt_id.endswith("_"):
-            ppkt_id = ppkt_id[:-1]
+        ppkt_id = ppkt_id.replace(" ", "_")
         return ppkt_id
 
-    def get_citation(self) -> Citation:
-        """
-        :returns: a Citation object with PMID and article title
-        :rtype: Citation
-        """
-        return self._citation
-
-
-    def _get_onset(self) -> Union[PyPheToolsAge,str]:
-        """The assumption of this method is that if we have a valid age of onset field, use this.
-        Otherwise, try to find an age of onset from the phenotypic features and take the youngest age
-        """
-        if self._age_of_onset is not None and self._age_of_onset != Constants.NOT_PROVIDED:
-            return self._age_of_onset
-        phenotypic_feature_onsets = set()
-        if isinstance(self._hpo_terms, list):
-            for hp in self._hpo_terms:
-                if not hp.measured:
-                    continue
-                pf = hp.to_ga4gh_phenotypic_feature()
-                if pf.onset.age.iso8601duration is None and self._age_of_onset != Constants.NOT_PROVIDED:
-                    phenotypic_feature_onsets.add(pf.onset.age.iso8601duration)
-        if len(phenotypic_feature_onsets) == 0:
-            return Constants.NOT_PROVIDED
-        age_format_list = list()
-        for o in phenotypic_feature_onsets:
-            age_format_list.append(IsoAge.from_iso8601(o))
-        sorted_age = sorted(age_format_list, lambda x: x.total_days)
-        youngest_age = sorted_age[0]
-        return youngest_age
-
-    def _get_disease_object(self):
-        iso_age = self._get_onset()
-        disease_term = PPKt.OntologyClass()
-        if self._disease is not None:
-            disease_term.id = self._disease.id
-            disease_term.label = self._disease.label
-        else:
-            disease_term.id = "MONDO:0000001"
-            disease_term.label = "disease"
-            print("[WARNING] could not find disease information")
-        disease_object = PPKt.Disease()
-        disease_object.term.CopyFrom(disease_term)
-        if self.age_of_onset is not None and self.age_of_onset.is_valid():
-            disease_object.onset.CopyFrom(self.age_of_onset.to_ga4gh_time_element())
-        if iso_age is not None and iso_age.is_valid():
-            disease_object.onset.CopyFrom(iso_age.to_ga4gh_time_element())
-        return disease_object
-
-
 
     def to_ga4gh_phenopacket(self, metadata, phenopacket_id=None) -> PPKt.Phenopacket:
         """
         Transform the data into GA4GH Phenopacket format
         :returns:  a GA4GH Phenopacket representing this individual
         :rtype: PPKt.Phenopacket
         """
         if isinstance(metadata, MetaData):
             metadata = metadata.to_ga4gh()
         if not isinstance(metadata, PPKt.MetaData):
             raise ValueError(f"metadata argument must be pyphetools.MetaData or GA4GH MetaData but was {type(metadata)}")
         php = PPKt.Phenopacket()
         php.id = self.get_phenopacket_id(phenopacket_id=phenopacket_id)
         php.subject.id = self._individual_id
-        if self._age_at_last_encounter is not None and self._age_at_last_encounter.is_valid():
-            php.subject.time_at_last_encounter.CopyFrom(self._age_at_last_encounter.to_ga4gh_time_element())
         if self._sex == Constants.MALE_SYMBOL:
             php.subject.sex = PPKt.Sex.MALE
         elif self._sex == Constants.FEMALE_SYMBOL:
             php.subject.sex = PPKt.Sex.FEMALE
         elif self._sex == Constants.OTHER_SEX_SYMBOL:
             php.subject.sex = PPKt.Sex.OTHER_SEX
-        elif self._sex == Constants.UNKNOWN_SEX_SYMBOL:
+        elif self._sex == Constants.UNKOWN_SEX_SYMBOL:
             php.subject.sex = PPKt.Sex.UNKNOWN_SEX
-        if self._vital_status is not None:
-            vs = self._vital_status.to_message()
-            php.subject.vital_status.CopyFrom(vs)
-        disease_object = self._get_disease_object()
-        php.diseases.append(disease_object)
+        if self._age is not None and self._age != Constants.NOT_PROVIDED:
+            php.subject.time_at_last_encounter.age.iso8601duration = self._age
         if isinstance(self._hpo_terms, list):
             for hp in self._hpo_terms:
                 if not hp.measured:
                     continue
                 pf = hp.to_ga4gh_phenotypic_feature()
-                if pf.onset.age.iso8601duration is None and self._age_of_onset != Constants.NOT_PROVIDED:
-                    pf.onset.age.iso8601duration = self._age_of_onset
+                if pf.onset.age.iso8601duration is None and self._age != Constants.NOT_PROVIDED:
+                    pf.onset.age.iso8601duration = self._age
                 php.phenotypic_features.append(pf)
         elif isinstance(self._hpo_terms, dict):
             for age_key, hpoterm_list in self._hpo_terms.items():
                 for hp in hpoterm_list:
                     if not hp.measured:
                         continue
                     pf = hp.to_phenotypic_feature()
@@ -336,31 +235,28 @@
                 # by assumption, variants passed to this package are all causative
                 genomic_interpretation.interpretation_status = PPKt.GenomicInterpretation.InterpretationStatus.CAUSATIVE
                 genomic_interpretation.variant_interpretation.CopyFrom(var)
                 interpretation.diagnosis.genomic_interpretations.append(genomic_interpretation)
             php.interpretations.append(interpretation)
         if self._citation is not None:
             # overrides the "general" setting of the external reference for the entire cohort
-            while len(metadata.external_references) > 0:
-                # `protobuf` devs must have removed `clear()` method
-                # This is a workaround to clear the list of external references.
-                _ = metadata.external_references.pop()
+            metadata.external_references.clear()
             extref = PPKt.ExternalReference()
             extref.id = self._citation.pmid
             pm = self._citation.pmid.replace("PMID:", "")
             extref.reference = f"https://pubmed.ncbi.nlm.nih.gov/{pm}"
             extref.description = self._citation.title
             metadata.external_references.append(extref)
         php.meta_data.CopyFrom(metadata)
         return php
 
     def __str__(self):
         hpo_list = [t.to_string() for t in self._hpo_terms]
         hpo_str = "\n" + "\n".join(hpo_list)
-        return f"{self._individual_id}: {self._age_of_onset}, {self._sex}: {self._disease} {hpo_str}"
+        return f"{self._individual_id}: {self._age}, {self._sex}: {self._disease} {hpo_str}"
 
     @staticmethod
     def output_individuals_as_phenopackets(individual_list, metadata:MetaData, outdir="phenopackets"):
         """write a list of Individual objects to file in GA4GH Phenopacket format
 
         This methods depends on the MetaData object having a PMID and will fail otherwise
 
@@ -437,15 +333,15 @@
         """
         if len(ppkt.interpretations) == 0:
             print(f"No interpretation found for {ppkt.id}")
             return None, []
         if len(ppkt.interpretations) > 1:
             raise ValueError(f"pyphetools dpoes not currently support multiple Interpretation messages in one phenopacket but we found {len(ppkt.interpretations)}")
         interpretation = ppkt.interpretations[0]
-        if interpretation.HasField("diagnosis") and interpretation.diagnosis.HasField("disease"):
+        if interpretation.diagnosis is not None and interpretation.diagnosis.disease is not None:
             d = interpretation.diagnosis.disease
             disease = Disease(disease_id=d.id, disease_label=d.label)
         else:
             disease = None
         if len(interpretation.diagnosis.genomic_interpretations) == 0:
             return disease, []
         else :
@@ -464,35 +360,29 @@
         """
         if not isinstance(ppkt, PPKt.Phenopacket):
             raise ValueError(f"argument must be a GA4GH Phenopacket Message but was {type(ppkt)}")
         #metadata = ppkt.meta_data
         #pypt_metadata = Individual.from_ga4gh_metadata(mdata=metadata)
         subject_id =  ppkt.subject.id
         sex = ppkt.subject.sex
-        age_at_last_encounter = ppkt.subject.time_at_last_encounter.age.iso8601duration
-        age_of_onset = NoneAge("na")
-        if len(ppkt.diseases) > 0:
-            d = ppkt.diseases[0]
-            if d.HasField("onset") and d.onset.HasField("age"):
-                age_of_onset = d.onset.age
+        age = ppkt.subject.time_at_last_encounter.age.iso8601duration
+        variant_interpretations = []
         hpo_terms = []
         for pf in ppkt.phenotypic_features:
             hpo_id = pf.type.id
             hpo_label = pf.type.label
             observed = not pf.excluded
-            onset_age = NoneAge("na")
-            if pf.HasField("onset"):
-                onset = pf.onset
-                if onset.HasField("age") and onset.age.HasField("iso8601duration"):
-                        onset_age = pf.onset.age.iso8601duration
+            if pf.onset.age.iso8601duration is not None and pf.onset.age.iso8601duration.startswith("P"):
+                onset_age = pf.onset.age.iso8601duration
+            else:
+                onset_age = None
             hpo_terms.append(HpTerm(hpo_id=hpo_id, label=hpo_label, observed=observed, onset=onset_age))
         disease, var_list = Individual.get_variants_and_disease(ppkt)
         indi = Individual(individual_id=subject_id,
                             hpo_terms=hpo_terms,
                             citation=None,
                             sex=sex,
-                            age_of_onset=age_of_onset,
-                            age_at_last_encounter=age_at_last_encounter,
+                            age=age,
                             interpretation_list=var_list)
         if disease is not None:
             indi.set_disease(disease=disease)
         return indi
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/metadata.py` & `pyphetools-0.9.9/src/pyphetools/creation/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,17 +197,14 @@
             if self._extref.id.startswith("PMID"):
                 return self._extref.id
             else:
                 raise ValueError(f"Malformed PMID in external reference: {self._extref.id}")
         else:
             raise ValueError("Could not get PMID because MetaData._extref was None")
 
-    def get_created_by(self) -> str:
-        return self._created_by
-
 
     def to_ga4gh(self):
         """
         Use a time stamp for the current instant
         :returns: A MetaData formated as a GA4GH Phenopacket Schema message
         :rtype: PPkt.MetaData
         """
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/option_column_mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,37 +2,36 @@
 from .column_mapper import ColumnMapper
 from .hpo_cr import HpoConceptRecognizer
 from typing import List, Set
 import pandas as pd
 import re
 from collections import defaultdict
 
-
 class OptionColumnMapper(ColumnMapper):
     """Class to map the contents of a table cell to one or more options (HPO terms)
 
     This mapper should be used if the column has a set of multiple defined items (strings) representing HPO terms.
     The excluded_d argument should be used if the column includes excluded (negated) HPO terms
-    :param column_name: name of the column in the pandas DataFrame
-    :type column_name: str
+
     :param concept_recognizer: HpoConceptRecognizer for text mining
     :type  concept_recognizer: pyphetools.creation.HpoConceptRecognizer
     :param option_d: dictionary with key: string corresponding to original table, value: corresponding HPO term label
     :type option_d:TypedDict[str,str]
     :param excluded_d: dictionary with key: similar to option_d but for excluded HPO terms, optional
     :type excluded_d:TypedDict[str,str]
-
+    :param assumeExcluded: Assume that any phenotype mentioned in `option_d` is absent if it is not mentioned in a cell
+    :type assumeExcluded: bool
     :param omitSet: set of strings to be excluded from concept recognition
     :type omitSet: Set[str]
     """
 
-    def __init__(self, column_name:str, concept_recognizer, option_d, excluded_d=None, omitSet:Set[str]=None):
+    def __init__(self, concept_recognizer, option_d, excluded_d=None, assumeExcluded:bool=False, omitSet:Set[str]=None):
         """Constructor
         """
-        super().__init__(column_name=column_name)
+        super().__init__()
         # Either have self._option_d be an empty dictionary or it must be a valid dictionary
         if option_d is None or not isinstance(option_d, dict):
             raise ValueError(f"option_d argument must be dictionary but was {type(option_d)}")
         self._option_d = option_d
         if not isinstance(concept_recognizer, HpoConceptRecognizer):
             raise ValueError("concept_recognizer arg must be HpoConceptRecognizer but was {type(concept_recognizer)}")
         self._hpo_cr = concept_recognizer
@@ -40,14 +39,24 @@
             excluded_d = defaultdict()
         self._excluded_d = excluded_d
         if omitSet is None:
             omitSet = set()
         elif not isinstance(omitSet, set):
             raise ValueError(f"argument 'omitSet' must be a Python set but was {type(omitSet)}")
         self._omit_set = omitSet
+        self._assumeExcluded = assumeExcluded
+        if assumeExcluded:
+            # if we assume excluded, then individuals do NOT have the items in option_d if they are not mentioned in the cell
+            self._assume_excluded_d = defaultdict(HpTerm)
+            for hpo_label in option_d.values():
+                hpo_term = self._hpo_cr.get_term_from_label(hpo_label)
+                hpo_term.excluded()
+                self._assume_excluded_d[hpo_label] = hpo_term
+        else:
+            self._assume_excluded_d = {}
 
 
     def map_cell(self, cell_contents) -> List[HpTerm]:
         """parse a single table cell
 
         :param cell_contents: contents of a cell of the original file
         :type cell_contents: str
@@ -64,46 +73,54 @@
                 for er in excluded_results:
                     er.excluded()
                     results.append(er)
                     # remove excluded terms from contents
                     cell_contents = cell_contents.replace(er.label.lower(), " ")
         results_obs = self._hpo_cr.parse_cell(cell_contents=cell_contents, custom_d=self._option_d)
         results.extend(results_obs)
+        if self._assumeExcluded:
+            current_labels = { hpo_term.label for hpo_term in results}
+            for k, v in self._assume_excluded_d.items():
+                if v.label not in current_labels:
+                    results.append(v)
         return results
 
-    def preview_column(self, df:pd.DataFrame) -> pd.DataFrame:
+    def preview_column(self, column) -> pd.DataFrame:
         """
         Generate a pandas dataframe with a summary of parsing of the entire column
 
         This method is intended for use in developing the code for ETL of an input column.
         It is only needed for development and debugging.
 
         :param column: A single column from the input table
         :type column: pd.Series
         :returns: a pandas dataframe with one row for each entry of the input column
         :rtype: pd.DataFrame
         """
-        if not isinstance(df, pd.DataFrame):
-            raise ValueError("df argument must be pandas DataFrame, but was {type(column)}")
-        column = df[self._column_name]
-        mapping_counter = defaultdict(int)
-        for _, value in column.items():
-            cell_contents = str(value)
-            term_list = self.map_cell(cell_contents)
-            for hpterm in term_list:
-                mapped = f"{hpterm.hpo_term_and_id} ({hpterm.display_value})"
-                mapping_counter[mapped] += 1
+        if not isinstance(column, pd.Series):
+            raise ValueError("column argument must be pandas Series, but was {type(column)}")
         dlist = []
-        for k, v in mapping_counter.items():
-            d = {"mapping": k, "count": str(v)}
+        for _, value in column.items():
+            d = {"original text": value}
+            column_val = []
+            results  = self.map_cell(str(value))
+            if results is None:
+                print(f"Got None results for {str(value)}")
+                d["terms"] = "n/a"
+            elif len(results) > 0:
+                for hpterm in results:
+                    column_val.append(f"{hpterm.id} ({hpterm.label}/{hpterm.display_value})")
+                d["terms"] = "; ".join(column_val)
+            else:
+                d["terms"] = "n/a"
             dlist.append(d)
         return pd.DataFrame(dlist)
 
     @staticmethod
-    def autoformat(df: pd.DataFrame, hpo_cr:HpoConceptRecognizer, delimiter:str=",", omit_columns:List[str]=None) -> str:
+    def autoformat(df: pd.DataFrame, concept_recognizer:HpoConceptRecognizer, delimiter:str=",", omit_columns:List[str]=None) -> str:
         """Autoformat code from the columns so that we can easily copy-paste and change it.
 
         This method intends to save time by preformatting code the create OptionMappers. The following commands
         will print out skeleton Python code that can be easily adapted to create a mapper.
 
             result = OptionColumnMapper.autoformat(df=dft, concept_recognizer=hpo_cr, delimiter=",")
             print(result)
@@ -112,62 +129,56 @@
         :type df: pd.DataFrame
         :param concept_recognizer: HpoConceptRecognizer for text mining
         :type  concept_recognizer: pyphetools.creation.HpoConceptRecognizer
         :param delimiter: the string used to delimit individual items in a cell (default: comma)
         :type delimiter: str
         :param omit_columns: names of columns to omit from this search
         :type omit_columns: List[str]
-        :param df_name: name of the variable that corresponds to the dataframe
-        :type df_name: str
         :returns: a string that should be displayed using a print() command in the notebook - has info about automatically mapped columns
         :rtype: str
         """
         lines = []
         if not isinstance(df, pd.DataFrame):
             raise ValueError(f"argument \"df\" must be a pandas DataFrame but was {type(df)}")
-        if not isinstance(hpo_cr, HpoConceptRecognizer):
-            raise ValueError(f"concept_recognizer arg must be HpoConceptRecognizer but was {type(hpo_cr)}")
+        if not isinstance(concept_recognizer, HpoConceptRecognizer):
+            raise ValueError(f"concept_recognizer arg must be HpoConceptRecognizer but was {type(concept_recognizer)}")
         if omit_columns is None:
             omit_columns = set()
         elif isinstance(omit_columns, list):
             omit_columns = set(omit_columns)
         elif not isinstance(omit_columns, set):
             raise ValueError(f"If passed, omit_columns argument must be set or list but was {type(omit_columns)}")
         # df.shape[1] gives us the number of columns
         for y in range(df.shape[1]):
-            original_column_name = str(df.columns[y])
-            clean_column_name = str(df.columns[y]).lower().replace(", ","_").replace(' ', '_').replace("/", "_")
-            col_name = clean_column_name.lower()
-            if original_column_name in omit_columns:
+            if y in omit_columns:
                 continue
             temp_dict = {}
             for i in range(len(df)):
                 if len(str(df.iloc[i, y])) > 1:
                     for entry in str(df.iloc[i, y]).split(delimiter):
-                        hpo_term = hpo_cr.parse_cell(entry.strip())
+                        hpo_term = concept_recognizer.parse_cell(entry.strip())
                         if len(hpo_term) > 0:
                             temp_dict[entry.strip()] = hpo_term[0].label
                         else:
                             temp_dict[entry.strip()] = 'PLACEHOLDER'
-
+            col_name = str(df.columns[y]).lower().replace(", ","_").replace(' ', '_')
+            col_name = col_name.lower()
             # skip columns that are unlikely to be interesting for the OptionColumnMapper
             if "patient" in col_name:
                 continue
             if "family" in col_name:
                 continue
             if "gender" in col_name:
                 continue
             if "mutation" in col_name or "varia" in col_name:
                 continue
             if "age" == col_name or "sex" == col_name or "gender" == col_name:
                 continue
             items_d_name = f"{col_name}_d"
             items_d_string = str(temp_dict).replace(',', ',\n')
             lines.append(f"{items_d_name} = {items_d_string}")
-            lines.append("excluded = {}")
-            lines.append(f"{col_name}Mapper = OptionColumnMapper(column_name=\"{original_column_name}\", concept_recognizer=hpo_cr, option_d={items_d_name}, excluded_d=excluded)")
-            lines.append(f"column_mapper_list.append({col_name}Mapper)")
-            lines.append(f"{col_name}Mapper.preview_column(df)")
-
+            lines.append(f"{col_name}Mapper = OptionColumnMapper(concept_recognizer=hpo_cr, option_d={items_d_name})")
+            lines.append(f"{col_name}Mapper.preview_column(df['" + str(df.columns[y]) + "'])")
+            lines.append(f"column_mapper_d['{str(df.columns[y])}'] = {col_name}Mapper")
             lines.append("")
         return "\n".join(lines)
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/scm_generator.py` & `pyphetools-0.9.9/src/pyphetools/creation/simple_column_mapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,86 @@
-
-from .hpo_cr import HpoConceptRecognizer
+from .hp_term import HpTerm
 from .column_mapper import ColumnMapper
-from .simple_column_mapper import SimpleColumnMapper
-from typing import List
+from typing import List, Dict
 import pandas as pd
-import re
+from collections import defaultdict
+
+
+def get_separate_hpos_from_df(df, hpo_cr):
+    """Loop through all the cells in a dataframe or series and try to parse each cell as HPO term.
+    Useful when the separate HPO terms are in the cells themselves.
+
+    :param df: dataframe with phenotypic data
+    :type df: pd.DataFrame
+    :param hpo_cr: instance of HpoConceptRecognizer to match HPO term and get label/id
+    :type hpo_cr: HpoConceptRecognizer
+    :returns: list of lists with the additional HPO terms per individual
+    :rtype: List[List[HpTerm]]
+    """
+    additional_hpos = []
+
+    for i in range(len(df)):
+        temp_hpos = []
+        for y in range(df.shape[1]):
+            hpo_term = hpo_cr.parse_cell(df.iloc[i, y])
+            if len(hpo_term) > 0:
+                temp_hpos.extend(hpo_term)
+        additional_hpos.append(list(set(temp_hpos)))
+    return additional_hpos
+
+
+class SimpleColumnMapper(ColumnMapper):
+    """ColumnMapper for columns that contain information about a single phenotypic abnormality only
+
+    :param hpo_id: HPO  id, e.g., HP:0004321
+    :type hpo_id: str
+    :param hpo_label: Corresponding term label
+    :type hpo_label: str
+    :param observed: symbol used in table if the phenotypic feature was observed
+    :type observed: str
+    :param excluded: symbol used if the feature was excluded
+    :type excluded: str
+    :param non_measured: symbol used if the feature was not measured or is N/A. Defaults to None, optional
+    :type non_measured: str
+    """
+    def __init__(self, hpo_id, hpo_label, observed=None, excluded=None, non_measured=None):
+        """
+        Constructor
+        """
+        super().__init__()
+        self._hpo_id = hpo_id
+        self._hpo_label = hpo_label
+        if observed is None or excluded is None:
+            raise ValueError(
+                    "Need to provide arguments for both observed and excluded")
+        self._observed = observed
+        self._excluded = excluded
+        self._not_measured = non_measured
+
+    def map_cell(self, cell_contents) -> List[HpTerm]:
+        if not isinstance(cell_contents, str):
+            raise ValueError(
+                f"Error: cell_contents argument ({cell_contents}) must be string but was {type(cell_contents)} -- coerced to string")
+        contents = cell_contents.strip()
+        if contents in self._observed:
+            return [HpTerm(hpo_id=self._hpo_id, label=self._hpo_label)]
+        elif contents in self._excluded:
+            return [HpTerm(hpo_id=self._hpo_id, label=self._hpo_label, observed=False)]
+        else:
+            return [HpTerm(hpo_id=self._hpo_id, label=self._hpo_label, measured=False)]
+
+    def preview_column(self, column) -> pd.DataFrame:
+        if not isinstance(column, pd.Series):
+            raise ValueError("column argument must be pandas Series, but was {type(column)}")
+        dlist = []
+        for _, value in column.items():
+            value = self.map_cell(str(value))
+            hpterm = value[0]
+            dlist.append({"term": hpterm.hpo_term_and_id, "status": hpterm.display_value})
+        return pd.DataFrame(dlist)
 
 class SimpleColumnMapperGenerator:
     """Convenience tool to provide mappings automatically
 
     Try to map the columns in a dataframe by matching the name of the column to correct HPO term.
     This class can be used to generate SimpleColumn mappers for exact matches found in the columns names.
 
@@ -17,62 +89,47 @@
     :param observed: symbol used in table if the phenotypic feature was observed
     :type observed: str
     :param excluded: symbol used if the feature was excluded
     :type excluded: str
     :param hpo_cr: instance of HpoConceptRecognizer to match HPO term and get label/id
     :type hpo_cr: HpoConceptRecognizer
     """
-    def __init__(self, df:pd.DataFrame, observed:str, excluded:str, hpo_cr:HpoConceptRecognizer) -> None:
+    def __init__(self, df, observed, excluded, hpo_cr) -> None:
         """
         Constructor
         """
         self._df = df
         self._observed = observed
         self._excluded = excluded
         self._hpo_cr = hpo_cr
         self._mapped_columns = []
         self._unmapped_columns = []
         self._error_messages = []
 
 
-    def try_mapping_columns(self) -> List[ColumnMapper]:
+    def try_mapping_columns(self) -> Dict[str, ColumnMapper]:
         """As a side effect, this class initializes three lists of mapped, unmapped, and error columns
 
         :returns: A dictionary with successfully mapped columns
         :rtype: Dict[str,ColumnMapper]
         """
-        simple_mapper_list = list()
+        simple_mappers = defaultdict(ColumnMapper)
         for col in self._df.columns:
             colname = str(col)
-            result = re.search(r"(HP:\d+)", colname)
             if self._hpo_cr.contains_term_label(colname):
                 hpo_term_list = self._hpo_cr.parse_cell(colname)
                 hpo_term = hpo_term_list[0]
-                scm = SimpleColumnMapper(column_name=colname,
-                                        hpo_id=hpo_term.id,
-                                        hpo_label=hpo_term.label,
-                                        observed=self._observed,
-                                        excluded=self._excluded)
-                simple_mapper_list.append(scm)
-            elif result:
-                hpo_id = result.group(1)
-                if self._hpo_cr.contains_term(hpo_id):
-                    hterm = self._hpo_cr.get_term_from_id(hpo_id)
-                    scm = SimpleColumnMapper(column_name=colname,
-                                            hpo_id=hterm.id,
-                                            hpo_label=hterm.label,
-                                            observed=self._observed,
-                                            excluded=self._excluded)
-                    simple_mapper_list.append(scm)
-                else:
-                    self._unmapped_columns.append(colname)
+                simple_mappers[col] = SimpleColumnMapper(hpo_id=hpo_term.id,
+                                                                    hpo_label=hpo_term.label,
+                                                                    observed=self._observed,
+                                                                    excluded=self._excluded)
             else:
                 self._unmapped_columns.append(colname)
-        self._mapped_columns = [scm.get_column_name() for scm in simple_mapper_list]
-        return simple_mapper_list
+        self._mapped_columns = list(simple_mappers.keys())
+        return simple_mappers
 
 
     def get_unmapped_columns(self):
         """
         :returns: A list of names of the columns that could not be mapped
         :rtype: List[str]
         """
@@ -81,60 +138,24 @@
     def get_mapped_columns(self) -> List[str]:
         """
         :returns: A list of names of the columns that were mapped
         :rtype: List[str]
         """
         return self._mapped_columns
 
-    @staticmethod
-    def from_map(column_name_to_hpo_label_map,
-                observed='+',
-                excluded='-') -> List[SimpleColumnMapper]:
-        """
-        Create SimpleColumnMapers from a map like this
-
-           items = {
-                'Developmental delay': ['Neurodevelopmental delay', 'HP:0012758'],
-                'Regression': ['Cognitive regression', 'HP:0034332'],
-                'Seizure': ['Seizure', 'HP:0001250'],
-            }
-
-        The keys are column names in the original file, and the values are used for creating the corresponding HPO terms
-
-        :param column_name_to_hpo_label_map (_type_): map as described above
-        :param observed: Symbol used to indicate observed. Defaults to '+'.
-        :param excluded: Symbol used to indicate excluded. Defaults to '+'. '-'.
-        :returns: list of SimpleColumnMapper
-        :rtype: List[SimpleColumnMapper]
-        """
-        simple_mapper_list = list()
-        for column_name, hpo_array in column_name_to_hpo_label_map.items():
-            hpo_term_id = hpo_array[1]
-            hpo_label = hpo_array[0]
-            scm = SimpleColumnMapper(column_name=column_name,
-                                    hpo_id=hpo_term_id,
-                                    hpo_label=hpo_label,
-                                    observed=observed,
-                                    excluded=excluded)
-            simple_mapper_list.append(scm)
-        return simple_mapper_list
-
-
-
-
     def to_html(self):
         """create an HTML table with names of mapped and unmapped columns
         """
         table_items = []
         table_items.append('<table style="border: 2px solid black;">\n')
         table_items.append("""<tr>
             <th>Result</th>
             <th>Columns</th>
         </tr>
-        """)
+      """)
         mapped_str = "; ".join(self._mapped_columns)
         unmapped_str = "; ".join([f"<q>{colname}</q>" for colname in self._unmapped_columns])
         def two_item_table_row(cell1, cell2):
             return f"<tr><td>{cell1}</td><td>{cell2}</td></tr>"
         table_items.append(two_item_table_row("Mapped", mapped_str))
         table_items.append(two_item_table_row("Unmapped", unmapped_str))
         table_items.append('</table>\n') # close table content
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/sex_column_mapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pandas as pd
-from collections import defaultdict
 from .constants import Constants
 
 
-
 class SexColumnMapper:
     """
     Mapper for a column that indicates the sex of the individual
 
     :param male_symbol: the synbol for males, e.g. "M", "male", "MALE"
     :type male_symbol: str
     :param female_symbol: the synbol for females, e.g. "F", "female", "FEMALE"
@@ -31,60 +29,48 @@
         self._female_symbol = female_symbol
         self._other_symbol = other_symbol
         self._unknown_symbol = unknown_symbol
         if column_name is None:
             raise ValueError("Must provide non-null column_name argument")
         self._column_name = column_name
         self._not_provided = not_provided
-        self._erroneous_input_counter = defaultdict(int)
-
 
     def map_cell(self, cell_contents) -> str:
         if self._not_provided:
-            return Constants.UNKNOWN_SEX_SYMBOL
+            return Constants.UNKOWN_SEX_SYMBOL
         contents = cell_contents.strip()
         if contents == self._female_symbol:
             return Constants.FEMALE_SYMBOL
         elif contents == self._male_symbol:
             return Constants.MALE_SYMBOL
         elif contents == self._other_symbol:
             return Constants.OTHER_SEX_SYMBOL
         elif contents == self._unknown_symbol:
-            return Constants.UNKNOWN_SEX_SYMBOL
+            return Constants.UNKOWN_SEX_SYMBOL
         else:
-            self._erroneous_input_counter[contents] += 1
-            return Constants.UNKNOWN_SEX_SYMBOL
+            print(f"Could not map sex symbol {contents}")
+            return Constants.UNKOWN_SEX_SYMBOL
 
-    def preview_column(self, df:pd.DataFrame):
-        if not isinstance(df, pd.DataFrame):
-            raise ValueError("df argument must be pandas DataFrame, but was {type(column)}")
-        column = df[self.get_column_name()]
+    def preview_column(self, column):
+        if not isinstance(column, pd.Series):
+            raise ValueError("column argument must be pandas Series, but was {type(column)}")
         dlist = []
-        for _, value in column.items():
+        for index, value in column.items():
             result = self.map_cell(str(value))
             if result is None:
                 dlist.append({"original column contents": value, "sex": "n/a"})
             else:
                 dlist.append({"original column contents": value, "sex": result})
         return pd.DataFrame(dlist)
 
     def get_column_name(self):
         return self._column_name
-
-    def has_error(self):
-        return len(self._erroneous_input_counter) > 0
-
-    def error_summary(self):
-        items = []
-        for k, v in self._erroneous_input_counter.items():
-            items.append(f"{k} (n={v})")
-        return f"Could not parse the following as sex descriptors: {', '.join(items)}"
-
+    
     @staticmethod
     def not_provided():
         """Create an object for cases where sex is not indicated.
         """
-        return SexColumnMapper(male_symbol=Constants.NOT_PROVIDED,
-                            female_symbol=Constants.NOT_PROVIDED,
-                            not_provided=True,
-                            column_name=Constants.NOT_PROVIDED)
+        return SexColumnMapper(male_symbol=Constants.NOT_PROVIDED, 
+                               female_symbol=Constants.NOT_PROVIDED, 
+                               not_provided=True, 
+                               column_name=Constants.NOT_PROVIDED)
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/structural_variant.py` & `pyphetools-0.9.9/src/pyphetools/creation/structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/variant.py` & `pyphetools-0.9.9/src/pyphetools/creation/variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/variant_column_mapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from typing import List, Dict
+
 from .variant import Variant
 
 ACCEPTABLE_GENOTYPES = {"heterozygous", "homozygous", "hemizygous"}
 
 
-
 class VariantColumnMapper:
     """Column mapper for the variants identified in individuals
 
     To use this mapper, first create a dictionary with all variants in the cohort using the
     VariantValidator (for HGVS) and the StructuralVariant classes. The key to the variant is
     the cell contents of the column with variant information in the original table. The Values
     are the Variant objects (implemented as HgvsVariant or StructuralVariant). This mapper will
@@ -21,19 +21,19 @@
     :type variant_column_name: str
     :param genotype_column_name: name of the genotype column in the original table, optional
     :type genotype_column_name: str
     :param delimiter: symbol used to separate variants if more than one variant is provided, optional
     :type delimiter: str
     """
     def __init__(self,
-                variant_d,
-                variant_column_name,
-                genotype_column_name=None,
-                default_genotype=None,
-                delimiter=None) -> None:
+                 variant_d,
+                 variant_column_name,
+                 genotype_column_name=None,
+                 default_genotype=None,
+                 delimiter=None) -> None:
 
         if default_genotype is not None and default_genotype not in ACCEPTABLE_GENOTYPES:
             raise ValueError(f"Did not recognize default genotype {default_genotype}")
         if not isinstance(variant_d, dict):
             raise ValueError(f"Argument variant_d must be a dictionary but was {type(variant_d)}")
         self._variant_d = variant_d
         self._default_genotype = default_genotype
```

### Comparing `pyphetools-0.9.83/src/pyphetools/creation/variant_validator.py` & `pyphetools-0.9.9/src/pyphetools/creation/variant_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/validation/cohort_validator.py` & `pyphetools-0.9.9/src/pyphetools/validation/cohort_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/validation/content_validator.py` & `pyphetools-0.9.9/src/pyphetools/validation/content_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,19 +31,18 @@
     annotations.
 
     :param min_hpo: minimum number of phenotypic features (HP terms) for this phenopacket to be considered valid
     :type min_hpo: int
     :param allelic_requirement: used to check number of alleles and variants
     :type allelic_requirement: AllelicRequirement
     """
-    def __init__(self, min_hpo: int, allelic_requirement: AllelicRequirement = None, minimum_disease_count:int=1) -> None:
+    def __init__(self, min_hpo: int, allelic_requirement: AllelicRequirement = None) -> None:
         super().__init__()
         self._min_hpo = min_hpo
         self._allelic_requirement = allelic_requirement
-        self._minimum_disease_count = minimum_disease_count
 
 
     def validate_individual(self, individual:Individual) -> List[ValidationResult]:
         """
         check a single Individual as to whether there are sufficient HPO terms and alleles/variants
         :returns: a potential empty list of validations
         :rtype: List[ValidationResult]
@@ -60,16 +59,15 @@
                     gtype = vdesc.allelic_state
                     if gtype.label == "heterozygous": # "GENO:0000135"
                         n_alleles += 1
                     elif gtype.label == "homozygous": # "GENO:0000136"
                         n_alleles += 2
                     elif gtype.label == "hemizygous": # "GENO:0000134"
                         n_alleles += 1
-        disease_count =  individual.disease_count()
-        return self._validate(pp_id=pp_id, n_hpo=n_pf, disease_count=disease_count, n_var=n_var, n_alleles=n_alleles)
+        return self._validate(pp_id=pp_id, n_hpo=n_pf, n_var=n_var, n_alleles=n_alleles)
 
 
 
     def validate_phenopacket(self, phenopacket) -> List[ValidationResult]:
         """
         check a single phenopacket as to whether there are sufficient HPO terms and alleles/variants
         :returns: a potential empty list of validations
@@ -108,37 +106,33 @@
                                 gtype = vdesc.allelic_state
                                 if gtype.label == "heterozygous": # "GENO:0000135"
                                     n_alleles += 1
                                 elif gtype.label == "homozygous": # "GENO:0000136"
                                     n_alleles += 2
                                 elif gtype.label == "hemizygous": # "GENO:0000134"
                                     n_alleles += 1
-        disease_count = len(phenopacket.diseases)
-        return self._validate(pp_id=pp_id, n_hpo=n_pf, disease_count=disease_count, n_var=n_var, n_alleles=n_alleles)
+        return self._validate(pp_id=pp_id, n_hpo=n_pf, n_var=n_var, n_alleles=n_alleles)
 
 
 
-    def _validate(self, pp_id:str, n_hpo:int, disease_count:int, n_var:int=None, n_alleles:int=None):
+    def _validate(self, pp_id:str, n_hpo:int, n_var:int=None, n_alleles:int=None):
         """
         private method called by validate_individual or validate_phenopacket.
         :param pp_id: phenopacket identifier
         :type pp_id: str
         :param n_hpo: Number of HPO terms
         :type n_hpo: int
         :param n_var: Number of variants found
         :type n_var: Optional[int]
         :param n_alleles: Number of alleles found
         :type n_alleles: Optional[int]
         """
         validation_results = []
         if n_hpo < self._min_hpo:
             validation_results.append(ValidationResultBuilder(phenopacket_id=pp_id).insufficient_hpos(min_hpo=self._min_hpo, n_hpo=n_hpo).build())
-        if disease_count < self._minimum_disease_count:
-            val_result = ValidationResultBuilder(phenopacket_id=pp_id).insufficient_disease_count(disease_count, self._minimum_disease_count).build()
-            validation_results.append(val_result)
         if self._allelic_requirement is None:
             return validation_results
         if self._allelic_requirement == AllelicRequirement.MONO_ALLELIC:
             if n_var != 1:
                 val_result = ValidationResultBuilder(phenopacket_id=pp_id).incorrect_variant_count(self._allelic_requirement, n_var).build()
                 validation_results.append(val_result)
             if n_alleles != 1:
```

### Comparing `pyphetools-0.9.83/src/pyphetools/validation/ontology_qc.py` & `pyphetools-0.9.9/src/pyphetools/validation/ontology_qc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import hpotk
 from collections import Counter
-from typing import List, Optional, Set
+from typing import List, Optional
 from ..creation.hp_term import HpTerm
 from .validation_result import ValidationResult, ValidationResultBuilder
 from collections import defaultdict
 from ..creation.individual import Individual
-from ..creation.constants import Constants
 
 
 
 class OntologyQC:
     """
     This class performs three kind of checks/cleansing of ontology data
     1. negated superclass and observed subclass (this is an error in the original data)
@@ -104,113 +103,51 @@
         if len(redundant_term_d) > 0:
             for term, descendant in redundant_term_d.items():
                 error = ValidationResultBuilder(self._phenopacket_id).redundant_term(ancestor_term=term, descendent_term=descendant).build()
                 self._errors.append(error)
         return non_redundant_terms
 
 
-    def _check_term_ids_and_labels(self, hpo_terms:List[HpTerm]) -> None:
-        """
-        Check whether the term identifiers (e.g., HP:0001234) are present in the ontology as primary ids and whether
-        the label matches the current priumary label; if not, flag the errors in self._errors
-        """
+    def _check_terms(self, hpo_terms:List[HpTerm]) -> None:
         for term in hpo_terms:
             hpo_id = term.id
             if not hpo_id in self._ontology:
                 error = ValidationResultBuilder(self._phenopacket_id).malformed_hpo_id(malformed_term=term).build()
                 self._errors.append(error)
             else:
                 hpo_term = self._ontology.get_term(term_id=hpo_id)
                 if hpo_term.name != term.label:
                     valid_term = HpTerm.from_hpo_tk_term(hpo_term)
-                    error = ValidationResultBuilder(self._phenopacket_id).malformed_hpo_label(malformed_label=term.label,
-                                                                                              valid_term=hpo_term).build()
+                    error = ValidationResultBuilder(self._phenopacket_id).malformed_hpo_label(term.label, valid_term=valid_term).build()
                     self._errors.append(error)
 
     def _clean_terms(self) -> List[HpTerm]:
         """
         :returns: list of HPO terms without redundancies/conflicts
         :rtype hpo_terms: List[HpTerm]
         """
         by_age_dictionary =  defaultdict(list)
-        # collect all terms without a defined age of onset
-        # We will assume these terms exist at all specific ages of onset, thus we need this to calculate redundancy
-        observed_terms_without_onset = list()
-        excluded_terms_without_onset = list()
         for term in self._individual.hpo_terms:
             if not term.measured:
                 self._errors.append(ValidationResultBuilder(self._phenopacket_id).not_measured(term=term).build())
             else:
-                if term.onset.is_valid():
-                    by_age_dictionary[term.onset.age_string].append(term)
-                else:
-                    if term.observed:
-                        observed_terms_without_onset.append(term)
-                    else:
-                        excluded_terms_without_onset.append(term)
-        self._check_term_ids_and_labels(self._individual.hpo_terms)
+                by_age_dictionary[term.onset].append(term)
+        self._check_terms(self._individual.hpo_terms)
         clean_terms = []
-
         for onset, term_list in by_age_dictionary.items():
             observed_hpo_terms = [term for term in term_list if term.observed]
             excluded_hpo_terms = [term for term in term_list if not term.observed]
             if self._fix_redundancy_flag:
                 observed_hpo_terms = self._fix_redundancies(observed_hpo_terms)
                 excluded_hpo_terms = self._fix_redundancies(excluded_hpo_terms)
             if self._fix_conflict_flag:
                 # this method checks and may fix the excluded terms (only)
                 excluded_hpo_terms = self._fix_conflicts(observed_hpo_terms, excluded_hpo_terms)
             clean_terms.extend(observed_hpo_terms)
             clean_terms.extend(excluded_hpo_terms)
-        # When we get here, clean terms contains terms with specific onsets and conflicting/redundant terms
-        # have been removed. There may be terms with no specific onset. We only add such terms if they are neither
-        # ancestors or descendants of the specific terms
-        observed_terms_without_onset = self._fix_redundancies(observed_terms_without_onset)
-        excluded_terms_without_onset = self._fix_redundancies(excluded_terms_without_onset)
-        all_term_set = set(clean_terms)
-        for t in observed_terms_without_onset:
-            addT = True
-            for s in all_term_set:
-                # keep the term with the age of onset regardless of whether it is more or less specific
-                if s.id == t.id:
-                    error = ValidationResultBuilder(self._phenopacket_id).duplicate_term(s).build()
-                    self._errors.append(error)
-                    addT = False
-                    break
-                if self._ontology.graph.is_ancestor_of(t.id, s.id):
-                    error = ValidationResultBuilder(self._phenopacket_id).redundant_term(t, s).build()
-                    self._errors.append(error)
-                    addT = False
-                    break
-                if self._ontology.graph.is_ancestor_of(s.id, t.id):
-                    error = ValidationResultBuilder(self._phenopacket_id).redundant_term(s, t).build()
-                    self._errors.append(error)
-                    addT = False
-                    break
-            if addT:
-                clean_terms.append(t)
-                all_term_set.add(t)
-        # now check for problems with excluded terms
-        for t in excluded_terms_without_onset:
-            addT = True
-            for s in all_term_set:
-                # if an excluded term is equal to or ancestor of an observed term this is an error
-                if s.id == t.id:
-                    error = ValidationResultBuilder(self._phenopacket_id).observed_and_excluded_term(term=s).build()
-                    self._errors.append(error)
-                    addT = False
-                elif self._ontology.graph.is_ancestor_of(t.id, s.id):
-                    error = ValidationResultBuilder(self._phenopacket_id).conflict(term=s, conflicting_term=t).build()
-                    self._errors.append(error)
-                    addT = False
-                    break
-            if addT:
-                clean_terms.append(t)
-                all_term_set.add(t)
-
         return clean_terms
 
     def has_error(self) -> bool:
         """
         :returns: True iff errors were encountered
         :rtype: boolean
         """
```

### Comparing `pyphetools-0.9.83/src/pyphetools/validation/validated_individual.py` & `pyphetools-0.9.9/src/pyphetools/validation/validated_individual.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,42 +3,37 @@
 from .content_validator import ContentValidator
 from typing import List
 from .validation_result import ValidationResult
 from .ontology_qc import OntologyQC
 import hpotk
 
 class ValidatedIndividual:
-    """
-    Class to coordinate quality assessment. In addition to ontology-based tests performed by the OntologyQC class,
-    we here test for a minimum number of HPO annotations, the present of at least one disease, and the correct
-    number of alleles.
-    """
 
     def __init__(self, individual:Individual) -> None:
         self._individual = individual
         self._clean_terms = []
         self._validation_errors = []
 
 
-    def validate(self, ontology:hpotk.MinimalOntology, min_hpo:int, allelic_requirement:AllelicRequirement=None, minimum_disease_count:int=1) -> None:
+    def validate(self, ontology:hpotk.MinimalOntology, min_hpo:int, allelic_requirement:AllelicRequirement=None) -> None:
         """validate an Individual object for errors in the Ontology or the minimum number of HPO terms/alleles/variants
 
         :param ontology: HPO object
         :type ontology: hpotk.MinimalOntology
         :param min_hpo: minimum number of phenotypic features (HP terms) for this phenopacket to be considered valid
         :type min_hpo: int
         :param allelic_requirement: used to check number of alleles and variants
         :type allelic_requirement: AllelicRequirement
         """
         qc = OntologyQC(individual=self._individual, ontology=ontology)
         qc_validation_results = qc.get_error_list()
         self._validation_errors.extend(qc_validation_results)
         self._clean_terms = qc.get_clean_terms()
         self._individual.set_hpo_terms(self._clean_terms)
-        cvalidator = ContentValidator(min_hpo=min_hpo, allelic_requirement=allelic_requirement, minimum_disease_count=minimum_disease_count)
+        cvalidator = ContentValidator(min_hpo=min_hpo, allelic_requirement=allelic_requirement)
         validation_results = cvalidator.validate_individual(individual=self._individual)
         self._validation_errors.extend(validation_results)
         # The following checks for remaining errors that would force us to remove the patient from the cohort
         self._unfixed_errors = [e  for e in self._validation_errors if e.is_unfixable_error()]
 
 
     def get_individual_with_clean_terms(self) -> Individual:
@@ -49,17 +44,14 @@
         indi = self._individual
         indi.set_hpo_terms(self._clean_terms)
         return indi
 
     def get_validation_errors(self) -> List[ValidationResult]:
         return self._validation_errors
 
-    def get_unfixed_errors(self)-> List[ValidationResult]:
-        return self._unfixed_errors
-
     def n_errors(self) -> int:
         return len(self._validation_errors)
 
     def has_error(self) -> bool:
         """
         :returns: True iff this Individual had oneor more errors
         :rtype: bool
```

### Comparing `pyphetools-0.9.83/src/pyphetools/validation/validation_result.py` & `pyphetools-0.9.9/src/pyphetools/validation/validation_result.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     INCORRECT_ALLELE_COUNT = 4
     INCORRECT_VARIANT_COUNT = 5
     MALFORMED_ID = 6
     MALFORMED_LABEL = 7
     NOT_MEASURED = 8
     OBSERVED_AND_EXCLUDED = 9
     DUPLICATE = 10
-    INSUFFICIENT_DISEASE_COUNT = 11
-    UNKNOWN = 12
+    UNKNOWN = 11
 
 
 class ValidationResult:
     """
     A helper class to store the results of validation
     :param phenopacket_id: Identifier of the phenopacket being validated
     :type phenopacket_id: str
@@ -117,18 +116,16 @@
     def get_items_as_array(self) -> List[str]:
         """
         :returns: A list of items (strings) intended for display
         :rtype: List[str]
         """
         if self._term is None:
             term = ""
-        elif isinstance(self._term, HpTerm):
-            term = self._term.hpo_term_and_id
         else:
-            term = f"{self._term.name} ({self._term.identifier.value})"
+            term = self._term.to_string()
         return [self.id, self.error_level, self.category, self.message, term]
 
     def __repr__(self):
         return f"{self._error_level}: {self._message}"
 
 
     @staticmethod
@@ -244,25 +241,19 @@
         return self
 
     def malformed_hpo_id(self, malformed_term:HpTerm):
         self._error_level = ErrorLevel.ERROR
         self._category = Category.MALFORMED_ID
         self._message = f"Malformed term {malformed_term.label} with invalid HPO id {malformed_term.id}"
         return self
-    
-    def insufficient_disease_count(self, observed_count:int, minimum_count:int):
-        self._error_level = ErrorLevel.ERROR
-        self._category = Category.INSUFFICIENT_DISEASE_COUNT
-        self._message = f"Individual had {observed_count} disease annotation(s) but the mininum required count is {minimum_count}"
-        return self
 
-    def malformed_hpo_label(self, malformed_label, valid_term:HpTerm):
+    def malformed_hpo_label(self, hpo_label, valid_term:HpTerm):
         self._error_level = ErrorLevel.ERROR
         self._category = Category.MALFORMED_LABEL
-        self._message = f"Invalid label '{malformed_label}' found for {valid_term.name} ({valid_term.identifier.value})"
+        self._message = f"Invalid label '{hpo_label}' found for {valid_term.to_string()}"
         self._term = valid_term
         return self
 
     def set_term(self, term:HpTerm):
         self._term = term
         return self
```

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/detailed_suppl_table.py` & `pyphetools-0.9.9/src/pyphetools/visualization/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/focus_count_table.py` & `pyphetools-0.9.9/src/pyphetools/visualization/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/hpo_category.py` & `pyphetools-0.9.9/src/pyphetools/visualization/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/html_table_generator.py` & `pyphetools-0.9.9/src/pyphetools/visualization/html_table_generator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/individual_table.py` & `pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_table.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,122 +5,103 @@
 
 from ..creation.constants import Constants
 from ..creation import Individual, HpTerm, MetaData
 from .simple_patient import SimplePatient
 from .html_table_generator import HtmlTableGenerator
 
 
+#
+
+
 class Age2Day:
     """
     Convenience function to help sort ages but converting ISO8601 strings into the number of days
 
         sorted_age = sorted(l, key=lambda x: x.days)
 
     following this, retrieve the original string as x.key
     """
     def __init__(self, age, days) -> None:
         self.key = age
         self.days = days
 
 
-class IndividualTable:
 
+class PhenopacketTable:
     """
-    This class creates a table with a summary of  data in a cohort of individuals
+    This class creates a table with a summary of all phenopackets in a cohort of individuals
     Create Individual objects and transform them into phenopackets, or import GA4GH phenopackets and display them.
 
         from IPython.display import HTML, display
         phenopackets = [i.to_ga4gh_phenopacket(metadata=metadata) for i in individuals]
         table = PhenopacketTable.from_phenopackets(phenopacket_list=phenopackets)
         display(HTML(table.to_html()))
 
     Alternatively,
 
         table = PhenopacketTable.from_individuals(individual_list=individuals, metadata=metadata)
         display(HTML(table.to_html()))
     """
-    def __init__(self,  individual_list:List[Individual],
+    def __init__(self, phenopacket_list:List[PPKt.Phenopacket]=None,
+                        individual_list:List[Individual]=None,
                         metadata:MetaData=None) -> None:
         """
+        :param phenopacket_list: List of GA4GH phenopackets to be displayed
+        :type phenopacket_list: List[PPKt.Phenopacket]
         :param individual_list: List of Indidivual objects to be displayed
         :type individual_list: List[Individual]
         :param metadata: metadata about the individuals
         :type metadata: MetaData
         """
-        self._spat_list = []
-        pmid_count_d = defaultdict(int)
-        no_pmid_found = 0
-        pmid_found = 0
-        for individual in individual_list:
-            pp = self._individual_to_phenopacket(individual, metadata)
-            spat = SimplePatient(ga4gh_phenopacket=pp)
-            if spat.has_pmid():
-                pmid_count_d[spat.get_pmid()] += 1
-                pmid_found += 1
-            else:
-                no_pmid_found += 1
-            self._spat_list.append(spat)
-        # Create caption
-        if pmid_found == 0:
-            self._caption = f"{len(individual_list)} individuals with no PMIDs (consider adding this information to the MetaData)"
-        else:
-            pmid_strings = []
-            for k, v in pmid_count_d.items():
-                pmid_strings.append(f"{k} (n={v})")
-            pmid_str = "; ".join(pmid_strings)
-            n_phenopackets = len(individual_list)
-            if n_phenopackets == 1:
-                self._caption = f"{n_phenopackets} phenopacket - {pmid_str}"
-            else:
-                self._caption = f"{n_phenopackets} phenopackets - {pmid_str}"
+        if phenopacket_list is None and individual_list is not None and metadata is not None:
+            self._phenopacket_list =  [i.to_ga4gh_phenopacket(metadata=metadata.to_ga4gh()) for i in individual_list]
+        elif phenopacket_list is not None and individual_list is None:
+            if metadata is not None:
+                raise ValueError("metadata argument not needed for phenopacket list")
+            self._phenopacket_list = phenopacket_list
 
+    @staticmethod
+    def from_phenopackets(phenopacket_list:List[PPKt.Phenopacket]):
+        """Initialize PhenopacketTable from list of GA4GH Phenopackets
 
-    def to_html(self):
-        header_items = ["Individual", "Disease", "Genotype", "Phenotypic features"]
-        rows = []
-        for spat in self._spat_list:
-            rows.append(self._simple_patient_to_table_row(spat))
-        generator = HtmlTableGenerator(caption=self._caption, header_items=header_items, rows=rows)
-        return generator.get_html()
+        :param phenopacket_list: list of GA4GH Phenopackets
+        :type phenopacket_list: List[PPKt.Phenopacket]
 
+        :returns: PhenopacketTable for displaying information about a cohort
+        :rtype: PhenopacketTable
+        """
+        if not isinstance(phenopacket_list, list):
+            raise ValueError(f"Expecting a list but got {type(phenopacket_list)}")
+        if len(phenopacket_list) == 0:
+            raise ValueError("phenopacket_list was empty")
+        ppkt = phenopacket_list[0]
+        if not isinstance(ppkt, PPKt.Phenopacket):
+            raise ValueError(f"phenopacket_list argument must be list of Phenopacket objects but was {type(ppkt)}")
+        return PhenopacketTable(phenopacket_list=phenopacket_list)
 
-    def _individual_to_phenopacket(self, individual, metadata):
-        """Create a phenopacket with the information from this individual
+    @staticmethod
+    def from_individuals(individual_list:List[Individual], metadata:MetaData):
+        """Initialize PhenopacketTable from list of GA4GH Phenopackets
 
-        We try to get information about the publication from the Individual object first. If this is not
-        available, we look for citation information in the metadata
+        :param phenopacket_list: list of GA4GH Phenopackets
+        :type phenopacket_list: List[PPKt.Phenopacket]
 
-        Args:
-            individual (_type_): _description_
-            metadata (_type_): _description_
-
-        Raises:
-            ValueError: _description_
-        """
-        citation = individual.get_citation()
-        if citation is None:
-            if  metadata is None:
-                raise ValueError("No citation information available in individual and metadata is None")
-            else:
-                citation = metadata.get_citation()
-        created_by = "pyphetools" # Note that this is only used to create a table showing variants, diagnoses, and HPOs
-        # the actual created by is not needed for this, and it is user to provide this constant here rather than demand the user enter it.
-        # similarly, we do not need to have the version of the HPO here.
-        # Note that this does not affect the code that outputs phenopackets, which need to have the correct version of this
-        mdata = MetaData(created_by=created_by)
-        mdata.default_versions_with_hpo(version="n/a")
-        metadata = mdata.to_ga4gh()
-        #  the external reference is use to show counts of PMIDs
-        extref = PPKt.ExternalReference()
-        extref.id = citation.pmid
-        pm = citation.pmid.replace("PMID:", "")
-        extref.reference = f"https://pubmed.ncbi.nlm.nih.gov/{pm}"
-        extref.description = citation.title
-        metadata.external_references.append(extref)
-        return individual.to_ga4gh_phenopacket(metadata=metadata)
+        :returns: PhenopacketTable for displaying information about a cohort
+        :rtype: PhenopacketTable
+        """
+        if not isinstance(individual_list, list):
+            raise ValueError(f"Expecting a list but got {type(individual_list)}")
+        if len(individual_list) == 0:
+            raise ValueError("individual_list was empty")
+        indi = individual_list[0]
+        if not isinstance(indi, Individual):
+            raise ValueError(f"individual_list argument must be list of Individual objects but was {type(indi)}")
+        if not isinstance(metadata, MetaData):
+            raise ValueError(f"metadata argument must be pyphetools MetaData object but was {type(metadata)}")
+        return PhenopacketTable(individual_list=individual_list, metadata=MetaData)
 
     def _simple_patient_to_table_row(self, spat:SimplePatient) -> List[str]:
         """
         private method intended to create one table row that represents one individual
         :param spat: An object that represents one individual
         :type spat: SimplePatient
         """
@@ -153,25 +134,61 @@
         """
         :param term_by_age_dict: A dictionary with key - ISO8601 string, value - list of HpTerm objects
         :type term_by_age_dict: Dict[str,HpTerm]
         :returns: HTML code for the HTML cell
         :rtype: str
         """
         lines = []
-        age2day_list = IndividualTable.get_sorted_age2data_list(term_by_age_dict.keys())
+        age2day_list = PhenopacketTable.get_sorted_age2data_list(term_by_age_dict.keys())
         sorted_age = sorted(age2day_list, key=lambda x: x.days)
         for onset in sorted_age:
             hpo_list = term_by_age_dict.get(onset.key)
             hpos = "; ".join([hpo.__str__() for hpo in hpo_list])
             if onset.key == Constants.NOT_PROVIDED:
                 lines.append(hpos)
             else:
                 lines.append(f"<b>{onset.key}</b>: {hpos}")
         return "<br/>".join(lines)
 
+    def to_html(self):
+        """create an HTML table with patient ID, age, sex, genotypes, and PhenotypicFeatures
+        """
+        ppack_list = self._phenopacket_list
+        spat_list = []
+        pmid_count_d = defaultdict(int)
+        no_pmid_found = 0
+        pmid_found = 0
+        for pp in ppack_list:
+            spat = SimplePatient(ga4gh_phenopacket=pp)
+            if spat.has_pmid():
+                pmid_count_d[spat.get_pmid()] += 1
+                pmid_found += 1
+            else:
+                no_pmid_found += 1
+            spat_list.append(spat)
+        # Create caption
+        if pmid_found == 0:
+            capt = f"{len(ppack_list)} phenopackets - no PMIDs (consider adding this information to the MetaData)"
+        else:
+            pmid_strings = []
+            for k, v in pmid_count_d.items():
+                pmid_strings.append(f"{k} (n={v})")
+            pmid_str = "; ".join(pmid_strings)
+            n_phenopackets = len(ppack_list)
+            if n_phenopackets == 1:
+                capt = f"{n_phenopackets} phenopacket - {pmid_str}"
+            else:
+                capt = f"{n_phenopackets} phenopackets - {pmid_str}"
+        header_items = ["Individual", "Disease", "Genotype", "Phenotypic features"]
+        rows = []
+        for spat in spat_list:
+            rows.append(self._simple_patient_to_table_row(spat))
+        generator = HtmlTableGenerator(caption=capt, header_items=header_items, rows=rows)
+        return generator.get_html()
+
     @staticmethod
     def iso_to_days(iso_age:str) -> int:
         """
         Transform the ISO8601 age strings (e.g., P3Y2M) into the corresponding number of days to facilitate sorting.
 
         Note that if age is not provided we want to sort it to the end of the list so we transform to a very high number of days.
 
@@ -207,10 +224,13 @@
         Create a sorted list of Age2Day objects that we use to display the age in the HTML output.
 
         :param ages: A set of ISO 8601 age strings
         :type ages: Set[str]
         :returns: A list of sorted Age2Day objects
         :rtype:  List[Age2Day]
         """
-        age2day_list = list(Age2Day(age, IndividualTable.iso_to_days(age)) for age in ages)
+        age2day_list = list(Age2Day(age, PhenopacketTable.iso_to_days(age)) for age in ages)
         sorted_list = sorted(age2day_list, key=lambda x: x.days)
         return sorted_list
+
+
+
```

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/qc_visualizer.py` & `pyphetools-0.9.9/src/pyphetools/visualization/qc_visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         total_validation_issues = 0
         distinct_item_d = defaultdict(set)
         for vi in validated_individual_list:
             verrors = vi.get_validation_errors()
             total_validation_issues += vi.n_errors()
             for ve in verrors:
                 error_count[ve.category] += 1
-                distinct_item_d[ve.category].add(ve.message)
+                distinct_item_d[ve.category].add(ve.term)
         html_lines = []
         n_individuals = len(validated_individual_list)
         n_individuals_with_errors = sum([1 for i in validated_individual_list if i.has_error()])
         html_lines.append("<h2>Cohort validation</h2>")
         if n_individuals_with_errors == 0:
             html_lines.append(f"<p>No errors found for the cohort with {n_individuals} individuals</p>")
         else:
@@ -120,49 +120,49 @@
                 html_lines.append(para)
             else:
                 para = f"<p>A total of {total_validation_issues} issues were fixed and {n_removed} individuals were removed from the cohort because of irreparable errors. The cohort validator will return {n_error_free_i} individual objects without errors.</p>"
                 html_lines.append(para)
                 if "MALFORMED_LABEL" in distinct_item_d:
                     malformed_label_set = distinct_item_d.get("MALFORMED_LABEL")
                     if len(malformed_label_set) > 0:
-                        malformed = "; ".join(malformed_label_set)
+                        malformed = "; ".join([t.hpo_term_and_id for t in malformed_label_set])
                         para = f"<p>The following malformed labels were found: {malformed}. These need to be corrected before continuing.</p>"
                         html_lines.append(para)
                 if "REDUNDANT" in distinct_item_d:
                     redundant_label_set = distinct_item_d.get("REDUNDANT")
-                    redundant = "; ".join(redundant_label_set)
+                    redundant = "; ".join([t.hpo_term_and_id for t in redundant_label_set])
                     para = f"<p>The following redundant terms were found: {redundant}. Redundant terms will be removed, keeping only one instance of the most specific term.</p>"
                     html_lines.append(para)
                 if "CONFLICT" in distinct_item_d:
                     conflict_label_set = distinct_item_d.get("CONFLICT")
-                    conflict = "; ".join(conflict_label_set)
+                    conflict = "; ".join([t.hpo_term_and_id for t in conflict_label_set])
                     para = f"<p>The following excluded terms were found to have a conflict with an observed descendent term: {conflict}. The ancestor terms will be removed.</p>"
                     html_lines.append(para)
                 if "OBSERVED_AND_EXCLUDED" in distinct_item_d:
                     o_and_e_set = distinct_item_d.get("OBSERVED_AND_EXCLUDED")
-                    o_and_e = "; ".join(o_and_e_set)
+                    o_and_e = "; ".join([t.hpo_term_and_id for t in o_and_e_set])
                     para = f"<p>The following terms were annotated as being both observed and excluded: {o_and_e}. This needs to be fixed manually.</p>"
                     html_lines.append(para)
                 if "DUPLICATE" in distinct_item_d:
                     dup_set = distinct_item_d.get("DUPLICATE")
-                    dup = "; ".join(dup_set)
+                    dup = "; ".join([t.to_string() for t in dup_set])
                     para = f"<p>The following terms were annotated as duplicates: {dup}. This will be fixed automatically.</p>"
                     html_lines.append(para)
                 html_lines.append(self._get_unfixable_error_table())
         return "\n".join(html_lines)
 
 
     def _get_unfixable_error_table(self):
         v_individuals_with_unfixable = self._cohort_validator.get_validated_individuals_with_unfixable_errors()
         html_lines = []
         html_lines.append("<h2>Individuals with unfixable errors</h2>")
         errors = []
         for vi in v_individuals_with_unfixable:
-            if vi.has_unfixed_error():
-                errors.extend(vi.get_unfixed_errors())
+            if vi.has_error():
+                errors.extend(vi.get_validation_errors())
         errors = sorted(errors, key=lambda x : (x._error_level, x._category, x._message))
         header_fields = ValidationResult.get_header_fields()
         rows = [row.get_items_as_array() for row in errors]
         generator = HtmlTableGenerator(header_items=header_fields, rows=rows, caption="Error analysis")
         html_lines.append(generator.get_html())
         return "\n".join(html_lines)
```

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/simple_patient.py` & `pyphetools-0.9.9/src/pyphetools/visualization/simple_patient.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,31 +24,26 @@
             raise ValueError(f"phenopacket argument must be GA4GH Phenopacket Schema Phenopacket but was {type(ga4gh_phenopacket)}")
         else:
             ppack = ga4gh_phenopacket
         observed_hpo_terms = defaultdict(HpTerm)
         excluded_hpo_terms = defaultdict(HpTerm)
         self._by_age_dictionary = defaultdict(list)
         self._phenopacket_id = ppack.id
-        if not ppack.HasField("subject"):
+        if ppack.subject is None:
             raise ValueError("Phenopackets must have a subject message to be used with this package")
         subj = ppack.subject
-        if not subj.id:
-            # This means the subject identifier was not set. This should never happen but is not critical.
-            self._subject_id = self._phenopacket_id
+        if subj.id is None:
+            raise ValueError("Phenopacket subjects must have an id field to be used with this package")
         else:
             self._subject_id = subj.id
-        self._time_at_last_encounter = None
-        if subj.HasField("time_at_last_encounter"):
-            time_at_last_encounter = phenopackets.TimeElement()
-            time_at_last_encounter.CopyFrom(subj.time_at_last_encounter)
-            if time_at_last_encounter.HasField("age"):
-                self._time_at_last_encounter = time_at_last_encounter.age.iso8601duration
-            elif time_at_last_encounter.HasField("ontology_class"):
-                clz = time_at_last_encounter.ontology_class
-                self._time_at_last_encounter = f"{clz.label} ({clz.id})"
+        if subj.time_at_last_encounter is None or subj.time_at_last_encounter.age.iso8601duration is None:
+            print("Warning: No age found for phenopacket")
+            self._time_at_last_encounter = None
+        else:
+            self._time_at_last_encounter = subj.time_at_last_encounter.age.iso8601duration
         if ppack.subject.sex == phenopackets.MALE:
             self._sex = "MALE"
         elif ppack.subject.sex == phenopackets.FEMALE:
             self._sex = "FEMALE"
         elif ppack.subject.sex == phenopackets.OTHER_SEX:
             self._sex = "OTHER"
         else:
@@ -119,48 +114,44 @@
         :param metadata: A GA4GH Phenopacket Schema MetaData object
         :type metadata: MetaData
         """
         ppack = individual.to_ga4gh_phenopacket(metadata)
         return SimplePatient(ga4gh_phenopacket=ppack)
 
 
-    def get_phenopacket_id(self) -> str:
+    def get_phenopacket_id(self):
         return self._phenopacket_id
 
-    def get_subject_id(self) -> str:
+    def get_subject_id(self):
         return self._subject_id
 
     def get_sex(self):
         return self._sex
 
-    def get_age(self)-> str:
-        return self._time_at_last_encounter or "n/a"
+    def get_age(self):
+        return self._time_at_last_encounter
 
-    def get_disease(self) -> str:
-        return self._disease or "n/a"
+    def get_disease(self):
+        if self._disease is None:
+            return "n/a"
+        else:
+            return self._disease
 
     def get_observed_hpo_d(self):
         """
         returns map of observed phenotypic features with key (string) HP id, value, HpTerm from creation submodule
         """
         return self._observed
 
     def get_excluded_hpo_d(self):
         """
         :return: map of excluded phenotypic features with key (string) HP id, value, HpTerm from creation submodule
         """
         return self._excluded
 
-    def get_total_hpo_count(self):
-        """
-        :return: total count of HPO terms (observed and excluded)
-        :rtype: int
-        """
-        return len(self._observed) + len(self._excluded)
-
     def get_variant_list(self):
         return self._variant_list
 
     def has_pmid(self):
         return self._pmid is not None
 
     def get_pmid(self):
```

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/simple_variant.py` & `pyphetools-0.9.9/src/pyphetools/visualization/simple_variant.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         else:
             self._gene_id = NA_STRING
             self._gene_symbol = NA_STRING
         self._hgvs = NA_STRING
         if vdescript.expressions is not None and len(vdescript.expressions) > 0:
             for exprsn in vdescript.expressions:
                 if exprsn.syntax == "hgvs.c":
-                    self._hgvs = exprsn.value
+                    self._hgvs = exprsn.value       
         if vdescript.vcf_record is not None and len(vdescript.vcf_record.chrom) > 0:
             vcf = vdescript.vcf_record
             self._genome_ass = vcf.genome_assembly
             self._chrom = vcf.chrom
             self._pos = int(vcf.pos)
             self._ref = vcf.ref
             self._alt = vcf.alt
@@ -78,15 +78,15 @@
     @property
     def gene_symbol(self):
         """
         :returns: the gene synbol, e.g., FBN1
         :rtype: str
         """
         return self._gene_symbol
-
+    
     @property
     def hgvs(self):
         """
         :returns: Human Genome Variation Society (HGVS) variant nomenclature for this variant
         :rtype: str
         """
         return self._hgvs
@@ -94,15 +94,15 @@
     @property
     def genome_assembly(self):
         """
         :returns: genome build used for reporting this variant, e.g. hg38
         :rtype: str
         """
         return self._genome_ass
-
+    
     @property
     def chrom(self):
         """
         :returns: chromosome on which the variant is located
         :rtype: str
         """
         return self._chrom
@@ -130,25 +130,25 @@
         :rtype: str
         """
         return self._alt
 
     @property
     def genotype_id(self):
         """
-        :returns: the Sequence Ontology id for the genotype of this variant, optional
-        :rtype: str
-        """
+       :returns: the Sequence Ontology id for the genotype of this variant, optional
+       :rtype: str
+       """
         return self._genotype_id
 
     @property
     def genotype_label(self):
         """
-        :returns: the Sequence Ontology label for the genotype of this variant, optional
-        :rtype: str
-        """
+       :returns: the Sequence Ontology label for the genotype of this variant, optional
+       :rtype: str
+       """
         return self._genotype_label
 
     def has_vcf(self):
         """
         :returns: True if there is VCF data for this variant, otherwise False
         :rtype: bool
         """
@@ -156,16 +156,16 @@
 
     def has_genotype(self):
         """
         :returns: True if there is a genotype for this variant, otherwise False
         :rtype: bool
         """
         return self._genotype_id != NA_STRING
-
-
+    
+    
     def get_display(self):
         """
         :returns: a string representing a human-readable representation of the variant
         :rtype: str
         """
         if self.has_genotype():
             genotype = "(" + self._genotype_label + ")"
```

### Comparing `pyphetools-0.9.83/src/pyphetools/visualization/term_count.py` & `pyphetools-0.9.9/src/pyphetools/visualization/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.83/src/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.9.9/pyphetools.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.9.83
+Version: 0.9.9
 Summary: Generate and work with GA4GH phenopackets
-Author-email: Peter Robinson <peter.robinson@bih-charite.de>, Daniel Danis <daniel.gordon.danis@protonmail.com>
+Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,30 +32,24 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: hpo-toolkit<0.6.0,>=0.5.0
-Requires-Dist: matplotlib<4.0,>=3.2.0
-Requires-Dist: pandas[excel]<3.0.0,>=2.0.0
-Requires-Dist: phenopackets>=2.0.2
-Requires-Dist: protobuf<4.0.0,>=3.15.0
-Requires-Dist: requests<3.0,>=2.25.0
+Requires-Dist: hpo-toolkit>=0.3.0
+Requires-Dist: openpyxl
+Requires-Dist: pandas
+Requires-Dist: phenopackets
+Requires-Dist: protobuf
+Requires-Dist: requests
 Provides-Extra: test
-Requires-Dist: pytest<8.0.0,>=7.0.0; extra == "test"
-Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]<10,>=9.5.10; extra == "docs"
-Requires-Dist: mkdocs-material-extensions<2.0,>=1.3; extra == "docs"
-Requires-Dist: mkdocstrings[python]<1.0,>=0.22; extra == "docs"
-Requires-Dist: pillow; extra == "docs"
-Requires-Dist: cairosvg; extra == "docs"
+Requires-Dist: pytest; extra == "test"
 
-[![CI](https://github.com/monarch-initiative/pyphetools/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
+[![CI](https://github.com/monarch-initiative/genophenocorr/workflows/CI/badge.svg)](https://github.com/monarch-initiative/pyphetools/actions/workflows/python_ci.yml)
 
 # pyphetools
 Python Phenopacket Tools
 
 This package currently is designed to test how to use the Python version of the phenopackets package together with pandas to create phenopackets from typical supplemental tables.
 
 Development goals include making builder code similar to the Java package to create valid phenopackets and to perform JSON Schema-based validation.
```

### Comparing `pyphetools-0.9.83/src/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.9.9/pyphetools.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,140 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+./ppt_venv/bin/rst2html.py
+./ppt_venv/bin/rst2html4.py
+./ppt_venv/bin/rst2html5.py
+./ppt_venv/bin/rst2latex.py
+./ppt_venv/bin/rst2man.py
+./ppt_venv/bin/rst2odt.py
+./ppt_venv/bin/rst2odt_prepstyles.py
+./ppt_venv/bin/rst2pseudoxml.py
+./ppt_venv/bin/rst2s5.py
+./ppt_venv/bin/rst2xetex.py
+./ppt_venv/bin/rst2xml.py
+./ppt_venv/bin/rstpep2html.py
+./src/pyphetools/__init__.py
+./src/pyphetools/creation/__init__.py
+./src/pyphetools/creation/abstract_encoder.py
+./src/pyphetools/creation/age_column_mapper.py
+./src/pyphetools/creation/age_isoformater.py
+./src/pyphetools/creation/allelic_requirement.py
+./src/pyphetools/creation/case_encoder.py
+./src/pyphetools/creation/citation.py
+./src/pyphetools/creation/cohort_encoder.py
+./src/pyphetools/creation/column_mapper.py
+./src/pyphetools/creation/constant_column_mapper.py
+./src/pyphetools/creation/constants.py
+./src/pyphetools/creation/disease.py
+./src/pyphetools/creation/disease_id_column_mapper.py
+./src/pyphetools/creation/hgvs_variant.py
+./src/pyphetools/creation/hp_term.py
+./src/pyphetools/creation/hpo_cr.py
+./src/pyphetools/creation/hpo_exact_cr.py
+./src/pyphetools/creation/hpo_parser.py
+./src/pyphetools/creation/individual.py
+./src/pyphetools/creation/metadata.py
+./src/pyphetools/creation/mixed_cohort_encoder.py
+./src/pyphetools/creation/option_column_mapper.py
+./src/pyphetools/creation/sex_column_mapper.py
+./src/pyphetools/creation/simple_column_mapper.py
+./src/pyphetools/creation/structural_variant.py
+./src/pyphetools/creation/thresholded_column_mapper.py
+./src/pyphetools/creation/variant.py
+./src/pyphetools/creation/variant_column_mapper.py
+./src/pyphetools/creation/variant_validator.py
+./src/pyphetools/validation/__init__.py
+./src/pyphetools/validation/cohort_validator.py
+./src/pyphetools/validation/content_validator.py
+./src/pyphetools/validation/ontology_qc.py
+./src/pyphetools/validation/phenopacket_validator.py
+./src/pyphetools/validation/validated_individual.py
+./src/pyphetools/validation/validation_result.py
+./src/pyphetools/visualization/__init__.py
+./src/pyphetools/visualization/detailed_suppl_table.py
+./src/pyphetools/visualization/focus_count_table.py
+./src/pyphetools/visualization/hpo_category.py
+./src/pyphetools/visualization/hpoa_table_creator.py
+./src/pyphetools/visualization/html_table_generator.py
+./src/pyphetools/visualization/phenopacket_ingestor.py
+./src/pyphetools/visualization/phenopacket_table.py
+./src/pyphetools/visualization/qc_visualizer.py
+./src/pyphetools/visualization/simple_patient.py
+./src/pyphetools/visualization/simple_variant.py
+./src/pyphetools/visualization/term_count.py
+pyphetools.egg-info/PKG-INFO
+pyphetools.egg-info/SOURCES.txt
+pyphetools.egg-info/dependency_links.txt
+pyphetools.egg-info/not-zip-safe
+pyphetools.egg-info/requires.txt
+pyphetools.egg-info/top_level.txt
 src/pyphetools/__init__.py
-src/pyphetools.egg-info/PKG-INFO
-src/pyphetools.egg-info/SOURCES.txt
-src/pyphetools.egg-info/dependency_links.txt
-src/pyphetools.egg-info/not-zip-safe
-src/pyphetools.egg-info/requires.txt
-src/pyphetools.egg-info/top_level.txt
 src/pyphetools/creation/__init__.py
 src/pyphetools/creation/abstract_encoder.py
 src/pyphetools/creation/age_column_mapper.py
 src/pyphetools/creation/age_isoformater.py
-src/pyphetools/creation/age_of_death_mapper.py
 src/pyphetools/creation/allelic_requirement.py
-src/pyphetools/creation/case_template_encoder.py
+src/pyphetools/creation/case_encoder.py
 src/pyphetools/creation/citation.py
 src/pyphetools/creation/cohort_encoder.py
 src/pyphetools/creation/column_mapper.py
 src/pyphetools/creation/constant_column_mapper.py
 src/pyphetools/creation/constants.py
-src/pyphetools/creation/create_template.py
 src/pyphetools/creation/disease.py
 src/pyphetools/creation/disease_id_column_mapper.py
 src/pyphetools/creation/hgvs_variant.py
 src/pyphetools/creation/hp_term.py
 src/pyphetools/creation/hpo_cr.py
 src/pyphetools/creation/hpo_exact_cr.py
 src/pyphetools/creation/hpo_parser.py
-src/pyphetools/creation/import_template.py
 src/pyphetools/creation/individual.py
 src/pyphetools/creation/metadata.py
+src/pyphetools/creation/mixed_cohort_encoder.py
 src/pyphetools/creation/option_column_mapper.py
-src/pyphetools/creation/pyphetools_age.py
-src/pyphetools/creation/scm_generator.py
 src/pyphetools/creation/sex_column_mapper.py
 src/pyphetools/creation/simple_column_mapper.py
 src/pyphetools/creation/structural_variant.py
 src/pyphetools/creation/thresholded_column_mapper.py
-src/pyphetools/creation/thresholder.py
 src/pyphetools/creation/variant.py
 src/pyphetools/creation/variant_column_mapper.py
-src/pyphetools/creation/variant_manager.py
 src/pyphetools/creation/variant_validator.py
-src/pyphetools/creation/data/thresholds.tsv
-src/pyphetools/pp/__init__.py
-src/pyphetools/pp/_api.py
-src/pyphetools/pp/_timestamp.py
-src/pyphetools/pp/parse/__init__.py
-src/pyphetools/pp/parse/_io.py
-src/pyphetools/pp/parse/_pb.py
-src/pyphetools/pp/parse/_test_util.py
-src/pyphetools/pp/parse/_util.py
-src/pyphetools/pp/parse/json/__init__.py
-src/pyphetools/pp/parse/json/_json.py
-src/pyphetools/pp/v202/__init__.py
-src/pyphetools/pp/v202/_base.py
-src/pyphetools/pp/v202/_biosample.py
-src/pyphetools/pp/v202/_disease.py
-src/pyphetools/pp/v202/_gene_descriptor.py
-src/pyphetools/pp/v202/_individual.py
-src/pyphetools/pp/v202/_interpretation.py
-src/pyphetools/pp/v202/_measurement.py
-src/pyphetools/pp/v202/_medical_action.py
-src/pyphetools/pp/v202/_meta_data.py
-src/pyphetools/pp/v202/_phenopackets.py
-src/pyphetools/pp/v202/_phenotypic_feature.py
-src/pyphetools/pp/v202/_test_individual.py
-src/pyphetools/pp/v202/_vrsatile.py
 src/pyphetools/validation/__init__.py
 src/pyphetools/validation/cohort_validator.py
 src/pyphetools/validation/content_validator.py
 src/pyphetools/validation/ontology_qc.py
 src/pyphetools/validation/phenopacket_validator.py
 src/pyphetools/validation/validated_individual.py
 src/pyphetools/validation/validation_result.py
 src/pyphetools/visualization/__init__.py
-src/pyphetools/visualization/counted_hpo_term.py
 src/pyphetools/visualization/detailed_suppl_table.py
 src/pyphetools/visualization/focus_count_table.py
 src/pyphetools/visualization/hpo_category.py
 src/pyphetools/visualization/hpoa_table_creator.py
 src/pyphetools/visualization/html_table_generator.py
-src/pyphetools/visualization/individual_table.py
-src/pyphetools/visualization/onset_calculator.py
-src/pyphetools/visualization/phenopacket_charts.py
 src/pyphetools/visualization/phenopacket_ingestor.py
 src/pyphetools/visualization/phenopacket_table.py
 src/pyphetools/visualization/qc_visualizer.py
-src/pyphetools/visualization/simple_age.py
 src/pyphetools/visualization/simple_patient.py
 src/pyphetools/visualization/simple_variant.py
 src/pyphetools/visualization/term_count.py
-src/pyphetools/visualization/variant_visualizer.py
 test/test_age_column_mapper.py
 test/test_age_isoformater.py
 test/test_assume_excluded.py
+test/test_case_encoder.py
 test/test_cohort_validator.py
 test/test_constant_column_mapper.py
-test/test_disease.py
 test/test_hp_term.py
 test/test_hpo_category.py
 test/test_hpo_cr.py
 test/test_hpo_parser.py
-test/test_individual.py
 test/test_metadata.py
 test/test_ontology_qc.py
 test/test_option_column_mapper.py
 test/test_option_column_mapper2.py
 test/test_phenopacket_table.py
-test/test_pyphetools_age.py
-test/test_simple_age.py
 test/test_simple_variant.py
 test/test_structural_variant.py
 test/test_threshold_column_mapper.py
-test/test_thresholder.py
 test/test_validation_result.py
-test/test_variant.py
-test/test_vital_status.py
+test/test_variant.py
```

### Comparing `pyphetools-0.9.83/test/test_age_column_mapper.py` & `pyphetools-0.9.9/test/test_age_column_mapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import os
 import re
-from pyphetools.creation import AgeColumnMapper
+from src.pyphetools.creation import AgeColumnMapper
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 # The API requires us to pass a column name but the column name will not be used in the tests
 TEST_COLUMN = "test"
 
 string_to_iso_dict = {
     'Fetus': 'nan',
@@ -27,54 +27,54 @@
 }
 
 class TestOptionMapper(unittest.TestCase):
 
     def test_year(self):
         ageMapper = AgeColumnMapper.by_year(column_name=TEST_COLUMN)
         p3 = ageMapper.map_cell("3")
-        self.assertEqual("P3Y", p3.age_string)
+        self.assertEqual("P3Y", p3)
         p42 = ageMapper.map_cell("42")
-        self.assertEqual("P42Y", p42.age_string)
+        self.assertEqual("P42Y", p42)
 
     def test_iso8601(self):
         ageMapper = AgeColumnMapper.iso8601(column_name=TEST_COLUMN)
         p3y = ageMapper.map_cell("P3Y")
-        self.assertEqual("P3Y", p3y.age_string)
+        self.assertEqual("P3Y", p3y)
         p3m25d = ageMapper.map_cell("P3Y2M5D")
-        self.assertEqual("P3Y2M5D", p3m25d.age_string)
+        self.assertEqual("P3Y2M5D", p3m25d)
 
     def test_year_month_both_1(self):
         ageMapper = AgeColumnMapper.by_year_and_month(column_name=TEST_COLUMN)
         age_string = "14 y 8 m"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P14Y8M", age_iso.age_string)
+        self.assertEqual("P14Y8M", age_iso)
 
     def test_year_month_both_2(self):
         ageMapper = AgeColumnMapper.by_year_and_month(column_name=TEST_COLUMN)
         age_string = "7 y 6 m"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P7Y6M", age_iso.age_string)
+        self.assertEqual("P7Y6M", age_iso)
 
     def test_year_month_both_3(self):
         ageMapper = AgeColumnMapper.by_year_and_month(column_name=TEST_COLUMN)
         age_string = "7y6m"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P7Y6M", age_iso.age_string)
+        self.assertEqual("P7Y6M", age_iso)
 
     def test_year_month_just_year_1(self):
         ageMapper = AgeColumnMapper.by_year_and_month(column_name=TEST_COLUMN)
         age_string = "7 y"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P7Y", age_iso.age_string)
+        self.assertEqual("P7Y", age_iso)
 
     def test_year_month_just_month_1(self):
         ageMapper = AgeColumnMapper.by_year_and_month(column_name=TEST_COLUMN)
         age_string = "2 m"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P2M", age_iso.age_string)
+        self.assertEqual("P2M", age_iso)
 
     def test_int_or_float_regex(self):
         int_or_float = r"(\d+)(\.\d+)?"
         p=re.compile(int_or_float)
         y_only = "42"
         results = p.search(y_only).groups()
         self.assertEqual(2, len(results))
@@ -86,58 +86,47 @@
         self.assertEqual('42', results[0])
         self.assertEqual('.25', results[1])
 
     def test_fractional_year_strings(self):
         ageMapper = AgeColumnMapper.by_year(column_name=TEST_COLUMN)
         age_string = "2"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P2Y", age_iso.age_string)
+        self.assertEqual("P2Y", age_iso)
         age_string = "4.75"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P4Y9M", age_iso.age_string)
+        self.assertEqual("P4Y9M", age_iso)
         age_string = "5.9"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P5Y11M", age_iso.age_string)
+        self.assertEqual("P5Y11M", age_iso)
         age_string = "6.25"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P6Y3M", age_iso.age_string)
+        self.assertEqual("P6Y3M", age_iso)
         age_string = "8.1"
         age_iso = ageMapper.map_cell(age_string)
-        self.assertEqual("P8Y1M", age_iso.age_string)
+        self.assertEqual("P8Y1M", age_iso)
 
     def test_custom_dictionary(self):
         ageMapper = AgeColumnMapper.custom_dictionary(column_name=TEST_COLUMN, string_to_iso_d=string_to_iso_dict)
         age_iso = ageMapper.map_cell("1.5")
-        self.assertEqual("P1Y6M", age_iso.age_string)
+        self.assertEqual("P1Y6M", age_iso)
         age_iso = ageMapper.map_cell("3.5")
-        self.assertEqual("P3Y6M", age_iso.age_string)
+        self.assertEqual("P3Y6M", age_iso)
         age_iso = ageMapper.map_cell("birth")
-        self.assertEqual("P1D", age_iso.age_string)
+        self.assertEqual("P1D", age_iso)
         age_iso = ageMapper.map_cell("NOT THERE")
-        self.assertFalse(age_iso.is_valid())
+        NOT_PROVIDED = 'NOT_PROVIDED' # from Constants.py which is not exported
+        self.assertEqual(NOT_PROVIDED, age_iso)
 
     def test_by_month(self):
         ageMapper = AgeColumnMapper.by_month(column_name=TEST_COLUMN)
         age_iso = ageMapper.map_cell(5)
-        self.assertEqual("P5M", age_iso.age_string)
-
-
-    def test_by_month2(self):
-        ageMapper = AgeColumnMapper.by_month(column_name=TEST_COLUMN)
-        age_iso = ageMapper.map_cell(0.5)
-        self.assertEqual("P15D", age_iso.age_string)
-
-    def test_by_month(self):
-        ageMapper = AgeColumnMapper.by_month(column_name=TEST_COLUMN)
+        self.assertEqual("P5M", age_iso)
         age_iso = ageMapper.map_cell("5")
-        self.assertEqual("P5M", age_iso.age_string)
+        self.assertEqual("P5M", age_iso)
+        age_iso = ageMapper.map_cell(0.5)
+        self.assertEqual("P15D", age_iso)
         age_iso = ageMapper.map_cell(0.8)
-        self.assertEqual("P24D", age_iso.age_string)
-
-    def test_by_month_one_year(self):
-        ageMapper = AgeColumnMapper.by_month(column_name=TEST_COLUMN)
+        self.assertEqual("P24D", age_iso)
         age_iso = ageMapper.map_cell(12)
-        self.assertEqual("P1Y", age_iso.age_string)
-
-
+        self.assertEqual("P1Y", age_iso)
```

### Comparing `pyphetools-0.9.83/test/test_age_isoformater.py` & `pyphetools-0.9.9/test/test_age_isoformater.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import unittest
-
-from pyphetools.creation import AgeIsoFormater
+from src.pyphetools.creation import AgeIsoFormater
 
 
 
 class TestAgeIsoFormater(unittest.TestCase):
 
     def test_basic1(self):
         iso_age = AgeIsoFormater.to_string(y=2, m=3, d=5)
```

### Comparing `pyphetools-0.9.83/test/test_assume_excluded.py` & `pyphetools-0.9.9/test/test_assume_excluded.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import os
 import unittest
-
-from pyphetools.creation import HpoParser, OptionColumnMapper
+import os
+from src.pyphetools.creation import HpoParser, OptionColumnMapper
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
 class TestAssumeExcluded(unittest.TestCase):
     """
     This test class checks the function of the assumeExcluded argument of the OptionColumnMapper.
@@ -23,46 +22,41 @@
 
     def test_without_assume_exclusion(self):
         comorbidities_d = {'Insulindependentdiabetes-onsetatage19': 'Type II diabetes mellitus',
                             'COPD': 'Chronic pulmonary obstruction',
                             'Diastolicdysfunction': 'Left ventricular diastolic dysfunction',
                             'Lymphocytosis': 'Lymphocytosis',
                             'Single kidney': 'Unilateral renal agenesis'}
-        comorbiditiesMapper = OptionColumnMapper(column_name="placeholder",
-                                                concept_recognizer=self.hpo_cr,
-                                                option_d=comorbidities_d)
+        comorbiditiesMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=comorbidities_d)
         results = comorbiditiesMapper.map_cell('COPD')
         self.assertEqual(1, len(results))
         hpo_term = results[0]
         self.assertEqual('Chronic pulmonary obstruction', hpo_term.label)
         self.assertEqual('HP:0006510', hpo_term.id)
 
     def test_with_assume_exclusion(self):
-        excluded_d = {'Insulindependentdiabetes-onsetatage19': 'Type II diabetes mellitus',
+        comorbidities_d = {'Insulindependentdiabetes-onsetatage19': 'Type II diabetes mellitus',
                             'COPD': 'Chronic pulmonary obstruction',
                             'Diastolicdysfunction': 'Left ventricular diastolic dysfunction',
                             'Lymphocytosis': 'Lymphocytosis',
                             'Single kidney': 'Unilateral renal agenesis'}
-        comorbiditiesMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d={}, excluded_d=excluded_d)
+        comorbiditiesMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=comorbidities_d, assumeExcluded=True)
         results = comorbiditiesMapper.map_cell('COPD')
-        self.assertEqual(1, len(results))
+        self.assertEqual(5, len(results))
+        results.sort(key=lambda x: x.label) # sort alphabetically
         hpo0 = results[0]
         self.assertEqual('Chronic pulmonary obstruction', hpo0.label)
         self.assertEqual('HP:0006510', hpo0.id)
-        self.assertFalse(hpo0.observed)
-        results = comorbiditiesMapper.map_cell('Diastolicdysfunction')
-        hpo1 = results[0]
+        self.assertTrue(hpo0.observed)
+        hpo1 = results[1]
         self.assertEqual("Left ventricular diastolic dysfunction", hpo1.label)
         self.assertEqual("HP:0025168", hpo1.id)
         self.assertFalse(hpo1.observed)
-        results = comorbiditiesMapper.map_cell('Lymphocytosis')
-        hpo2 = results[0]
+        hpo2 = results[2]
         self.assertEqual("Lymphocytosis", hpo2.label)
         self.assertFalse(hpo2.observed)
-        results = comorbiditiesMapper.map_cell('Insulindependentdiabetes-onsetatage19')
-        hpo3 = results[0]
+        hpo3 = results[3]
         self.assertEqual("Type II diabetes mellitus", hpo3.label)
         self.assertFalse(hpo3.observed)
-        results = comorbiditiesMapper.map_cell('Single kidney')
-        hpo4 = results[0]
+        hpo4 = results[4]
         self.assertEqual("Unilateral renal agenesis", hpo4.label)
         self.assertFalse(hpo4.observed)
```

### Comparing `pyphetools-0.9.83/test/test_cohort_validator.py` & `pyphetools-0.9.9/test/test_cohort_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,80 @@
-import hpotk
-import pytest
+import os
+import unittest
 
-from pyphetools.creation import Disease,Individual, HpTerm
-from pyphetools.validation import CohortValidator
+from src.pyphetools.creation import Individual, HpTerm, HpoParser
+from src.pyphetools.validation import CohortValidator
+from src.pyphetools.validation.validation_result import ErrorLevel, Category
 
+HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 # The API requires us to pass a column name but the column name will not be used in the tests
 TEST_COLUMN = "test"
 
+HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
-class TestCohortValidator:
+class TestCohortValidator(unittest.TestCase):
 
-    @pytest.fixture
-    def ind_a(self) -> Individual:
-        i = Individual(individual_id="A")
-        i.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
-        i.add_hpo_term(HpTerm(hpo_id="HP:0011525", label="Iris nevus"))
-        i.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
-        i.set_disease(disease=Disease(disease_id="OMIM:123456", disease_label="label"))
-        return i
-
-    @pytest.fixture
-    def ind_b(self) -> Individual:
-        i = Individual(individual_id="B")
-        i.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
-        i.add_hpo_term(HpTerm(hpo_id="HP:0011525", label="Iris nevus"))
-        i.set_disease(disease=Disease(disease_id="OMIM:123456", disease_label="label"))
-        return i
-
-    def test_redundant_term(
-            self,
-            hpo: hpotk.Ontology,
-            ind_a: Individual,
-    ):
-        cohort = [ind_a]
-        cvalidator = CohortValidator(cohort=cohort, ontology=hpo, min_hpo=1)
+    @classmethod
+    def setUpClass(cls) -> None:
+        individual_A = Individual(individual_id="A")
+        individual_A.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
+        individual_A.add_hpo_term(HpTerm(hpo_id="HP:0011525", label="Iris nevus"))
+        individual_A.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
+        individual_B = Individual(individual_id="B")
+        individual_B.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
+        individual_B.add_hpo_term(HpTerm(hpo_id="HP:0011525", label="Iris nevus"))
+        cls._individual_A = individual_A
+        cls._individual_B = individual_B
+        parser = HpoParser(hpo_json_file=HP_JSON_FILENAME)
+        cls.hpo_cr = parser.get_hpo_concept_recognizer()
+
+
+    def test_redundant_term(self):
+        cohort = [self._individual_A]
+        hpo_ontology = self.hpo_cr.get_hpo_ontology()
+        cvalidator = CohortValidator(cohort=cohort, ontology=hpo_ontology, min_hpo=1)
         validated_individuals = cvalidator.get_validated_individual_list()
-        assert len(validated_individuals) == 1
-
+        self.assertEqual(1, len(validated_individuals))
         vindindividualA = validated_individuals[0]
-        assert vindindividualA.has_error()
-
+        self.assertTrue(vindindividualA.has_error())
         errors = vindindividualA.get_validation_errors()
-        assert len(errors) == 1
-
+        self.assertEqual(1, len(errors))
         error = errors[0]
-        assert error.error_level == "WARNING"
-        assert error.category == "DUPLICATE"
-        assert error.message == "<b>Deeply set eye</b> is listed multiple times"
-        assert error.term.id == "HP:0000490"
-        assert error.term.label == "Deeply set eye"
-
-    def test_no_redundant_term(
-            self,
-            hpo: hpotk.Ontology,
-            ind_b: Individual,
-    ):
-        cohort = [ind_b]
-        cvalidator = CohortValidator(cohort=cohort, ontology=hpo, min_hpo=1)
-
+        self.assertEqual("WARNING", error.error_level)
+        self.assertEqual("DUPLICATE", error.category)
+        self.assertEqual("<b>Deeply set eye</b> is listed multiple times", error.message)
+        self.assertEqual("HP:0000490", error.term.id)
+        self.assertEqual("Deeply set eye", error.term.label)
+
+    def test_no_redundant_term(self):
+        cohort = [self._individual_B]
+        hpo_ontology = self.hpo_cr.get_hpo_ontology()
+        cvalidator = CohortValidator(cohort=cohort, ontology=hpo_ontology, min_hpo=1)
         validated_individuals = cvalidator.get_validated_individual_list()
-        assert len(validated_individuals) == 1
-
+        self.assertEqual(1, len(validated_individuals))
         vindindividualB = validated_individuals[0]
-        assert not vindindividualB.has_error()
+        self.assertFalse(vindindividualB.has_error())
 
-    def test_redundant_in_hierarchy(self, hpo: hpotk.Ontology):
+    def test_redundant_in_hierarchy(self):
         """
         0358596_patientA.json,ERROR,HpoAncestryValidator,Violation of the annotation propagation rule,
         "Phenotypic features of PMID_20358596_patient_A must not contain both an
         observed term (Bilateral facial palsy, HP:0430025) and an observed ancestor (Facial palsy, HP:0010628)"
         """
         individual_C = Individual(individual_id="C")
         individual_C.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
         individual_C.add_hpo_term(HpTerm(hpo_id="HP:0011525", label="Iris nevus"))
         individual_C.add_hpo_term(HpTerm(hpo_id="HP:0430025", label="Bilateral facial palsy"))
         individual_C.add_hpo_term(HpTerm(hpo_id="HP:0010628", label="Facial palsy"))
-        individual_C.set_disease(disease=Disease(disease_id="OMIM:123456", disease_label="label"))
         cohort = [individual_C]
-        cvalidator = CohortValidator(cohort=cohort, ontology=hpo, min_hpo=1)
+        hpo_ontology = self.hpo_cr.get_hpo_ontology()
+        cvalidator = CohortValidator(cohort=cohort, ontology=hpo_ontology, min_hpo=1)
         validated_individuals = cvalidator.get_validated_individual_list()
-        assert len(validated_individuals) == 1
-
+        self.assertEqual(1, len(validated_individuals))
         individual_C = validated_individuals[0]
-        assert individual_C.has_error()
-
+        self.assertTrue(individual_C.has_error())
         errors = individual_C.get_validation_errors()
-        assert len(errors) == 1
-
+        self.assertEqual(1, len(errors))
         error = errors[0]
-        assert error.message == "<b>Facial palsy</b> is redundant because of <b>Bilateral facial palsy</b>"
+        self.assertEqual("<b>Facial palsy</b> is redundant because of <b>Bilateral facial palsy</b>", error.message)
 
-    def test_error_if_no_disease(self, hpo: hpotk.Ontology):
-        individual_D = Individual(individual_id="D")
-        individual_D.add_hpo_term(HpTerm(hpo_id="HP:0000490", label="Deeply set eye"))
-        cohort = [individual_D]
-        cvalidator = CohortValidator(cohort=cohort, ontology=hpo, min_hpo=1)
-        validated_individuals = cvalidator.get_validated_individual_list()
-        assert len(validated_individuals) == 1
-        individual_D = validated_individuals[0]
-        errors = individual_D.get_validation_errors()
-        assert len(errors) == 1
-        error = errors[0]
-        assert error.message == "Individual had 0 disease annotation(s) but the mininum required count is 1"
```

### Comparing `pyphetools-0.9.83/test/test_constant_column_mapper.py` & `pyphetools-0.9.9/test/test_constant_column_mapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import unittest
-from pyphetools.creation import ConstantColumnMapper
+from src.pyphetools.creation import ConstantColumnMapper
 
 
 
 class TestConstantMapper(unittest.TestCase):
-
+        
     def test_observed_constant(self):
         hp_id =  "HP:0031956"
         hp_label = "Elevated circulating aspartate aminotransferase concentration"
-        mapper = ConstantColumnMapper(column_name="placeholder",hpo_id=hp_id, hpo_label=hp_label)
+        mapper = ConstantColumnMapper(hpo_id=hp_id, hpo_label=hp_label)
         hp_term_list = mapper.map_cell("n/a")
         self.assertEqual(1, len(hp_term_list))
         result = hp_term_list[0]
         self.assertEqual(hp_id, result.id)
         self.assertEqual(hp_label, result.label)
         self.assertTrue(result.observed)
-
+        
     def test_excluded_constant(self):
         hp_id =  "HP:0031956"
         hp_label = "Elevated circulating aspartate aminotransferase concentration"
-        mapper = ConstantColumnMapper(column_name="placeholder", hpo_id=hp_id, hpo_label=hp_label, excluded=True)
+        mapper = ConstantColumnMapper(hpo_id=hp_id, hpo_label=hp_label, excluded=True)
         hp_term_list = mapper.map_cell("n/a")
         self.assertEqual(1, len(hp_term_list))
         result = hp_term_list[0]
         self.assertEqual(hp_id, result.id)
         self.assertEqual(hp_label, result.label)
         self.assertFalse(result.observed)
         self.assertTrue(result.excluded)
```

### Comparing `pyphetools-0.9.83/test/test_hpo_category.py` & `pyphetools-0.9.9/test/test_hpo_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from pyphetools.visualization import HpoCategorySet
+from src.pyphetools.visualization import HpoCategorySet
 
 from hpotk.ontology.load.obographs import load_ontology
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
 class TestHpoCategorySet(unittest.TestCase):
```

### Comparing `pyphetools-0.9.83/test/test_hpo_cr.py` & `pyphetools-0.9.9/test/test_hpo_cr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import unittest
 
-from pyphetools.creation import HpoParser
+from src.pyphetools.creation import HpoParser
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
 class TestOptionMapper(unittest.TestCase):
 
     @classmethod
```

### Comparing `pyphetools-0.9.83/test/test_hpo_parser.py` & `pyphetools-0.9.9/test/test_hpo_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from pyphetools.creation import HpoParser
+from src.pyphetools.creation import HpoParser
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 class TestHpoParser(unittest.TestCase):
     
     @classmethod
     def setUpClass(cls) -> None:
```

### Comparing `pyphetools-0.9.83/test/test_metadata.py` & `pyphetools-0.9.9/test/test_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import pytest
 
-from pyphetools.creation import MetaData, Citation
+from src.pyphetools.creation import MetaData, Citation
 
 
 class TestMetaData(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         hpo_version = "fake.version"
```

### Comparing `pyphetools-0.9.83/test/test_ontology_qc.py` & `pyphetools-0.9.9/test/test_ontology_qc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,110 @@
-import hpotk
-import pytest
+import unittest
+import os
+from src.pyphetools.creation import HpoParser, HpTerm, Individual
+from src.pyphetools.validation import OntologyQC
 
-from pyphetools.creation import HpTerm, Individual, IsoAge
-from pyphetools.validation import OntologyQC
 
+HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
-
-class TestOntologyQC:
-
-    @pytest.fixture
-    def ontology_qc(self, hpo: hpotk.Ontology) -> OntologyQC:
+class TestOntologyQC(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls) -> None:
+        parser = HpoParser(hpo_json_file=HP_JSON_FILENAME)
+        hpo_cr = parser.get_hpo_concept_recognizer()
+        cls._ontology = hpo_cr.get_hpo_ontology()
         individual = Individual(individual_id="id")
-        return OntologyQC(ontology=hpo, individual=individual)
+        cls._qc = OntologyQC(ontology=cls._ontology, individual=individual)
 
+    def test_non_null(self):
+        self.assertIsNotNone(self._qc)
 
-    def test_conflict(self, hpo: hpotk.Ontology):
+    def test_conflict(self):
         """
         Arachnodactyly is a child of Slender finger, and so the following is a conflict
         """
         arachTerm = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         slenderTerm = HpTerm(hpo_id="HP:0001238", label="Slender finger", observed=False)
         hpo_terms = [arachTerm, slenderTerm]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-
-        qc = OntologyQC(ontology=hpo, individual=individual)
-
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         qc_hpo_terms = qc.get_clean_terms()
-        assert len(qc_hpo_terms) == 1
+        self.assertEqual(1, len(qc_hpo_terms))
 
-    def test_do_not_detect_conflict_if_there_is_no_conflict(self, hpo: hpotk.Ontology):
+    def test_do_not_detect_conflict_if_there_is_no_conflict(self):
         """
         These terms are unrelated so it is NOT a conflict
         """
         arachTerm = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         # the following is not a conflict and should not be removed
         hipDislocation = HpTerm(hpo_id="HP:0002827", label="Hip dislocation", observed=False)
         hpo_terms = [arachTerm, hipDislocation]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-
-        qc = OntologyQC(ontology=hpo, individual=individual)
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         qc_hpo_terms = qc.get_clean_terms()
+        self.assertEqual(2, len(qc_hpo_terms))
 
-        assert len(qc_hpo_terms) == 2
-
-    def test_do_not_detect_conflict_if_there_is_no_conflict_2(self, hpo: hpotk.Ontology):
+    def test_do_not_detect_conflict_if_there_is_no_conflict_2(self):
         """
         This is not a conflict because the subclass is excluded while the superclass is observed
         """
         arachTerm = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=False)
         slenderTerm = HpTerm(hpo_id="HP:0001238", label="Slender finger", observed=True)
         hpo_terms = [arachTerm, slenderTerm]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-        qc = OntologyQC(ontology=hpo, individual=individual)
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         qc_hpo_terms = qc.get_clean_terms()
-        assert len(qc_hpo_terms) == 2
+        self.assertEqual(2, len(qc_hpo_terms))
 
-    def test_redundancy(self, hpo: hpotk.Ontology):
+    def test_redundancy(self):
         arachTerm = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         slenderTerm = HpTerm(hpo_id="HP:0001238", label="Slender finger", observed=True)
         hpo_terms = [arachTerm, slenderTerm]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-        qc = OntologyQC(ontology=hpo, individual=individual)
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         qc_hpo_terms = qc.get_clean_terms()
+        self.assertEqual(1, len(qc_hpo_terms))
 
-        assert len(qc_hpo_terms) == 1
-
-    def test_do_not_remove_if_not_redundant(self, hpo: hpotk.Ontology):
+    def test_do_not_remove_if_not_redundant(self):
         arachTerm = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         hipDislocation = HpTerm(hpo_id="HP:0002827", label="Hip dislocation", observed=False)
         hpo_terms = [arachTerm, hipDislocation]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-        qc = OntologyQC(ontology=hpo, individual=individual)
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         qc_hpo_terms = qc.get_clean_terms()
-
-        assert len(qc_hpo_terms) == 2
+        self.assertEqual(2, len(qc_hpo_terms))
 
 
-    def test_exact_redundancy(self, hpo: hpotk.Ontology):
+    def test_redundancy(self):
         arachTerm = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         arachTerm2 = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         hipDislocation = HpTerm(hpo_id="HP:0002827", label="Hip dislocation", observed=False)
         hpo_terms = [arachTerm, arachTerm2, hipDislocation]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-        qc = OntologyQC(ontology=hpo, individual=individual)
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         qc_hpo_terms = qc.get_clean_terms()
-
-        assert len(qc_hpo_terms) == 2
-
+        self.assertEqual(2, len(qc_hpo_terms))
         error_list = qc.get_error_list()
-
-        assert len(error_list) == 1
-
+        self.assertEqual(1, len(error_list))
         error = error_list[0]
-
-        assert error.error_level == 'WARNING'
-        assert error.category == 'DUPLICATE'
+        self.assertEqual("WARNING", error.error_level)
+        self.assertEqual("DUPLICATE", error.category)
 
 
-    def test_same_term_observed_and_excluded(self, hpo: hpotk.Ontology):
+    def test_same_term_observed_and_excluded(self):
         arachTermObserved = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=True)
         arachTermExcluded = HpTerm(hpo_id="HP:0001166", label="Arachnodactyly", observed=False)
         hipDislocation = HpTerm(hpo_id="HP:0002827", label="Hip dislocation", observed=True)
         hpo_terms = [arachTermObserved, hipDislocation, arachTermExcluded]
         individual = Individual(individual_id="id", hpo_terms=hpo_terms)
-        qc = OntologyQC(ontology=hpo, individual=individual)
+        qc = OntologyQC(ontology=self._ontology, individual=individual)
         error_list = qc.get_error_list()
-
-        assert len(error_list) == 1
-
+        self.assertEqual(1, len(error_list))
         error = error_list[0]
+        self.assertEqual("ERROR", error.error_level)
+        self.assertEqual("OBSERVED_AND_EXCLUDED", error.category)
+        self.assertEqual("Term Arachnodactyly (HP:0001166) was annotated to be both observed and excluded.", error.message)
 
-        assert error.error_level == "ERROR"
-        assert error.category == "OBSERVED_AND_EXCLUDED"
-        assert error.message == "Term Arachnodactyly (HP:0001166) was annotated to be both observed and excluded."
 
-    def test_redundancy_with_and_without_onset(self, hpo: hpotk.Ontology):
-        """
-        If we have Myoclonic seizure with onset P1Y and Seizure with no onset, then we do not want to include
-        Seizure in the final output because it is redundant.
-        Myoclonic seizure HP:0032794 ("grandchild" of Seizure)
-        Seizure HP:0001250
-        """
-        onset = IsoAge.from_iso8601("P1Y")
-        myoclonic_seiz = HpTerm(hpo_id="HP:0032794", label="Myoclonic seizure", observed=True, onset=onset)
-        seiz = HpTerm(hpo_id="HP:0001250", label="Seizure", observed=True)
-        hpo_terms = [myoclonic_seiz, seiz]
-        individual = Individual(individual_id="id", hpo_terms=hpo_terms)
 
-        qc = OntologyQC(ontology=hpo, individual=individual)
-
-        qc_hpo_terms = qc.get_clean_terms()
 
-        assert len(qc_hpo_terms) == 1
```

### Comparing `pyphetools-0.9.83/test/test_option_column_mapper.py` & `pyphetools-0.9.9/test/test_option_column_mapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from pyphetools.creation import HpoParser, OptionColumnMapper
+from src.pyphetools.creation import HpoParser, OptionColumnMapper
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
 class TestOptionMapper(unittest.TestCase):
 
     @classmethod
@@ -14,48 +14,48 @@
         cls.severity_d = {'mild': 'Intellectual disability, mild',
                         'moderate': 'Intellectual disability, moderate',
                         'severe': 'Intellectual disability, severe'
                         }
 
     def test_hpo_cr_mild(self):
         """We should retrieve Intellectual disability, mild (HP:0001256)"""
-        optionMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=self.severity_d)
+        optionMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=self.severity_d)
         results = optionMapper.map_cell("mild")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0001256", result.id)
         self.assertEqual("Intellectual disability, mild", result.label)
 
     def test_hpo_cr_moderate(self):
         """We should retrieve Intellectual disability, moderate (HP:0002342)"""
-        optionMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=self.severity_d)
+        optionMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=self.severity_d)
         results = optionMapper.map_cell("moderate")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0002342", result.id)
         self.assertEqual("Intellectual disability, moderate", result.label)
 
     def test_hpo_cr_severe(self):
         """We should retrieve Intellectual disability, severe (HP:0010864) """
-        optionMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=self.severity_d)
+        optionMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=self.severity_d)
         results = optionMapper.map_cell("severe")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0010864", result.id)
         self.assertEqual("Intellectual disability, severe", result.label)
 
     def test_with_acronyms(self):
         other_d = {
             "HP": "High palate",
             "D": "Dolichocephaly",
             "En": "Deeply set eye",  # i.e., Enophthalmus
             "DE": "Dural ectasia",
             "St": "Striae distensae"
         }
-        otherMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=other_d)
+        otherMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=other_d)
         res1 = otherMapper.map_cell("HP")
         res1.sort(key=lambda x: x.label) # sort alphabetically
         self.assertIsNotNone(res1)
         self.assertEqual(1, len(res1))
         hpterm = res1[0]
         self.assertEqual("High palate", hpterm.label)
         self.assertEqual("HP:0000218", hpterm.id)
@@ -69,27 +69,27 @@
         hpterm = res2[1]
         self.assertEqual("High palate", hpterm.label)
         self.assertEqual("HP:0000218", hpterm.id)
 
     def test_eso(self):
         oph_d = {"strabismus": "Strabismus",
                 "esotropia": "Esotropia"}
-        ophMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=oph_d)
+        ophMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=oph_d)
         res = ophMapper.map_cell("right sided esotropia")
         self.assertIsNotNone(res)
         self.assertEqual(1, len(res))
         hpterm = res[0]
         self.assertEqual("Esotropia", hpterm.label)
         self.assertEqual("HP:0000565", hpterm.id)
 
     def test_option_list(self):
         thumb_d = {"BT": "Broad thumb",
                     "BH": "Broad hallux",
                     "+": ["Broad thumb", "Broad hallux"]}
-        thumbMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=thumb_d)
+        thumbMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=thumb_d)
         res = thumbMapper.map_cell("+")
         res.sort(key=lambda x: x.label) # sort alphabetically
         self.assertIsNotNone(res)
         self.assertEqual(2, len(res))
         hpterm0 = res[0]
         self.assertEqual("Broad hallux", hpterm0.label)
         self.assertEqual("HP:0010055", hpterm0.id)
@@ -97,15 +97,15 @@
         self.assertEqual("Broad thumb", hpterm1.label)
         self.assertEqual("HP:0011304", hpterm1.id)
 
     def test_options_broad(self):
         thumb_d = {"BT": "Broad thumb",
                     "BH": "Broad hallux",
                     "+": [ "Broad thumb", "Broad hallux"]}
-        thumbMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=thumb_d)
+        thumbMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=thumb_d)
         res = thumbMapper.map_cell("BT, BH")
         res.sort(key=lambda x: x.label) # sort alphabetically
         self.assertIsNotNone(res)
         self.assertEqual(2, len(res))
         hpterm0 = res[0]
         self.assertEqual("Broad hallux", hpterm0.label)
         self.assertEqual("HP:0010055", hpterm0.id)
@@ -114,15 +114,15 @@
         self.assertEqual("HP:0011304", hpterm1.id)
 
     def test_options_negative(self):
         thumb_d = {"BT": "Broad thumb",
                 "BH": "Broad hallux",
                 "+": ["Broad thumb", "Broad hallux"]}
         excluded_d = {"-":"Broad thumb"}
-        thumbMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=thumb_d,
+        thumbMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=thumb_d,
                                         excluded_d=excluded_d)
         res = thumbMapper.map_cell("-")
         self.assertIsNotNone(res)
         self.assertEqual(1, len(res))
         hpterm0 = res[0]
         self.assertEqual("Broad thumb", hpterm0.label)
         self.assertEqual("HP:0011304", hpterm0.id)
@@ -136,16 +136,15 @@
         autistic_like_behavior_d = {
             'stereotypies': 'Motor stereotypy',
             'yes - was being investigated': 'Autism',
             'Severe autism': 'Autism',
             'yes': 'Autism'}
         exluded_d = {'no': 'Autism',
                     'no formal testing (no concern for ASD)': 'Autism', }
-        autisticMapper = OptionColumnMapper(column_name="placeholder",
-                                            concept_recognizer=self.hpo_cr,
+        autisticMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr,
                                             option_d=autistic_like_behavior_d,
                                             excluded_d=exluded_d)
         hpo_term_list = autisticMapper.map_cell("yes - was being investigated")
         self.assertEqual(1, len(hpo_term_list))
 
     def test_metabolic(self):
         """
@@ -154,16 +153,15 @@
         """
         urine_xa_d = {'11.7umol/mmolCr': "Xanthinuria",
                     '1.7umol/mmolCr': "Xanthinuria"}
         urine_not_xa_d = {'0.04mmol/L': "Xanthinuria",
                         "1.6umol/mmolCr": "Xanthinuria",
                         "0.0214XA/Cr": "Xanthinuria",
                         "normal": "Xanthinuria"}
-        urineXAmapper = OptionColumnMapper(column_name="placeholder",
-                                        concept_recognizer=self.hpo_cr,
+        urineXAmapper = OptionColumnMapper(concept_recognizer=self.hpo_cr,
                                         option_d=urine_xa_d,
                                         excluded_d=urine_not_xa_d)
         hpo_term_list = urineXAmapper.map_cell('11.7umol/mmolCr')
         self.assertEqual(1, len(hpo_term_list))
         hpterm = hpo_term_list[0]
         self.assertEqual("Xanthinuria", hpterm.label)
         self.assertEqual("HP:0010934", hpterm.id)
```

### Comparing `pyphetools-0.9.83/test/test_option_column_mapper2.py` & `pyphetools-0.9.9/test/test_option_column_mapper2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from pyphetools.creation import HpoParser, OptionColumnMapper
+from src.pyphetools.creation import HpoParser, OptionColumnMapper
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
 class TestOptionColumnMapper2(unittest.TestCase):
 
     @classmethod
@@ -14,31 +14,29 @@
 
     def test_multiple_items_in_cell_1(self):
         seizure_d = {'Absence': 'Typical absence seizure',
                     'Infantile spasms': "Infantile spasms" ,
                     'GTC': 'Bilateral tonic-clonic seizure' ,
                     'ESES': "Status epilepticus"
                     }
-        seizureMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=seizure_d)
+        seizureMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=seizure_d)
         results = seizureMapper.map_cell("Absence")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0011147", result.id)
         self.assertEqual("Typical absence seizure", result.label)
         self.assertTrue(result.observed)
         self.assertTrue(result.measured)
 
     def test_multiple_items_in_cell_2(self):
         seizure_d = {'Absence': 'Typical absence seizure',
                     'Infantile spasms': "Infantile spasms",
                     'GTC': 'Bilateral tonic-clonic seizure',
                     'ESES': "Status epilepticus"}
-        seizureMapper = OptionColumnMapper(column_name="placeholder",
-                                        concept_recognizer=self.hpo_cr,
-                                        option_d=seizure_d)
+        seizureMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=seizure_d)
         results = seizureMapper.map_cell("Absence and GTC")
         self.assertEqual(2, len(results))
         results = sorted(results, key=lambda x: x.id, reverse=True)
         result = results[0]
         self.assertEqual("HP:0011147", result.id)
         self.assertEqual("Typical absence seizure", result.label)
         self.assertTrue(result.observed)
@@ -53,57 +51,57 @@
         morph_d = {
             'bulbous nasal tip': "Bulbous nose",
             'prominent lobule of ear': "Large earlobe",
             'tapering fingers': "Tapered finger",
             'deeply set eyes': 'Deeply set eye'
         }
         cell_contents = "Broad forehead, deeply set eyes, ptosis, bulbous nasal tip, micrognathia, prominent lobule of ear, tapering fingers"
-        morphMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=morph_d)
+        morphMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=morph_d)
         results = morphMapper.map_cell(cell_contents)
         self.assertEqual(7, len(results))
         results = sorted(results, key=lambda x: x.id, reverse=True)
 
     def test_hpo_cr_non_null(self):
         """sanity check"""
         self.assertIsNotNone(self.hpo_cr)
 
     def test_hpo_cr_ataxia(self):
         """We should retrieve Ataxia (HP:0001251)"""
-        neuroMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d={})
+        neuroMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d={})
         results = neuroMapper.map_cell("ataxia")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0001251", result.id)
         self.assertEqual("Ataxia", result.label)
 
     def test_hpo_cr_spastic_paraplegia(self):
         """We should retrieve Spastic paraplegia (HP:0001258)"""
-        neuroMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d={})
+        neuroMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d={})
         results = neuroMapper.map_cell("spastic paraplegia")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0001258", result.id)
         self.assertEqual("Spastic paraplegia", result.label)
 
     def test_hpo_cr_multiple_concepts_with_custom_map(self):
         text = 'spasticity; nerve conduction and EMG studies with abnormal findings "remarkable for the failure to activate the leg muscles due to an upper motor neuron pattern of aberrant motor unit potential firing rates. These findings are consistent with dysfunction of the corticospinal pathways rather than a lower motor unit."'
-        neuroMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d={})
+        neuroMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d={})
         results = neuroMapper.map_cell(text)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("HP:0001257", result.id)
         self.assertEqual("Spasticity", result.label)
 
     def test_hpo_cr_multiple_concepts_no_custom_map(self):
         text = 'spasticity; nerve conduction and EMG studies with abnormal findings "remarkable for the failure to activate the leg muscles due to an upper motor neuron pattern of aberrant motor unit potential firing rates. These findings are consistent with dysfunction of the corticospinal pathways rather than a lower motor unit." Significant low extremity weakness.'
         neuro_exam_custom_map = {'low extremity weakness': 'Lower limb muscle weakness',
                                 'unstable gait': 'Unsteady gait',
                                 'dysfunction of the corticospinal pathways': 'Upper motor neuron dysfunction',
                                 }
-        neuroMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=neuro_exam_custom_map)
+        neuroMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=neuro_exam_custom_map)
         results = neuroMapper.map_cell(text)
         self.assertEqual(3, len(results))
         term_d = dict([(hpo_term.id, hpo_term.label) for hpo_term in results])
         self.assertTrue("HP:0001257" in term_d)
         self.assertEqual("Spasticity", term_d.get("HP:0001257"))
         self.assertTrue("HP:0007340" in term_d)
         self.assertEqual("Lower limb muscle weakness", term_d.get("HP:0007340"))
@@ -113,37 +111,34 @@
     def test_SETD2(self):
         text = """Extra fluid in the back of the cerebellum at 35 weeks; fetal MRI at 35 weeks showed VSD,
         small cerebellum, and agenesis of the corpus callosum; pre-eclampsia; \nIUGR 	n/a """
         prenatal_custom_map = {'agenesis of the corpus callosum': 'Agenesis of corpus callosum',
                             '\nIUGR': 'Intrauterine growth retardation',
                             'small cerebellum': 'Cerebellar hypoplasia',
                             }
-        prenatalMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=prenatal_custom_map)
+        prenatalMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=prenatal_custom_map)
         results = prenatalMapper.map_cell(text)
         self.assertEqual(3, len(results))
 
     def test_get_maximal_match(self):
         text = "severe global developmental delay"
         dev_custom_map = {'Severe global developmental delay': 'Severe global developmental delay'}
-        devMapper = OptionColumnMapper(column_name="placeholder", concept_recognizer=self.hpo_cr, option_d=dev_custom_map)
+        devMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=dev_custom_map)
         results = devMapper.map_cell(text)
         self.assertEqual(1, len(results))
         res = results[0]
         self.assertEqual(res.label, "Severe global developmental delay")
 
 
     def test_list(self):
         agressivenes_d = {'yes': 'Aggressive behavior',
                         'auto and heteroagressivity': ['Self-injurious behavior', 'Aggressive behavior']
                         }
         excluded_D = {"no":'Aggressive behavior' }
-        mapper = OptionColumnMapper(column_name="placeholder",
-                                    concept_recognizer=self.hpo_cr,
-                                    option_d=agressivenes_d,
-                                    excluded_d=excluded_D)
+        mapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=agressivenes_d, excluded_d=excluded_D)
         results = mapper.map_cell("yes")
         self.assertEqual(1, len(results))
         res = results[0]
         self.assertEqual(res.label, "Aggressive behavior")
         self.assertEqual(res.id, "HP:0000718")
         results = mapper.map_cell("auto and heteroagressivity")
         self.assertEqual(2, len(results))
@@ -158,31 +153,29 @@
         """
         The text "muscular hypotonia in the first years" was being recorded as both observed and excluded "Hypotonia"
         """
         hypotonia_d = {'yes hyper elastic': 'Hypotonia',
                         'yes': 'Hypotonia',
                         'axial tone more affected than  appendicular': 'Axial hypotonia',
                         'muscular hypotonia in the first years': 'Hypotonia'}
-        hypotoniaMapper = OptionColumnMapper(column_name="placeholder",
-                                            concept_recognizer=self.hpo_cr, option_d=hypotonia_d,
-                                            excluded_d={'no': 'Hypotonia'})
+        hypotoniaMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=hypotonia_d,
+                                    excluded_d={'no': 'Hypotonia'})
         results = hypotoniaMapper.map_cell("muscular hypotonia in the first years")
         self.assertEqual(1, len(results))
 
     def test_obs_excluded_ventriculomegaly(self):
         """
         The text "no ventriculomegaly" was being recorded as both observed and excluded "Ventriculomegaly"
         """
         ventricles_d = {
             'moderate enlargement of the lateral ventricles': 'Lateral ventricle dilatation',
             'left greater than right': 'Lateral ventricle dilatation',
         }
-        ventriclesMapper = OptionColumnMapper(column_name="placeholder",
-                                            concept_recognizer=self.hpo_cr, option_d=ventricles_d,
-                                            excluded_d={"normal": "Ventriculomegaly", 'no ventriculomegaly': 'Ventriculomegaly'})
+        ventriclesMapper = OptionColumnMapper(concept_recognizer=self.hpo_cr, option_d=ventricles_d,
+                                    excluded_d={"normal": "Ventriculomegaly", 'no ventriculomegaly': 'Ventriculomegaly'})
         results = ventriclesMapper.map_cell("no ventriculomegaly")
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("Ventriculomegaly", result.label)
         self.assertEqual("HP:0002119", result.id)
         self.assertFalse(result.observed)
```

### Comparing `pyphetools-0.9.83/test/test_phenopacket_table.py` & `pyphetools-0.9.9/test/test_phenopacket_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 import os
-from pyphetools.visualization import PhenopacketTable
+from src.pyphetools.visualization import PhenopacketTable
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 
 class TestPhenopacketTable(unittest.TestCase):
 
     def test_age_1(self):
```

### Comparing `pyphetools-0.9.83/test/test_simple_variant.py` & `pyphetools-0.9.9/test/test_simple_variant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import os
 import phenopackets as PPkt
-from pyphetools.visualization import SimpleVariant
-from pyphetools.creation import StructuralVariant
+from src.pyphetools.visualization import SimpleVariant
+from src.pyphetools.creation import StructuralVariant
 
 HP_JSON_FILENAME = os.path.join(os.path.dirname(__file__), 'data', 'hp.json')
 
 class TestHpoParser(unittest.TestCase):
 
 
     def test_structural_variant_display(self):
```

### Comparing `pyphetools-0.9.83/test/test_structural_variant.py` & `pyphetools-0.9.9/test/test_structural_variant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from pyphetools.creation import StructuralVariant
+from src.pyphetools.creation import StructuralVariant
 
 
 class TestVariantValidator(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls) -> None:
         variant = "46,XY.ish del(7)(p14.1)(RP11-816F16-)"
```

### Comparing `pyphetools-0.9.83/test/test_validation_result.py` & `pyphetools-0.9.9/test/test_validation_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
-from pyphetools.creation import HpTerm, AllelicRequirement
-from pyphetools.validation import ValidationResultBuilder
+from src.pyphetools.creation import HpTerm, AllelicRequirement
+from src.pyphetools.validation import ValidationResultBuilder
 
 
 
 class TestValidationResult(unittest.TestCase):
 
     def test_redundant(self):
         """
@@ -56,14 +56,8 @@
 
     def test_conflict_is_not_unfixable(self):
         vresult = ValidationResultBuilder("id3").conflict(conflicting_term=HpTerm(hpo_id="HP:0012345", label="Something"),term=HpTerm(hpo_id="HP:0072345", label="Something else")).build()
         self.assertEqual("ERROR", vresult.error_level)
         self.assertEqual("CONFLICT", vresult.category)
         self.assertFalse(vresult.is_unfixable_error())
 
-    def test_insufficient_disease(self):
-        vresult = ValidationResultBuilder("id3").insufficient_disease_count(observed_count=7, minimum_count=42).build()
-        self.assertEqual("ERROR", vresult.error_level)
-        self.assertEqual("INSUFFICIENT_DISEASE_COUNT", vresult.category)
-        self.assertFalse(vresult.is_unfixable_error())
-
```

### Comparing `pyphetools-0.9.83/test/test_variant.py` & `pyphetools-0.9.9/test/test_variant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from pyphetools.creation import HgvsVariant
+from src.pyphetools.creation import HgvsVariant
 
 # The following dictionary has the same structure as a subelement of the response from Variant Validator
 VCF_DICTIONARY =  {'alt': 'C', 'chr': '16', 'pos': '1756403', 'ref': 'CG'}
 GENOME_ASSEMBLY = 'hg38'
 transcript = 'NM_015133.4'
 symbol = 'MAPK8IP3'
 hgvs = 'NM_015133.4:c.111C>G'
```

