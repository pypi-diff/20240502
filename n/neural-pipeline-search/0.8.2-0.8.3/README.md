# Comparing `tmp/neural_pipeline_search-0.8.2.tar.gz` & `tmp/neural_pipeline_search-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_pipeline_search-0.8.2.tar", max compression
+gzip compressed data, was "neural_pipeline_search-0.8.3.tar", max compression
```

## Comparing `neural_pipeline_search-0.8.2.tar` & `neural_pipeline_search-0.8.3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0     1068 2023-03-16 17:27:25.573134 neural_pipeline_search-0.8.2/LICENSE
--rw-r--r--   0        0        0     3827 2023-03-17 23:50:21.760097 neural_pipeline_search-0.8.2/README.md
--rw-r--r--   0        0        0      432 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/README.md
--rw-r--r--   0        0        0      985 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/basic_usage/analyse.py
--rw-r--r--   0        0        0     3883 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/basic_usage/architecture.py
--rw-r--r--   0        0        0     3899 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/basic_usage/architecture_and_hyperparameters.py
--rw-r--r--   0        0        0      793 2023-03-18 00:15:48.983780 neural_pipeline_search-0.8.2/neps_examples/basic_usage/hyperparameters.py
--rw-r--r--   0        0        0      944 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/convenience/logging_additional_info.py
--rw-r--r--   0        0        0      979 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/convenience/working_directory_per_pipeline.py
--rw-r--r--   0        0        0     1091 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/efficiency/expert_priors_for_hyperparameters.py
--rw-r--r--   0        0        0     2655 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/efficiency/multi_fidelity.py
--rw-r--r--   0        0        0      877 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/efficiency/multi_fidelity_and_expert_priors.py
--rw-r--r--   0        0        0      501 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/efficiency/parallelization.md
--rw-r--r--   0        0        0     1156 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/experimental/cost_aware.py
--rw-r--r--   0        0        0     3762 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/experimental/expert_priors_for_architecture_and_hyperparameters.py
--rw-r--r--   0        0        0     2803 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/experimental/fault_tolerance.py
--rw-r--r--   0        0        0     2855 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/experimental/hierarchical_architecture.py
--rw-r--r--   0        0        0     4092 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/neps_examples/experimental/hierarchical_architecture_hierarchical_GP.py
--rw-r--r--   0        0        0     8261 2023-03-18 00:21:15.528675 neural_pipeline_search-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       87 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/metahyper/__init__.py
--rw-r--r--   0        0        0     1026 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/metahyper/_locker.py
--rw-r--r--   0        0        0    19024 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/metahyper/api.py
--rw-r--r--   0        0        0      905 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/metahyper/example.py
--rw-r--r--   0        0        0     5593 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/metahyper/utils.py
--rw-r--r--   0        0        0     1524 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/NOTICE
--rw-r--r--   0        0        0      595 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/__init__.py
--rw-r--r--   0        0        0    10127 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/api.py
--rw-r--r--   0        0        0     1907 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/__init__.py
--rw-r--r--   0        0        0     2759 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/base_optimizer.py
--rw-r--r--   0        0        0      783 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/__init__.py
--rw-r--r--   0        0        0     8784 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/_ehvi.py
--rw-r--r--   0        0        0      508 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/base_acquisition.py
--rw-r--r--   0        0        0     1603 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/cost_cooling.py
--rw-r--r--   0        0        0     4367 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/ei.py
--rw-r--r--   0        0        0     3278 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/gp_ucb.py
--rw-r--r--   0        0        0     2085 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/prior_weighted.py
--rw-r--r--   0        0        0      266 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/__init__.py
--rw-r--r--   0        0        0      868 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/base_acq_sampler.py
--rw-r--r--   0        0        0     9190 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/evolution_sampler.py
--rw-r--r--   0        0        0     4489 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/mutation_sampler.py
--rw-r--r--   0        0        0      533 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/random_sampler.py
--rw-r--r--   0        0        0    10233 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/cost_cooling.py
--rw-r--r--   0        0        0      659 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/__init__.py
--rw-r--r--   0        0        0     7018 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels.py
--rw-r--r--   0        0        0     8838 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels_hierarchy.py
--rw-r--r--   0        0        0     9515 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/encoding.py
--rw-r--r--   0        0        0     1593 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/get_kernels.py
--rw-r--r--   0        0        0     5119 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/edge_histogram.py
--rw-r--r--   0        0        0     2418 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/utils.py
--rw-r--r--   0        0        0    16859 2023-03-16 17:27:25.576467 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/vertex_histogram.py
--rw-r--r--   0        0        0    31306 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/weisfeiler_lehman.py
--rw-r--r--   0        0        0      972 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/graph_kernel.py
--rw-r--r--   0        0        0     4910 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/utils.py
--rw-r--r--   0        0        0     9523 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/vectorial_kernels.py
--rw-r--r--   0        0        0    13110 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/weisfilerlehman.py
--rw-r--r--   0        0        0    31459 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/mf_tpe.py
--rw-r--r--   0        0        0      260 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/__init__.py
--rw-r--r--   0        0        0    25840 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/gp.py
--rw-r--r--   0        0        0    42814 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/gp_hierarchy.py
--rw-r--r--   0        0        0    10469 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/kde.py
--rw-r--r--   0        0        0    13132 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/optimizer.py
--rw-r--r--   0        0        0     1227 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/grid_search/optimizer.py
--rw-r--r--   0        0        0    21675 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/hyperband.py
--rw-r--r--   0        0        0     7686 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/mf_bo.py
--rw-r--r--   0        0        0     4089 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/promotion_policy.py
--rw-r--r--   0        0        0    16825 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/sampling_policy.py
--rw-r--r--   0        0        0    27117 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/successive_halving.py
--rw-r--r--   0        0        0        0 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/__init__.py
--rw-r--r--   0        0        0    12303 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/async_priorband.py
--rw-r--r--   0        0        0    20042 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/priorband.py
--rw-r--r--   0        0        0    42769 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/raceband.py
--rw-r--r--   0        0        0     5142 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/utils.py
--rw-r--r--   0        0        0     2960 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/multiple_knowledge_sources/prototype_optimizer.py
--rw-r--r--   0        0        0     1073 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/random_search/optimizer.py
--rw-r--r--   0        0        0     5478 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/optimizers/regularized_evolution/optimizer.py
--rw-r--r--   0        0        0        0 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/plot/__init__.py
--rw-r--r--   0        0        0     3998 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/plot/__main__.py
--rw-r--r--   0        0        0     4896 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/plot/plot.py
--rw-r--r--   0        0        0     6148 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/plot/plotting.py
--rw-r--r--   0        0        0     2002 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/plot/read_results.py
--rw-r--r--   0        0        0      463 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/search_spaces/__init__.py
--rw-r--r--   0        0        0     6347 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/api.py
--rw-r--r--   0        0        0    33135 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/cfg.py
--rw-r--r--   0        0        0    14865 2023-03-16 17:27:25.579800 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/cfg_variants/cfg_resolution.py
--rw-r--r--   0        0        0    31518 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/cfg_variants/constrained_cfg.py
--rw-r--r--   0        0        0    74697 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/core_graph_grammar.py
--rw-r--r--   0        0        0     6719 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/crossover.py
--rw-r--r--   0        0        0    50567 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/graph.py
--rw-r--r--   0        0        0    31778 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/graph_grammar.py
--rw-r--r--   0        0        0     4835 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/mutations.py
--rw-r--r--   0        0        0    13266 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/primitives.py
--rw-r--r--   0        0        0     6417 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/topologies.py
--rw-r--r--   0        0        0     6281 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/categorical.py
--rw-r--r--   0        0        0     1043 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/constant.py
--rw-r--r--   0        0        0     6501 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/float.py
--rw-r--r--   0        0        0     3831 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/integer.py
--rw-r--r--   0        0        0      470 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/numerical.py
--rw-r--r--   0        0        0     1022 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/parameter.py
--rw-r--r--   0        0        0    15592 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/search_spaces/search_space.py
--rw-r--r--   0        0        0     1768 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/status/__main__.py
--rw-r--r--   0        0        0     4549 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/status/status.py
--rw-r--r--   0        0        0     1489 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/utils/common.py
--rw-r--r--   0        0        0     6024 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/utils/data_loading.py
--rw-r--r--   0        0        0     1639 2023-03-16 17:27:25.583134 neural_pipeline_search-0.8.2/src/neps/utils/result_utils.py
--rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 neural_pipeline_search-0.8.2/setup.py
--rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 neural_pipeline_search-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-21 19:29:56.600249 neural_pipeline_search-0.8.3/LICENSE
+-rw-r--r--   0        0        0     3827 2023-03-21 19:29:56.600249 neural_pipeline_search-0.8.3/README.md
+-rw-r--r--   0        0        0      432 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/README.md
+-rw-r--r--   0        0        0      985 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/basic_usage/analyse.py
+-rw-r--r--   0        0        0     3883 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/basic_usage/architecture.py
+-rw-r--r--   0        0        0     3899 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/basic_usage/architecture_and_hyperparameters.py
+-rw-r--r--   0        0        0      793 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/basic_usage/hyperparameters.py
+-rw-r--r--   0        0        0      944 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/convenience/logging_additional_info.py
+-rw-r--r--   0        0        0      979 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/convenience/working_directory_per_pipeline.py
+-rw-r--r--   0        0        0     1091 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/efficiency/expert_priors_for_hyperparameters.py
+-rw-r--r--   0        0        0     2655 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/efficiency/multi_fidelity.py
+-rw-r--r--   0        0        0      877 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/efficiency/multi_fidelity_and_expert_priors.py
+-rw-r--r--   0        0        0      501 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/efficiency/parallelization.md
+-rw-r--r--   0        0        0     1156 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/experimental/cost_aware.py
+-rw-r--r--   0        0        0     3762 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/experimental/expert_priors_for_architecture_and_hyperparameters.py
+-rw-r--r--   0        0        0     2803 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/experimental/fault_tolerance.py
+-rw-r--r--   0        0        0     2855 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/experimental/hierarchical_architecture.py
+-rw-r--r--   0        0        0     4092 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/neps_examples/experimental/hierarchical_architecture_hierarchical_GP.py
+-rw-r--r--   0        0        0     8261 2023-03-21 19:39:04.970780 neural_pipeline_search-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/src/metahyper/__init__.py
+-rw-r--r--   0        0        0     1026 2023-03-21 19:29:56.603582 neural_pipeline_search-0.8.3/src/metahyper/_locker.py
+-rw-r--r--   0        0        0    19024 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/metahyper/api.py
+-rw-r--r--   0        0        0      905 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/metahyper/example.py
+-rw-r--r--   0        0        0     5593 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/metahyper/utils.py
+-rw-r--r--   0        0        0     1524 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/NOTICE
+-rw-r--r--   0        0        0      595 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/__init__.py
+-rw-r--r--   0        0        0    10127 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/api.py
+-rw-r--r--   0        0        0     1907 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/__init__.py
+-rw-r--r--   0        0        0     2759 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/base_optimizer.py
+-rw-r--r--   0        0        0      783 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/__init__.py
+-rw-r--r--   0        0        0     8784 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/_ehvi.py
+-rw-r--r--   0        0        0      508 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/base_acquisition.py
+-rw-r--r--   0        0        0     1603 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/cost_cooling.py
+-rw-r--r--   0        0        0     4367 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/ei.py
+-rw-r--r--   0        0        0     3278 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/gp_ucb.py
+-rw-r--r--   0        0        0     2085 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/prior_weighted.py
+-rw-r--r--   0        0        0      266 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/__init__.py
+-rw-r--r--   0        0        0      868 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/base_acq_sampler.py
+-rw-r--r--   0        0        0     9190 2023-03-21 19:29:56.606915 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/evolution_sampler.py
+-rw-r--r--   0        0        0     4489 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/mutation_sampler.py
+-rw-r--r--   0        0        0      533 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/random_sampler.py
+-rw-r--r--   0        0        0    10233 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/cost_cooling.py
+-rw-r--r--   0        0        0      659 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/__init__.py
+-rw-r--r--   0        0        0     7018 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels.py
+-rw-r--r--   0        0        0     8838 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels_hierarchy.py
+-rw-r--r--   0        0        0     9515 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/encoding.py
+-rw-r--r--   0        0        0     1593 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/get_kernels.py
+-rw-r--r--   0        0        0     5119 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/edge_histogram.py
+-rw-r--r--   0        0        0     2418 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/utils.py
+-rw-r--r--   0        0        0    16859 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/vertex_histogram.py
+-rw-r--r--   0        0        0    31306 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/weisfeiler_lehman.py
+-rw-r--r--   0        0        0      972 2023-03-21 19:29:56.610248 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/graph_kernel.py
+-rw-r--r--   0        0        0     4910 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/utils.py
+-rw-r--r--   0        0        0     9523 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/vectorial_kernels.py
+-rw-r--r--   0        0        0    13110 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/weisfilerlehman.py
+-rw-r--r--   0        0        0    31459 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/mf_tpe.py
+-rw-r--r--   0        0        0      260 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/__init__.py
+-rw-r--r--   0        0        0    25840 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/gp.py
+-rw-r--r--   0        0        0    42814 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/gp_hierarchy.py
+-rw-r--r--   0        0        0    10469 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/kde.py
+-rw-r--r--   0        0        0    13132 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/optimizer.py
+-rw-r--r--   0        0        0     1227 2023-03-21 19:29:56.613582 neural_pipeline_search-0.8.3/src/neps/optimizers/grid_search/optimizer.py
+-rw-r--r--   0        0        0    21675 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/hyperband.py
+-rw-r--r--   0        0        0     7697 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/mf_bo.py
+-rw-r--r--   0        0        0     4089 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/promotion_policy.py
+-rw-r--r--   0        0        0    17020 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/sampling_policy.py
+-rw-r--r--   0        0        0    27145 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/successive_halving.py
+-rw-r--r--   0        0        0        0 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/__init__.py
+-rw-r--r--   0        0        0    12303 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/async_priorband.py
+-rw-r--r--   0        0        0    18748 2023-03-21 19:29:56.616915 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/priorband.py
+-rw-r--r--   0        0        0    42769 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/raceband.py
+-rw-r--r--   0        0        0     5710 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/utils.py
+-rw-r--r--   0        0        0     2960 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/optimizers/multiple_knowledge_sources/prototype_optimizer.py
+-rw-r--r--   0        0        0     1073 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/optimizers/random_search/optimizer.py
+-rw-r--r--   0        0        0     5478 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/optimizers/regularized_evolution/optimizer.py
+-rw-r--r--   0        0        0        0 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/plot/__init__.py
+-rw-r--r--   0        0        0     3998 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/plot/__main__.py
+-rw-r--r--   0        0        0     4896 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/plot/plot.py
+-rw-r--r--   0        0        0     6148 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/plot/plotting.py
+-rw-r--r--   0        0        0     2002 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/plot/read_results.py
+-rw-r--r--   0        0        0      463 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/search_spaces/__init__.py
+-rw-r--r--   0        0        0     6347 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/api.py
+-rw-r--r--   0        0        0    33135 2023-03-21 19:29:56.620248 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/cfg.py
+-rw-r--r--   0        0        0    14865 2023-03-21 19:29:56.623582 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/cfg_variants/cfg_resolution.py
+-rw-r--r--   0        0        0    31518 2023-03-21 19:29:56.623582 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/cfg_variants/constrained_cfg.py
+-rw-r--r--   0        0        0    74697 2023-03-21 19:29:56.623582 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/core_graph_grammar.py
+-rw-r--r--   0        0        0     6719 2023-03-21 19:29:56.623582 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/crossover.py
+-rw-r--r--   0        0        0    50567 2023-03-21 19:29:56.623582 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/graph.py
+-rw-r--r--   0        0        0    31778 2023-03-21 19:29:56.623582 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/graph_grammar.py
+-rw-r--r--   0        0        0     4835 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/mutations.py
+-rw-r--r--   0        0        0    13266 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/primitives.py
+-rw-r--r--   0        0        0     6417 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/topologies.py
+-rw-r--r--   0        0        0     6281 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/categorical.py
+-rw-r--r--   0        0        0     1043 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/constant.py
+-rw-r--r--   0        0        0     6501 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/float.py
+-rw-r--r--   0        0        0     3973 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/integer.py
+-rw-r--r--   0        0        0      470 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/numerical.py
+-rw-r--r--   0        0        0     1022 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/parameter.py
+-rw-r--r--   0        0        0    15606 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/search_spaces/search_space.py
+-rw-r--r--   0        0        0     1768 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/status/__main__.py
+-rw-r--r--   0        0        0     4549 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/status/status.py
+-rw-r--r--   0        0        0     1489 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/utils/common.py
+-rw-r--r--   0        0        0     6024 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/utils/data_loading.py
+-rw-r--r--   0        0        0     1639 2023-03-21 19:29:56.626915 neural_pipeline_search-0.8.3/src/neps/utils/result_utils.py
+-rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 neural_pipeline_search-0.8.3/setup.py
+-rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 neural_pipeline_search-0.8.3/PKG-INFO
```

### Comparing `neural_pipeline_search-0.8.2/LICENSE` & `neural_pipeline_search-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/README.md` & `neural_pipeline_search-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/basic_usage/analyse.py` & `neural_pipeline_search-0.8.3/neps_examples/basic_usage/analyse.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/basic_usage/architecture.py` & `neural_pipeline_search-0.8.3/neps_examples/basic_usage/architecture.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/basic_usage/architecture_and_hyperparameters.py` & `neural_pipeline_search-0.8.3/neps_examples/basic_usage/architecture_and_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/basic_usage/hyperparameters.py` & `neural_pipeline_search-0.8.3/neps_examples/basic_usage/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/convenience/logging_additional_info.py` & `neural_pipeline_search-0.8.3/neps_examples/convenience/logging_additional_info.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/convenience/working_directory_per_pipeline.py` & `neural_pipeline_search-0.8.3/neps_examples/convenience/working_directory_per_pipeline.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/efficiency/expert_priors_for_hyperparameters.py` & `neural_pipeline_search-0.8.3/neps_examples/efficiency/expert_priors_for_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/efficiency/multi_fidelity.py` & `neural_pipeline_search-0.8.3/neps_examples/efficiency/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/efficiency/multi_fidelity_and_expert_priors.py` & `neural_pipeline_search-0.8.3/neps_examples/efficiency/multi_fidelity_and_expert_priors.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/experimental/cost_aware.py` & `neural_pipeline_search-0.8.3/neps_examples/experimental/cost_aware.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/experimental/expert_priors_for_architecture_and_hyperparameters.py` & `neural_pipeline_search-0.8.3/neps_examples/experimental/expert_priors_for_architecture_and_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/experimental/fault_tolerance.py` & `neural_pipeline_search-0.8.3/neps_examples/experimental/fault_tolerance.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/experimental/hierarchical_architecture.py` & `neural_pipeline_search-0.8.3/neps_examples/experimental/hierarchical_architecture.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/neps_examples/experimental/hierarchical_architecture_hierarchical_GP.py` & `neural_pipeline_search-0.8.3/neps_examples/experimental/hierarchical_architecture_hierarchical_GP.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/pyproject.toml` & `neural_pipeline_search-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neural-pipeline-search"
-version = "v0.8.2"
+version = "v0.8.3"
 description = "Neural Pipeline Search helps deep learning experts find the best neural pipeline."
 authors = [
     "Danny Stoll <stolld@cs.uni-freiburg.de>",
     "Simon Schrodi <schrodi@cs.uni-freiburg.de>",
     "Maciej Janowski <janowski@cs.uni-freiburg.de>",
     "Neeratyoy Mallik <mallik@cs.uni-freiburg.de>",
     "Carl Hvarfner",
```

### Comparing `neural_pipeline_search-0.8.2/src/metahyper/_locker.py` & `neural_pipeline_search-0.8.3/src/metahyper/_locker.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/metahyper/api.py` & `neural_pipeline_search-0.8.3/src/metahyper/api.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/metahyper/example.py` & `neural_pipeline_search-0.8.3/src/metahyper/example.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/metahyper/utils.py` & `neural_pipeline_search-0.8.3/src/metahyper/utils.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/NOTICE` & `neural_pipeline_search-0.8.3/src/neps/NOTICE`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/__init__.py` & `neural_pipeline_search-0.8.3/src/neps/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/api.py` & `neural_pipeline_search-0.8.3/src/neps/api.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/__init__.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/base_optimizer.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/__init__.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/_ehvi.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/_ehvi.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/cost_cooling.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/cost_cooling.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/ei.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/ei.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/gp_ucb.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/gp_ucb.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_functions/prior_weighted.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_functions/prior_weighted.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/base_acq_sampler.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/base_acq_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/evolution_sampler.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/evolution_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/mutation_sampler.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/mutation_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/acquisition_samplers/random_sampler.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/acquisition_samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/cost_cooling.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/cost_cooling.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/__init__.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels_hierarchy.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/combine_kernels_hierarchy.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/encoding.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/encoding.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/get_kernels.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/get_kernels.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/edge_histogram.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/edge_histogram.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/utils.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/utils.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/vertex_histogram.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/vertex_histogram.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/weisfeiler_lehman.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/grakel_replace/weisfeiler_lehman.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/graph_kernel.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/graph_kernel.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/utils.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/utils.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/vectorial_kernels.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/vectorial_kernels.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/kernels/weisfilerlehman.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/kernels/weisfilerlehman.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/mf_tpe.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/mf_tpe.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/gp.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/gp.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/gp_hierarchy.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/gp_hierarchy.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/models/kde.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/models/kde.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/bayesian_optimization/optimizer.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/bayesian_optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/grid_search/optimizer.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/grid_search/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/hyperband.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/hyperband.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/mf_bo.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/mf_bo.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
             rung = self._active_rung()
             # inside here rung should not be None
             if rung is None:
                 raise ValueError(
                     "Returned rung is None. Should not be so when not init phase."
                 )
-            print(f"Building model at rung {rung}")
+            self.logger.info(f"Building model at rung {rung}")
             # collecting finished evaluations at `rung`
             train_df = self.observed_configs.loc[
                 self.rung_histories[rung]["config"]
             ].copy()
 
             # setting the fidelity value and performance to match the rung history
             # a promoted configuration may have a different fidelity than the
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/promotion_policy.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/promotion_policy.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/sampling_policy.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/sampling_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Any
 
+import logging
 import numpy as np
 import pandas as pd
 import torch
 
 from metahyper import instance_from_map
 
 from ...search_spaces.search_space import SearchSpace
@@ -34,17 +35,18 @@
 DELTA_THRESHOLD = 1e-2  # 1%
 TOP_EI_SAMPLE_COUNT = 10
 
 
 class SamplingPolicy(ABC):
     """Base class for implementing a sampling strategy for SH and its subclasses"""
 
-    def __init__(self, pipeline_space: SearchSpace, patience: int = 100):
+    def __init__(self, pipeline_space: SearchSpace, patience: int = 100, logger=None):
         self.pipeline_space = pipeline_space
         self.patience = patience
+        self.logger = logger or logging.getLogger("neps")
 
     @abstractmethod
     def sample(self, *args, **kwargs) -> SearchSpace:
         pass
 
 
 class RandomUniformPolicy(SamplingPolicy):
@@ -53,30 +55,33 @@
     Args:
         SamplingPolicy ([type]): [description]
     """
 
     def __init__(
         self,
         pipeline_space: SearchSpace,
+        logger=None,
     ):
-        super().__init__(pipeline_space=pipeline_space)
+        super().__init__(pipeline_space=pipeline_space, logger=logger)
 
     def sample(self, *args, **kwargs) -> SearchSpace:
         return self.pipeline_space.sample(
             patience=self.patience, user_priors=False, ignore_fidelity=True
         )
 
 
 class FixedPriorPolicy(SamplingPolicy):
     """A random policy for sampling configuration, i.e. the default for SH but samples
     a fixed fraction from the prior.
     """
 
-    def __init__(self, pipeline_space: SearchSpace, fraction_from_prior: float = 1):
-        super().__init__(pipeline_space=pipeline_space)
+    def __init__(
+        self, pipeline_space: SearchSpace, fraction_from_prior: float = 1, logger=None
+    ):
+        super().__init__(pipeline_space=pipeline_space, logger=logger)
         assert 0 <= fraction_from_prior <= 1
         self.fraction_from_prior = fraction_from_prior
 
     def sample(self, *args, **kwargs) -> SearchSpace:
         """Samples from the prior with a certain probabiliyu
 
         Returns:
@@ -98,14 +103,15 @@
         SamplingPolicy ([type]): [description]
     """
 
     def __init__(
         self,
         pipeline_space: SearchSpace,
         inc_type: str = "mutation",
+        logger=None,
     ):
         """Samples a policy as per its weights and performs the selected sampling.
 
         Args:
             pipeline_space: Space in which to search
             inc_type: str
                 if "hypersphere", uniformly samples from around the incumbent within its
@@ -113,15 +119,15 @@
                 if "gaussian", samples from a gaussian around the incumbent
                 if "crossover", generates a config by crossover between a random sample
                     and the incumbent
                 if "mutation", generates a config by perturbing each hyperparameter with
                     50% (mutation_rate=0.5) probability of selecting each hyperparmeter
                     for perturbation, sampling a deviation N(value, mutation_std=0.5))
         """
-        super().__init__(pipeline_space=pipeline_space)
+        super().__init__(pipeline_space=pipeline_space, logger=logger)
         self.inc_type = inc_type
         # setting all probabilities uniformly
         self.policy_map = {"random": 0.33, "prior": 0.34, "inc": 0.33}
 
     def sample_neighbour(self, incumbent, distance, tolerance=TOLERANCE):
         """Samples a config from around the `incumbent` within radius as `distance`."""
         # TODO: how does tolerance affect optimization on landscapes of different scale
@@ -154,39 +160,38 @@
         Returns:
             SearchSpace: [description]
         """
         if weights is not None:
             for key, value in sorted(weights.items()):
                 self.policy_map[key] = value
         else:
-            print(f"Using default policy weights: {self.policy_map}")
+            self.logger.info(f"Using default policy weights: {self.policy_map}")
         prob_weights = [v for _, v in sorted(self.policy_map.items())]
         policy_idx = np.random.choice(range(len(prob_weights)), p=prob_weights)
         policy = sorted(self.policy_map.keys())[policy_idx]
 
+        self.logger.info(f"Sampling from {policy} with weights (i, p, r)={prob_weights}")
+
         if policy == "prior":
-            print(f"Sampling from prior with weights (i, p, r)={prob_weights}")
             config = self.pipeline_space.sample(
                 patience=self.patience, user_priors=True, ignore_fidelity=True
             )
         elif policy == "inc":
-            print(f"Sampling from inc with weights (i, p, r)={prob_weights}")
-
             # pylint: disable=simplifiable-if-statement
             if (
                 hasattr(self.pipeline_space, "has_prior")
                 and self.pipeline_space.has_prior
             ):
                 user_priors = True
             else:
                 user_priors = False
 
             if inc is None:
                 inc = deepcopy(self.pipeline_space.sample_default_configuration())
-                print("No incumbent config found, using default as the incumbent.")
+                self.logger.warning("No incumbent config found, using default as the incumbent.")
 
             if self.inc_type == "hypersphere":
                 distance = kwargs["distance"]
                 config = self.sample_neighbour(inc, distance)
             elif self.inc_type == "gaussian":
                 # use inc to set the defaults of the configuration
                 _inc = deepcopy(inc)
@@ -211,15 +216,17 @@
                 probs = [1 - score_diff, score_diff]  # the order is [prior, random]
                 user_priors = np.random.choice([True, False], p=probs)
                 if (
                     hasattr(self.pipeline_space, "has_prior")
                     and not self.pipeline_space.has_prior
                 ):
                     user_priors = False
-                print(f"Crossing over with user_priors={user_priors} with p={probs}")
+                self.logger.info(
+                    f"Crossing over with user_priors={user_priors} with p={probs}"
+                )
                 # sampling a configuration either randomly or from a prior
                 _config = self.pipeline_space.sample(
                     patience=self.patience, user_priors=user_priors, ignore_fidelity=True
                 )
                 # injecting hyperparameters from the sampled config into the incumbent
                 # TODO: ideally lower crossover prob overtime
                 config = custom_crossover(inc, _config, crossover_prob=0.5)
@@ -230,18 +237,18 @@
                         mutation_rate=kwargs["inc_mutation_rate"],
                         std=kwargs["inc_mutation_std"]
                     )
                 else:
                     config = local_mutation(inc)
             else:
                 raise ValueError(
-                    f"{self.inc_type} is not in {{'mutation', 'crossover', 'hypersphere', 'gaussian'}}"
+                    f"{self.inc_type} is not in "
+                    f"{{'mutation', 'crossover', 'hypersphere', 'gaussian'}}"
                 )
         else:
-            print(f"Sampling from uniform with weights (i, p, r)={prob_weights}")
             # random
             config = self.pipeline_space.sample(
                 patience=self.patience, user_priors=False, ignore_fidelity=True
             )
         return config
 
 
@@ -259,16 +266,17 @@
         domain_se_kernel: str = None,
         hp_kernels: list = None,
         surrogate_model_args: dict = None,
         acquisition: str | BaseAcquisition = "EI",
         log_prior_weighted: bool = False,
         acquisition_sampler: str | AcquisitionSampler = "random",
         patience: int = 100,
+        logger=None,
     ):
-        super().__init__(pipeline_space=pipeline_space)
+        super().__init__(pipeline_space=pipeline_space, logger=logger)
 
         surrogate_model_args = surrogate_model_args or {}
 
         _, hp_kernels = get_kernels(
             pipeline_space=pipeline_space,
             domain_se_kernel=domain_se_kernel,
             graph_kernels=None,
@@ -349,15 +357,15 @@
               `fidelity` where the new sample will be evaluated. The top-10 are selected,
               and the EI for them is evaluated at the target/mmax fidelity.
             * If active_max_fidelity is not None, triggers the case when a surrogate is
               trained per fidelity. In this case, all samples have their fidelity
               variable set to the same value. This value is same as that of the fidelity
               value of the configs in the training data.
         """
-        print("Acquiring...")
+        self.logger.info("Acquiring...")
 
         # sampling random configurations
         samples = [
             self.pipeline_space.sample(user_priors=False, ignore_fidelity=True)
             for _ in range(SAMPLE_THRESHOLD)
         ]
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity/successive_halving.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity/successive_halving.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,21 +87,21 @@
             logger=logger,
         )
         if random_interleave_prob < 0 or random_interleave_prob > 1:
             raise ValueError("random_interleave_prob should be in [0.0, 1.0]")
         self.random_interleave_prob = random_interleave_prob
         self.sample_default_first = sample_default_first
 
-        self.min_budget = pipeline_space.fidelity.lower
-        self.max_budget = pipeline_space.fidelity.upper
+        self.min_budget = self.pipeline_space.fidelity.lower
+        self.max_budget = self.pipeline_space.fidelity.upper
         self.eta = eta
         # SH implicitly sets early_stopping_rate to 0
         # the parameter is exposed to allow HB to call SH with different stopping rates
         self.early_stopping_rate = early_stopping_rate
-        self.sampling_policy = sampling_policy(pipeline_space)
+        self.sampling_policy = sampling_policy(self.pipeline_space, self.logger)
         self.promotion_policy = promotion_policy(self.eta)
 
         # `max_budget_init` checks for the number of configurations that have been
         # evaluated at the target budget
         self.initial_design_type = initial_design_type
         self.use_priors = use_priors
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/async_priorband.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/async_priorband.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/priorband.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/priorband.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from ..bayesian_optimization.acquisition_samplers.base_acq_sampler import (
     AcquisitionSampler,
 )
 from ..multi_fidelity.hyperband import HyperbandCustomDefault
 from ..multi_fidelity.mf_bo import MFBOBase
 from ..multi_fidelity.promotion_policy import SyncPromotionPolicy
 from ..multi_fidelity.sampling_policy import EnsemblePolicy, ModelPolicy
-from .utils import calc_total_resources_spent, compute_config_dist, compute_scores
+from .utils import (
+    calc_total_resources_spent,
+    compute_config_dist, compute_scores,
+    get_prior_weight_for_decay
+)
 
 
 class PriorBandBase:
     """Class that defines essential properties needed by PriorBand.
 
     Designed to work with the topmost parent class as SuccessiveHalvingBase.
     """
@@ -159,74 +163,51 @@
         else:
             raise ValueError(f"{self.prior_weight_type} not in {{'linear', 'geometric'}}")
 
         # normalizing weights of random and prior sampling
         w_prior = _w_prior / (_w_prior + _w_random)
         w_random = _w_random / (_w_prior + _w_random)
         # calculating ratio of prior and incumbent weights
-        _w_prior, _w_inc = self.prior_to_incumbent_ratio(1, 0, self.max_rung)
+        _w_prior, _w_inc = self.prior_to_incumbent_ratio()
         # scaling back such that w_random + w_prior + w_inc = 1
         w_inc = _w_inc * w_prior
         w_prior = _w_prior * w_prior
 
         sampling_args = {
             "prior": w_prior,
             "inc": w_inc,
             "random": w_random,
         }
         return sampling_args
 
-    def prior_to_incumbent_ratio(self, w1: float, w2: float, rung: int) -> float | float:
+    def prior_to_incumbent_ratio(self) -> float | float:
         """Calculates the normalized weight distribution between prior and incumbent.
 
         Sum of the weights should be 1.
         """
         if self.inc_style == "constant":
             return self._prior_to_incumbent_ratio_constant()
         elif self.inc_style == "decay":
-            return self._prior_to_incumbent_ratio_decay(w1, w2)
+            resources = calc_total_resources_spent(self.observed_configs, self.rung_map)
+            return self._prior_to_incumbent_ratio_decay(
+                resources, self.eta, self.min_budget, self.max_budget
+            )
         elif self.inc_style == "dynamic":
-            return self._prior_to_incumbent_ratio_dynamic(rung)
+            return self._prior_to_incumbent_ratio_dynamic(self.max_rung)
         else:
             raise ValueError(f"Invalid option {self.inc_style}")
 
-    def _get_alpha(self, crossover: int = 0.5) -> float:
-        """Calculating approximate alpha rate for a specific crossover point.
-
-        Since with every iteration, the weight is reduced by alpha. We can approximately
-        calculate at which iteration (n) we can achieve the crossover value, by
-        calculating the n-th root of the crossover value. n is chosen as the total number
-        of samples seen in a single, full Hyperband bracket.
-        """
-        nconfigs = 0
-        for bracket in self.sh_brackets.values():
-            nconfigs += bracket.config_map[bracket.min_rung]
-        alpha = np.power(crossover, 1 / nconfigs)
-        return alpha
-
-    def _prior_to_incumbent_ratio_decay(self, w1: float, w2: float) -> float | float:
+    def _prior_to_incumbent_ratio_decay(
+        self, resources: float, eta: int, min_budget, max_budget
+    ) -> float | float:
         """Decays the prior weightage and increases the incumbent weightage.
-
-        The sum of weightage for prior and incumbents is always 1 here. `alpha` controls
-        the rate of decay. The `crossover` point is where the weightage is equal.
-        `alpha` is calculated to be such that given the HB allocations, the crossover
-        will happen roughly when (eta-1) * N/eta configurations have been seen. Where,
-        N is the total number of configurations sampled in 1 full HB bracket.
         """
-        # 0.5 is the crossover point in between w_prior=1 and w_inc=0
-        alpha = self._get_alpha(crossover=0.5)
-        _w1 = w1
-        _w2 = w2
-        t = np.count_nonzero(
-            ~np.isnan(self.observed_configs.perf.values.tolist() + [np.nan])
-        )
-        for _t in range(t):
-            _w1 = alpha * _w1 + (1 - alpha) * w2
-            _w2 = alpha * _w2 + (1 - alpha) * w1
-        return _w1, _w2
+        w_prior = get_prior_weight_for_decay(resources, eta, min_budget, max_budget)
+        w_inc = 1 - w_prior
+        return w_prior, w_inc
 
     def _prior_to_incumbent_ratio_constant(self) -> float | float:
         """Fixes the weightage of incumbent sampling to 1/eta of prior sampling."""
         # fixing weight of incumbent to 1/eta of prior
         _w_prior = self.eta
         _w_inc = 1
         w_prior = _w_prior / (_w_prior + _w_inc)
@@ -390,20 +371,18 @@
         self,
     ) -> tuple[SearchSpace, str, str | None]:
         """...and this is the method that decides which point to query.
 
         Returns:
             [type]: [description]
         """
-        print(f"Rung={self.current_sh_bracket}")
         self.set_sampling_weights_and_inc(rung=self.current_sh_bracket)
 
         for _, sh in self.sh_brackets.items():
             sh.sampling_args = self.sampling_args
-        print(sh.sampling_args["weights"])  # pylint: disable=undefined-loop-variable
         return super().get_config_and_ids()
 
 
 class PriorBandNoIncToPrior(PriorBand):
     """Disables incumbent sampling to replace with prior-based sampling."""
 
     def set_sampling_weights_and_inc(self, rung: int):
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/raceband.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/raceband.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multi_fidelity_prior/utils.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multi_fidelity_prior/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,7 +130,23 @@
     rungs_used = [
         observed_configs.at[i, "rung"]
         for i in range(len(observed_configs))
         if not np.isnan(observed_configs.at[i, "perf"])
     ]
     total_resources = sum(rung_map[r] for r in rungs_used)
     return total_resources
+
+
+def get_prior_weight_for_decay(
+    resources_used: float, eta: int, min_budget, max_budget
+) -> float:
+    nrungs = np.floor(np.log(max_budget/min_budget) / np.log(eta)).astype(int) + 1
+    unit_HB_resources = nrungs * eta * max_budget
+    idx = resources_used // unit_HB_resources
+    start_weight = 1 / eta ** idx
+    end_weight = start_weight / eta
+    _resources = resources_used / unit_HB_resources - idx
+
+    # equation for line in the idx-th HB bracket in terms of resource usage
+    y = (end_weight - start_weight) * _resources + start_weight
+
+    return y
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/multiple_knowledge_sources/prototype_optimizer.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/multiple_knowledge_sources/prototype_optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/random_search/optimizer.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/random_search/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/optimizers/regularized_evolution/optimizer.py` & `neural_pipeline_search-0.8.3/src/neps/optimizers/regularized_evolution/optimizer.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/plot/__main__.py` & `neural_pipeline_search-0.8.3/src/neps/plot/__main__.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/plot/plot.py` & `neural_pipeline_search-0.8.3/src/neps/plot/plot.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/plot/plotting.py` & `neural_pipeline_search-0.8.3/src/neps/plot/plotting.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/plot/read_results.py` & `neural_pipeline_search-0.8.3/src/neps/plot/read_results.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/api.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/api.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/cfg.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/cfg.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/cfg_variants/cfg_resolution.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/cfg_variants/cfg_resolution.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/cfg_variants/constrained_cfg.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/cfg_variants/constrained_cfg.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/core_graph_grammar.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/core_graph_grammar.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/crossover.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/crossover.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/graph.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/graph.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/graph_grammar.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/graph_grammar.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/mutations.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/mutations.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/primitives.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/primitives.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/architecture/topologies.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/architecture/topologies.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/categorical.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/categorical.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/constant.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/constant.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/float.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/float.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/hyperparameters/integer.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/hyperparameters/integer.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,17 @@
         self.value: None | int = None
 
     def __repr__(self):
         return f"<Integer, range: [{self.lower}, {self.upper}], value: {self.value}>"
 
     def _set_float_hp_val(self):
         # IMPORTANT function to call wherever `self.float_hp` is used in this class
-        self.float_hp.value = float(self.value)
-        self.float_hp.default = float(self.default)
+        self.float_hp.value = None if self.value is None else float(self.value)
+        self.float_hp.default = None if self.default is None else float(self.default)
+        self.float_hp._set_log_values()
 
     def sample(self, user_priors: bool = False):
         self.float_hp.sample(user_priors=user_priors)
         self.value = int(round(self.float_hp.value))  # type: ignore[arg-type]
 
     def mutate(
         self,
@@ -105,10 +106,10 @@
 
 def float_to_integer(float_hp):
     int_hp = IntegerParameter(
         lower=int(round(float_hp.lower)),
         upper=int(round(float_hp.upper)),
         log=float_hp.log,
     )
-    int_hp.value = int(round(float_hp.value))
+    int_hp.value = None if float_hp.value is None else int(round(float_hp.value))
 
     return int_hp
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/parameter.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/parameter.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/search_spaces/search_space.py` & `neural_pipeline_search-0.8.3/src/neps/search_spaces/search_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
             hp = new_config[hp_name]
             if isinstance(hp, NumericalParameter) and hp.is_fidelity:
                 continue
             try:
                 new_config[hp_name] = hp.mutate(**kwargs)
                 break
             except Exception as e:
-                print(f"{hp_name} FAILED!")
+                self.logger.warning(f"{hp_name} FAILED!")
                 continue
         return new_config
 
     def crossover(
         self,
         config2,
         crossover_probability_per_hyperparameter: float = 1.0,
```

### Comparing `neural_pipeline_search-0.8.2/src/neps/status/__main__.py` & `neural_pipeline_search-0.8.3/src/neps/status/__main__.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/status/status.py` & `neural_pipeline_search-0.8.3/src/neps/status/status.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/utils/common.py` & `neural_pipeline_search-0.8.3/src/neps/utils/common.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/utils/data_loading.py` & `neural_pipeline_search-0.8.3/src/neps/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/src/neps/utils/result_utils.py` & `neural_pipeline_search-0.8.3/src/neps/utils/result_utils.py`

 * *Files identical despite different names*

### Comparing `neural_pipeline_search-0.8.2/setup.py` & `neural_pipeline_search-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['numpy>=1.21.0,<1.22.0'],
  ':python_version >= "3.8"': ['numpy>=1.22.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'neural-pipeline-search',
-    'version': '0.8.2',
+    'version': '0.8.3',
     'description': 'Neural Pipeline Search helps deep learning experts find the best neural pipeline.',
     'long_description': '# Neural Pipeline Search (NePS)\n\n[![PyPI version](https://img.shields.io/pypi/v/neural-pipeline-search?color=informational)](https://pypi.org/project/neural-pipeline-search/)\n[![Python versions](https://img.shields.io/pypi/pyversions/neural-pipeline-search)](https://pypi.org/project/neural-pipeline-search/)\n[![License](https://img.shields.io/pypi/l/neural-pipeline-search?color=informational)](LICENSE)\n[![Tests](https://github.com/automl/neps/actions/workflows/tests.yaml/badge.svg)](https://github.com/automl/neps/actions)\n\nNePS helps deep learning experts to optimize the hyperparameters and/or architecture of their deep learning pipeline with:\n\n- Hyperparameter Optimization (HPO) ([example](neps_examples/basic_usage/hyperparameters.py))\n- Neural Architecture Search (NAS) ([example](neps_examples/basic_usage/architecture.py), [paper](https://openreview.net/forum?id=Ok58hMNXIQ))\n- Joint Architecture and Hyperparameter Search (JAHS) ([example](neps_examples/basic_usage/architecture_and_hyperparameters.py), [paper](https://openreview.net/forum?id=_HLcjaVlqJ))\n\nFor efficiency and convenience NePS allows you to\n\n- Add your intuition as priors for the search ([example HPO](neps_examples/efficiency/expert_priors_for_hyperparameters.py), [example JAHS](neps_examples/experimental/expert_priors_for_architecture_and_hyperparameters.py), [paper](https://openreview.net/forum?id=MMAeCXIa89))\n- Utilize low fidelity (e.g., low epoch) evaluations to focus on promising configurations ([example](neps_examples/efficiency/multi_fidelity.py), [paper](https://openreview.net/forum?id=ds21dwfBBH))\n- Trivially parallelize across machines ([example](neps_examples/efficiency/parallelization.md), [documentation](https://automl.github.io/neps/latest/parallelization/))\n\nOr [all of the above](neps_examples/efficiency/multi_fidelity_and_expert_priors.py) for maximum efficiency!\n\n## Note\n\nAs indicated with the `v0.x.x` version number, NePS is early stage code and APIs might change in the future.\n\n## Documentation\n\nPlease have a look at our [documentation](https://automl.github.io/neps/latest/) and [examples](neps_examples).\n\n## Installation\n\nUsing pip\n\n```bash\npip install neural-pipeline-search\n```\n\n## Usage\n\nUsing `neps` always follows the same pattern:\n\n1. Define a `run_pipeline` function that evaluates architectures/hyperparameters for your problem\n1. Define a search space `pipeline_space` of architectures/hyperparameters\n1. Call `neps.run` to optimize `run_pipeline` over `pipeline_space`\n\nIn code, the usage pattern can look like this:\n\n```python\nimport neps\nimport logging\n\n# 1. Define a function that accepts hyperparameters and computes the validation error\ndef run_pipeline(hyperparameter_a: float, hyperparameter_b: int):\n    validation_error = -hyperparameter_a * hyperparameter_b\n    return validation_error\n\n\n# 2. Define a search space of hyperparameters; use the same names as in run_pipeline\npipeline_space = dict(\n    hyperparameter_a=neps.FloatParameter(lower=0, upper=1),\n    hyperparameter_b=neps.IntegerParameter(lower=1, upper=100),\n)\n\n# 3. Call neps.run to optimize run_pipeline over pipeline_space\nlogging.basicConfig(level=logging.INFO)\nneps.run(\n    run_pipeline=run_pipeline,\n    pipeline_space=pipeline_space,\n    root_directory="usage_example",\n    max_evaluations_total=5,\n)\n```\n\nFor more details and features please have a look at our [documentation](https://automl.github.io/neps/latest/) and [examples](neps_examples).\n\n## Analysing runs\n\nSee our [documentation on analysing runs](https://automl.github.io/neps/latest/analyse).\n\n## Alternatives\n\nNePS does not cover your use-case? Have a look at [some alternatives](https://automl.github.io/neps/latest/alternatives).\n\n## Contributing\n\nPlease see the [documentation for contributors](https://automl.github.io/neps/latest/contributing/).\n',
     'author': 'Danny Stoll',
     'author_email': 'stolld@cs.uni-freiburg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/automl/neps',
```

### Comparing `neural_pipeline_search-0.8.2/PKG-INFO` & `neural_pipeline_search-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural-pipeline-search
-Version: 0.8.2
+Version: 0.8.3
 Summary: Neural Pipeline Search helps deep learning experts find the best neural pipeline.
 Home-page: https://github.com/automl/neps
 License: MIT
 Keywords: Neural Pipeline Search,Neural Architecture Search,Hyperparameter Optimization,AutoML
 Author: Danny Stoll
 Author-email: stolld@cs.uni-freiburg.de
 Requires-Python: >=3.7.1,<3.11
```

