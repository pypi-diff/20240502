# Comparing `tmp/macrosynergy-0.1.8.tar.gz` & `tmp/macrosynergy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrosynergy-0.1.8.tar", last modified: Thu Feb 29 16:54:23 2024, max compression
+gzip compressed data, was "macrosynergy-0.1.9.tar", last modified: Thu Mar  7 18:44:08 2024, max compression
```

## Comparing `macrosynergy-0.1.8.tar` & `macrosynergy-0.1.9.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.434896 macrosynergy-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21206 2024-02-29 16:54:23.434896 macrosynergy-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.418896 macrosynergy-0.1.8/macrosynergy/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.418896 macrosynergy-0.1.8/macrosynergy/download/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42056 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/download/dataquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/download/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    36636 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/download/jpmaqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.418896 macrosynergy-0.1.8/macrosynergy/learning/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/cv_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    30290 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/panel_time_series_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    31343 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/predictors.py
--rw-r--r--   0 runner    (1001) docker     (127)    37965 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/signal_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28279 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/learning/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.422896 macrosynergy-0.1.8/macrosynergy/management/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.422896 macrosynergy-0.1.8/macrosynergy/management/simulate/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/simulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/simulate/simulate_quantamental_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/simulate/simulate_vintage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.422896 macrosynergy-0.1.8/macrosynergy/management/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/utils/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    32736 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/utils/df_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/management/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.426896 macrosynergy-0.1.8/macrosynergy/panel/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35382 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/basket.py
--rw-r--r--   0 runner    (1001) docker     (127)    35417 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/category_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/converge_row.py
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/granger_causality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/historic_vol.py
--rw-r--r--   0 runner    (1001) docker     (127)    19406 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/linear_composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/make_blacklist.py
--rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/make_relative_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/make_zn_scores.py
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/panel_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17942 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/return_beta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/view_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/view_grades.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/view_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/view_ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/panel/view_timelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.426896 macrosynergy-0.1.8/macrosynergy/pnl/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/pnl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47372 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/pnl/naive_pnl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.426896 macrosynergy-0.1.8/macrosynergy/signal/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58833 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/signal/signal_return_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    24469 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/signal/target_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-29 16:54:23.000000 macrosynergy-0.1.8/macrosynergy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.426896 macrosynergy-0.1.8/macrosynergy/visuals/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)    30367 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/facetplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/multiple_reg_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/ranges.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    13996 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/timelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/macrosynergy/visuals/view_panel_dates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:54:23.426896 macrosynergy-0.1.8/macrosynergy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21206 2024-02-29 16:54:23.000000 macrosynergy-0.1.8/macrosynergy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-02-29 16:54:23.000000 macrosynergy-0.1.8/macrosynergy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 16:54:23.000000 macrosynergy-0.1.8/macrosynergy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-29 16:54:23.000000 macrosynergy-0.1.8/macrosynergy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-29 16:54:23.000000 macrosynergy-0.1.8/macrosynergy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 16:54:23.434896 macrosynergy-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-02-29 16:47:14.000000 macrosynergy-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.186215 macrosynergy-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21206 2024-03-07 18:44:08.186215 macrosynergy-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.170215 macrosynergy-0.1.9/macrosynergy/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.170215 macrosynergy-0.1.9/macrosynergy/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42140 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/download/dataquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/download/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36636 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/download/jpmaqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.174215 macrosynergy-0.1.9/macrosynergy/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/cv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30290 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/panel_time_series_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31811 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67800 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/signal_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32233 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/learning/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.174215 macrosynergy-0.1.9/macrosynergy/management/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11885 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.174215 macrosynergy-0.1.9/macrosynergy/management/simulate/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/simulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16138 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/simulate/simulate_quantamental_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/simulate/simulate_vintage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.174215 macrosynergy-0.1.9/macrosynergy/management/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/utils/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33462 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/utils/df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/management/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.178215 macrosynergy-0.1.9/macrosynergy/panel/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35382 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35417 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/category_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/converge_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/granger_causality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/historic_vol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19406 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/linear_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/make_blacklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11679 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/make_relative_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15529 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/make_zn_scores.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/panel_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17942 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/return_beta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/view_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/view_grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/view_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/view_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/panel/view_timelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.178215 macrosynergy-0.1.9/macrosynergy/pnl/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/pnl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47372 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/pnl/naive_pnl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.178215 macrosynergy-0.1.9/macrosynergy/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58833 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/signal/signal_return_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24469 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/signal/target_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-07 18:44:08.000000 macrosynergy-0.1.9/macrosynergy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.182215 macrosynergy-0.1.9/macrosynergy/visuals/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17590 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30367 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/facetplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8649 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/multiple_reg_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8707 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/timelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/macrosynergy/visuals/view_panel_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 18:44:08.182215 macrosynergy-0.1.9/macrosynergy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21206 2024-03-07 18:44:08.000000 macrosynergy-0.1.9/macrosynergy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-03-07 18:44:08.000000 macrosynergy-0.1.9/macrosynergy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 18:44:08.000000 macrosynergy-0.1.9/macrosynergy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-07 18:44:08.000000 macrosynergy-0.1.9/macrosynergy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-07 18:44:08.000000 macrosynergy-0.1.9/macrosynergy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 18:44:08.186215 macrosynergy-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-03-07 18:33:28.000000 macrosynergy-0.1.9/setup.py
```

### Comparing `macrosynergy-0.1.8/LICENSE` & `macrosynergy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/PKG-INFO` & `macrosynergy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrosynergy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Macrosynergy Quant Research Package
 Author-email: Macrosynergy <info@macrosynergy.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Macrosynergy
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `macrosynergy-0.1.8/README.md` & `macrosynergy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/__init__.py` & `macrosynergy-0.1.9/macrosynergy/__init__.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/download/dataquery.py` & `macrosynergy-0.1.9/macrosynergy/download/dataquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 OAUTH_BASE_URL: str = (
     "https://api-developer.jpmorgan.com/research/dataquery-authe/api/v2"
 )
 OAUTH_TOKEN_URL: str = "https://authe.jpmchase.com/as/token.oauth2"
 OAUTH_DQ_RESOURCE_ID: str = "JPMC:URI:RS-06785-DataQueryExternalApi-PROD"
 JPMAQS_GROUP_ID: str = "JPMAQS"
 API_DELAY_PARAM: float = 0.2  # 300ms delay between requests
+TOKEN_EXPIRY_BUFFER: float = 0.9  # 90% of token expiry time.
 API_RETRY_COUNT: int = 5  # retry count for transient errors
 HL_RETRY_COUNT: int = 5  # retry count for "high-level" requests
 MAX_CONTINUOUS_FAILURES: int = 5  # max number of continuous errors before stopping
 HEARTBEAT_ENDPOINT: str = "/services/heartbeat"
 TIMESERIES_ENDPOINT: str = "/expressions/time-series"
 CATALOGUE_ENDPOINT: str = "/group/instruments"
 HEARTBEAT_TRACKING_ID: str = "heartbeat"
@@ -306,15 +307,15 @@
         """
         if self._stored_token is None:
             logger.debug("No token stored")
             return False
 
         created: datetime = self._stored_token["created_at"]  # utc time of creation
         expires: datetime = created + timedelta(
-            seconds=self._stored_token["expires_in"]
+            seconds=self._stored_token["expires_in"] * TOKEN_EXPIRY_BUFFER
         )
 
         utcnow = datetime.now(timezone.utc)
         is_active: bool = expires > utcnow
 
         logger.debug(
             "Active token: %s, created: %s, expires: %s, now: %s",
```

### Comparing `macrosynergy-0.1.8/macrosynergy/download/exceptions.py` & `macrosynergy-0.1.9/macrosynergy/download/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/download/jpmaqs.py` & `macrosynergy-0.1.9/macrosynergy/download/jpmaqs.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/learning/__init__.py` & `macrosynergy-0.1.9/macrosynergy/learning/__init__.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/learning/cv_tools.py` & `macrosynergy-0.1.9/macrosynergy/learning/cv_tools.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/learning/metrics.py` & `macrosynergy-0.1.9/macrosynergy/learning/metrics.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/learning/panel_time_series_split.py` & `macrosynergy-0.1.9/macrosynergy/learning/panel_time_series_split.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/learning/predictors.py` & `macrosynergy-0.1.9/macrosynergy/learning/predictors.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,19 @@
                 "The indices of the input dataframe X and the output dataframe y don't "
                 "match."
             )
 
         # Fit
         self.sample_weights = self._calculate_sample_weights(y)
         self.model.fit(X, y, sample_weight=self.sample_weights)
+        if hasattr(self.model, "coef_"):
+            self.coef_ = self.model.coef_
+        if hasattr(self.model, "intercept_"):
+            self.intercept_ = self.model.intercept_
+
         return self
 
     def predict(self, X: pd.DataFrame):
         """
         Predict method to make model predictions on the input feature matrix X based on
         the previously fit model.
 
@@ -235,14 +240,16 @@
         self.positive = positive
         model = LinearRegression(
             fit_intercept=self.fit_intercept,
             copy_X=self.copy_X,
             n_jobs=self.n_jobs,
             positive=self.positive,
         )
+        self.coef_ = None 
+        self.intercept_ = None
         super().__init__(model)
 
     def set_params(self, **params):
         super().set_params(**params)
         if 'fit_intercept' in params or 'positive' in params:
             # Re-initialize the LinearRegression instance with updated parameters
             self.model = LinearRegression(
@@ -289,14 +296,16 @@
         self.positive = positive
         model = LinearRegression(
             fit_intercept=self.fit_intercept,
             copy_X=self.copy_X,
             n_jobs=self.n_jobs,
             positive=self.positive,
         )
+        self.coef_ = None
+        self.intercept_ = None
         super().__init__(half_life=half_life, model=model)
 
     def set_params(self, **params):
         super().set_params(**params)
         if 'fit_intercept' in params or 'positive' in params:
             # Re-initialize the LinearRegression instance with updated parameters
             self.model = LinearRegression(
@@ -334,14 +343,16 @@
 
         self.fit_intercept = fit_intercept
         self.positive = positive
         model = LADRegressor(
             fit_intercept=self.fit_intercept,
             positive=self.positive,
         )
+        self.coef_ = None
+        self.intercept_ = None
         super().__init__(model)
 
     def set_params(self, **params):
         super().set_params(**params)
         if 'fit_intercept' in params or 'positive' in params:
             # Re-initialize the LinearRegression instance with updated parameters
             self.model = LADRegressor(
@@ -374,14 +385,16 @@
 
         self.fit_intercept = fit_intercept
         self.positive = positive
         model = LADRegressor(
             fit_intercept=self.fit_intercept,
             positive=self.positive,
         )
+        self.coef_ = None
+        self.intercept_ = None
         super().__init__(half_life=half_life, model=model)
 
     def set_params(self, **params):
         super().set_params(**params)
         if 'fit_intercept' in params or 'positive' in params:
             # Re-initialize the LinearRegression instance with updated parameters
             self.model = LADRegressor(
@@ -420,14 +433,16 @@
         if tol is not None and tol <= 0:
             raise ValueError("'tol' must be a positive number.")
 
         # Initialise
         self.fit_intercept = fit_intercept
         self.positive = positive
         self.tol = tol
+        self.coef_ = None
+        self.intercept_ = None
 
     def fit(
         self,
         X: pd.DataFrame,
         y: Union[pd.DataFrame, pd.Series],
         sample_weight: np.ndarray = None,
     ):
```

### Comparing `macrosynergy-0.1.8/macrosynergy/learning/transformers.py` & `macrosynergy-0.1.9/macrosynergy/learning/transformers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 import numpy as np
 import pandas as pd
 
 import datetime
 
 from sklearn.linear_model import Lasso
 from sklearn.base import BaseEstimator, TransformerMixin, OneToOneFeatureMixin
+from sklearn.feature_selection import SelectorMixin
+
+from sklearn.exceptions import NotFittedError
 
 from statsmodels.tools.tools import add_constant
 from statsmodels.regression.mixed_linear_model import MixedLM
 
 from typing import Union, Any, List, Optional
 
-import logging
+import warnings
 
 
-class LassoSelector(BaseEstimator, TransformerMixin):
+class LassoSelector(BaseEstimator, SelectorMixin):
     def __init__(self, alpha: Union[float, int], positive: bool = True):
         """
         Transformer class to use the Lasso as a feature selection algorithm.
         Given a hyper-parameter, alpha, the Lasso model is fit and
         the non-zero coefficients are used to extract features from an input dataframe.
         The underlying features as input to the Lasso model are expected to be positively
         correlated with the target variable.
@@ -38,14 +41,15 @@
         if alpha < 0:
             raise ValueError("The 'alpha' hyper-parameter must be non-negative.")
         if not isinstance(positive, bool):
             raise TypeError("The 'positive' hyper-parameter must be a boolean.")
 
         self.alpha = alpha
         self.positive = positive
+        self.feature_names_in_ = None
 
     def fit(self, X: pd.DataFrame, y: Union[pd.Series, pd.DataFrame]):
         """
         Fit method to fit a Lasso regression and obtain the selected features.
 
         :param <pd.DataFrame> X: Pandas dataframe of input features.
         :param <Union[pd.Series,pd.DataFrame]> y: Pandas series or dataframe of targets
@@ -82,24 +86,66 @@
 
         if not X.index.equals(y.index):
             raise ValueError(
                 "The indices of the input dataframe X and the output dataframe y "
                 "don't match as input to the LASSO selector."
             )
 
-        self.p = X.shape[-1]
+        self.feature_names_in_ = np.array(X.columns)
+        self.p = X.shape[1]
 
         if self.positive:
             self.lasso = Lasso(alpha=self.alpha, positive=True).fit(X, y)
         else:
             self.lasso = Lasso(alpha=self.alpha).fit(X, y)
 
         self.selected_ftr_idxs = [i for i in range(self.p) if self.lasso.coef_[i] != 0]
 
         return self
+    
+    def _get_support_mask(self):
+        """
+        Private method to return a boolean mask of the features selected for the Pandas dataframe.
+        """
+        mask = np.zeros(self.p, dtype=bool)
+        mask[self.selected_ftr_idxs] = True
+        return mask
+    
+    def get_support(self, indices=False):
+        """
+        Method to return a mask, or integer index, of the features selected for the Pandas dataframe.
+        
+        :param <bool> indices: Boolean to specify whether to return the column indices of the selected features instead of a boolean mask
+        
+        :return <np.ndarray>: Boolean mask or integer index of the selected features
+        """
+        if self.feature_names_in_ is None:
+            raise NotFittedError(
+                "The LASSO selector has not been fitted. Please fit the selector before calling get_support()."
+            )
+        if not isinstance(indices, (bool, np.bool_)):
+            raise ValueError(
+                "The 'indices' parameter must be a boolean."
+            )
+        if indices:
+            return self.selected_ftr_idxs
+        else:
+            mask = self._get_support_mask()
+            return mask
+        
+    def get_feature_names_out(self):
+        """
+        Method to mask feature names according to selected features.
+        """
+        if self.feature_names_in_ is None:
+            raise NotFittedError(
+                "The LASSO selector has not been fitted. Please fit the selector before calling get_feature_names_out()."
+            )
+        
+        return self.feature_names_in_[self.get_support(indices=False)]
 
     def transform(self, X: pd.DataFrame):
         """
         Transform method to return only the selected features of the dataframe.
 
         :param <pd.DataFrame> X: Pandas dataframe of input features.
 
@@ -121,43 +167,49 @@
             raise ValueError(
                 "The number of columns of the dataframe to be transformed, X, doesn't "
                 "match the number of columns of the training dataframe."
             )
         if len(self.selected_ftr_idxs) == 0:
             # Then no features were selected
             # Then at the given time, no trading decisions can be made based on these features
-            # Hence, we return a dataframe of zeros
-            return pd.DataFrame(
-                index=X.index, columns=["no_signal"], data=0, dtype=np.float16
+            warnings.warn(
+                "No features were selected. At the given time, no trading decisions can be made based on these features.",
+                UserWarning,
             )
+            return X.iloc[:, :0]
 
         return X.iloc[:, self.selected_ftr_idxs]
 
 
-class MapSelector(BaseEstimator, TransformerMixin):
-    def __init__(self, threshold: float):
+class MapSelector(BaseEstimator, SelectorMixin):
+    def __init__(self, threshold: float, positive: bool = False):
         """
-        Transformer class to select features from a training set
+        Selector class to select features from a training set
         based on the Macrosynergy panel test. This test involves creating
         a linear mixed effects model with period-specific random effects to
         account for cross-sectional correlations. The p-value for the slope
         parameter is used to perform the significance test.
 
         :param <float> threshold: Significance threshold. This should be in
             the interval (0,1).
+        :param <bool> positive: Boolean indicating whether or not to only keep features
+            with positive estimated model coefficients.
         """
         if type(threshold) != float:
             raise TypeError("The threshold must be a float.")
-
         if (threshold <= 0) or (threshold > 1):
             raise ValueError(
                 "The threshold must be in between 0 (inclusive) and 1 (exclusive)."
             )
+        if not isinstance(positive, (bool, np.bool_)):
+            raise TypeError("The 'positive' parameter must be a boolean.")
 
         self.threshold = threshold
+        self.positive = positive
+        self.feature_names_in_ = None
 
     def fit(self, X: pd.DataFrame, y: Union[pd.Series, pd.DataFrame]):
         """
         Fit method to assess significance of each feature using
         the Macrosynergy panel test.
 
         :param <pd.DataFrame> X: Pandas dataframe of input features.
@@ -195,27 +247,70 @@
         if not X.index.equals(y.index):
             raise ValueError(
                 "The indices of the input dataframe X and the output dataframe y don't "
                 "match."
             )
 
         self.ftrs = []
-        self.cols = X.columns
+        self.feature_names_in_ = np.array(X.columns)
 
-        for col in self.cols:
+        for col in self.feature_names_in_:
             ftr = X[col]
             ftr = add_constant(ftr)
             groups = ftr.index.get_level_values(1)
             model = MixedLM(y.values, ftr, groups).fit(reml=False)
             est = model.params.iloc[1]
             pval = model.pvalues.iloc[1]
-            if (pval < self.threshold) & (est > 0):
-                self.ftrs.append(col)
+            if (pval < self.threshold):
+                if self.positive:
+                    if est > 0:
+                        self.ftrs.append(col)
+                else:
+                    self.ftrs.append(col)
 
         return self
+    
+    def _get_support_mask(self):
+        """
+        Private method to return a boolean mask of the features selected for the Pandas dataframe.
+        """
+        mask = [col in self.ftrs for col in self.feature_names_in_]
+        return np.array(mask)
+    
+    def get_support(self, indices=False):
+        """
+        Method to return a mask, or integer index, of the features selected for the Pandas dataframe.
+        
+        :param <bool> indices: Boolean to specify whether to return the column indices of the selected features instead of a boolean mask
+        
+        :return <np.ndarray>: Boolean mask or integer index of the selected features
+        """
+        if not isinstance(indices, (bool, np.bool_)):
+            raise TypeError(
+                "The 'indices' parameter must be a boolean."
+            )
+        if self.feature_names_in_ is None:
+            raise NotFittedError(
+                "The MAP selector has not been fitted. Please fit the selector before calling get_support()."
+            )
+        mask = self._get_support_mask()
+
+        if indices:
+            return np.where(mask)[0]
+        
+        return mask
+        
+    def get_feature_names_out(self):
+        """
+        Method to mask feature names according to selected features.
+        """
+        if self.feature_names_in_ is None:
+            raise ValueError("The feature names are not available. Please fit the transformer first.")
+        
+        return self.feature_names_in_[self.get_support(indices=False)]
 
     def transform(self, X: pd.DataFrame):
         """
         Transform method to return the significant training features.
 
         :param <pd.DataFrame> X: Pandas dataframe of input features.
 
@@ -229,27 +324,27 @@
                 "If used as part of an sklearn pipeline, ensure that previous steps "
                 "return a pandas dataframe."
             )
         if not isinstance(X.index, pd.MultiIndex):
             raise ValueError("X must be multi-indexed.")
         if not isinstance(X.index.get_level_values(1)[0], datetime.date):
             raise TypeError("The inner index of X must be datetime.date.")
-        if not X.columns.equals(self.cols):
+        if not np.all(np.array(X.columns) == self.feature_names_in_):
             raise ValueError(
                 "The columns of the dataframe to be transformed, X, don't match the "
                 "columns of the training dataframe."
             )
         # transform
         if self.ftrs == []:
             # Then no features were selected
             # Then at the given time, no trading decisions can be made based on these features
-            # Hence, we return a dataframe of zeros
-            return pd.DataFrame(
-                index=X.index, columns=["no_signal"], data=0, dtype=np.float16
+            warnings.warn(
+                "No features were selected. At the given time, no trading decisions can be made based on these features."
             )
+            return X.iloc[:, :0]
 
         return X[self.ftrs]
 
 
 class FeatureAverager(BaseEstimator, TransformerMixin):
     def __init__(self, use_signs: Optional[bool] = False):
         """
@@ -655,22 +750,25 @@
     black = {"GBP": ["2009-01-01", "2012-06-30"], "CAD": ["2018-01-01", "2100-01-01"]}
     dfd2 = msm.reduce_df(df=dfd2, cids=cids, xcats=xcats, blacklist=black)
 
     dfd2 = dfd2.pivot(index=["cid", "real_date"], columns="xcat", values="value")
     X = dfd2.drop(columns=["XR"])
     y = dfd2["XR"]
 
-    selector = MapSelector(0.05)
+
+    selector = LassoSelector(0.2)
     selector.fit(X, y)
     print(selector.transform(X).columns)
-
-    selector = LassoSelector(10000)
+    
+    selector = MapSelector(1e-20)
     selector.fit(X, y)
     print(selector.transform(X).columns)
 
+
+
     # Split X and y into training and test sets
     X_train, X_test = (
         X[X.index.get_level_values(1) < pd.Timestamp(day=1, month=1, year=2018)],
         X[X.index.get_level_values(1) >= pd.Timestamp(day=1, month=1, year=2018)],
     )
     y_train, y_test = (
         y[y.index.get_level_values(1) < pd.Timestamp(day=1, month=1, year=2018)],
```

### Comparing `macrosynergy-0.1.8/macrosynergy/management/__init__.py` & `macrosynergy-0.1.9/macrosynergy/management/__init__.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/decorators.py` & `macrosynergy-0.1.9/macrosynergy/management/decorators.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/simulate/simulate_quantamental_data.py` & `macrosynergy-0.1.9/macrosynergy/management/simulate/simulate_quantamental_data.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/simulate/simulate_vintage_data.py` & `macrosynergy-0.1.9/macrosynergy/management/simulate/simulate_vintage_data.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/types.py` & `macrosynergy-0.1.9/macrosynergy/management/types.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/utils/__init__.py` & `macrosynergy-0.1.9/macrosynergy/management/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/utils/check_availability.py` & `macrosynergy-0.1.9/macrosynergy/management/utils/check_availability.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/utils/core.py` & `macrosynergy-0.1.9/macrosynergy/management/utils/core.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/utils/df_utils.py` & `macrosynergy-0.1.9/macrosynergy/management/utils/df_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import warnings
 from typing import Any, Dict, Iterable, List, Optional, Set, Union, overload
 
 import numpy as np
 import pandas as pd
 import requests
 import requests.compat
-from .core import get_cid, get_xcat, _map_to_business_day_frequency
+from .core import get_cid, get_xcat, _map_to_business_day_frequency, is_valid_iso_date
+
 
 def standardise_dataframe(
     df: pd.DataFrame, verbose: bool = False
 ) -> QuantamentalDataFrame:
     """
     Applies the standard JPMaQS Quantamental DataFrame format to a DataFrame.
 
@@ -345,14 +346,15 @@
         df = update_tickers(df, df_add)
 
     else:
         df = update_categories(df, df_add)
 
     return df.reset_index(drop=True)
 
+
 def update_tickers(df: pd.DataFrame, df_add: pd.DataFrame):
     """
     Method used to update aggregate DataFrame on a ticker level.
 
     :param <pd.DataFrame> df: aggregate DataFrame used to store all tickers.
     :param <pd.DataFrame> df_add: DataFrame with the latest values.
 
@@ -844,40 +846,57 @@
         )
 
     if bool(start_date) and bool(dates):
         raise ValueError(
             "Only one of `dates` or `start_date` and `end_date` must be passed."
         )
 
-    dts: pd.DataFrame = (
-        pd.DataFrame(dates, columns=["real_date"]).apply(pd.to_datetime, axis=1)
-        if dates is not None
-        else pd.Series(pd.bdate_range(start_date, end_date))
-    )
-    if dates is not None:
-        dts = dts[
-            dts["real_date"].isin(
-                pd.bdate_range(start=dts["real_date"].min(), end=dts["real_date"].max())
-            )
-        ]
+    if bool(start_date):
+        assert bool(end_date)
+        for date, dname in zip([start_date, end_date], ["start_date", "end_date"]):
+            if not isinstance(date, (str, pd.Timestamp)):
+                raise TypeError(f"{dname} must be a string or a pandas Timestamp.")
+            if isinstance(date, str):
+                if not is_valid_iso_date(date):
+                    raise ValueError(
+                        "Both `start_date` and `end_date` must be valid ISO dates when passed as "
+                        "strings."
+                    )
+
+        if pd.Timestamp(start_date) > pd.Timestamp(end_date):
+            start_date, end_date = end_date, start_date
+
+    dts: pd.DataFrame = pd.DataFrame(
+        (
+            dates
+            if (dates is not None)
+            else pd.bdate_range(start=start_date, end=end_date)
+        ),
+        columns=["real_date"],
+    ).apply(pd.to_datetime, axis=1)
 
     min_date: pd.Timestamp = dts["real_date"].min()
 
+    if freq == "D":
+        max_date = dts["real_date"].max()
+        dtx = pd.bdate_range(start=min_date, end=max_date)
+        return dtx[dtx.isin(dts["real_date"])]
+
     if freq == "M":
         func = months_btwn_dates
     elif freq == "W":
         func = weeks_btwn_dates
     elif freq == "Q":
         func = quarters_btwn_dates
     elif freq == "A":
         func = years_btwn_dates
-    elif freq == "D":
-        func = lambda x, y: len(pd.bdate_range(x, y)) - 1
+    # elif freq == "D":
+    #     func = lambda x, y: len(pd.bdate_range(x, y)) - 1
     else:
-        raise ValueError("Frequency parameter must be one of D, M, W, or Q")
+        raise ValueError("Frequency parameter must be one of D, M, W, Q, or A.")
 
     dts["period"] = dts["real_date"].apply(func, args=(min_date,))
 
     t_indices: pd.Series = dts["period"].shift(-1) != dts["period"]
 
     t_dates: pd.Series = dts["real_date"].loc[t_indices].reset_index(drop=True)
```

### Comparing `macrosynergy-0.1.8/macrosynergy/management/utils/math.py` & `macrosynergy-0.1.9/macrosynergy/management/utils/math.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/management/validation.py` & `macrosynergy-0.1.9/macrosynergy/management/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import warnings
+import datetime
 from typing import (
     Dict,
     List,
     NamedTuple,
     Optional,
+    Union,
 )
 import pandas as pd
 
 from macrosynergy.management.utils import reduce_df, is_valid_iso_date
 from macrosynergy.management.utils.df_utils import standardise_dataframe
 
 
@@ -241,7 +243,30 @@
             f"The following {col_name}(s), passed in `{param_name}`,"
             " are not in the DataFrame `df`: "
             f"{list(set(values) - set(df[col_name].unique()))}."
         )
         missing = list(set(values) - set(df[col_name].unique()))
 
     return missing
+
+def _validate_Xy_learning(X: pd.DataFrame, y: Union[pd.DataFrame, pd.Series]):
+    """
+    Validates the expected long-format inputs and targets expected for the learning
+    submodule.
+    """
+    if not isinstance(X, pd.DataFrame):
+        raise TypeError("The X argument must be a pandas DataFrame.")
+    if not isinstance(y, pd.Series) and not isinstance(y, pd.DataFrame):
+        raise TypeError("The y argument must be a pandas Series or DataFrame.")
+    if not isinstance(X.index, pd.MultiIndex):
+        raise ValueError("X must be multi-indexed.")
+    if not isinstance(y.index, pd.MultiIndex):
+        raise ValueError("y must be multi-indexed.")
+    if not isinstance(X.index.get_level_values(1)[0], datetime.date):
+        raise TypeError("The inner index of X must be datetime.date.")
+    if not isinstance(y.index.get_level_values(1)[0], datetime.date):
+        raise TypeError("The inner index of y must be datetime.date.")
+    if not X.index.equals(y.index):
+        raise ValueError(
+            "The indices of the input dataframe X and the output dataframe y don't "
+            "match."
+        )
```

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/__init__.py` & `macrosynergy-0.1.9/macrosynergy/panel/__init__.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/basket.py` & `macrosynergy-0.1.9/macrosynergy/panel/basket.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/category_relations.py` & `macrosynergy-0.1.9/macrosynergy/panel/category_relations.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/converge_row.py` & `macrosynergy-0.1.9/macrosynergy/panel/converge_row.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/granger_causality_test.py` & `macrosynergy-0.1.9/macrosynergy/panel/granger_causality_test.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/historic_vol.py` & `macrosynergy-0.1.9/macrosynergy/panel/historic_vol.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/linear_composite.py` & `macrosynergy-0.1.9/macrosynergy/panel/linear_composite.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/make_blacklist.py` & `macrosynergy-0.1.9/macrosynergy/panel/make_blacklist.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/make_relative_value.py` & `macrosynergy-0.1.9/macrosynergy/panel/make_relative_value.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/make_zn_scores.py` & `macrosynergy-0.1.9/macrosynergy/panel/make_zn_scores.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/panel_calculator.py` & `macrosynergy-0.1.9/macrosynergy/panel/panel_calculator.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/return_beta.py` & `macrosynergy-0.1.9/macrosynergy/panel/return_beta.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/view_correlations.py` & `macrosynergy-0.1.9/macrosynergy/panel/view_correlations.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/view_grades.py` & `macrosynergy-0.1.9/macrosynergy/panel/view_grades.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/view_metrics.py` & `macrosynergy-0.1.9/macrosynergy/panel/view_metrics.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/view_ranges.py` & `macrosynergy-0.1.9/macrosynergy/panel/view_ranges.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/panel/view_timelines.py` & `macrosynergy-0.1.9/macrosynergy/panel/view_timelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 def view_timelines(
     df: pd.DataFrame,
     xcats: Optional[List[str]] = None,
     cids: Optional[List[str]] = None,
     intersect: bool = False,
-    blacklist: Optional[dict] = None,
     val: str = "value",
     cumsum: bool = False,
     start: str = "2000-01-01",
     end: Optional[str] = None,
     ncol: int = 3,
     legend_ncol: int = 1,
     same_y: bool = True,
@@ -81,15 +80,14 @@
 
     """
     msv.timelines(
         df=df,
         xcats=xcats,
         cids=cids,
         intersect=intersect,
-        blacklist=blacklist,
         val=val,
         cumsum=cumsum,
         start=start,
         end=end,
         ncol=ncol,
         same_y=same_y,
         all_xticks=all_xticks,
```

### Comparing `macrosynergy-0.1.8/macrosynergy/pnl/naive_pnl.py` & `macrosynergy-0.1.9/macrosynergy/pnl/naive_pnl.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/signal/signal_return_relations.py` & `macrosynergy-0.1.9/macrosynergy/signal/signal_return_relations.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/signal/target_positions.py` & `macrosynergy-0.1.9/macrosynergy/signal/target_positions.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/__init__.py` & `macrosynergy-0.1.9/macrosynergy/visuals/__init__.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/correlation.py` & `macrosynergy-0.1.9/macrosynergy/visuals/correlation.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/facetplot.py` & `macrosynergy-0.1.9/macrosynergy/visuals/facetplot.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/grades.py` & `macrosynergy-0.1.9/macrosynergy/visuals/grades.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/heatmap.py` & `macrosynergy-0.1.9/macrosynergy/visuals/heatmap.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/lineplot.py` & `macrosynergy-0.1.9/macrosynergy/visuals/lineplot.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/metrics.py` & `macrosynergy-0.1.9/macrosynergy/visuals/metrics.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/multiple_reg_scatter.py` & `macrosynergy-0.1.9/macrosynergy/visuals/multiple_reg_scatter.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/plotter.py` & `macrosynergy-0.1.9/macrosynergy/visuals/plotter.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/ranges.py` & `macrosynergy-0.1.9/macrosynergy/visuals/ranges.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/table.py` & `macrosynergy-0.1.9/macrosynergy/visuals/table.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/timelines.py` & `macrosynergy-0.1.9/macrosynergy/visuals/timelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,19 @@
 from macrosynergy.management.utils import standardise_dataframe, reduce_df
 from macrosynergy.visuals import FacetPlot, LinePlot
 from macrosynergy.management.types import Numeric
 import time
 
 IDX_COLS: List[str] = ["cid", "xcat", "real_date"]
 
-
 def timelines(
     df: pd.DataFrame,
     xcats: Optional[List[str]] = None,
     cids: Optional[List[str]] = None,
     intersect: bool = False,
-    blacklist: Optional[dict] = None,
     val: str = "value",
     cumsum: bool = False,
     start: str = "2000-01-01",
     end: Optional[str] = None,
     ncol: int = 3,
     square_grid: bool = False,
     legend_ncol: int = 1,
@@ -97,18 +95,18 @@
     :param <Numeric> aspect: width-height ratio for plots in facet. Default is 1.7.
     :param <Numeric> height: height of plots in facet. Default is 3.
     :param <int> legend_fontsize: font size of legend. Default is 12.
 
     """
     if not isinstance(df, pd.DataFrame):
         raise TypeError("`df` must be a pandas DataFrame.")
-
+    
     if len(df.columns) < 4:
         df = df.copy().reset_index()
-
+    
     if val not in df.columns:
         if len(df.columns) == len(IDX_COLS) + 1:
             val: str = list(set(df.columns) - set(IDX_COLS))[0]
             if not pd.api.types.is_numeric_dtype(df[val]):
                 raise ValueError(
                     f"Column '{val}' (passed as `metric`) is not numeric, and there are "
                     f"no other numeric columns in the DataFrame."
@@ -147,38 +145,29 @@
         raise ValueError(
             "`xcat_grid` cannot be True when multiple cross-sections are selected."
         )
 
     if xcats is None:
         if xcat_labels:
             raise ValueError("`xcat_labels` requires `xcats` to be defined.")
-        xcats: List[str] = df["xcats"].unique().tolist()
+        xcats: List[str] = df["xcat"].unique().tolist()
 
     if cids is None:
         cids: List[str] = df["cid"].unique().tolist()
 
-    if not isinstance(blacklist, dict):
-        if blacklist is not None:
-            raise TypeError("`blacklist` must be a dictionary.")
-
     if cumsum:
-        df = reduce_df(
-            df, xcats=xcats, cids=cids, start=start, end=end, blacklist=blacklist
-        )
-        df[val] = (
-            df.sort_values(["cid", "xcat", "real_date"])[["cid", "xcat", val]]
+        df = reduce_df(df, xcats=xcats, cids=cids, start=start, end=end)
+        df[val] = (df.sort_values(["cid", "xcat", "real_date"])
+            [["cid", "xcat", val]]
             .groupby(["cid", "xcat"])
-            .cumsum()
-        )
+            .cumsum())
 
     cross_mean_series: Optional[str] = f"mean_{xcats[0]}" if cs_mean else None
     if cs_mean:
-        df = reduce_df(
-            df, xcats=xcats, cids=cids, start=start, end=end, blacklist=blacklist
-        )
+        df = reduce_df(df, xcats=xcats, cids=cids, start=start, end=end)
         if len(xcats) > 1:
             raise ValueError("`cs_mean` cannot be True for multiple categories.")
 
         if len(cids) == 1:
             raise ValueError("`cs_mean` cannot be True for a single cross section.")
 
         df_mean: pd.DataFrame = (
@@ -221,21 +210,20 @@
             ncol: int = len(xcats)
 
         with FacetPlot(
             df=df,
             xcats=xcats,
             cids=cids,
             intersect=intersect,
-            blacklist=blacklist,
             metrics=[val],
             tickers=[cross_mean_series] if cs_mean else None,
             start=start,
             end=end,
         ) as fp:
-
+            
             fp.lineplot(
                 share_y=same_y,
                 share_x=not all_xticks,
                 figsize=size,
                 xcat_grid=True,  # Not to be confused with `xcat_grid` parameter
                 # legend_labels=xcat_labels or None,
                 facet_titles=xcat_labels or None,
@@ -255,15 +243,14 @@
     elif single_chart or (len(cids) == 1):
         with LinePlot(
             df=df,
             cids=cids,
             xcats=xcats,
             intersect=intersect,
             metrics=[val],
-            blacklist=blacklist,
             tickers=[cross_mean_series] if cs_mean else None,
             start=start,
             end=end,
         ) as lp:
             lp.plot(
                 metric=val,
                 figsize=size,
@@ -281,15 +268,14 @@
     else:
         with FacetPlot(
             df=df,
             xcats=xcats,
             cids=cids,
             intersect=intersect,
             metrics=[val],
-            blacklist=blacklist,
             tickers=[cross_mean_series] if cs_mean else None,
             start=start,
             end=end,
         ) as fp:
             show_legend: bool = True if cross_mean_series else False
             show_legend = show_legend or (len(xcats) > 1)
             if ncol > len(cids):
```

### Comparing `macrosynergy-0.1.8/macrosynergy/visuals/view_panel_dates.py` & `macrosynergy-0.1.9/macrosynergy/visuals/view_panel_dates.py`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy.egg-info/PKG-INFO` & `macrosynergy-0.1.9/macrosynergy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrosynergy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Macrosynergy Quant Research Package
 Author-email: Macrosynergy <info@macrosynergy.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Macrosynergy
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `macrosynergy-0.1.8/macrosynergy.egg-info/SOURCES.txt` & `macrosynergy-0.1.9/macrosynergy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/macrosynergy.egg-info/requires.txt` & `macrosynergy-0.1.9/macrosynergy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/pyproject.toml` & `macrosynergy-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `macrosynergy-0.1.8/setup.py` & `macrosynergy-0.1.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 if sys.version_info[:2] < (3, 8):
     raise RuntimeError("Python version >= 3.8 required.")
 
 MAJOR = 0
 MINOR = 1
-MICRO = 8
+MICRO = 9
 ISRELEASED = True
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, MICRO)
 
 if sys.version_info >= (3, 12):
     # The first version not in the `Programming Language :: Python :: ...` classifiers above
     warnings.warn(
         f"Macrosynergy {VERSION} may not yet support Python "
```

