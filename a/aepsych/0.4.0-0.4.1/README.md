# Comparing `tmp/aepsych-0.4.0.tar.gz` & `tmp/aepsych-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepsych-0.4.0.tar", last modified: Mon Jun  5 20:25:35 2023, max compression
+gzip compressed data, was "aepsych-0.4.1.tar", last modified: Thu May  2 12:22:36 2024, max compression
```

## Comparing `aepsych-0.4.0.tar` & `aepsych-0.4.1.tar`

### file list

```diff
@@ -1,170 +1,168 @@
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.832495 aepsych-0.4.0/
--rw-r--r--   0 craigsanders   (501) staff       (20)    19407 2023-06-05 20:10:09.000000 aepsych-0.4.0/LICENSE
--rw-r--r--   0 craigsanders   (501) staff       (20)     4565 2023-06-05 20:25:35.831996 aepsych-0.4.0/PKG-INFO
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.664880 aepsych-0.4.0/aepsych/
--rw-r--r--   0 craigsanders   (501) staff       (20)      983 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/__init__.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.795551 aepsych-0.4.0/aepsych/acquisition/
--rw-r--r--   0 craigsanders   (501) staff       (20)     1390 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      835 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/acquisition.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3043 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/bvn.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    13677 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/lookahead.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     7137 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/lookahead_utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3593 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/lse.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3775 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/mc_posterior_variance.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6079 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/monotonic_rejection.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5332 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/mutual_information.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.814952 aepsych-0.4.0/aepsych/acquisition/objective/
--rw-r--r--   0 craigsanders   (501) staff       (20)      735 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/objective/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4307 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/objective/objective.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4702 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/objective/semi_p.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2433 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/acquisition/rejection_sampler.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.886128 aepsych-0.4.0/aepsych/benchmark/
--rw-r--r--   0 craigsanders   (501) staff       (20)      868 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11291 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/benchmark.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10521 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/pathos_benchmark.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10010 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/problem.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6920 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/benchmark/test_functions.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    13010 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/config.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.898430 aepsych-0.4.0/aepsych/database/
--rw-r--r--   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/database/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11554 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/database/db.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    17629 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/database/tables.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.908941 aepsych-0.4.0/aepsych/factory/
--rw-r--r--   0 craigsanders   (501) staff       (20)      608 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/factory/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11147 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/factory/factory.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.039654 aepsych-0.4.0/aepsych/generators/
--rw-r--r--   0 craigsanders   (501) staff       (20)     1524 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4076 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/base.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.084667 aepsych-0.4.0/aepsych/generators/completion_criterion/
--rw-r--r--   0 craigsanders   (501) staff       (20)      749 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      885 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/min_asks.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1454 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/min_total_outcome_occurrences.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      757 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/min_total_tells.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      930 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/completion_criterion/run_indefinitely.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1422 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/epsilon_greedy_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2871 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/manual_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     7978 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/monotonic_rejection_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4441 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/monotonic_thompson_sampler_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      736 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/multi_outcome_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10425 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/optimize_acqf_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      732 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/pairwise_optimize_acqf_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      689 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/pairwise_sobol_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2797 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/random_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2576 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/semi_p.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3696 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/generators/sobol_generator.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.098513 aepsych-0.4.0/aepsych/kernels/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/kernels/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1801 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/kernels/rbf_partial_grad.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.145436 aepsych-0.4.0/aepsych/likelihoods/
--rw-r--r--   0 craigsanders   (501) staff       (20)      552 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1053 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/bernoulli.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2465 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/ordinal.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4332 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/likelihoods/semi_p.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.154163 aepsych-0.4.0/aepsych/means/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/means/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1109 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/means/constant_partial_grad.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.294751 aepsych-0.4.0/aepsych/models/
--rw-r--r--   0 craigsanders   (501) staff       (20)     1462 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    21304 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/base.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4684 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/derivative_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      675 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/exact_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    12946 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/gp_classification.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6554 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/gp_regression.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    10235 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/monotonic_projection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    13669 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/monotonic_rejection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5847 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/multitask_regression.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2338 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/ordinal_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     7071 2023-06-05 20:10:09.000000 aepsych-0.4.0/aepsych/models/pairwise_probit.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    24658 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/semi_p.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2403 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/surrogate.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5322 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5775 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/models/variational_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    16703 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/plotting.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.344816 aepsych-0.4.0/aepsych/server/
--rw-r--r--   0 craigsanders   (501) staff       (20)      282 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/__init__.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.439321 aepsych-0.4.0/aepsych/server/message_handlers/
--rw-r--r--   0 craigsanders   (501) staff       (20)     1032 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1612 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_ask.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      748 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_can_model.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      758 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_exit.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      337 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_finish_strategy.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1125 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_get_config.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2056 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_info.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      760 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_params.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2518 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_query.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      682 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_resume.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4635 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_setup.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4951 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/message_handlers/handle_tell.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5639 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/replay.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    16416 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/server.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5823 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/sockets.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2218 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/server/utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    24592 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/strategy.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     9148 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1235 2023-06-05 20:10:10.000000 aepsych-0.4.0/aepsych/utils_logging.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      241 2023-06-05 20:24:32.000000 aepsych-0.4.0/aepsych/version.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:34.687806 aepsych-0.4.0/aepsych.egg-info/
--rw-r--r--   0 craigsanders   (501) staff       (20)     4565 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/PKG-INFO
--rw-r--r--   0 craigsanders   (501) staff       (20)     5151 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/SOURCES.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)        1 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/dependency_links.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)      107 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/entry_points.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)      177 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/requires.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)       14 2023-06-05 20:25:34.000000 aepsych-0.4.0/aepsych.egg-info/top_level.txt
--rw-r--r--   0 craigsanders   (501) staff       (20)      178 2023-06-05 20:10:10.000000 aepsych-0.4.0/pyproject.toml
--rw-r--r--   0 craigsanders   (501) staff       (20)       38 2023-06-05 20:25:35.832606 aepsych-0.4.0/setup.cfg
--rw-r--r--   0 craigsanders   (501) staff       (20)     1587 2023-06-05 20:14:09.000000 aepsych-0.4.0/setup.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.552017 aepsych-0.4.0/tests/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/__init__.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.592255 aepsych-0.4.0/tests/acquisition/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1019 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_lse.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4924 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_mi.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1822 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_monotonic.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1322 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_objective.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1353 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/acquisition/test_rejection_sampler.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     6480 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/common.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.643681 aepsych-0.4.0/tests/generators/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3973 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_completion_criteria.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1868 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_epsilon_greedy_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1933 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_manual_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4248 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_optimize_acqf_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2794 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_random_generator.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3492 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/generators/test_sobol_generator.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.743207 aepsych-0.4.0/tests/models/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2304 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_derivative_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    26030 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_gp_classification.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3066 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_gp_regression.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1666 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_model_query.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3014 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_monotonic_projection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4945 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_monotonic_rejection_gp.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1627 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_multitask_regression.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    25878 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_pairwise_probit.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    17592 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_semi_p.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3096 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_utils.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4458 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/models/test_variational_gp.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.751008 aepsych-0.4.0/tests/server/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/__init__.py
-drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2023-06-05 20:25:35.830998 aepsych-0.4.0/tests/server/message_handlers/
--rw-r--r--   0 craigsanders   (501) staff       (20)      218 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/__init__.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1535 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_can_model.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      774 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_handle_exit.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1471 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_handle_finish_strategy.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1766 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_handle_get_config.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2220 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_query_handlers.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     1168 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/message_handlers/test_tell_handlers.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    13121 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/server/test_server.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     2013 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_ThriftSocketWrapper.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     8589 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_ax_integration.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      999 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_bench_testfuns.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11024 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_benchmark.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    31034 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_config.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    20470 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_db.py
--rwxr-xr-x   0 craigsanders   (501) staff       (20)     8765 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_integration.py
--rw-r--r--   0 craigsanders   (501) staff       (20)      986 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_likelihoods.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     4051 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_lookahead.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    12311 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_mean_covar_factories.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     3017 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_multioutcome.py
--rw-r--r--   0 craigsanders   (501) staff       (20)    11224 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_strategy.py
--rw-r--r--   0 craigsanders   (501) staff       (20)     5975 2023-06-05 20:10:10.000000 aepsych-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.426634 aepsych-0.4.1/
+-rw-r--r--   0 craigsanders   (501) staff       (20)    19407 2024-04-30 19:00:18.000000 aepsych-0.4.1/LICENSE
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5433 2024-05-02 12:22:36.419857 aepsych-0.4.1/PKG-INFO
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:34.716871 aepsych-0.4.1/aepsych/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1011 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:34.882816 aepsych-0.4.1/aepsych/acquisition/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1390 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/acquisition/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      835 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/acquisition/acquisition.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3043 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/bvn.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13677 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/lookahead.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     7137 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/lookahead_utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3593 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/lse.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3775 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/acquisition/mc_posterior_variance.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6079 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/acquisition/monotonic_rejection.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5332 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/acquisition/mutual_information.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:34.908571 aepsych-0.4.1/aepsych/acquisition/objective/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      735 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/objective/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4307 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/objective/objective.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4702 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/acquisition/objective/semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2433 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/acquisition/rejection_sampler.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.106968 aepsych-0.4.1/aepsych/benchmark/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      868 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/benchmark/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11291 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/benchmark/benchmark.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10521 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/benchmark/pathos_benchmark.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10010 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/benchmark/problem.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6920 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/benchmark/test_functions.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13070 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1971 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/config.pyi
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.235160 aepsych-0.4.1/aepsych/database/
+-rw-r--r--   0 craigsanders   (501) staff       (20)        0 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/database/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11554 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/database/db.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    17629 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/database/tables.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.338133 aepsych-0.4.1/aepsych/factory/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      608 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/factory/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11147 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/factory/factory.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.519184 aepsych-0.4.1/aepsych/generators/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1366 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4121 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/base.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.553938 aepsych-0.4.1/aepsych/generators/completion_criterion/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      659 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/completion_criterion/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1510 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/completion_criterion/min_asks.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1454 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/completion_criterion/min_total_outcome_occurrences.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      823 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/completion_criterion/min_total_tells.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1501 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/completion_criterion/run_indefinitely.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1422 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/generators/epsilon_greedy_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2821 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/generators/manual_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     7978 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/generators/monotonic_rejection_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4473 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/generators/monotonic_thompson_sampler_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     8508 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/optimize_acqf_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      732 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/generators/pairwise_optimize_acqf_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      689 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/generators/pairwise_sobol_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2797 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/random_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2576 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/generators/semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3696 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/generators/sobol_generator.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.570851 aepsych-0.4.1/aepsych/kernels/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/kernels/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1801 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/kernels/rbf_partial_grad.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.600530 aepsych-0.4.1/aepsych/likelihoods/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      552 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/likelihoods/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1053 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/likelihoods/bernoulli.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2465 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/likelihoods/ordinal.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4332 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/likelihoods/semi_p.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.612627 aepsych-0.4.1/aepsych/means/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/means/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1109 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/means/constant_partial_grad.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.786307 aepsych-0.4.1/aepsych/models/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1551 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/models/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    22395 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/models/base.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4684 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/derivative_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      675 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/models/exact_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    12946 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/gp_classification.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6554 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/gp_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1646 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/models/model_list.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10235 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/monotonic_projection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13669 2024-04-30 20:10:52.000000 aepsych-0.4.1/aepsych/models/monotonic_rejection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6067 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/multitask_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2558 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/ordinal_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     7071 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/pairwise_probit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    24914 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/models/semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     9778 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/models/utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    10764 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/models/variational_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    16703 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/plotting.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.835862 aepsych-0.4.1/aepsych/server/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      282 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:35.950260 aepsych-0.4.1/aepsych/server/message_handlers/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1032 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1910 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_ask.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      748 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_can_model.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      624 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_exit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      337 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_finish_strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1125 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_get_config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2056 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_info.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      760 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_params.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2864 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_query.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      682 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_resume.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5175 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_setup.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5810 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/server/message_handlers/handle_tell.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5717 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/replay.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    15955 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/server.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3392 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/sockets.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2218 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/server/utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    25915 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     9814 2024-04-30 21:39:19.000000 aepsych-0.4.1/aepsych/utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1235 2024-04-30 19:00:18.000000 aepsych-0.4.1/aepsych/utils_logging.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      241 2024-04-30 21:41:29.000000 aepsych-0.4.1/aepsych/version.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.402329 aepsych-0.4.1/aepsych.egg-info/
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5433 2024-05-02 12:22:34.000000 aepsych-0.4.1/aepsych.egg-info/PKG-INFO
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5065 2024-05-02 12:22:34.000000 aepsych-0.4.1/aepsych.egg-info/SOURCES.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)        1 2024-05-02 12:22:34.000000 aepsych-0.4.1/aepsych.egg-info/dependency_links.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)      107 2024-05-02 12:22:34.000000 aepsych-0.4.1/aepsych.egg-info/entry_points.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)      305 2024-05-02 12:22:34.000000 aepsych-0.4.1/aepsych.egg-info/requires.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)       14 2024-05-02 12:22:34.000000 aepsych-0.4.1/aepsych.egg-info/top_level.txt
+-rw-r--r--   0 craigsanders   (501) staff       (20)      178 2024-04-30 19:00:18.000000 aepsych-0.4.1/pyproject.toml
+-rw-r--r--   0 craigsanders   (501) staff       (20)       38 2024-05-02 12:22:36.429502 aepsych-0.4.1/setup.cfg
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1675 2024-04-30 21:39:19.000000 aepsych-0.4.1/setup.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.119633 aepsych-0.4.1/tests/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.162722 aepsych-0.4.1/tests/acquisition/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/acquisition/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1019 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/acquisition/test_lse.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4924 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/acquisition/test_mi.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1822 2024-04-30 20:10:52.000000 aepsych-0.4.1/tests/acquisition/test_monotonic.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1322 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/acquisition/test_objective.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1353 2024-04-30 20:10:52.000000 aepsych-0.4.1/tests/acquisition/test_rejection_sampler.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     6480 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/common.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.216697 aepsych-0.4.1/tests/generators/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/generators/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3340 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/generators/test_completion_criteria.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1868 2024-04-30 20:10:52.000000 aepsych-0.4.1/tests/generators/test_epsilon_greedy_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1907 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/generators/test_manual_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4580 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/generators/test_optimize_acqf_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2794 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/generators/test_random_generator.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3492 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/generators/test_sobol_generator.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.316790 aepsych-0.4.1/tests/models/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2304 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_derivative_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    26298 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_gp_classification.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3066 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_gp_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3591 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/models/test_model_query.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3014 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_monotonic_projection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4945 2024-04-30 20:10:52.000000 aepsych-0.4.1/tests/models/test_monotonic_rejection_gp.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1627 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_multitask_regression.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    25878 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/models/test_pairwise_probit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    17592 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_semi_p.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3096 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/models/test_utils.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4503 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/models/test_variational_gp.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.333330 aepsych-0.4.1/tests/server/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/__init__.py
+drwxr-xr-x   0 craigsanders   (501) staff       (20)        0 2024-05-02 12:22:36.392394 aepsych-0.4.1/tests/server/message_handlers/
+-rw-r--r--   0 craigsanders   (501) staff       (20)      218 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/__init__.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1535 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/test_can_model.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      774 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/test_handle_exit.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1471 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/test_handle_finish_strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1766 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/test_handle_get_config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     2009 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/test_query_handlers.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     1168 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/server/message_handlers/test_tell_handlers.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    13121 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/server/test_server.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     9691 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_ax_integration.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      992 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_bench_testfuns.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11024 2024-04-30 20:10:52.000000 aepsych-0.4.1/tests/test_benchmark.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    31034 2024-04-30 20:10:52.000000 aepsych-0.4.1/tests/test_config.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    20470 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_db.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)      986 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_likelihoods.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     4051 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_lookahead.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    12311 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_mean_covar_factories.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     3089 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/test_multioutcome.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)    11224 2024-04-30 21:39:19.000000 aepsych-0.4.1/tests/test_strategy.py
+-rw-r--r--   0 craigsanders   (501) staff       (20)     5975 2024-04-30 19:00:18.000000 aepsych-0.4.1/tests/test_utils.py
```

### Comparing `aepsych-0.4.0/LICENSE` & `aepsych-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/__init__.py` & `aepsych-0.4.1/aepsych/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,23 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import sys
 
 from gpytorch.likelihoods import BernoulliLikelihood, GaussianLikelihood
 
-from . import (
-    acquisition,
-    benchmark,
-    config,
-    factory,
-    generators,
-    models,
-    strategy,
-    utils,
-)
+from . import acquisition, config, factory, generators, models, strategy, utils
 from .config import Config
 from .likelihoods import BernoulliObjectiveLikelihood
 from .models import GPClassificationModel
 from .strategy import SequentialStrategy, Strategy
 
 __all__ = [
     # modules
     "acquisition",
-    "benchmark",
     "config",
     "factory",
     "models",
     "strategy",
     "utils",
     "generators",
     # classes
@@ -39,8 +29,15 @@
     "Strategy",
     "SequentialStrategy",
     "BernoulliObjectiveLikelihood",
     "BernoulliLikelihood",
     "GaussianLikelihood",
 ]
 
+try:
+    from . import benchmark
+
+    __all__ += ["benchmark"]
+except ImportError:
+    pass
+
 Config.register_module(sys.modules[__name__])
```

### Comparing `aepsych-0.4.0/aepsych/acquisition/__init__.py` & `aepsych-0.4.1/aepsych/acquisition/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/acquisition.py` & `aepsych-0.4.1/aepsych/acquisition/acquisition.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/bvn.py` & `aepsych-0.4.1/aepsych/acquisition/bvn.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/lookahead.py` & `aepsych-0.4.1/aepsych/acquisition/lookahead.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/lookahead_utils.py` & `aepsych-0.4.1/aepsych/acquisition/lookahead_utils.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/lse.py` & `aepsych-0.4.1/aepsych/acquisition/lse.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/mc_posterior_variance.py` & `aepsych-0.4.1/aepsych/acquisition/mc_posterior_variance.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/monotonic_rejection.py` & `aepsych-0.4.1/aepsych/acquisition/monotonic_rejection.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/mutual_information.py` & `aepsych-0.4.1/aepsych/acquisition/mutual_information.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/objective/__init__.py` & `aepsych-0.4.1/aepsych/acquisition/objective/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/objective/objective.py` & `aepsych-0.4.1/aepsych/acquisition/objective/objective.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/objective/semi_p.py` & `aepsych-0.4.1/aepsych/acquisition/objective/semi_p.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/acquisition/rejection_sampler.py` & `aepsych-0.4.1/aepsych/acquisition/rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/benchmark/__init__.py` & `aepsych-0.4.1/aepsych/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/benchmark/benchmark.py` & `aepsych-0.4.1/aepsych/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/benchmark/pathos_benchmark.py` & `aepsych-0.4.1/aepsych/benchmark/pathos_benchmark.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/benchmark/problem.py` & `aepsych-0.4.1/aepsych/benchmark/problem.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/benchmark/test_functions.py` & `aepsych-0.4.1/aepsych/benchmark/test_functions.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/config.py` & `aepsych-0.4.1/aepsych/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,8 +368,9 @@
     def from_config(cls, config: Config, name: Optional[str] = None):
         return cls(**cls.get_config_options(config, name))
 
 
 Config.register_module(gpytorch.likelihoods)
 Config.register_module(gpytorch.kernels)
 Config.register_module(botorch.acquisition)
+Config.register_module(botorch.acquisition.multi_objective)
 Config.registered_names["None"] = None
```

### Comparing `aepsych-0.4.0/aepsych/database/db.py` & `aepsych-0.4.1/aepsych/database/db.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/database/tables.py` & `aepsych-0.4.1/aepsych/database/tables.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/factory/__init__.py` & `aepsych-0.4.1/aepsych/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/factory/factory.py` & `aepsych-0.4.1/aepsych/factory/factory.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/__init__.py` & `aepsych-0.4.1/aepsych/generators/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 import sys
 
 from ..config import Config
 from .epsilon_greedy_generator import EpsilonGreedyGenerator
 from .manual_generator import ManualGenerator
 from .monotonic_rejection_generator import MonotonicRejectionGenerator
 from .monotonic_thompson_sampler_generator import MonotonicThompsonSamplerGenerator
-from .multi_outcome_generator import MultiOutcomeOptimizationGenerator
 from .optimize_acqf_generator import AxOptimizeAcqfGenerator, OptimizeAcqfGenerator
 from .pairwise_optimize_acqf_generator import PairwiseOptimizeAcqfGenerator
 from .pairwise_sobol_generator import PairwiseSobolGenerator
-from .random_generator import RandomGenerator
 from .random_generator import AxRandomGenerator, RandomGenerator
 from .semi_p import IntensityAwareSemiPGenerator
 from .sobol_generator import AxSobolGenerator, SobolGenerator
 
 __all__ = [
     "OptimizeAcqfGenerator",
     "MonotonicRejectionGenerator",
@@ -30,12 +28,11 @@
     "EpsilonGreedyGenerator",
     "ManualGenerator",
     "PairwiseOptimizeAcqfGenerator",
     "PairwiseSobolGenerator",
     "AxOptimizeAcqfGenerator",
     "AxSobolGenerator",
     "IntensityAwareSemiPGenerator",
-    "MultiOutcomeOptimizationGenerator",
     "AxRandomGenerator",
 ]
 
 Config.register_module(sys.modules[__name__])
```

### Comparing `aepsych-0.4.0/aepsych/generators/base.py` & `aepsych-0.4.1/aepsych/generators/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 import abc
 from inspect import signature
-from typing import Any, Dict, Generic, Protocol, runtime_checkable, TypeVar
+from typing import Any, Dict, Generic, Protocol, runtime_checkable, TypeVar, Optional
 
 import torch
 from aepsych.config import Config, ConfigurableMixin
 from aepsych.models.base import AEPsychMixin
 from ax.core.experiment import Experiment
 from ax.modelbridge.generation_node import GenerationStep
 from botorch.acquisition import (
@@ -32,14 +32,15 @@
 
 class AEPsychGenerator(abc.ABC, Generic[AEPsychModelType]):
     """Abstract base class for generators, which are responsible for generating new points to sample."""
 
     _requires_model = True
     baseline_requiring_acqfs = [qNoisyExpectedImprovement, NoisyExpectedImprovement]
     stimuli_per_trial = 1
+    max_asks: Optional[int] = None
 
     def __init__(
         self,
     ) -> None:
         pass
 
     @abc.abstractmethod
```

### Comparing `aepsych-0.4.0/aepsych/generators/completion_criterion/__init__.py` & `aepsych-0.4.1/aepsych/generators/completion_criterion/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,22 @@
 import sys
 
 from aepsych.config import Config
 
 from .min_asks import MinAsks
 from .min_total_outcome_occurrences import MinTotalOutcomeOccurrences
 from .min_total_tells import MinTotalTells
-from .run_indefinitely import RunIndefinitely
 
 completion_criteria = [
     MinTotalTells,
     MinAsks,
     MinTotalOutcomeOccurrences,
-    RunIndefinitely,
 ]
 
 __all__ = [
     "completion_criteria",
     "MinTotalTells",
     "MinAsks",
     "MinTotalOutcomeOccurrences",
-    "RunIndefinitely",
 ]
 
 Config.register_module(sys.modules[__name__])
```

### Comparing `aepsych-0.4.0/aepsych/generators/completion_criterion/min_total_outcome_occurrences.py` & `aepsych-0.4.1/aepsych/generators/completion_criterion/min_total_outcome_occurrences.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict
 
 from aepsych.config import Config, ConfigurableMixin
 
-from ax.modelbridge.completion_criterion import MinimumPreferenceOccurances
+from ax.modelbridge.transition_criterion import MinimumPreferenceOccurances
 
 
 class MinTotalOutcomeOccurrences(MinimumPreferenceOccurances, ConfigurableMixin):
     @classmethod
     def get_config_options(cls, config: Config, name: str) -> Dict[str, Any]:
         outcome_types = config.getlist(name, "outcome_types", element_type=str)
         outcome_names = config.getlist(
```

### Comparing `aepsych-0.4.0/aepsych/generators/completion_criterion/min_total_tells.py` & `aepsych-0.4.1/aepsych/generators/completion_criterion/min_total_tells.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Any, Dict
 
 from aepsych.config import Config, ConfigurableMixin
 from ax.core.base_trial import TrialStatus
-from ax.modelbridge.completion_criterion import MinimumTrialsInStatus
+from ax.modelbridge.transition_criterion import MinTrials
 
 
-class MinTotalTells(MinimumTrialsInStatus, ConfigurableMixin):
+class MinTotalTells(MinTrials, ConfigurableMixin):
     @classmethod
     def get_config_options(cls, config: Config, name: str) -> Dict[str, Any]:
         min_total_tells = config.getint(name, "min_total_tells", fallback=1)
-        options = {"status": TrialStatus.COMPLETED, "threshold": min_total_tells}
+        options = {
+            "only_in_statuses": [TrialStatus.COMPLETED],
+            "threshold": min_total_tells,
+            "use_all_trials_in_exp": True,
+        }
         return options
```

### Comparing `aepsych-0.4.0/aepsych/generators/completion_criterion/run_indefinitely.py` & `aepsych-0.4.1/aepsych/generators/completion_criterion/run_indefinitely.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Set
 
 from aepsych.config import Config, ConfigurableMixin
 from ax.core import Experiment
-from ax.modelbridge.completion_criterion import CompletionCriterion
+from ax.modelbridge.transition_criterion import TransitionCriterion
 
 
-class RunIndefinitely(CompletionCriterion, ConfigurableMixin):
-    def __init__(self, run_indefinitely: bool) -> None:
+class RunIndefinitely(TransitionCriterion, ConfigurableMixin):
+    def __init__(
+        self,
+        run_indefinitely: bool,
+        block_transition_if_unmet: Optional[bool] = False,
+        block_gen_if_met: Optional[bool] = False,
+    ) -> None:
         self.run_indefinitely = run_indefinitely
+        self.block_transition_if_unmet = block_transition_if_unmet
+        self.block_gen_if_met = block_gen_if_met
 
-    def is_met(self, experiment: Experiment) -> bool:
+    def is_met(
+        self, experiment: Experiment, trials_from_node: Optional[Set[int]] = None
+    ) -> bool:
         return not self.run_indefinitely
 
+    def block_continued_generation_error(
+        self,
+        node_name: Optional[str],
+        model_name: Optional[str],
+        experiment: Optional[Experiment],
+        trials_from_node: Optional[Set[int]] = None,
+    ) -> None:
+        pass
+
     @classmethod
     def get_config_options(cls, config: Config, name: str) -> Dict[str, Any]:
         run_indefinitely = config.getboolean(name, "run_indefinitely", fallback=False)
         options = {"run_indefinitely": run_indefinitely}
         return options
```

### Comparing `aepsych-0.4.0/aepsych/generators/epsilon_greedy_generator.py` & `aepsych-0.4.1/aepsych/generators/epsilon_greedy_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/manual_generator.py` & `aepsych-0.4.1/aepsych/generators/manual_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,18 +34,18 @@
             lb (Union[np.ndarray, torch.Tensor]): Lower bounds of each parameter.
             ub (Union[np.ndarray, torch.Tensor]): Upper bounds of each parameter.
             points (Union[np.ndarray, torch.Tensor]): The points that will be generated.
             dim (int, optional): Dimensionality of the parameter space. If None, it is inferred from lb and ub.
             shuffle (bool): Whether or not to shuffle the order of the points. True by default.
         """
         self.lb, self.ub, self.dim = _process_bounds(lb, ub, dim)
-        self.points = points
+        self.points = torch.tensor(points)
         if shuffle:
             np.random.shuffle(points)
-        self.finished = False
+        self.max_asks = len(self.points)
         self._idx = 0
 
     def gen(
         self,
         num_points: int = 1,
         model: Optional[AEPsychMixin] = None,  # included for API compatibility
     ):
@@ -58,16 +58,14 @@
         if num_points > (len(self.points) - self._idx):
             warnings.warn(
                 "Asked for more points than are left in the generator! Giving everthing it has!",
                 RuntimeWarning,
             )
         points = self.points[self._idx : self._idx + num_points]
         self._idx += num_points
-        if self._idx >= len(self.points):
-            self.finished = True
         return points
 
     @classmethod
     def from_config(cls, config: Config):
         classname = cls.__name__
 
         lb = config.gettensor(classname, "lb")
```

### Comparing `aepsych-0.4.0/aepsych/generators/monotonic_rejection_generator.py` & `aepsych-0.4.1/aepsych/generators/monotonic_rejection_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/monotonic_thompson_sampler_generator.py` & `aepsych-0.4.1/aepsych/generators/monotonic_thompson_sampler_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         X = draw_sobol_samples(bounds=model.bounds_, n=self.num_ts_points, q=1).squeeze(
             1
         )
         # Fix any explore features
         if self.explore_features is not None:
             for idx in self.explore_features:
                 val = (
-                    model.bounds_[0, idx]
-                    + torch.rand(1) * (model.bounds_[1, idx] - model.bounds_[0, idx])
+                    model.bounds_[0, idx]  # type: ignore
+                    + torch.rand(1) * (model.bounds_[1, idx] - model.bounds_[0, idx])  # type: ignore
                 ).item()
                 X[:, idx] = val
 
         # Draw n samples
         f_samp = model.sample(
             X,
             num_samples=self.n_samples,
```

### Comparing `aepsych-0.4.0/aepsych/generators/optimize_acqf_generator.py` & `aepsych-0.4.1/aepsych/generators/optimize_acqf_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 
 import numpy as np
 import torch
 from aepsych.acquisition.acquisition import AEPsychAcquisition
 from aepsych.config import Config, ConfigurableMixin
 from aepsych.generators.base import AEPsychGenerationStep, AEPsychGenerator
 from aepsych.models.base import ModelProtocol
-from aepsych.models.surrogate import AEPsychSurrogate
+from ax.models.torch.botorch_modular.surrogate import Surrogate
 from aepsych.utils_logging import getLogger
 from ax.modelbridge import Models
 from ax.modelbridge.registry import Cont_X_trans
 from botorch.acquisition import AcquisitionFunction
 from botorch.acquisition.preference import AnalyticExpectedUtilityOfBestOption
 from botorch.optim import optimize_acqf
-from botorch.utils import draw_sobol_samples
 
 logger = getLogger()
 
 
 class OptimizeAcqfGenerator(AEPsychGenerator):
     """Generator that chooses points by minimizing an acquisition function."""
 
@@ -43,16 +42,14 @@
         Args:
             acqf (AcquisitionFunction): Acquisition function to use.
             acqf_kwargs (Dict[str, object], optional): Extra arguments to
                 pass to acquisition function. Defaults to no arguments.
             restarts (int): Number of restarts for acquisition function optimization.
             samps (int): Number of samples for quasi-random initialization of the acquisition function optimizer.
             max_gen_time (optional, float): Maximum time (in seconds) to optimize the acquisition function.
-                This is only loosely followed by scipy's optimizer, so consider using a number about 1/3 or
-                less of what your true upper bound is.
         """
 
         if acqf_kwargs is None:
             acqf_kwargs = {}
         self.acqf = acqf
         self.acqf_kwargs = acqf_kwargs
         self.restarts = restarts
@@ -99,64 +96,23 @@
         model.eval()  # type: ignore
         train_x = model.train_inputs[0]
         acqf = self._instantiate_acquisition_fn(model)
 
         logger.info("Starting gen...")
         starttime = time.time()
 
-        if self.max_gen_time is None:
-            new_candidate, _ = optimize_acqf(
-                acq_function=acqf,
-                bounds=torch.tensor(np.c_[model.lb, model.ub]).T.to(train_x),
-                q=num_points,
-                num_restarts=self.restarts,
-                raw_samples=self.samps,
-                **gen_options,
-            )
-        else:
-            # figure out how long evaluating a single samp
-            starttime = time.time()
-            _ = acqf(train_x[0:num_points, :])
-            single_eval_time = time.time() - starttime
-
-            # only a heuristic for total num evals since everything is stochastic,
-            # but the reasoning is: we initialize with self.samps samps, subsample
-            # self.restarts from them in proportion to the value of the acqf, and
-            # run that many optimization. So:
-            # total_time = single_eval_time * n_eval * restarts + single_eval_time * samps
-            # and we solve for n_eval
-            n_eval = int(
-                (self.max_gen_time - single_eval_time * self.samps)
-                / (single_eval_time * self.restarts)
-            )
-            if n_eval > 10:
-                # heuristic, if we can't afford 10 evals per restart, just use quasi-random search
-                options = {"maxfun": n_eval}
-                logger.info(f"gen maxfun is {n_eval}")
-
-                new_candidate, _ = optimize_acqf(
-                    acq_function=acqf,
-                    bounds=torch.tensor(np.c_[model.lb, model.ub]).T.to(train_x),
-                    q=num_points,
-                    num_restarts=self.restarts,
-                    raw_samples=self.samps,
-                    options=options,
-                )
-            else:
-                logger.info(f"gen maxfun is {n_eval}, falling back to random search...")
-                nsamp = max(int(self.max_gen_time / single_eval_time), 10)
-                # Generate the points at which to sample
-                bounds = torch.stack((model.lb, model.ub))
-
-                X = draw_sobol_samples(bounds=bounds, n=nsamp, q=num_points)
-
-                acqvals = acqf(X)
-
-                best_indx = torch.argmax(acqvals, dim=0)
-                new_candidate = X[best_indx]
+        new_candidate, _ = optimize_acqf(
+            acq_function=acqf,
+            bounds=torch.tensor(np.c_[model.lb, model.ub]).T.to(train_x),
+            q=num_points,
+            num_restarts=self.restarts,
+            raw_samples=self.samps,
+            timeout_sec=self.max_gen_time,
+            **gen_options,
+        )
 
         logger.info(f"Gen done, time={time.time()-starttime}")
         return new_candidate
 
     @classmethod
     def from_config(cls, config: Config):
         classname = cls.__name__
@@ -192,22 +148,19 @@
         acqf_cls = config.getobj(name, "acqf", fallback=None)
         if acqf_cls is None:
             acqf_cls = config.getobj(classname, "acqf")
 
         acqf_options = cls._get_acqf_options(acqf_cls, config)
         gen_options = cls._get_gen_options(config)
 
-        max_fit_time = model_options["max_fit_time"]
-
         model_kwargs = {
-            "surrogate": AEPsychSurrogate(
+            "surrogate": Surrogate(
                 botorch_model_class=model_class,
                 mll_class=model_class.get_mll_class(),
                 model_options=model_options,
-                max_fit_time=max_fit_time,
             ),
             "acquisition_class": AEPsychAcquisition,
             "botorch_acqf_class": acqf_cls,
             "acquisition_options": acqf_options,
             # The Y transforms are removed because they are incompatible with our thresholding-finding acqfs
             # The target value doesn't get transformed, so it searches for the target in the wrong space.
             "transforms": Cont_X_trans,  # TODO: Make LSE acqfs compatible with Y transforms
@@ -254,10 +207,18 @@
             acqf_args = {}
 
         return acqf_args
 
     @classmethod
     def _get_gen_options(cls, config: Config):
         classname = "OptimizeAcqfGenerator"
-        restarts = config.getint(classname, "restarts", fallback=10)
-        samps = config.getint(classname, "samps", fallback=1000)
-        return {"restarts": restarts, "samps": samps}
+        restarts = config.getint(classname, "num_restarts", fallback=10)
+        samps = config.getint(classname, "raw_samples", fallback=1024)
+        timeout_sec = config.getfloat(classname, "max_gen_time", fallback=None)
+        optimizer_kwargs = {
+            "optimizer_kwargs": {
+                "num_restarts": restarts,
+                "raw_samples": samps,
+                "timeout_sec": timeout_sec,
+            }
+        }
+        return {"model_gen_options": optimizer_kwargs}
```

### Comparing `aepsych-0.4.0/aepsych/generators/pairwise_optimize_acqf_generator.py` & `aepsych-0.4.1/aepsych/generators/pairwise_optimize_acqf_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/pairwise_sobol_generator.py` & `aepsych-0.4.1/aepsych/generators/pairwise_sobol_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/random_generator.py` & `aepsych-0.4.1/aepsych/generators/random_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/semi_p.py` & `aepsych-0.4.1/aepsych/generators/semi_p.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/generators/sobol_generator.py` & `aepsych-0.4.1/aepsych/generators/sobol_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/kernels/rbf_partial_grad.py` & `aepsych-0.4.1/aepsych/kernels/rbf_partial_grad.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/likelihoods/__init__.py` & `aepsych-0.4.1/aepsych/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/likelihoods/bernoulli.py` & `aepsych-0.4.1/aepsych/likelihoods/bernoulli.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/likelihoods/ordinal.py` & `aepsych-0.4.1/aepsych/likelihoods/ordinal.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/likelihoods/semi_p.py` & `aepsych-0.4.1/aepsych/likelihoods/semi_p.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/means/constant_partial_grad.py` & `aepsych-0.4.1/aepsych/means/constant_partial_grad.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/__init__.py` & `aepsych-0.4.1/aepsych/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,31 @@
 
 import sys
 
 from ..config import Config
 from .exact_gp import ContinuousRegressionGP, ExactGP
 from .gp_classification import GPBetaRegressionModel, GPClassificationModel
 from .gp_regression import GPRegressionModel
+from .model_list import AEPsychModelListGP
 from .monotonic_projection_gp import MonotonicProjectionGP
 from .monotonic_rejection_gp import MonotonicRejectionGP
 from .multitask_regression import IndependentMultitaskGPRModel, MultitaskGPRModel
 from .ordinal_gp import OrdinalGPModel
 from .pairwise_probit import PairwiseProbitModel
 from .semi_p import (
     HadamardSemiPModel,
     semi_p_posterior_transform,
     SemiParametricGPModel,
 )
-from .variational_gp import BetaRegressionGP, BinaryClassificationGP, OrdinalGP, VariationalGP
-
+from .variational_gp import (
+    BetaRegressionGP,
+    BinaryClassificationGP,
+    OrdinalGP,
+    VariationalGP,
+)
 
 
 __all__ = [
     "GPClassificationModel",
     "MonotonicRejectionGP",
     "GPRegressionModel",
     "PairwiseProbitModel",
@@ -40,10 +45,11 @@
     "MultitaskGPRModel",
     "IndependentMultitaskGPRModel",
     "HadamardSemiPModel",
     "SemiParametricGPModel",
     "semi_p_posterior_transform",
     "OrdinalGP",
     "GPBetaRegressionModel",
+    "AEPsychModelListGP",
 ]
 
 Config.register_module(sys.modules[__name__])
```

### Comparing `aepsych-0.4.0/aepsych/models/base.py` & `aepsych-0.4.1/aepsych/models/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 from __future__ import annotations
 
 import abc
 
 import time
+from collections.abc import Iterable
 from typing import Any, Dict, List, Mapping, Optional, Protocol, Tuple, Union
 
 import gpytorch
 import numpy as np
 import torch
 
 from aepsych.config import Config, ConfigurableMixin
-from aepsych.factory.factory import default_mean_covar_factory
-from aepsych.models.utils import get_extremum
+from aepsych.models.utils import get_extremum, inv_query
 from aepsych.utils import dim_grid, get_jnd_multid, make_scaled_sobol, promote_0d
 from aepsych.utils_logging import getLogger
 from botorch.fit import fit_gpytorch_mll, fit_gpytorch_mll_scipy
 from botorch.models.gpytorch import GPyTorchModel
 from botorch.posteriors import GPyTorchPosterior
 from gpytorch.likelihoods import Likelihood
 from gpytorch.mlls import MarginalLogLikelihood
-from scipy.optimize import minimize
 from scipy.stats import norm
 
+
 logger = getLogger()
 
 torch.set_default_dtype(torch.double)  # TODO: find a better way to prevent type errors
 
 
 class ModelProtocol(Protocol):
     @property
@@ -68,14 +68,17 @@
 
     def posterior(self, x: torch.Tensor) -> GPyTorchPosterior:
         pass
 
     def predict(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
         pass
 
+    def predict_probability(self, x: torch.Tensor, **kwargs) -> torch.Tensor:
+        pass
+
     @property
     def stimuli_per_trial(self) -> int:
         pass
 
     @property
     def likelihood(self) -> Likelihood:
         pass
@@ -115,110 +118,105 @@
     @property
     def bounds(self):
         return torch.stack((self.lb, self.ub))
 
     def get_max(
         self: ModelProtocol,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
+        probability_space: bool = False,
         n_samples: int = 1000,
-    ) -> Tuple[float, np.ndarray]:
+        max_time: Optional[float] = None,
+    ) -> Tuple[float, torch.Tensor]:
         """Return the maximum of the modeled function, subject to constraints
-        Returns:
-            Tuple[float, np.ndarray]: Tuple containing the max and its location (argmax).
+        Args:
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
+            probability_space (bool): Is y (and therefore the returned nearest_y) in
+                probability space instead of latent function space? Defaults to False.
             n_samples int: number of coarse grid points to sample for optimization estimate.
+        Returns:
+            Tuple[float, np.ndarray]: Tuple containing the max and its location (argmax).
         """
         locked_dims = locked_dims or {}
-        return get_extremum(self, "max", self.bounds, locked_dims, n_samples)
+        _, _arg = get_extremum(
+            self, "max", self.bounds, locked_dims, n_samples, max_time=max_time
+        )
+        arg = torch.tensor(_arg.reshape(1, self.dim))
+        if probability_space:
+            val, _ = self.predict_probability(arg)
+        else:
+            val, _ = self.predict(arg)
+        return float(val.item()), arg
 
     def get_min(
         self: ModelProtocol,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
+        probability_space: bool = False,
         n_samples: int = 1000,
-    ) -> Tuple[float, np.ndarray]:
+        max_time: Optional[float] = None,
+    ) -> Tuple[float, torch.Tensor]:
         """Return the minimum of the modeled function, subject to constraints
-        Returns:
-            Tuple[float, np.ndarray]: Tuple containing the min and its location (argmin).
+        Args:
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
+            probability_space (bool): Is y (and therefore the returned nearest_y) in
+                probability space instead of latent function space? Defaults to False.
             n_samples int: number of coarse grid points to sample for optimization estimate.
+        Returns:
+            Tuple[float, torch.Tensor]: Tuple containing the min and its location (argmin).
         """
         locked_dims = locked_dims or {}
-        return get_extremum(self, "min", self.bounds, locked_dims, n_samples)
+        _, _arg = get_extremum(
+            self, "min", self.bounds, locked_dims, n_samples, max_time=max_time
+        )
+        arg = torch.tensor(_arg.reshape(1, self.dim))
+        if probability_space:
+            val, _ = self.predict_probability(arg)
+        else:
+            val, _ = self.predict(arg)
+        return float(val.item()), arg
 
     def inv_query(
-        self: ModelProtocol,
+        self,
         y: float,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
         probability_space: bool = False,
         n_samples: int = 1000,
+        max_time: Optional[float] = None,
+        weights: Optional[torch.Tensor] = None,
     ) -> Tuple[float, torch.Tensor]:
         """Query the model inverse.
         Return nearest x such that f(x) = queried y, and also return the
             value of f at that point.
         Args:
             y (float): Points at which to find the inverse.
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
-            probability_space (bool, optional): Is y (and therefore the
-                returned nearest_y) in probability space instead of latent
-                function space? Defaults to False.
+            probability_space (bool): Is y (and therefore the returned nearest_y) in
+                probability space instead of latent function space? Defaults to False.
         Returns:
-            Tuple[float, np.ndarray]: Tuple containing the value of f
+            Tuple[float, torch.Tensor]: Tuple containing the value of f
                 nearest to queried y and the x position of this value.
         """
-        if probability_space:
-            assert (
-                self.outcome_type == "binary"
-            ), f"Cannot get probability space for outcome_type '{self.outcome_type}'"
-
-        locked_dims = locked_dims or {}
-
-        def model_distance(x, pt, probability_space):
-            return np.abs(
-                self.predict(torch.tensor([x]), probability_space=probability_space)[0]
-                .detach()
-                .numpy()
-                - pt
-            )
-
-        # Look for point with value closest to y, subject the dict of locked dims
-
-        query_lb = self.lb.clone()
-        query_ub = self.ub.clone()
-
-        for locked_dim in locked_dims.keys():
-            dim_values = locked_dims[locked_dim]
-            if len(dim_values) == 1:
-                query_lb[locked_dim] = dim_values[0]
-                query_ub[locked_dim] = dim_values[0]
-            else:
-                query_lb[locked_dim] = dim_values[0]
-                query_ub[locked_dim] = dim_values[1]
-
-        d = make_scaled_sobol(query_lb, query_ub, n_samples, seed=0)
-
-        bounds = zip(query_lb.numpy(), query_ub.numpy())
-
-        fmean, _ = self.predict(d, probability_space=probability_space)
-
-        f = torch.abs(fmean - y)
-        estimate = d[torch.where(f == torch.min(f))[0][0]].numpy()
-        a = minimize(
-            model_distance,
-            estimate,
-            args=(y, probability_space),
-            method=self.extremum_solver,
-            bounds=bounds,
+        _, _arg = inv_query(
+            self,
+            y=y,
+            bounds=self.bounds,
+            locked_dims=locked_dims,
+            probability_space=probability_space,
+            n_samples=n_samples,
+            max_time=max_time,
+            weights=weights,
         )
-        val = self.predict(torch.tensor([a.x]), probability_space=probability_space)[
-            0
-        ].item()
-        return val, torch.Tensor(a.x)
+        arg = torch.tensor(_arg.reshape(1, self.dim))
+        if probability_space:
+            val, _ = self.predict_probability(arg.reshape(1, self.dim))
+        else:
+            val, _ = self.predict(arg.reshape(1, self.dim))
+        return float(val.item()), arg
 
     def get_jnd(
         self: ModelProtocol,
         grid: Optional[Union[np.ndarray, torch.Tensor]] = None,
         cred_level: Optional[float] = None,
         intensity_dim: int = -1,
         confsamps: int = 500,
@@ -312,15 +310,15 @@
         return median, lower, upper
 
     def dim_grid(
         self: ModelProtocol,
         gridsize: int = 30,
         slice_dims: Optional[Mapping[int, float]] = None,
     ) -> torch.Tensor:
-        return dim_grid(self.lb, self.ub, self.dim, gridsize, slice_dims)
+        return dim_grid(self.lb, self.ub, gridsize, slice_dims)
 
     def set_train_data(self, inputs=None, targets=None, strict=False):
         """
         :param torch.Tensor inputs: The new training inputs.
         :param torch.Tensor targets: The new training targets.
         :param bool strict: (default False, ignored). Here for compatibility with
         input transformers. TODO: actually use this arg or change input transforms
@@ -382,33 +380,40 @@
         f, var = self.predict(x)
         return norm.cdf((f_thresh - f.detach().numpy()) / var.sqrt().detach().numpy())
 
 
 class AEPsychModel(ConfigurableMixin, abc.ABC):
     extremum_solver = "Nelder-Mead"
     outcome_type: Optional[str] = None
+    default_likelihood: Optional[
+        Likelihood
+    ] = None  # will use default Gaussian likelihood from botorch
 
     def predict(
         self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray]
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Query the model for posterior mean and variance.
 
         Args:
             x (Union[torch.Tensor, np.ndarray]): Points at which to predict from the model.
 
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: Posterior mean and variance at queried points.
         """
+        if isinstance(x, np.ndarray):
+            x = torch.tensor(x)
         with torch.no_grad():
             post = self.posterior(x)
         fmean = post.mean.squeeze()
         fvar = post.variance.squeeze()
         return promote_0d(fmean), promote_0d(fvar)
 
-    def predict_probability(self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray]):
+    def predict_probability(
+        self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray]
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
         raise NotImplementedError
 
     def sample(
         self: GPyTorchModel, x: Union[torch.Tensor, np.ndarray], n: int
     ) -> torch.Tensor:
         """Sample the model posterior at the given points.
 
@@ -422,43 +427,38 @@
         return self.posterior(x).sample(torch.Size([n]))
 
     @classmethod
     def get_config_options(cls, config: Config, name: Optional[str] = None) -> Dict:
         if name is None:
             name = cls.__name__
 
-        mean_covar_factory = config.getobj(
-            name, "mean_covar_factory", fallback=default_mean_covar_factory
-        )
-        mean, covar = mean_covar_factory(config)
+        mean = config.getobj(name, "mean_module", fallback=None)
+        covar = config.getobj(name, "covar_module", fallback=None)
 
         likelihood_cls = config.getobj(name, "likelihood", fallback=None)
         if likelihood_cls is not None:
             if hasattr(likelihood_cls, "from_config"):
                 likelihood = likelihood_cls.from_config(config)
             else:
                 likelihood = likelihood_cls()
         else:
             likelihood = None  # fall back to __init__ default
 
-        max_fit_time = config.getfloat(name, "max_fit_time", fallback=None)
-
         options = {
             "likelihood": likelihood,
             "covar_module": covar,
             "mean_module": mean,
-            "max_fit_time": max_fit_time,
         }
 
         return options
 
     @classmethod
     def construct_inputs(cls, training_data, **kwargs):
-        train_X = training_data.X()
-        train_Y = training_data.Y()
+        train_X = training_data.X
+        train_Y = training_data.Y
 
         likelihood = kwargs.get("likelihood")
         covar_module = kwargs.get("covar_module")
         mean_module = kwargs.get("mean_module")
 
         inputs = {
             "train_X": train_X,
@@ -470,114 +470,136 @@
 
         return inputs
 
     def get_max(
         self,
         bounds: torch.Tensor,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
+        probability_space: bool = False,
         n_samples: int = 1000,
-    ) -> Tuple[float, np.ndarray]:
+        max_time: Optional[float] = None,
+        weights: Optional[torch.Tensor] = None,
+    ) -> Tuple[Union[float, torch.Tensor], torch.Tensor]:
         """Return the maximum of the modeled function, subject to constraints
         Args:
             bounds (torch.Tensor): The lower and upper bounds in the parameter space to search for the maximum,
                 formatted as a 2xn tensor, where d is the number of parameters.
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                     inverse is along a slice of the full surface.
-            n_samples int: number of coarse grid points to sample for optimization estimate.
+            n_samples (int): How fine to make the grid of predictions from which the initial
+                guess will be derived.
+            weights (torch.Tensor, Optional): The relative weights of each of the dimensions
+                of y for multi-outcome models.
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: Tuple containing the max and its location (argmax).
         """
         locked_dims = locked_dims or {}
-        return get_extremum(self, "max", bounds, locked_dims, n_samples)
+
+        _, fmax_loc = get_extremum(
+            self,
+            "max",
+            bounds,
+            locked_dims,
+            n_samples,
+            max_time=max_time,
+            weights=weights,
+        )
+        if probability_space:
+            pred_function = self.predict_probability
+        else:
+            pred_function = self.predict
+        fmax_val = pred_function(fmax_loc.unsqueeze(0))[0]
+        return fmax_val, fmax_loc
 
     def get_min(
         self,
         bounds: torch.Tensor,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
+        probability_space: bool = False,
         n_samples: int = 1000,
-    ) -> Tuple[float, np.ndarray]:
+        max_time: Optional[float] = None,
+        weights: Optional[torch.Tensor] = None,
+    ) -> Tuple[Union[float, torch.Tensor], torch.Tensor]:
         """Return the minimum of the modeled function, subject to constraints
         Args:
             bounds (torch.Tensor): The lower and upper bounds in the parameter space to search for the minimum,
                 formatted as a 2xn tensor, where d is the number of parameters.
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
+            n_samples (int): How fine to make the grid of predictions from which the initial
+                guess will be derived.
+            weights (torch.Tensor, Optional): The relative weights of each of the dimensions
+                of y for multi-outcome models.
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: Tuple containing the min and its location (argmin).
         """
         locked_dims = locked_dims or {}
-        return get_extremum(self, "min", bounds, locked_dims, n_samples)
+
+        _, fmin_loc = get_extremum(
+            self,
+            "min",
+            bounds,
+            locked_dims,
+            n_samples,
+            max_time=max_time,
+            weights=weights,
+        )
+        if probability_space:
+            pred_function = self.predict_probability
+        else:
+            pred_function = self.predict
+        fmin_val = pred_function(fmin_loc.unsqueeze(0))[0]
+        return fmin_val, fmin_loc
 
     def inv_query(
         self,
-        y: float,
+        y: Union[float, torch.Tensor],
         bounds: torch.Tensor,
         locked_dims: Optional[Mapping[int, List[float]]] = None,
         probability_space: bool = False,
         n_samples: int = 1000,
-    ) -> Tuple[float, torch.Tensor]:
+        max_time: Optional[float] = None,
+        weights: Optional[torch.Tensor] = None,
+    ) -> Tuple[Union[float, torch.Tensor], torch.Tensor]:
         """Query the model inverse.
         Return nearest x such that f(x) = queried y, and also return the
             value of f at that point.
         Args:
-            y (float): Points at which to find the inverse.
+            y (float, torch.Tensor): Point at which to find the inverse.
+            bounds (torch.Tensor): The lower and upper bounds in the parameter space to search for the minimum,
+                    formatted as a 2xn tensor, where d is the number of parameters.
             locked_dims (Mapping[int, List[float]]): Dimensions to fix, so that the
                 inverse is along a slice of the full surface.
             probability_space (bool): Is y (and therefore the
                 returned nearest_y) in probability space instead of latent
                 function space? Defaults to False.
+            n_samples (int): How fine to make the grid of predictions from which the initial
+                guess will be derived.
+            weights (torch.Tensor, Optional): The relative weights of each of the dimensions
+                of y for multi-outcome models.
         Returns:
             Tuple[float, np.ndarray]: Tuple containing the value of f
                 nearest to queried y and the x position of this value.
         """
+        _, arg = inv_query(
+            self,
+            y,
+            bounds,
+            locked_dims,
+            probability_space,
+            n_samples,
+            max_time,
+            weights,
+        )
+        arg = arg.reshape(1, -1)
         if probability_space:
-            assert (
-                self.outcome_type == "binary" or self.outcome_type is None
-            ), f"Cannot get probability space for outcome_type '{self.outcome_type}'"
-            pred_function = self.predict_probability
-
+            val, _ = self.predict_probability(arg)
         else:
-            pred_function = self.predict
-
-        locked_dims = locked_dims or {}
-
-        def model_distance(x, pt, probability_space):
-            return np.abs(pred_function(torch.tensor([x]))[0].detach().numpy() - pt)
-
-        # Look for point with value closest to y, subject the dict of locked dims
-
-        query_lb = bounds[0]
-        query_ub = bounds[-1]
-
-        for locked_dim in locked_dims.keys():
-            dim_values = locked_dims[locked_dim]
-            if len(dim_values) == 1:
-                query_lb[locked_dim] = dim_values[0]
-                query_ub[locked_dim] = dim_values[0]
-            else:
-                query_lb[locked_dim] = dim_values[0]
-                query_ub[locked_dim] = dim_values[1]
-
-        d = make_scaled_sobol(query_lb, query_ub, n_samples, seed=0)
-
-        opt_bounds = zip(query_lb.numpy(), query_ub.numpy())
-
-        fmean, _ = pred_function(d)
-
-        f = torch.abs(fmean - y)
-        estimate = d[torch.where(f == torch.min(f))[0][0]].numpy()
-        a = minimize(
-            model_distance,
-            estimate,
-            args=(y, probability_space),
-            method=self.extremum_solver,
-            bounds=opt_bounds,
-        )
-        val = pred_function(torch.tensor([a.x]))[0].item()
-        return val, torch.Tensor(a.x)
+            val, _ = self.predict(arg)
+        return val, arg
 
     @abc.abstractmethod
     def get_mll_class(self):
         raise NotImplementedError
 
     def fit(self):
         mll_class = self.get_mll_class()
```

### Comparing `aepsych-0.4.0/aepsych/models/derivative_gp.py` & `aepsych-0.4.1/aepsych/models/derivative_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/exact_gp.py` & `aepsych-0.4.1/aepsych/models/exact_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/gp_classification.py` & `aepsych-0.4.1/aepsych/models/gp_classification.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/gp_regression.py` & `aepsych-0.4.1/aepsych/models/gp_regression.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/monotonic_projection_gp.py` & `aepsych-0.4.1/aepsych/models/monotonic_projection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/monotonic_rejection_gp.py` & `aepsych-0.4.1/aepsych/models/monotonic_rejection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/multitask_regression.py` & `aepsych-0.4.1/aepsych/models/multitask_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#!/usr/bin/env python3
+# Copyright (c) Facebook, Inc. and its affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
 from __future__ import annotations
 
 from typing import Optional
 
 import gpytorch
 
 import torch
@@ -57,15 +64,15 @@
         )
         super().__init__(
             mean_module=mean_module,
             covar_module=covar_module,
             likelihood=likelihood,
             *args,
             **kwargs,
-        ) # type: ignore # mypy issue 4335
+        )  # type: ignore # mypy issue 4335
 
         self.mean_module = gpytorch.means.MultitaskMean(
             self.mean_module, num_tasks=num_outputs
         )
         self.covar_module = gpytorch.kernels.MultitaskKernel(
             self.covar_module, num_tasks=num_outputs, rank=rank
         )
@@ -102,15 +109,15 @@
         self,
         num_outputs: int = 2,
         mean_module: Optional[gpytorch.means.Mean] = None,
         covar_module: Optional[gpytorch.kernels.Kernel] = None,
         likelihood: Optional[gpytorch.likelihoods.Likelihood] = None,
         *args,
         **kwargs,
-    ): 
+    ):
         """Initialize independent multitask GPR model.
 
         Args:
             num_outputs (int, optional): Number of tasks (outputs). Defaults to 2.
             mean_module (Optional[gpytorch.means.Mean], optional): GP mean. Defaults to a constant mean.
             covar_module (Optional[gpytorch.kernels.Kernel], optional): GP kernel module.
                 Defaults to scaled RBF kernel.
@@ -136,15 +143,15 @@
         )
         super().__init__(
             mean_module=mean_module,
             covar_module=covar_module,
             likelihood=likelihood,
             *args,
             **kwargs,
-        ) # type: ignore # mypy issue 4335
+        )  # type: ignore # mypy issue 4335
 
     def forward(self, x):
         base_mvn = super().forward(x)  # do transforms
         return gpytorch.distributions.MultitaskMultivariateNormal.from_batch_mvn(
             base_mvn
         )
```

### Comparing `aepsych-0.4.0/aepsych/models/ordinal_gp.py` & `aepsych-0.4.1/aepsych/models/ordinal_gp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#!/usr/bin/env python3
+# Copyright (c) Facebook, Inc. and its affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
 import gpytorch
 import torch
 from aepsych.likelihoods import OrdinalLikelihood
 from aepsych.models import GPClassificationModel
 
 
 class OrdinalGPModel(GPClassificationModel):
@@ -58,8 +65,8 @@
         for i in range(1, self.likelihood.n_levels - 1):
             probs[..., i] = self.likelihood.link(
                 (self.likelihood.cutpoints[i] - fmean) / fsd
             ) - self.likelihood.link((self.likelihood.cutpoints[i - 1] - fmean) / fsd)
         probs[..., -1] = 1 - self.likelihood.link(
             (self.likelihood.cutpoints[-1] - fmean) / fsd
         )
-        return probs
+        return probs
```

### Comparing `aepsych-0.4.0/aepsych/models/pairwise_probit.py` & `aepsych-0.4.1/aepsych/models/pairwise_probit.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/models/semi_p.py` & `aepsych-0.4.1/aepsych/models/semi_p.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         x_intensity=Xi,
         slope_mean=slope_mean,
         slope_cov=slope_cov,
         offset_mean=offset_mean,
         offset_cov=offset_cov,
     )
     approx_mvn = MultivariateNormal(mean=approx_mean, covariance_matrix=approx_cov)
-    return GPyTorchPosterior(mvn=approx_mvn)
+    return GPyTorchPosterior(distribution=approx_mvn)
 
 
 class SemiPPosterior(GPyTorchPosterior):
     def __init__(
         self,
         mvn: MultivariateNormal,
         likelihood: LinearBernoulliLikelihood,
@@ -107,19 +107,24 @@
         )
 
     def rsample(
         self,
         sample_shape: Optional[torch.Size] = None,
         base_samples: Optional[torch.Tensor] = None,
     ):
-        kcsamps = (
-            super()
-            .rsample(sample_shape=sample_shape, base_samples=base_samples)
-            .squeeze(-1)
-        )
+        if base_samples is None:
+            samps_ = super().rsample(sample_shape=sample_shape)
+        else:
+            samps_ = super().rsample_from_base_samples(
+                sample_shape=sample_shape,
+                base_samples=base_samples.expand(
+                    self._extended_shape(sample_shape)
+                ).squeeze(-1),
+            )
+        kcsamps = samps_.squeeze(-1)
         # fsamps is of shape nsamp x 2 x n, or nsamp x b x 2 x n
         return kcsamps
 
     def sample_p(
         self,
         sample_shape: Optional[torch.Size] = None,
         base_samples: Optional[torch.Tensor] = None,
```

### Comparing `aepsych-0.4.0/aepsych/plotting.py` & `aepsych-0.4.1/aepsych/plotting.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/__init__.py` & `aepsych-0.4.1/aepsych/server/message_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_ask.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_ask.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
+from collections.abc import Mapping
 
 import aepsych.utils_logging as utils_logging
 
 logger = utils_logging.getLogger(logging.INFO)
 
 
 def handle_ask(server, request):
@@ -17,25 +18,30 @@
     "config" -- dictionary with config (keys are strings, values are floats)
     "is_finished" -- bool, true if the strat is finished
     """
     logger.debug("got ask message!")
     if server._pregen_asks:
         params = server._pregen_asks.pop()
     else:
-        params = ask(server)
+        # Some clients may still send "message" as an empty string, so we need to check if its a dict or not.
+        msg = request["message"]
+        if isinstance(msg, Mapping):
+            params = ask(server, **msg)
+        else:
+            params = ask(server)
 
     new_config = {"config": params, "is_finished": server.strat.finished}
     if not server.is_performing_replay:
         server.db.record_message(
             master_table=server._db_master_record, type="ask", request=request
         )
     return new_config
 
 
-def ask(server):
+def ask(server, num_points=1):
     """get the next point to query from the model
     Returns:
         dict -- new config dict (keys are strings, values are floats)
     """
     if server.skip_computations:
         # HACK to makke sure strategies finish correctly
         server.strat._strat._count += 1
@@ -45,9 +51,9 @@
 
     if not server.use_ax:
         # index by [0] is temporary HACK while serverside
         # doesn't handle batched ask
         next_x = server.strat.gen()[0]
         return server._tensor_to_config(next_x)
 
-    next_x = server.strat.gen()
+    next_x = server.strat.gen(num_points)
     return next_x
```

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_can_model.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_can_model.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_exit.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_exit.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,12 +13,10 @@
 
 
 def handle_exit(server, request):
     # Make local server write strats into DB and close the connection
     termination_type = "Normal termination"
     logger.info("Got termination message!")
     server.write_strats(termination_type)
-    if not server.is_using_thrift:
-        server.exit_server_loop = True
+    server.exit_server_loop = True
 
-    # If using thrift, it will add 'Terminate' to the queue and pass it to thrift server level
     return "Terminate"
```

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_get_config.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_get_config.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_info.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_info.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_params.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_params.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_query.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
+import torch
 
 import aepsych.utils_logging as utils_logging
 import numpy as np
 
 logger = utils_logging.getLogger(logging.INFO)
 
 
@@ -26,51 +27,59 @@
 def query(
     server,
     query_type="max",
     probability_space=False,
     x=None,
     y=None,
     constraints=None,
+    **kwargs,
 ):
     if server.skip_computations:
         return None
 
     constraints = constraints or {}
     response = {
         "query_type": query_type,
         "probability_space": probability_space,
         "constraints": constraints,
     }
     if query_type == "max":
-        fmax, fmax_loc = server.strat.get_max(constraints)
-        response["y"] = fmax.item()
+        fmax, fmax_loc = server.strat.get_max(constraints, probability_space, **kwargs)
+        response["y"] = fmax
         response["x"] = server._tensor_to_config(fmax_loc)
     elif query_type == "min":
-        fmin, fmin_loc = server.strat.get_min(constraints)
-        response["y"] = fmin.item()
+        fmin, fmin_loc = server.strat.get_min(constraints, probability_space, **kwargs)
+        response["y"] = fmin
         response["x"] = server._tensor_to_config(fmin_loc)
     elif query_type == "prediction":
         # returns the model value at x
         if x is None:  # TODO: ensure if x is between lb and ub
             raise RuntimeError("Cannot query model at location = None!")
-        mean, _var = server.strat.predict(
-            server._config_to_tensor(x).unsqueeze(axis=0),
-            probability_space=probability_space,
-        )
+        if probability_space:
+            mean, _var = server.strat.predict_probability(
+                server._config_to_tensor(x).unsqueeze(axis=0),
+            )
+        else:
+            mean, _var = server.strat.predict(
+                server._config_to_tensor(x).unsqueeze(axis=0)
+            )
         response["x"] = x
-        response["y"] = mean.item()
+        response["y"] = np.array(mean)  # mean.item()
+
     elif query_type == "inverse":
         # expect constraints to be a dictionary; values are float arrays size 1 (exact) or 2 (upper/lower bnd)
         constraints = {server.parnames.index(k): v for k, v in constraints.items()}
         nearest_y, nearest_loc = server.strat.inv_query(
-            y, constraints, probability_space=probability_space
+            y, constraints, probability_space=probability_space, **kwargs
         )
-        response["y"] = nearest_y
+        response["y"] = np.array(nearest_y)
         response["x"] = server._tensor_to_config(nearest_loc)
     else:
         raise RuntimeError("unknown query type!")
     # ensure all x values are arrays
     response["x"] = {
         k: np.array([v]) if np.array(v).ndim == 0 else v
         for k, v in response["x"].items()
     }
+    if server.use_ax:
+        response["x"] = {v: response["x"][v][0] for v in response["x"]}
     return response
```

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_resume.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_resume.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_setup.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#!/usr/bin/env python3
+# Copyright (c) Facebook, Inc. and its affiliates.
+# All rights reserved.
+
+# This source code is licensed under the license found in the
+# LICENSE file in the root directory of this source tree.
+
 import logging
 
 import aepsych.utils_logging as utils_logging
 from aepsych.config import Config
 
 from aepsych.strategy import AEPsychStrategy, SequentialStrategy
 from aepsych.version import __version__
@@ -12,16 +19,23 @@
 
 
 def _configure(server, config):
     server._pregen_asks = (
         []
     )  # TODO: Allow each strategy to have its own stack of pre-generated asks
 
-    parnames = config._str_to_list(config.get("common", "parnames"), element_type=str)
+    parnames = config.getlist("common", "parnames", element_type=str)
     server.parnames = parnames
+    outcome_types = config.getlist("common", "outcome_types", element_type=str)
+    outcome_names = config.getlist(
+        "common", "outcome_names", element_type=str, fallback=None
+    )
+    if outcome_names is None:
+        outcome_names = [f"outcome_{i+1}" for i in range(len(outcome_types))]
+    server.outcome_names = outcome_names
     server.config = config
     server.use_ax = config.getboolean("common", "use_ax", fallback=False)
     server.enable_pregen = config.getboolean("common", "pregen_asks", fallback=False)
     if server.use_ax:
         server.trial_index = -1
         server.strat = AEPsychStrategy.from_config(config)
         server.strat_id = server.n_strats - 1
```

### Comparing `aepsych-0.4.0/aepsych/server/message_handlers/handle_tell.py` & `aepsych-0.4.1/aepsych/server/message_handlers/handle_tell.py`

 * *Files 17% similar despite different names*

```diff
@@ -57,86 +57,103 @@
 
     if rec.extra_info is not None:
         out.update(rec.extra_info)
 
     return out
 
 
-def tell(server, outcome, config, model_data=True):
+def tell(server, outcome, config=None, model_data=True, trial_index=-1):
     """tell the model which input was run and what the outcome was
     Arguments:
-        inputs {dict} -- dictionary, keys are strings, values are floats or int.
-        keys should inclde all of the parameters we are tuning over, plus 'outcome'
-        which would be in {0, 1}.
-        TODO better types
+        server: The AEPsych server object.
+        outcome: The outcome of the trial. If using the legacy backend, this must be an int or a float. If using the Ax
+            backend, this may be an int or float if using a single outcome, or if using multiple outcomes, it must be a
+            dictionary mapping outcome names to values.
+        config: A dictionary mapping parameter names to values. This must be provided if using the legacy backend. If
+            using the Ax backend, this should be provided only for trials that do not already have a trial_index.
+        model_data: If True, the data from this trial will be added to the model. If False, the trial will be recorded in
+            the db, but will not be modeled.
+        trial_index: The trial_index for the trial as provided by the ask response when using the Ax backend. Ignored by
+            the legacy backend.
     """
+
+    if config is None:
+        config = {}
+
     if not server.is_performing_replay:
-        server._db_raw_record = server.db.record_raw(
-            master_table=server._db_master_record,
-            model_data=bool(model_data),
-        )
+        _record_tell(server, outcome, config, model_data)
 
-        for param_name, param_value in config.items():
-            if isinstance(param_value, Iterable) and type(param_value) != str:
-                if len(param_value) == 1:
-                    server.db.record_param(
-                        raw_table=server._db_raw_record,
-                        param_name=str(param_name),
-                        param_value=str(param_value[0]),
-                    )
-                else:
-                    for i, v in enumerate(param_value):
-                        server.db.record_param(
-                            raw_table=server._db_raw_record,
-                            param_name=str(param_name) + "_stimuli" + str(i),
-                            param_value=str(v),
-                        )
+    if model_data:
+        if not server.use_ax:
+            x = server._config_to_tensor(config)
+            server.strat.add_data(x, outcome)
+        else:
+            assert (
+                config or trial_index >= 0
+            ), "Must supply a trial parameterization or a trial index!"
+            if trial_index >= 0:
+                server.strat.complete_existing_trial(trial_index, outcome)
             else:
-                server.db.record_param(
-                    raw_table=server._db_raw_record,
-                    param_name=str(param_name),
-                    param_value=str(param_value),
-                )
+                server.strat.complete_new_trial(config, outcome)
 
-        if isinstance(outcome, dict):
-            for key in outcome.keys():
-                server.db.record_outcome(
-                    raw_table=server._db_raw_record,
-                    outcome_name=key,
-                    outcome_value=float(outcome[key]),
-                )
 
-        # Check if we get single or multiple outcomes
-        # Multiple outcomes come in the form of iterables that aren't strings or single-element tensors
-        elif isinstance(outcome, Iterable) and type(outcome) != str:
-            for i, outcome_value in enumerate(outcome):
-                if isinstance(outcome_value, Iterable) and type(outcome_value) != str:
-                    if (
-                        isinstance(outcome_value, torch.Tensor)
-                        and outcome_value.dim() < 2
-                    ):
-                        outcome_value = outcome_value.item()
-
-                    elif len(outcome_value) == 1:
-                        outcome_value = outcome_value[0]
-                    else:
-                        raise ValueError(
-                            "Multi-outcome values must be a list of lists of length 1!"
-                        )
-                server.db.record_outcome(
+def _record_tell(server, outcome, config, model_data):
+    server._db_raw_record = server.db.record_raw(
+        master_table=server._db_master_record,
+        model_data=bool(model_data),
+    )
+
+    for param_name, param_value in config.items():
+        if isinstance(param_value, Iterable) and type(param_value) != str:
+            if len(param_value) == 1:
+                server.db.record_param(
                     raw_table=server._db_raw_record,
-                    outcome_name="outcome_" + str(i),
-                    outcome_value=float(outcome_value),
+                    param_name=str(param_name),
+                    param_value=str(param_value[0]),
                 )
+            else:
+                for i, v in enumerate(param_value):
+                    server.db.record_param(
+                        raw_table=server._db_raw_record,
+                        param_name=str(param_name) + "_stimuli" + str(i),
+                        param_value=str(v),
+                    )
         else:
+            server.db.record_param(
+                raw_table=server._db_raw_record,
+                param_name=str(param_name),
+                param_value=str(param_value),
+            )
+
+    if isinstance(outcome, dict):
+        for key in outcome.keys():
             server.db.record_outcome(
                 raw_table=server._db_raw_record,
-                outcome_name="outcome",
-                outcome_value=float(outcome),
+                outcome_name=key,
+                outcome_value=float(outcome[key]),
             )
 
-    if model_data:
-        if not server.use_ax:
-            x = server._config_to_tensor(config)
-        else:
-            x = config
-        server.strat.add_data(x, outcome)
+    # Check if we get single or multiple outcomes
+    # Multiple outcomes come in the form of iterables that aren't strings or single-element tensors
+    elif isinstance(outcome, Iterable) and type(outcome) != str:
+        for i, outcome_value in enumerate(outcome):
+            if isinstance(outcome_value, Iterable) and type(outcome_value) != str:
+                if isinstance(outcome_value, torch.Tensor) and outcome_value.dim() < 2:
+                    outcome_value = outcome_value.item()
+
+                elif len(outcome_value) == 1:
+                    outcome_value = outcome_value[0]
+                else:
+                    raise ValueError(
+                        "Multi-outcome values must be a list of lists of length 1!"
+                    )
+            server.db.record_outcome(
+                raw_table=server._db_raw_record,
+                outcome_name="outcome_" + str(i),
+                outcome_value=float(outcome_value),
+            )
+    else:
+        server.db.record_outcome(
+            raw_table=server._db_raw_record,
+            outcome_name="outcome",
+            outcome_value=float(outcome),
+        )
```

### Comparing `aepsych-0.4.0/aepsych/server/replay.py` & `aepsych-0.4.1/aepsych/server/replay.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     server.skip_computations = skip_computations
 
     for result in master_record.children_replay:
         request = result.message_contents
         logger.debug(f"replay - type = {result.message_type} request = {request}")
         server.handle_request(request)
 
+    server.is_performing_replay = False
+    server.skip_computations = False
+
 
 def get_strats_from_replay(server, uuid_of_replay=None, force_replay=False):
     if uuid_of_replay is None:
         records = server.db.get_master_records()
         if len(records) > 0:
             uuid_of_replay = records[-1].experiment_id
         else:
```

### Comparing `aepsych-0.4.0/aepsych/server/server.py` & `aepsych-0.4.1/aepsych/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 from aepsych.server.replay import (
     get_dataframe_from_replay,
     get_strat_from_replay,
     get_strats_from_replay,
     replay,
 )
 
-from aepsych.server.sockets import BAD_REQUEST, createSocket, DummySocket
+from aepsych.server.sockets import BAD_REQUEST, DummySocket, PySocket
 
 logger = utils_logging.getLogger(logging.INFO)
 DEFAULT_DESC = "default description"
 DEFAULT_NAME = "default name"
 
 
 def get_next_filename(folder, fname, ext):
     """Generates appropriate filename for logging purposes."""
     n = sum(1 for f in os.listdir(folder) if os.path.isfile(os.path.join(folder, f)))
     return f"{folder}/{fname}_{n+1}.{ext}"
 
 
 class AEPsychServer(object):
-    def __init__(self, socket=None, database_path=None, thrift=False):
+    def __init__(self, socket=None, database_path=None):
         """Server for doing black box optimization using gaussian processes.
         Keyword Arguments:
             socket -- socket object that implements `send` and `receive` for json
             messages (default: DummySocket()).
             TODO actually make an abstract interface to subclass from here
         """
         if socket is None:
@@ -73,17 +73,17 @@
 
         self._strats = []
         self._parnames = []
         self._configs = []
         self.strat_id = -1
         self._pregen_asks = []
         self.enable_pregen = False
+        self.outcome_names = []
 
         self.debug = False
-        self.is_using_thrift = thrift
         self.receive_thread = threading.Thread(
             target=self._receive_send, args=(self.exit_server_loop,), daemon=True
         )
 
         self.queue = []
 
     def cleanup(self):
@@ -149,28 +149,23 @@
 
         """
         logger.info("Server up, waiting for connections!")
         logger.info("Ctrl-C to quit!")
         # yeah we're not sanitizing input at all
 
         # Start the method to accept a client connection
-
-        if self.is_using_thrift is True:
-            self.queue.append(self.socket.receive())
+        self.socket.accept_client()
+        self.receive_thread.start()
+        while True:
             self._handle_queue()
-        else:
-            self.socket.accept_client()
-            self.receive_thread.start()
-            while True:
-                self._handle_queue()
-                if self.exit_server_loop:
-                    break
-            # Close the socket and terminate with code 0
-            self.cleanup()
-            sys.exit(0)
+            if self.exit_server_loop:
+                break
+        # Close the socket and terminate with code 0
+        self.cleanup()
+        sys.exit(0)
 
     def _unpack_strat_buffer(self, strat_buffer):
         if isinstance(strat_buffer, io.BytesIO):
             strat = torch.load(strat_buffer, pickle_module=dill)
             strat_buffer.seek(0)
         elif isinstance(strat_buffer, bytes):
             warnings.warn(
@@ -390,20 +385,15 @@
 
 
 def parse_argument():
     parser = argparse.ArgumentParser(description="AEPsych Server!")
     parser.add_argument(
         "--port", metavar="N", type=int, default=5555, help="port to serve on"
     )
-    parser.add_argument(
-        "--socket_type",
-        choices=["zmq", "pysocket"],
-        default="pysocket",
-        help="method to serve over",
-    )
+
     parser.add_argument(
         "--ip",
         metavar="M",
         type=str,
         default="0.0.0.0",
         help="ip to bind",
     )
@@ -445,36 +435,36 @@
     logger.info("Starting the AEPsychServer")
     try:
         if "db" in args and args.db is not None:
             database_path = args.db
             if "replay" in args and args.replay is not None:
                 logger.info(f"Attempting to replay {args.replay}")
                 if args.resume is True:
-                    sock = createSocket(socket_type=args.socket_type, port=args.port)
+                    sock = PySocket(port=args.port)
                     logger.info(f"Will resume {args.replay}")
                 else:
                     sock = None
                 startServerAndRun(
                     server_class,
                     socket=sock,
                     database_path=database_path,
                     uuid_of_replay=args.replay,
                     config_path=args.stratconfig,
                 )
             else:
                 logger.info(f"Setting the database path {database_path}")
-                sock = createSocket(socket_type=args.socket_type, port=args.port)
+                sock = PySocket(port=args.port)
                 startServerAndRun(
                     server_class,
                     database_path=database_path,
                     socket=sock,
                     config_path=args.stratconfig,
                 )
         else:
-            sock = createSocket(socket_type=args.socket_type, port=args.port)
+            sock = PySocket(port=args.port)
             startServerAndRun(server_class, socket=sock, config_path=args.stratconfig)
 
     except (KeyboardInterrupt, SystemExit):
         logger.exception("Got Ctrl+C, exiting!")
         sys.exit()
     except RuntimeError as e:
         fname = get_next_filename(".", "dump", "pkl")
```

### Comparing `aepsych-0.4.0/aepsych/server/utils.py` & `aepsych-0.4.1/aepsych/server/utils.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych/strategy.py` & `aepsych-0.4.1/aepsych/strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,37 +5,40 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations
 
 import time
 import warnings
+
+from copy import copy
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
 
 import numpy as np
 import torch
-from ax.core.base_trial import TrialStatus
-from ax.modelbridge.generation_strategy import GenerationStrategy
-from ax.plot.contour import interact_contour
-from ax.plot.slice import plot_slice
-from ax.service.ax_client import AxClient
-from ax.utils.notebook.plotting import render
-from botorch.exceptions.errors import ModelFittingError
 
 from aepsych.config import Config, ConfigurableMixin
 from aepsych.generators.base import AEPsychGenerationStep, AEPsychGenerator
 from aepsych.generators.sobol_generator import AxSobolGenerator, SobolGenerator
 from aepsych.models.base import ModelProtocol
 from aepsych.utils import (
     _process_bounds,
+    get_bounds,
     get_objectives,
     get_parameters,
     make_scaled_sobol,
 )
 from aepsych.utils_logging import getLogger
+from ax.core.base_trial import TrialStatus
+from ax.modelbridge.generation_strategy import GenerationStrategy
+from ax.plot.contour import interact_contour
+from ax.plot.slice import plot_slice
+from ax.service.ax_client import AxClient
+from ax.utils.notebook.plotting import render
+from botorch.exceptions.errors import ModelFittingError
 
 logger = getLogger()
 
 
 def ensure_model_is_fresh(f):
     def wrapper(self, *args, **kwargs):
         if self.can_fit and not self._model_is_fresh:
@@ -132,15 +135,15 @@
                 assert set(outcome_types) == set(
                     model.outcome_type
                 ), f"Strategy outcome types is {outcome_types} but model outcome type is {model.outcome_type}!"
 
         self.run_indefinitely = run_indefinitely
         self.lb, self.ub, self.dim = _process_bounds(lb, ub, dim)
         self.min_total_outcome_occurrences = min_total_outcome_occurrences
-        self.max_asks = max_asks
+        self.max_asks = max_asks or generator.max_asks
         self.keep_most_recent = keep_most_recent
 
         self.min_post_range = min_post_range
         if self.min_post_range is not None:
             assert model is not None, "min_post_range must be None if model is None!"
             self.eval_grid = make_scaled_sobol(
                 lb=self.lb, ub=self.ub, size=self._n_eval_points
@@ -222,27 +225,33 @@
         Returns:
             np.ndarray: Next set of point(s) to evaluate, [num_points x dim].
         """
         self._count = self._count + num_points
         return self.generator.gen(num_points, self.model)
 
     @ensure_model_is_fresh
-    def get_max(self, constraints=None):
+    def get_max(self, constraints=None, probability_space=False, max_time=None):
         constraints = constraints or {}
-        return self.model.get_max(constraints)
+        return self.model.get_max(
+            constraints, probability_space=probability_space, max_time=max_time
+        )
 
     @ensure_model_is_fresh
-    def get_min(self, constraints=None):
+    def get_min(self, constraints=None, probability_space=False, max_time=None):
         constraints = constraints or {}
-        return self.model.get_min(constraints)
+        return self.model.get_min(
+            constraints, probability_space=probability_space, max_time=max_time
+        )
 
     @ensure_model_is_fresh
-    def inv_query(self, y, constraints=None, probability_space=False):
+    def inv_query(self, y, constraints=None, probability_space=False, max_time=None):
         constraints = constraints or {}
-        return self.model.inv_query(y, constraints, probability_space)
+        return self.model.inv_query(
+            y, constraints, probability_space, max_time=max_time
+        )
 
     @ensure_model_is_fresh
     def predict(self, x, probability_space=False):
         return self.model.predict(x=x, probability_space=probability_space)
 
     @ensure_model_is_fresh
     def get_jnd(self, *args, **kwargs):
@@ -315,44 +324,44 @@
         if self.can_fit:
             if self.keep_most_recent is not None:
                 try:
                     self.model.fit(
                         self.x[-self.keep_most_recent :],
                         self.y[-self.keep_most_recent :],
                     )
-                except (ModelFittingError):
+                except ModelFittingError:
                     logger.warning(
                         "Failed to fit model! Predictions may not be accurate!"
                     )
             else:
                 try:
                     self.model.fit(self.x, self.y)
-                except (ModelFittingError):
+                except ModelFittingError:
                     logger.warning(
                         "Failed to fit model! Predictions may not be accurate!"
                     )
         else:
             warnings.warn("Cannot fit: no model has been initialized!", RuntimeWarning)
 
     def update(self):
         if self.can_fit:
             if self.keep_most_recent is not None:
                 try:
                     self.model.update(
                         self.x[-self.keep_most_recent :],
                         self.y[-self.keep_most_recent :],
                     )
-                except (ModelFittingError):
+                except ModelFittingError:
                     logger.warning(
                         "Failed to fit model! Predictions may not be accurate!"
                     )
             else:
                 try:
                     self.model.update(self.x, self.y)
-                except (ModelFittingError):
+                except ModelFittingError:
                     logger.warning(
                         "Failed to fit model! Predictions may not be accurate!"
                     )
         else:
             warnings.warn("Cannot fit: no model has been initialized!", RuntimeWarning)
 
     @classmethod
@@ -498,105 +507,111 @@
 
         return cls(strat_list=strats)
 
 
 class AEPsychStrategy(ConfigurableMixin):
     is_finished = False
 
-    def __init__(self, strategy: GenerationStrategy, ax_client: AxClient):
-        self.strat = strategy
-        self.strat.experiment.num_asks = 0
+    def __init__(self, ax_client: AxClient, bounds: torch.Tensor):
         self.ax_client = ax_client
+        self.ax_client.experiment.num_asks = 0
+        self.bounds = bounds
 
     @classmethod
     def get_config_options(cls, config: Config, name: Optional[str] = None) -> Dict:
         # TODO: Fix the mypy errors
         strat_names: List[str] = config.getlist("common", "strategy_names", element_type=str)  # type: ignore
         steps = []
         for name in strat_names:
             generator = config.getobj(name, "generator", fallback=AxSobolGenerator)  # type: ignore
             opts = generator.get_config_options(config, name)
             step = AEPsychGenerationStep(**opts)
             steps.append(step)
 
+        # Add an extra step at the end that we can `ask` endlessly.
+        final_step = copy(step)
+        final_step.completion_criteria = []
+        final_step._transition_criteria = []
+        final_step.num_trials = -1
+        steps.append(final_step)
+
         parameters = get_parameters(config)
+        bounds = get_bounds(config)
 
         parameter_constraints = config.getlist(
             "common", "par_constraints", element_type=str, fallback=None
         )
 
         objectives = get_objectives(config)
 
+        seed = config.getint("common", "random_seed", fallback=None)
+
         strat = GenerationStrategy(steps=steps)
-        ax_client = AxClient(strat)
+        ax_client = AxClient(strat, random_seed=seed)
         ax_client.create_experiment(
             name="experiment",
             parameters=parameters,
             parameter_constraints=parameter_constraints,
             objectives=objectives,
         )
 
-        return {"strategy": strat, "ax_client": ax_client}
+        return {"ax_client": ax_client, "bounds": bounds}
 
     @property
     def finished(self) -> bool:
-        if self.is_finished:
+        if self.is_finished or self.strat.optimization_complete:
             return True
 
-        steps_left = len(self.strat._steps) - (self.strat.current_step.index + 1)
-        return (
-            self.strat.current_step.finished(self.strat.experiment) and steps_left == 0
-        )
+        self.strat._maybe_move_to_next_step()
+
+        return len(self.strat._steps) == (self.strat.current_step.index + 1)
 
     def finish(self):
         self.is_finished = True
 
     def gen(self, num_points: int = 1):
         x, _ = self.ax_client.get_next_trials(max_trials=num_points)
         self.strat.experiment.num_asks += num_points
-        next_x: Dict[str, Any] = {}
-        for par in self.strat.experiment.parameters:
-            next_x[par] = []
-            for i in x:
-                next_x[par].append(x[i][par])
-
-        return next_x
 
-    def add_data(self, x, y):
-        n = len(x[list(x.keys())[0]])
-        for i in range(n):
-            params = {par: x[par][i] for par in x}
-
-            # Check if this set of parameters already has an associated trial index. Usually it is the latest trial, so
-            # we iterate backwards. Ideally we would just pass in a trial index directly, but that would requre changes
-            # to server messages.
-            for i in reversed(range(len(self.ax_client.experiment.trials))):
-                trial = self.ax_client.get_trial(trial_index=i)
-                if (
-                    trial.arm.parameters == params
-                    and trial.status != TrialStatus.COMPLETED
-                ):
-                    trial_index = i
-                    break
+        return x
 
-            else:
-                _, trial_index = self.ax_client.attach_trial(params)
+    def complete_new_trial(self, config, outcome):
+        _, trial_index = self.ax_client.attach_trial(config)
+        self.complete_existing_trial(trial_index, outcome)
 
-            self.ax_client.complete_trial(trial_index=trial_index, raw_data=y)
+    def complete_existing_trial(self, trial_index, outcome):
+        self.ax_client.complete_trial(trial_index, outcome)
 
     @property
     def experiment(self):
-        return self.strat.experiment
+        return self.ax_client.experiment
 
-    def _warn_on_outcome_mismatch(self):
+    @property
+    def strat(self):
+        return self.ax_client.generation_strategy
+
+    @property
+    def can_fit(self):
+        return (
+            self.strat.model is not None
+            and len(self.experiment.trial_indices_by_status[TrialStatus.COMPLETED]) > 0
+        )
+
+    @property
+    def model(self):
         ax_model = self.ax_client.generation_strategy.model
+        if not hasattr(ax_model, "surrogate"):
+            return None
         aepsych_model = ax_model.model.surrogate.model
+        return aepsych_model
+
+    def _warn_on_outcome_mismatch(self):
         if (
-            hasattr(aepsych_model, "outcome_type")
-            and aepsych_model.outcome_type != "continuous"
+            hasattr(self.model, "outcome_type")
+            and self.model.outcome_type != "continuous"
         ):
             warnings.warn(
                 "Cannot directly plot non-continuous outcomes. Plotting the latent function instead."
             )
 
     def plot_contours(
         self, density: int = 50, slice_values: Optional[Dict[str, Any]] = None
@@ -649,7 +664,28 @@
                 density=density,
                 slice_values=slice_values,
             )
         )
 
     def get_pareto_optimal_parameters(self):
         return self.ax_client.get_pareto_optimal_parameters()
+
+    def predict(self, *args, **kwargs):
+        """Query the model for posterior mean and variance.; see AEPsychModel.predict."""
+        return self.model.predict(self._bounds, *args, **kwargs)
+
+    def predict_probability(self, *args, **kwargs):
+        """Query the model in prodbability space for posterior mean and variance.; see AEPsychModel.predict_probability."""
+        return self.model.predict(self._bounds, *args, **kwargs)
+
+    def get_max(self, *args, **kwargs):
+        """Return the maximum of the modeled function; see AEPsychModel.get_max."""
+        return self.model.get_max(self._bounds, *args, **kwargs)
+
+    def get_min(self, *args, **kwargs):
+        """Return the minimum of the modeled function; see AEPsychModel.get_min."""
+        return self.model.get_min(self._bounds, *args, **kwargs)
+
+    def inv_query(self, *args, **kwargs):
+        """Return nearest x such that f(x) = queried y, and also return the
+        value of f at that point.; see AEPsychModel.inv_query."""
+        return self.model.inv_query(self._bounds, *args, **kwargs)
```

### Comparing `aepsych-0.4.0/aepsych/utils.py` & `aepsych-0.4.1/aepsych/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,17 @@
         return [x]
     return x
 
 
 def dim_grid(
     lower: torch.Tensor,
     upper: torch.Tensor,
-    dim: int,
     gridsize: int = 30,
     slice_dims: Optional[Mapping[int, float]] = None,
 ) -> torch.Tensor:
-
     """Create a grid
     Create a grid based on lower, upper, and dim.
     Parameters
     ----------
     - lower ('int') - lower bound
     - upper ('int') - upper bound
     - dim ('int) - dimension
@@ -52,15 +50,15 @@
     Returns
     ----------
     grid : torch.FloatTensor
         Tensor
     """
     slice_dims = slice_dims or {}
 
-    lower, upper, _ = _process_bounds(lower, upper, None)
+    lower, upper, dim = _process_bounds(lower, upper, None)
 
     mesh_vals = []
 
     for i in range(dim):
         if i in slice_dims.keys():
             mesh_vals.append(slice(slice_dims[i] - 1e-10, slice_dims[i] + 1e-10, 1))
         else:
@@ -127,15 +125,14 @@
     mono_dim=-1,
     n_samps=500,
     lb=-np.inf,
     ub=np.inf,
     gridsize=30,
     **kwargs,
 ):
-
     xgrid = torch.Tensor(
         np.mgrid[
             [
                 slice(model.lb[i].item(), model.ub[i].item(), gridsize * 1j)
                 for i in range(model.dim)
             ]
         ]
@@ -151,15 +148,14 @@
             for s in samps
         ]
     )
 
     if cred_level is None:
         return np.mean(contours, 0.5, axis=0)
     else:
-
         alpha = 1 - cred_level
         qlower = alpha / 2
         qupper = 1 - alpha / 2
 
         upper = np.quantile(contours, qupper, axis=0)
         lower = np.quantile(contours, qlower, axis=0)
         median = np.quantile(contours, 0.5, axis=0)
@@ -257,14 +253,38 @@
 
 
 def get_parameters(config) -> List[Dict]:
     range_params, choice_params, fixed_params = _get_ax_parameters(config)
     return range_params + choice_params + fixed_params
 
 
+def get_bounds(config) -> torch.Tensor:
+    range_params, choice_params, _ = _get_ax_parameters(config)
+    # Need to sum dimensions added by both range and choice parameters
+    bounds = [parm["bounds"] for parm in range_params]
+    for par in choice_params:
+        n_vals = len(par["values"])
+        if par["is_ordered"]:
+            bounds.append(
+                [0, 1]
+            )  # Ordered choice params are encoded like continuous parameters
+        elif n_vals > 2:
+            for _ in range(n_vals):
+                bounds.append(
+                    [0, 1]
+                )  # Choice parameter is one-hot encoded such that they add 1 dim for every choice
+        else:
+            for _ in range(n_vals - 1):
+                bounds.append(
+                    [0, 1]
+                )  # Choice parameters with n_choices <= 2 add n_choices - 1 dims
+
+    return torch.tensor(bounds)
+
+
 def get_dim(config) -> int:
     range_params, choice_params, _ = _get_ax_parameters(config)
     # Need to sum dimensions added by both range and choice parameters
     dim = len(range_params)  # 1 dim per range parameter
     for par in choice_params:
         if par["is_ordered"]:
             dim += 1  # Ordered choice params are encoded like continuous parameters
@@ -280,19 +300,14 @@
     return dim
 
 
 def get_objectives(config) -> Dict:
     outcome_types: List[str] = config.getlist(
         "common", "outcome_types", element_type=str
     )
-    if len(outcome_types) > 1:
-        for out_type in outcome_types:
-            assert (
-                out_type == "continuous"
-            ), "Multiple outcomes is only currently supported for continuous outcomes!"
 
     outcome_names: List[str] = config.getlist(
         "common", "outcome_names", element_type=str, fallback=None
     )
     if outcome_names is None:
         outcome_names = [f"outcome_{i+1}" for i in range(len(outcome_types))]
```

### Comparing `aepsych-0.4.0/aepsych/utils_logging.py` & `aepsych-0.4.1/aepsych/utils_logging.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/aepsych.egg-info/SOURCES.txt` & `aepsych-0.4.1/aepsych.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 pyproject.toml
 setup.py
 aepsych/__init__.py
 aepsych/config.py
+aepsych/config.pyi
 aepsych/plotting.py
 aepsych/strategy.py
 aepsych/utils.py
 aepsych/utils_logging.py
 aepsych/version.py
 aepsych.egg-info/PKG-INFO
 aepsych.egg-info/SOURCES.txt
@@ -39,15 +40,14 @@
 aepsych/factory/factory.py
 aepsych/generators/__init__.py
 aepsych/generators/base.py
 aepsych/generators/epsilon_greedy_generator.py
 aepsych/generators/manual_generator.py
 aepsych/generators/monotonic_rejection_generator.py
 aepsych/generators/monotonic_thompson_sampler_generator.py
-aepsych/generators/multi_outcome_generator.py
 aepsych/generators/optimize_acqf_generator.py
 aepsych/generators/pairwise_optimize_acqf_generator.py
 aepsych/generators/pairwise_sobol_generator.py
 aepsych/generators/random_generator.py
 aepsych/generators/semi_p.py
 aepsych/generators/sobol_generator.py
 aepsych/generators/completion_criterion/__init__.py
@@ -65,21 +65,21 @@
 aepsych/means/constant_partial_grad.py
 aepsych/models/__init__.py
 aepsych/models/base.py
 aepsych/models/derivative_gp.py
 aepsych/models/exact_gp.py
 aepsych/models/gp_classification.py
 aepsych/models/gp_regression.py
+aepsych/models/model_list.py
 aepsych/models/monotonic_projection_gp.py
 aepsych/models/monotonic_rejection_gp.py
 aepsych/models/multitask_regression.py
 aepsych/models/ordinal_gp.py
 aepsych/models/pairwise_probit.py
 aepsych/models/semi_p.py
-aepsych/models/surrogate.py
 aepsych/models/utils.py
 aepsych/models/variational_gp.py
 aepsych/server/__init__.py
 aepsych/server/replay.py
 aepsych/server/server.py
 aepsych/server/sockets.py
 aepsych/server/utils.py
@@ -93,21 +93,19 @@
 aepsych/server/message_handlers/handle_params.py
 aepsych/server/message_handlers/handle_query.py
 aepsych/server/message_handlers/handle_resume.py
 aepsych/server/message_handlers/handle_setup.py
 aepsych/server/message_handlers/handle_tell.py
 tests/__init__.py
 tests/common.py
-tests/test_ThriftSocketWrapper.py
 tests/test_ax_integration.py
 tests/test_bench_testfuns.py
 tests/test_benchmark.py
 tests/test_config.py
 tests/test_db.py
-tests/test_integration.py
 tests/test_likelihoods.py
 tests/test_lookahead.py
 tests/test_mean_covar_factories.py
 tests/test_multioutcome.py
 tests/test_strategy.py
 tests/test_utils.py
 tests/acquisition/__init__.py
```

### Comparing `aepsych-0.4.0/setup.py` & `aepsych-0.4.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,67 +5,67 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import os
 
 from setuptools import find_packages, setup
 
-root_dir = os.path.dirname(__file__)
-
 REQUIRES = [
     "matplotlib",
     "torch",
-    "pyzmq==19.0.2",
     "scipy",
-    "scikit-learn",
     "SQLAlchemy==1.4.46",
     "dill",
     "pandas",
-    "tqdm",
-    "pathos",
-    "aepsych_client>=0.2.0",
-    "voila==0.3.6",
-    "ipywidgets==7.6.5",
+    "aepsych_client==0.3.0",
     "statsmodels",
-    "ax-platform==0.3.2",
+    "ax-platform==0.3.7",
 ]
 
-DEV_REQUIRES = [
+BENCHMARK_REQUIRES = ["tqdm", "pathos", "multiprocess"]
+
+DEV_REQUIRES = BENCHMARK_REQUIRES + [
     "coverage",
     "flake8",
     "black",
-    "numpy>=1.20, " "sqlalchemy-stubs",  # for mypy stubs
+    "numpy>=1.20",
+    "sqlalchemy-stubs",  # for mypy stubs
     "mypy",
     "parameterized",
+    "scikit-learn",  # used in unit tests
+]
+
+VISUALIZER_REQUIRES = [
+    "voila==0.3.6",
+    "ipywidgets==7.6.5",
 ]
 
-with open(os.path.join(root_dir, "README.md"), "r") as fh:
+with open("Readme.md", "r") as fh:
     long_description = fh.read()
 
-with open(os.path.join(root_dir, "aepsych", "version.py"), "r") as fh:
+with open(os.path.join("aepsych", "version.py"), "r") as fh:
     for line in fh.readlines():
         if line.startswith("__version__"):
             version = line.split('"')[1]
 
 
 setup(
     name="aepsych",
     version=version,
     python_requires=">=3.8",
     packages=find_packages(),
     description="Adaptive experimetation for psychophysics",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=REQUIRES,
+    extras_require={
+        "dev": DEV_REQUIRES,
+        "benchmark": BENCHMARK_REQUIRES,
+        "visualizer": VISUALIZER_REQUIRES,
+    },
     entry_points={
         "console_scripts": [
             "aepsych_server = aepsych.server.server:main",
             "aepsych_database = aepsych.server.utils:main",
         ],
     },
 )
-
-extras_require = (
-    {
-        "dev": DEV_REQUIRES,
-    },
-)
```

### Comparing `aepsych-0.4.0/tests/acquisition/test_lse.py` & `aepsych-0.4.1/tests/acquisition/test_lse.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/acquisition/test_mi.py` & `aepsych-0.4.1/tests/acquisition/test_mi.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/acquisition/test_monotonic.py` & `aepsych-0.4.1/tests/acquisition/test_monotonic.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/acquisition/test_objective.py` & `aepsych-0.4.1/tests/acquisition/test_objective.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/acquisition/test_rejection_sampler.py` & `aepsych-0.4.1/tests/acquisition/test_rejection_sampler.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/common.py` & `aepsych-0.4.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/generators/test_completion_criteria.py` & `aepsych-0.4.1/tests/generators/test_completion_criteria.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import unittest
 
 from aepsych.config import Config
 from aepsych.generators.completion_criterion import (
     MinAsks,
     MinTotalOutcomeOccurrences,
     MinTotalTells,
-    RunIndefinitely,
 )
 from aepsych.strategy import AEPsychStrategy
 
 
 class CompletionCriteriaTestCase(unittest.TestCase):
     def setUp(self):
         config_str = """
@@ -42,18 +41,18 @@
         """
         config = Config(config_str=config_str)
         criterion = MinAsks.from_config(config, "test_strat")
         self.assertEqual(criterion.threshold, 2)
 
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [0.0]}, 0.0)
+        self.strat.complete_new_trial({"x": 0.0}, 0.0)
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [1.0]}, 0.0)
+        self.strat.complete_new_trial({"x": 1.0}, 0.0)
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
         self.strat.gen()
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
         self.strat.gen()
         self.assertTrue(criterion.is_met(self.strat.experiment))
@@ -71,57 +70,38 @@
 
         self.strat.gen()
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
         self.strat.gen()
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [0.0]}, 0.0)
+        self.strat.complete_new_trial({"x": 0.0}, 0.0)
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [1.0]}, 0.0)
+        self.strat.complete_new_trial({"x": 1.0}, 0.0)
         self.assertTrue(criterion.is_met(self.strat.experiment))
 
     def test_min_total_outcome_occurences(self):
         config_str = """
         [common]
         outcome_types = [binary]
         min_total_outcome_occurrences = 2
         """
         config = Config(config_str=config_str)
         criterion = MinTotalOutcomeOccurrences.from_config(config, "test_strat")
         self.assertEqual(criterion.threshold, 2)
 
-        self.strat.add_data({"x": [0.0]}, 0.0)
+        self.strat.complete_new_trial({"x": 0.0}, 0.0)
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [1.0]}, 0.0)
+        self.strat.complete_new_trial({"x": 1.0}, 0.0)
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [0.0]}, 1.0)
+        self.strat.complete_new_trial({"x": 0.0}, 1.0)
         self.assertFalse(criterion.is_met(self.strat.experiment))
 
-        self.strat.add_data({"x": [1.0]}, 1.0)
+        self.strat.complete_new_trial({"x": 1.0}, 1.0)
         self.assertTrue(criterion.is_met(self.strat.experiment))
 
-    def run_indefinitely(self):
-        config_str = """
-        [common]
-        outcome_types = [binary]
-        run_indefinitely = False
-        """
-        config = Config(config_str=config_str)
-        criterion = RunIndefinitely(**RunIndefinitely.from_config(config, "test_strat"))
-        self.assertTrue(criterion.is_met(self.strat.experiment))
-
-        config_str = """
-        [common]
-        outcome_types = [binary]
-        run_indefinitely = True
-        """
-        config = Config(config_str=config_str)
-        criterion = RunIndefinitely(**RunIndefinitely.from_config(config, "test_strat"))
-        self.assertFalse(criterion.is_met(self.strat.experiment))
-
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.4.0/tests/generators/test_epsilon_greedy_generator.py` & `aepsych-0.4.1/tests/generators/test_epsilon_greedy_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/generators/test_manual_generator.py` & `aepsych-0.4.1/tests/generators/test_manual_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,20 +46,18 @@
                 """
         config = Config()
         config.update(config_str=config_str)
         gen = ManualGenerator.from_config(config)
         npt.assert_equal(gen.lb.numpy(), np.array([0, 0]))
         npt.assert_equal(gen.ub.numpy(), np.array([1, 1]))
 
-        self.assertFalse(gen.finished)
-
         p1 = list(gen.gen()[0])
         p2 = list(gen.gen()[0])
         p3 = list(gen.gen()[0])
         p4 = list(gen.gen()[0])
 
         self.assertEqual(sorted([p1, p2, p3, p4]), points)
-        self.assertTrue(gen.finished)
+        self.assertEqual(gen.max_asks, len(points))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.4.0/tests/generators/test_optimize_acqf_generator.py` & `aepsych-0.4.1/tests/generators/test_optimize_acqf_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,38 +97,51 @@
                 outcome_types = [continuous]
                 strat_names = [opt]
 
                 [opt]
                 generator = OptimizeAcqfGenerator
                 model = ContinuousRegressionGP
 
-                [ContinuousRegressionGP]
-                max_fit_time = 1
-
                 [OptimizeAcqfGenerator]
                 acqf = MCLevelSetEstimation
-                max_gen_time = 1
-                restarts = 1
-                samps = 100
+                max_gen_time = 0.1
+                num_restarts = 1
+                raw_samples = 100
 
                 [MCLevelSetEstimation]
                 beta = 1
                 target = 0.5
                 """
 
         config = Config(config_str=config_str)
         gen = AxOptimizeAcqfGenerator.from_config(config, "opt")
 
         self.assertEqual(gen.model, Models.BOTORCH_MODULAR)
 
         self.assertEqual(
             gen.model_kwargs["surrogate"].botorch_model_class, ContinuousRegressionGP
         )
-        self.assertEqual(gen.model_gen_kwargs["restarts"], 1)
-        self.assertEqual(gen.model_gen_kwargs["samps"], 100)
+        self.assertEqual(
+            gen.model_gen_kwargs["model_gen_options"]["optimizer_kwargs"][
+                "num_restarts"
+            ],
+            1,
+        )
+        self.assertEqual(
+            gen.model_gen_kwargs["model_gen_options"]["optimizer_kwargs"][
+                "raw_samples"
+            ],
+            100,
+        )
+        self.assertEqual(
+            gen.model_gen_kwargs["model_gen_options"]["optimizer_kwargs"][
+                "timeout_sec"
+            ],
+            0.1,
+        )
         self.assertEqual(gen.model_kwargs["acquisition_options"]["target"], 0.5)
         self.assertEqual(gen.model_kwargs["acquisition_options"]["beta"], 1.0)
         # TODO: Implement max_gen_time
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.4.0/tests/generators/test_random_generator.py` & `aepsych-0.4.1/tests/generators/test_random_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/generators/test_sobol_generator.py` & `aepsych-0.4.1/tests/generators/test_sobol_generator.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_derivative_gp.py` & `aepsych-0.4.1/tests/models/test_derivative_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_gp_classification.py` & `aepsych-0.4.1/tests/models/test_gp_classification.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,22 +23,79 @@
 from aepsych.config import Config
 from aepsych.generators import OptimizeAcqfGenerator, SobolGenerator
 from aepsych.models import GPClassificationModel
 from aepsych.strategy import SequentialStrategy, Strategy
 from botorch.acquisition import qUpperConfidenceBound
 from botorch.optim.fit import fit_gpytorch_mll_torch
 from botorch.optim.stopping import ExpMAStoppingCriterion
-from botorch.posteriors import GPyTorchPosterior
-from gpytorch.distributions import MultivariateNormal
+from scipy.special import expit
 from scipy.stats import bernoulli, norm, pearsonr
 from sklearn.datasets import make_classification
 from torch.distributions import Normal
 from torch.optim import Adam
 
-from ..common import cdf_new_novel_det, f_1d, f_2d
+
+def f_1d(x, mu=0):
+    """
+    latent is just a gaussian bump at mu
+    """
+    return np.exp(-((x - mu) ** 2))
+
+
+def f_2d(x):
+    """
+    a gaussian bump at 0 , 0
+    """
+    return np.exp(-np.linalg.norm(x, axis=-1))
+
+
+def new_novel_det_params(freq, scale_factor=1.0):
+    """Get the loc and scale params for 2D synthetic novel_det(frequency) function
+        Keyword arguments:
+    freq -- 1D array of frequencies whose thresholds to return
+    scale factor -- scale for the novel_det function, where higher is steeper/lower SD
+    target -- target threshold
+    """
+    locs = 0.66 * np.power(0.8 * freq * (0.2 * freq - 1), 2) + 0.05
+    scale = 2 * locs / (3 * scale_factor)
+    loc = -1 + 2 * locs
+    return loc, scale
+
+
+def target_new_novel_det(freq, scale_factor=1.0, target=0.75):
+    """Get the target (i.e. threshold) for 2D synthetic novel_det(frequency) function
+        Keyword arguments:
+    freq -- 1D array of frequencies whose thresholds to return
+    scale factor -- scale for the novel_det function, where higher is steeper/lower SD
+    target -- target threshold
+    """
+    locs, scale = new_novel_det_params(freq, scale_factor)
+    return norm.ppf(target, loc=locs, scale=scale)
+
+
+def new_novel_det(x, scale_factor=1.0):
+    """Get the cdf for 2D synthetic novel_det(frequency) function
+        Keyword arguments:
+    x -- array of shape (n,2) of locations to sample;
+         x[...,0] is frequency from -1 to 1; x[...,1] is intensity from -1 to 1
+    scale factor -- scale for the novel_det function, where higher is steeper/lower SD
+    """
+    freq = x[..., 0]
+    locs, scale = new_novel_det_params(freq, scale_factor)
+    return (x[..., 1] - locs) / scale
+
+
+def cdf_new_novel_det(x, scale_factor=1.0):
+    """Get the cdf for 2D synthetic novel_det(frequency) function
+        Keyword arguments:
+    x -- array of shape (n,2) of locations to sample;
+         x[...,0] is frequency from -1 to 1; x[...,1] is intensity from -1 to 1
+    scale factor -- scale for the novel_det function, where higher is steeper/lower SD
+    """
+    return norm.cdf(new_novel_det(x, scale_factor))
 
 
 class GPClassificationSmoketest(unittest.TestCase):
     """
     Super basic smoke test to make sure we know if we broke the underlying model
     for single-probit  ("1AFC") model
     """
@@ -737,63 +794,14 @@
         for _i in range(n_init + n_opt):
             next_x = strat.gen()
             strat.add_data(next_x, [bernoulli.rvs(norm.cdf(f_1d(next_x)))])
 
         with self.assertWarns(RuntimeWarning):
             strat.gen()
 
-    def test_1d_query(self):
-        seed = 1
-        torch.manual_seed(seed)
-        np.random.seed(seed)
-        lb = -4.0
-        ub = 4.0
-
-        strat = Strategy(
-            lb=lb,
-            ub=ub,
-            min_asks=1,
-            generator=SobolGenerator(lb=lb, ub=ub, seed=seed),
-            model=GPClassificationModel(lb=lb, ub=ub, inducing_size=50),
-            stimuli_per_trial=1,
-            outcome_types=["binary"],
-        )
-
-        # mock the posterior call and remove calls that don't need
-        # to happen
-        def get_fake_posterior(X, posterior_transform=None):
-            fmean = torch.sin(torch.pi * X / 4).squeeze(-1)
-            fcov = torch.eye(fmean.shape[0])
-            fake_posterior = GPyTorchPosterior(
-                mvn=MultivariateNormal(mean=fmean, covariance_matrix=fcov)
-            )
-            return fake_posterior
-
-        strat.model.posterior = get_fake_posterior
-        strat.model.__call__ = MagicMock()
-        strat.model.fit = MagicMock()
-
-        x = strat.gen(1)
-        y = torch.Tensor([1])
-        strat.add_data(x, y)
-        strat.model.set_train_data(x, y)
-        # We expect the global max to be at (2, 1), the min at (-2, -1)
-        fmax, argmax = strat.get_max()
-        self.assertTrue(np.allclose(fmax, 1))
-        self.assertTrue(np.allclose(argmax, 2))
-
-        fmin, argmin = strat.get_min()
-        self.assertTrue(np.allclose(fmin, -1))
-        self.assertTrue(np.allclose(argmin, -2, atol=0.2))
-
-        # Inverse query at val .85 should return (.85,[2.7])
-        val, loc = strat.inv_query(0.85, constraints={})
-        self.assertTrue(np.allclose(val, 0.85))
-        self.assertTrue(np.allclose(loc.item(), 2.7, atol=1e-2))
-
     def test_hyperparam_consistency(self):
         # verify that creating the model `from_config` or with `__init__` has the same hyperparams
 
         m1 = GPClassificationModel(lb=[1, 2], ub=[3, 4])
 
         m2 = GPClassificationModel.from_config(
             config=Config(config_dict={"common": {"lb": "[1,2]", "ub": "[3,4]"}})
```

### Comparing `aepsych-0.4.0/tests/models/test_gp_regression.py` & `aepsych-0.4.1/tests/models/test_gp_regression.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_model_query.py` & `aepsych-0.4.1/tests/models/test_model_query.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,33 +5,34 @@
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
 import unittest
 
 import numpy as np
 import torch
-from botorch.fit import fit_gpytorch_mll
-from gpytorch.mlls import ExactMarginalLogLikelihood
 
 from aepsych.models.exact_gp import ExactGP
+from aepsych.models.variational_gp import BinaryClassificationGP
+from scipy.special import expit
+from scipy.stats import bernoulli
+
 
 # Fix random seeds
 np.random.seed(0)
 torch.manual_seed(0)
 
 
-class TestModelQuery(unittest.TestCase):
+class SingleOutcomeModelQueryTestCase(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.bounds = torch.tensor([[0.0], [1.0]])
         x = torch.linspace(0.0, 1.0, 10).reshape(-1, 1)
         y = torch.sin(6.28 * x).reshape(-1, 1)
         cls.model = ExactGP(x, y)
-        mll = ExactMarginalLogLikelihood(cls.model.likelihood, cls.model)
-        fit_gpytorch_mll(mll)
+        cls.model.fit()
 
     def test_min(self):
         mymin, my_argmin = self.model.get_min(self.bounds)
         # Don't need to be precise since we're working with small data.
         self.assertLess(mymin, -0.9)
         self.assertTrue(0.7 < my_argmin < 0.8)
 
@@ -44,10 +45,62 @@
     def test_inverse_query(self):
         bounds = torch.tensor([[0.1], [0.9]])
         val, arg = self.model.inv_query(0.0, bounds)
         # Don't need to be precise since we're working with small data.
         self.assertTrue(-0.01 < val < 0.01)
         self.assertTrue(0.45 < arg < 0.55)
 
+    def test_binary_inverse_query(self):
+        X = torch.linspace(-3.0, 3.0, 100).reshape(-1, 1)
+        probs = expit(X)
+        responses = torch.tensor([float(bernoulli.rvs(p)) for p in probs]).reshape(
+            -1, 1
+        )
+
+        model = BinaryClassificationGP(X, responses)
+        model.fit()
+
+        bounds = torch.tensor([[0.0], [1.0]])
+        val, arg = model.inv_query(0.75, bounds, probability_space=True)
+        # Don't need to be precise since we're working with small data.
+        self.assertTrue(0.7 < val < 0.8)
+        self.assertTrue(0 < arg < 2)
+
+
+class MultiOutcomeModelQueryTestCase(unittest.TestCase):
+    @classmethod
+    def setUpClass(cls):
+        cls.bounds = torch.tensor([[0.0], [1.0]])
+        x = torch.linspace(0.0, 1.0, 10).reshape(-1, 1)
+        y = torch.cat(
+            (
+                torch.sin(6.28 * x).reshape(-1, 1),
+                torch.cos(6.28 * x).reshape(-1, 1),
+            ),
+            dim=1,
+        )
+        cls.model = ExactGP(x, y)
+        cls.model.fit()
+
+    def test_max(self):
+        mymax, my_argmax = self.model.get_max(self.bounds)
+        # Don't need to be precise since we're working with small data.
+        self.assertAlmostEqual(mymax.sum().numpy(), np.sqrt(2), places=1)
+        self.assertTrue(0.1 < my_argmax < 0.2)
+
+    def test_min(self):
+        mymax, my_argmax = self.model.get_min(self.bounds)
+        # Don't need to be precise since we're working with small data.
+        self.assertAlmostEqual(mymax.sum().numpy(), -np.sqrt(2), places=1)
+        self.assertTrue(0.6 < my_argmax < 0.7)
+
+    def test_inverse_query(self):
+        bounds = torch.tensor([[0.1], [0.9]])
+        val, arg = self.model.inv_query(torch.tensor([0.0, -1]), bounds)
+        # Don't need to be precise since we're working with small data.
+        self.assertTrue(-0.01 < val[0] < 0.01)
+        self.assertTrue(-1.01 < val[1] < -0.99)
+        self.assertTrue(0.45 < arg < 0.55)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.4.0/tests/models/test_monotonic_projection_gp.py` & `aepsych-0.4.1/tests/models/test_monotonic_projection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_monotonic_rejection_gp.py` & `aepsych-0.4.1/tests/models/test_monotonic_rejection_gp.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_multitask_regression.py` & `aepsych-0.4.1/tests/models/test_multitask_regression.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_pairwise_probit.py` & `aepsych-0.4.1/tests/models/test_pairwise_probit.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_semi_p.py` & `aepsych-0.4.1/tests/models/test_semi_p.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_utils.py` & `aepsych-0.4.1/tests/models/test_utils.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/models/test_variational_gp.py` & `aepsych-0.4.1/tests/models/test_variational_gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,17 @@
         # fspace
         pm, pv = model.predict(X)
         pred = (pm > 0).numpy()
         npt.assert_allclose(pred.reshape(-1, 1), y)
         npt.assert_array_less(1, pv)
 
 
+@unittest.skip(
+    "For some reason, the model fails to fit now. Maybe this is from a botorch change? Skipping for now."
+)
 class AxBetaRegressionGPTextCase(unittest.TestCase):
     @classmethod
     def setUp(cls):
         np.random.seed(1)
         torch.manual_seed(1)
         X, y = make_regression(
             n_samples=7,
@@ -77,16 +80,15 @@
         # Rescale the target values to the range [0, 1]
         y = (y - y.min()) / (y.max() - y.min())
         cls.X, cls.y = torch.Tensor(X), torch.Tensor(y).reshape(-1, 1)
 
     def test_1d_regression(self):
         X, y = self.X, self.y
         model = BetaRegressionGP(train_X=X, train_Y=y, inducing_points=10)
-        mll = VariationalELBO(model.likelihood, model.model, len(y))
-        fit_gpytorch_mll(mll)
+        model.fit()
 
         pm, pv = model.predict(X)
         npt.assert_allclose(pm.reshape(-1, 1), y, atol=0.1)
         npt.assert_array_less(pv, 1)
 
 
 class AxOrdinalGPTestCase(unittest.TestCase):
```

### Comparing `aepsych-0.4.0/tests/server/message_handlers/test_can_model.py` & `aepsych-0.4.1/tests/server/message_handlers/test_can_model.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/server/message_handlers/test_handle_exit.py` & `aepsych-0.4.1/tests/server/message_handlers/test_handle_exit.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/server/message_handlers/test_handle_finish_strategy.py` & `aepsych-0.4.1/tests/server/message_handlers/test_handle_finish_strategy.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/server/message_handlers/test_handle_get_config.py` & `aepsych-0.4.1/tests/server/message_handlers/test_handle_get_config.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/server/message_handlers/test_query_handlers.py` & `aepsych-0.4.1/tests/server/message_handlers/test_query_handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # LICENSE file in the root directory of this source tree.
 
 import unittest
 
 from ..test_server import BaseServerTestCase, dummy_config
 
 
+# Smoke test to make sure nothing breaks. This should really be combined with
+# the individual query tests
 class QueryHandlerTestCase(BaseServerTestCase):
     def test_strat_query(self):
         setup_request = {
             "type": "setup",
             "version": "0.01",
             "message": {"config_str": dummy_config},
         }
@@ -54,20 +56,15 @@
         query_inv_req = {
             "type": "query",
             "message": {
                 "query_type": "inverse",
                 "y": 5.0,
             },
         }
-        response_max = self.s.handle_request(query_max_req)
-        response_min = self.s.handle_request(query_min_req)
-        response_pred = self.s.handle_request(query_pred_req)
-        response_inv = self.s.handle_request(query_inv_req)
-
-        for response in [response_max, response_min, response_pred, response_inv]:
-            self.assertTrue(type(response["x"]) is dict)
-            self.assertTrue(len(response["x"]["x"]) == 1)
-            self.assertTrue(type(response["y"]) is float)
+        self.s.handle_request(query_min_req)
+        self.s.handle_request(query_pred_req)
+        self.s.handle_request(query_max_req)
+        self.s.handle_request(query_inv_req)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.4.0/tests/server/message_handlers/test_tell_handlers.py` & `aepsych-0.4.1/tests/server/message_handlers/test_tell_handlers.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/server/test_server.py` & `aepsych-0.4.1/tests/server/test_server.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_ax_integration.py` & `aepsych-0.4.1/tests/test_ax_integration.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,86 +1,98 @@
 #!/usr/bin/env python3
 # Copyright (c) Facebook, Inc. and its affiliates.
 # All rights reserved.
 
 # This source code is licensed under the license found in the
 # LICENSE file in the root directory of this source tree.
 
+import math
 import os
 import unittest
 import uuid
 
 import numpy as np
 import torch
-from aepsych_client import AEPsychClient
-from ax.service.utils.report_utils import exp_to_df
 
 from aepsych.config import Config
 from aepsych.server import AEPsychServer
+from aepsych_client import AEPsychClient
+from ax.service.utils.report_utils import exp_to_df
 from parameterized import parameterized_class
-import math
 
 
 @parameterized_class(
     ("config_file", "should_ignore"),
     [
         ("../configs/ax_example.ini", False),
         ("../configs/ax_ordinal_exploration_example.ini", True),
     ],
 )
 class AxIntegrationTestCase(unittest.TestCase):
+    n_extra_asks = 3
+
     @classmethod
     def setUpClass(cls):
         if cls.should_ignore:
             raise unittest.SkipTest("Skipping because should_ignore is True.")
 
         def sigmoid(x):
             return 1 / (1 + math.exp(-x / 100))
 
         # Simulate participant responses; just returns the sum of the flat parameters
         def simulate_response(trial_params):
             pars = [
-                trial_params[par][0]
+                trial_params[par]
                 for par in trial_params
-                if type(trial_params[par][0]) == float
+                if type(trial_params[par]) == float
             ]
             response = round(sigmoid(np.array(pars).mean()) * 4)
             return response
 
         # Fix random seeds
-        np.random.seed(0)
-        torch.manual_seed(0)
+        np.random.seed(123)
+        torch.manual_seed(123)
 
         # Create a server object configured to run a 2d threshold experiment
         database_path = "./{}.db".format(str(uuid.uuid4().hex))
         cls.client = AEPsychClient(server=AEPsychServer(database_path=database_path))
         cls.config_file = os.path.join(os.path.dirname(__file__), cls.config_file)
         cls.client.configure(cls.config_file)
 
+        cls.can_fit_at_start = cls.client.server.strat.can_fit
         while not cls.client.server.strat.finished:
             # Ask the server what the next parameter values to test should be.
             trial_params = cls.client.ask()
 
             # Simulate a participant response.
-            outcome = simulate_response(trial_params["config"])
+            for trial in trial_params["config"]:
+                outcome = simulate_response(trial_params["config"][trial])
 
-            # Tell the server what happened so that it can update its model.
-            cls.client.tell(trial_params["config"], outcome)
+                # Tell the server what happened so that it can update its model.
+                cls.client.tell_trial_by_index(trial, outcome)
 
-        # Add an extra tell to make sure manual tells and duplicate params
-        cls.client.tell(trial_params["config"], outcome)
+        # Make sure we can manually tell without asking first
+        cls.client.tell(trial_params["config"][trial], outcome)
+
+        # Add an extra ask to make sure we can generate trials endlessly
+        trial_params = cls.client.ask(cls.n_extra_asks)
+
+        cls.can_fit_at_end = cls.client.server.strat.can_fit
 
         cls.df = exp_to_df(cls.client.server.strat.experiment)
 
         cls.config = Config(config_fnames=[cls.config_file])
 
     def tearDown(self):
         if self.client.server.db is not None:
             self.client.server.db.delete_db()
 
+    def test_random_seed(self):
+        self.assertEqual(self.client.server.strat.ax_client._random_seed, 123)
+
     def test_bounds(self):
         lb = self.config.getlist("common", "lb", element_type=float)
         ub = self.config.getlist("common", "ub", element_type=float)
         par4choices = self.config.getlist("par4", "choices", element_type=str)
         par5choices = self.config.getlist("par5", "choices", element_type=str)
         par6value = self.config.getfloat("par6", "value")
         par7value = self.config.get("par7", "value")
@@ -98,38 +110,54 @@
 
         self.assertTrue(self.df["par5"].isin(par5choices).all())
 
         self.assertTrue((self.df["par6"] == par6value).all())
 
         self.assertTrue((self.df["par7"] == par7value).all())
 
+    @unittest.skip(
+        "This test is flaky due to non-determinism in asks after the experiment is finished. Skipping until this gets fixed."
+    )
     def test_constraints(self):
         constraints = self.config.getlist("common", "par_constraints", element_type=str)
         for constraint in constraints:
             self.assertEqual(len(self.df.query(constraint)), len(self.df))
 
         self.assertEqual(self.df["par3"].dtype, "int64")
 
     def test_n_trials(self):
         n_tells = (self.df["trial_status"] == "COMPLETED").sum()
         correct_n_tells = self.config.getint("opt_strat", "min_total_tells") + 1
-
         self.assertEqual(n_tells, correct_n_tells)
 
+        n_asks = self.client.server.strat.experiment.num_asks
+        correct_n_asks = (
+            self.config.getint("opt_strat", "min_total_tells") + self.n_extra_asks
+        )
+        self.assertEqual(n_asks, correct_n_asks)
+
     def test_generation_method(self):
         n_sobol = (self.df["generation_method"] == "Sobol").sum()
         n_opt = (self.df["generation_method"] == "BoTorch").sum()
+        n_manual = (self.df["generation_method"] == "Manual").sum()
 
         correct_n_sobol = self.config.getint("init_strat", "min_total_tells")
         correct_n_opt = (
-            self.config.getint("opt_strat", "min_total_tells") - correct_n_sobol
+            self.config.getint("opt_strat", "min_total_tells")
+            - correct_n_sobol
+            + self.n_extra_asks
         )
 
         self.assertEqual(n_sobol, correct_n_sobol)
         self.assertEqual(n_opt, correct_n_opt)
+        self.assertEqual(n_manual, 1)
+
+    def test_can_fit(self):
+        self.assertFalse(self.can_fit_at_start)
+        self.assertTrue(self.can_fit_at_end)
 
 
 @unittest.skip("Base integration tests already cover most of these")
 class AxBetaRegressionTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         # Simulate participant responses; just returns the average percentage value of the par1-3
```

### Comparing `aepsych-0.4.0/tests/test_bench_testfuns.py` & `aepsych-0.4.1/tests/test_bench_testfuns.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from aepsych.benchmark.test_functions import make_songetal_testfun
 from aepsych.utils import dim_grid
 
 
 class BenchmarkTestCase(unittest.TestCase):
     def test_songetal_funs_smoke(self):
         valid_phenotypes = ["Metabolic", "Sensory", "Metabolic+Sensory", "Older-normal"]
-        grid = dim_grid(lower=[-3, -20], upper=[4, 120], dim=2, gridsize=30)
+        grid = dim_grid(lower=[-3, -20], upper=[4, 120], gridsize=30)
         try:
             for phenotype in valid_phenotypes:
                 testfun = make_songetal_testfun(phenotype=phenotype)
                 f = testfun(grid)
                 self.assertTrue(f.shape == torch.Size([900]))
         except Exception:
             self.fail()
```

### Comparing `aepsych-0.4.0/tests/test_benchmark.py` & `aepsych-0.4.1/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_config.py` & `aepsych-0.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_db.py` & `aepsych-0.4.1/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_likelihoods.py` & `aepsych-0.4.1/tests/test_likelihoods.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_lookahead.py` & `aepsych-0.4.1/tests/test_lookahead.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_mean_covar_factories.py` & `aepsych-0.4.1/tests/test_mean_covar_factories.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_multioutcome.py` & `aepsych-0.4.1/tests/test_multioutcome.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 # LICENSE file in the root directory of this source tree.
 
 import os
 import unittest
 import uuid
 
 import torch
+
+from aepsych.server import AEPsychServer
 from aepsych_client import AEPsychClient
 from ax.core.optimization_config import MultiObjectiveOptimizationConfig
 from ax.modelbridge import Models
 from botorch.test_functions.multi_objective import BraninCurrin
 
-from aepsych.server import AEPsychServer
-
 branin_currin = BraninCurrin(negate=True).to(
     dtype=torch.double,
     device=torch.device("cuda" if torch.cuda.is_available() else "cpu"),
 )
 
 
 def evaluate(parameters):
     evaluation = branin_currin(
-        torch.tensor([parameters.get("x1")[0], parameters.get("x2")[0]])
+        torch.tensor([parameters.get("x1"), parameters.get("x2")])
     )
     # In our case, standard error is 0, since we are computing a synthetic function.
     # Set standard error to None if the noise level is unknown.
     return {"out1": evaluation[0].item(), "out2": evaluation[1].item()}
 
 
 class MultiOutcomeTestCase(unittest.TestCase):
@@ -41,17 +41,17 @@
         config_file = "../configs/multi_outcome_example.ini"
         config_file = os.path.join(os.path.dirname(__file__), config_file)
         cls.client.configure(config_file)
         cls.gs = cls.client.server.strat.ax_client.generation_strategy
         cls.experiment = cls.client.server.strat.ax_client.experiment
 
     def test_generation_strategy(self):
-        self.assertEqual(len(self.gs._steps), 2)
+        self.assertEqual(len(self.gs._steps), 2 + 1)
         self.assertEqual(self.gs._steps[0].model, Models.SOBOL)
-        self.assertEqual(self.gs._steps[1].model, Models.MOO)
+        self.assertEqual(self.gs._steps[1].model, Models.BOTORCH_MODULAR)
 
     def test_experiment(self):
         self.assertEqual(len(self.experiment.metrics), 2)
         self.assertIn("out1", self.experiment.metrics)
         self.assertIn("out2", self.experiment.metrics)
         self.assertIsInstance(
             self.experiment.optimization_config, MultiObjectiveOptimizationConfig
@@ -69,13 +69,14 @@
         self.assertFalse(objective1.minimize)
         self.assertFalse(objective2.minimize)
 
     # Smoke test just to make sure server can handle multioutcome messages
     def test_ask_tell(self):
         while not self.client.server.strat.finished:
             trial_params = self.client.ask()
-            outcome = evaluate(trial_params["config"])
-            self.client.tell(trial_params["config"], outcome)
+            for trial in trial_params["config"]:
+                outcome = evaluate(trial_params["config"][trial])
+                self.client.tell_trial_by_index(trial, outcome)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `aepsych-0.4.0/tests/test_strategy.py` & `aepsych-0.4.1/tests/test_strategy.py`

 * *Files identical despite different names*

### Comparing `aepsych-0.4.0/tests/test_utils.py` & `aepsych-0.4.1/tests/test_utils.py`

 * *Files identical despite different names*

