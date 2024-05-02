# Comparing `tmp/qtealeaves-1.1.1.tar.gz` & `tmp/qtealeaves-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtealeaves-1.1.1.tar", last modified: Fri Apr 19 13:18:46 2024, max compression
+gzip compressed data, was "qtealeaves-1.1.2.tar", last modified: Thu May  2 13:15:55 2024, max compression
```

## Comparing `qtealeaves-1.1.1.tar` & `qtealeaves-1.1.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/
--rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/LICENSE
--rw-r--r--   0 quantum    (128) quantum    (128)     3285 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-1.1.1/README.md
--rw-r--r--   0 quantum    (128) quantum    (128)      101 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/pyproject.toml
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.523728 qtealeaves-1.1.1/qtealeaves/
--rw-r--r--   0 quantum    (128) quantum    (128)     1088 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/__init__.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.523728 qtealeaves-1.1.1/qtealeaves/convergence_parameters/
--rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/convergence_parameters/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20340 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params_finite_temp.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/emulator/
--rw-r--r--   0 quantum    (128) quantum    (128)     1485 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    89626 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/abstract_tn.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13132 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/attn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9504 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/ed_simulation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    42376 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/lptn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    22059 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/mpi_mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)   110894 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/mps_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19742 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/state_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    39080 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/tn_simulation.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2535 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/tnnode.py
--rw-r--r--   0 quantum    (128) quantum    (128)   168825 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/ttn_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    46305 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/tto_simulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2125 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/emulator/unitariesprojmeas.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/modeling/
--rw-r--r--   0 quantum    (128) quantum    (128)     1289 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6956 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/baseterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7625 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/blockterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    16787 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/localterm.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7379 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/plaquetteterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    32850 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/quantummodel.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-1.1.1/qtealeaves/modeling/stringterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13223 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm1d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13088 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm2d.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10657 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm3d.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/models/
--rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/models/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/models/bosehubbard.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/qtealeaves/models/quantumising.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/models/xxzmodel.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/mpos/
--rw-r--r--   0 quantum    (128) quantum    (128)     1239 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4018 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/abstracteffop.py
--rw-r--r--   0 quantum    (128) quantum    (128)    15982 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/densempos.py
--rw-r--r--   0 quantum    (128) quantum    (128)    15908 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/disentangler.py
--rw-r--r--   0 quantum    (128) quantum    (128)    76751 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/indexedtpo.py
--rw-r--r--   0 quantum    (128) quantum    (128)    23290 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/sparsematrixoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20242 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/sparsematrixproductoperator.py
--rw-r--r--   0 quantum    (128) quantum    (128)    21798 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/mpos/tensorproductoperator.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.527727 qtealeaves-1.1.1/qtealeaves/observables/
--rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-1.1.1/qtealeaves/observables/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6009 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/bond_entropy.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19724 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/custom_correlation.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4703 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/distance2pure.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5908 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/local.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7874 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/probabilities.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5653 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/projective.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5110 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/state2file.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5834 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/tensor_product.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5609 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/timecorrelator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6351 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/tnobase.py
--rw-r--r--   0 quantum    (128) quantum    (128)    18721 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/tnobservables.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10161 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/observables/weighted_sum.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/operators/
--rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/qtealeaves/operators/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2894 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/operators/bosonicoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2622 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/qtealeaves/operators/combinedoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/qtealeaves/operators/quditoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1368 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/operators/spinoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9216 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/operators/tnoperators.py
--rw-r--r--   0 quantum    (128) quantum    (128)    68904 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/simulation_setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/solvers/
--rw-r--r--   0 quantum    (128) quantum    (128)      698 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/solvers/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4067 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/solvers/eigen_solver.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7352 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/solvers/krylovexp_solver.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/tensors/
--rw-r--r--   0 quantum    (128) quantum    (128)      801 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    17043 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/abstracttensor.py
--rw-r--r--   0 quantum    (128) quantum    (128)    75601 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/tensor.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1663 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tensors/tensor_backend.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves/tooling/
--rw-r--r--   0 quantum    (128) quantum    (128)     1179 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/fortran_interfaces.py
--rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5883 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/lattice_layout.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4080 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/parameterized.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1768 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/permutations.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1785 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/tooling/restrictedclasses.py
--rw-r--r--   0 quantum    (128) quantum    (128)      531 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/qtealeaves/version.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/qtealeaves.egg-info/
--rw-r--r--   0 quantum    (128) quantum    (128)     3285 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/SOURCES.txt
--rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/dependency_links.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/requires.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-04-19 13:18:46.000000 qtealeaves-1.1.1/qtealeaves.egg-info/top_level.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/setup.cfg
--rw-r--r--   0 quantum    (128) quantum    (128)     2979 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-04-19 13:18:46.531727 qtealeaves-1.1.1/tests/
--rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/tests/tests_formatting.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/tests/tests_fortran_interface.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9311 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/tests/tests_hilbert_curvature.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2732 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_lattice_layout.py
--rw-r--r--   0 quantum    (128) quantum    (128)    27539 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_linter.py
--rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-1.1.1/tests/tests_model_terms.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9812 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_observables.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-1.1.1/tests/tests_operators.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2962 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_quantum_trajectories.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-1.1.1/tests/tests_rydberg_model.py
--rw-r--r--   0 quantum    (128) quantum    (128)     4401 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_simulation_setup.py
--rw-r--r--   0 quantum    (128) quantum    (128)    11537 2024-04-19 13:00:15.000000 qtealeaves-1.1.1/tests/tests_tn_simulation.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.799699 qtealeaves-1.1.2/
+-rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/LICENSE
+-rw-r--r--   0 quantum    (128) quantum    (128)     3319 2024-05-02 13:15:55.799699 qtealeaves-1.1.2/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2572 2023-12-13 17:32:06.000000 qtealeaves-1.1.2/README.md
+-rw-r--r--   0 quantum    (128) quantum    (128)      101 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/pyproject.toml
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.791699 qtealeaves-1.1.2/qtealeaves/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1088 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/__init__.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.791699 qtealeaves-1.1.2/qtealeaves/convergence_parameters/
+-rw-r--r--   0 quantum    (128) quantum    (128)      758 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/qtealeaves/convergence_parameters/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20340 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/convergence_parameters/conv_params.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6745 2024-01-12 22:24:30.000000 qtealeaves-1.1.2/qtealeaves/convergence_parameters/conv_params_finite_temp.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.791699 qtealeaves-1.1.2/qtealeaves/emulator/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1485 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    89626 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/abstract_tn.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13132 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/attn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9504 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/ed_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    42376 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/lptn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    22059 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/mpi_mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   110894 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/mps_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19742 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/state_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    39080 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/tn_simulation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2535 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/tnnode.py
+-rw-r--r--   0 quantum    (128) quantum    (128)   168825 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/ttn_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    46305 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/tto_simulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2125 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/emulator/unitariesprojmeas.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/modeling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1289 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6956 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/baseterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7625 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/blockterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    16787 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/localterm.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7379 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/plaquetteterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    32850 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/quantummodel.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5632 2024-02-26 14:55:43.000000 qtealeaves-1.1.2/qtealeaves/modeling/stringterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13223 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/twobodyterm1d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13088 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/twobodyterm2d.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10657 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/modeling/twobodyterm3d.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/models/
+-rw-r--r--   0 quantum    (128) quantum    (128)      766 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/qtealeaves/models/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2720 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/qtealeaves/models/bosehubbard.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4682 2023-10-26 07:55:27.000000 qtealeaves-1.1.2/qtealeaves/models/quantumising.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1736 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/qtealeaves/models/xxzmodel.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/mpos/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1239 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4018 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/abstracteffop.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15982 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/densempos.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15908 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/disentangler.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    76751 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/indexedtpo.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    23290 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/sparsematrixoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20242 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/sparsematrixproductoperator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    21798 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/mpos/tensorproductoperator.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/observables/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1530 2024-01-12 22:24:30.000000 qtealeaves-1.1.2/qtealeaves/observables/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6009 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/bond_entropy.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19724 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    12681 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/custom_correlation.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4703 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/distance2pure.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5908 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/local.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7874 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/probabilities.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5653 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/projective.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5110 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/state2file.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5834 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/tensor_product.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5609 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/timecorrelator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6351 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/tnobase.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    18721 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/tnobservables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10161 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/observables/weighted_sum.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/operators/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1004 2023-10-26 07:55:27.000000 qtealeaves-1.1.2/qtealeaves/operators/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2894 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/operators/bosonicoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2620 2024-05-02 10:53:18.000000 qtealeaves-1.1.2/qtealeaves/operators/combinedoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4143 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/qtealeaves/operators/quditoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1368 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/operators/spinoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9216 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/operators/tnoperators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    68904 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/simulation_setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/solvers/
+-rw-r--r--   0 quantum    (128) quantum    (128)      698 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/solvers/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4067 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/solvers/eigen_solver.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7352 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/solvers/krylovexp_solver.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.795699 qtealeaves-1.1.2/qtealeaves/tensors/
+-rw-r--r--   0 quantum    (128) quantum    (128)      801 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tensors/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17043 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tensors/abstracttensor.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    75601 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tensors/tensor.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1663 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tensors/tensor_backend.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.799699 qtealeaves-1.1.2/qtealeaves/tooling/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1179 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    17831 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/fortran_interfaces.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    47759 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5883 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4080 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/parameterized.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1768 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/permutations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1785 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/qtealeaves/tooling/restrictedclasses.py
+-rw-r--r--   0 quantum    (128) quantum    (128)      531 2024-05-02 10:53:18.000000 qtealeaves-1.1.2/qtealeaves/version.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.799699 qtealeaves-1.1.2/qtealeaves.egg-info/
+-rw-r--r--   0 quantum    (128) quantum    (128)     3319 2024-05-02 13:15:55.000000 qtealeaves-1.1.2/qtealeaves.egg-info/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-05-02 13:15:55.000000 qtealeaves-1.1.2/qtealeaves.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-05-02 13:15:55.000000 qtealeaves-1.1.2/qtealeaves.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       42 2024-05-02 13:15:55.000000 qtealeaves-1.1.2/qtealeaves.egg-info/requires.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-05-02 13:15:55.000000 qtealeaves-1.1.2/qtealeaves.egg-info/top_level.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-05-02 13:15:55.799699 qtealeaves-1.1.2/setup.cfg
+-rw-r--r--   0 quantum    (128) quantum    (128)     3041 2024-05-02 10:53:18.000000 qtealeaves-1.1.2/setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-02 13:15:55.799699 qtealeaves-1.1.2/tests/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1332 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/tests/tests_formatting.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1504 2023-10-26 07:55:27.000000 qtealeaves-1.1.2/tests/tests_fortran_interface.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9311 2023-10-26 07:55:27.000000 qtealeaves-1.1.2/tests/tests_hilbert_curvature.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2732 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/tests/tests_lattice_layout.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    27539 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/tests/tests_linter.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     5818 2023-10-26 07:55:27.000000 qtealeaves-1.1.2/tests/tests_model_terms.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9812 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/tests/tests_observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1858 2023-01-26 15:54:33.000000 qtealeaves-1.1.2/tests/tests_operators.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2962 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/tests/tests_quantum_trajectories.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2553 2022-11-30 17:54:07.000000 qtealeaves-1.1.2/tests/tests_rydberg_model.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     4401 2024-04-19 13:19:04.000000 qtealeaves-1.1.2/tests/tests_simulation_setup.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    14207 2024-05-02 10:53:18.000000 qtealeaves-1.1.2/tests/tests_tn_simulation.py
```

### Comparing `qtealeaves-1.1.1/LICENSE` & `qtealeaves-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/PKG-INFO` & `qtealeaves-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 1.1.1
+Version: 1.1.2
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
-Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Marco Rigobello, Nora Reinić, Simone Scarlatella
+Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Davide Rattacaso, Marco Rigobello, Nora Reinić, Simone Scarlatella, Darvin Wanisch
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `qtealeaves-1.1.1/README.md` & `qtealeaves-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/__init__.py` & `qtealeaves-1.1.2/qtealeaves/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/convergence_parameters/__init__.py` & `qtealeaves-1.1.2/qtealeaves/convergence_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params.py` & `qtealeaves-1.1.2/qtealeaves/convergence_parameters/conv_params.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/convergence_parameters/conv_params_finite_temp.py` & `qtealeaves-1.1.2/qtealeaves/convergence_parameters/conv_params_finite_temp.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/__init__.py` & `qtealeaves-1.1.2/qtealeaves/emulator/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/abstract_tn.py` & `qtealeaves-1.1.2/qtealeaves/emulator/abstract_tn.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/attn_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/attn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/ed_simulation.py` & `qtealeaves-1.1.2/qtealeaves/emulator/ed_simulation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/lptn_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/lptn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/mpi_mps_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/mpi_mps_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/mps_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/mps_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/state_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/state_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/tn_simulation.py` & `qtealeaves-1.1.2/qtealeaves/emulator/tn_simulation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/tnnode.py` & `qtealeaves-1.1.2/qtealeaves/emulator/tnnode.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/ttn_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/ttn_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/tto_simulator.py` & `qtealeaves-1.1.2/qtealeaves/emulator/tto_simulator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/emulator/unitariesprojmeas.py` & `qtealeaves-1.1.2/qtealeaves/emulator/unitariesprojmeas.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/__init__.py` & `qtealeaves-1.1.2/qtealeaves/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/baseterm.py` & `qtealeaves-1.1.2/qtealeaves/modeling/baseterm.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/blockterm2d.py` & `qtealeaves-1.1.2/qtealeaves/modeling/blockterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/localterm.py` & `qtealeaves-1.1.2/qtealeaves/modeling/localterm.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/plaquetteterm2d.py` & `qtealeaves-1.1.2/qtealeaves/modeling/plaquetteterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/quantummodel.py` & `qtealeaves-1.1.2/qtealeaves/modeling/quantummodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/stringterm1d.py` & `qtealeaves-1.1.2/qtealeaves/modeling/stringterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm1d.py` & `qtealeaves-1.1.2/qtealeaves/modeling/twobodyterm1d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm2d.py` & `qtealeaves-1.1.2/qtealeaves/modeling/twobodyterm2d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/modeling/twobodyterm3d.py` & `qtealeaves-1.1.2/qtealeaves/modeling/twobodyterm3d.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/models/__init__.py` & `qtealeaves-1.1.2/qtealeaves/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/models/bosehubbard.py` & `qtealeaves-1.1.2/qtealeaves/models/bosehubbard.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/models/quantumising.py` & `qtealeaves-1.1.2/qtealeaves/models/quantumising.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/models/xxzmodel.py` & `qtealeaves-1.1.2/qtealeaves/models/xxzmodel.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/__init__.py` & `qtealeaves-1.1.2/qtealeaves/mpos/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/abstracteffop.py` & `qtealeaves-1.1.2/qtealeaves/mpos/abstracteffop.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/densempos.py` & `qtealeaves-1.1.2/qtealeaves/mpos/densempos.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/disentangler.py` & `qtealeaves-1.1.2/qtealeaves/mpos/disentangler.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/indexedtpo.py` & `qtealeaves-1.1.2/qtealeaves/mpos/indexedtpo.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/sparsematrixoperator.py` & `qtealeaves-1.1.2/qtealeaves/mpos/sparsematrixoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/sparsematrixproductoperator.py` & `qtealeaves-1.1.2/qtealeaves/mpos/sparsematrixproductoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/mpos/tensorproductoperator.py` & `qtealeaves-1.1.2/qtealeaves/mpos/tensorproductoperator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/__init__.py` & `qtealeaves-1.1.2/qtealeaves/observables/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/bond_entropy.py` & `qtealeaves-1.1.2/qtealeaves/observables/bond_entropy.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/correlation.py` & `qtealeaves-1.1.2/qtealeaves/observables/correlation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/custom_correlation.py` & `qtealeaves-1.1.2/qtealeaves/observables/custom_correlation.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/distance2pure.py` & `qtealeaves-1.1.2/qtealeaves/observables/distance2pure.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/local.py` & `qtealeaves-1.1.2/qtealeaves/observables/local.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/probabilities.py` & `qtealeaves-1.1.2/qtealeaves/observables/probabilities.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/projective.py` & `qtealeaves-1.1.2/qtealeaves/observables/projective.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/state2file.py` & `qtealeaves-1.1.2/qtealeaves/observables/state2file.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/tensor_product.py` & `qtealeaves-1.1.2/qtealeaves/observables/tensor_product.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/timecorrelator.py` & `qtealeaves-1.1.2/qtealeaves/observables/timecorrelator.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/tnobase.py` & `qtealeaves-1.1.2/qtealeaves/observables/tnobase.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/tnobservables.py` & `qtealeaves-1.1.2/qtealeaves/observables/tnobservables.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/observables/weighted_sum.py` & `qtealeaves-1.1.2/qtealeaves/observables/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/operators/__init__.py` & `qtealeaves-1.1.2/qtealeaves/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/operators/bosonicoperators.py` & `qtealeaves-1.1.2/qtealeaves/operators/bosonicoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/operators/combinedoperators.py` & `qtealeaves-1.1.2/qtealeaves/operators/combinedoperators.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,13 +76,13 @@
         ----------
         key_a : str
             Operator name of class a.
         key_b : str
             Operator name of class b.
         """
 
-        def get_any_operator(self=self, key_a=key_a, key_b=key_b, **kwargs):
-            op_a = self.ops_a.get_operator(key_a, kwargs)
-            op_b = self.ops_b.get_operator(key_b, kwargs)
+        def get_any_operator(params, self=self, key_a=key_a, key_b=key_b):
+            op_a = self.ops_a.get_operator(key_a, params)
+            op_b = self.ops_b.get_operator(key_b, params)
             return np.kron(op_a, op_b)
 
         return get_any_operator
```

### Comparing `qtealeaves-1.1.1/qtealeaves/operators/quditoperators.py` & `qtealeaves-1.1.2/qtealeaves/operators/quditoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/operators/spinoperators.py` & `qtealeaves-1.1.2/qtealeaves/operators/spinoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/operators/tnoperators.py` & `qtealeaves-1.1.2/qtealeaves/operators/tnoperators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/simulation_setup.py` & `qtealeaves-1.1.2/qtealeaves/simulation_setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/solvers/__init__.py` & `qtealeaves-1.1.2/qtealeaves/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/solvers/eigen_solver.py` & `qtealeaves-1.1.2/qtealeaves/solvers/eigen_solver.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/solvers/krylovexp_solver.py` & `qtealeaves-1.1.2/qtealeaves/solvers/krylovexp_solver.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tensors/__init__.py` & `qtealeaves-1.1.2/qtealeaves/tensors/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tensors/abstracttensor.py` & `qtealeaves-1.1.2/qtealeaves/tensors/abstracttensor.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tensors/tensor.py` & `qtealeaves-1.1.2/qtealeaves/tensors/tensor.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tensors/tensor_backend.py` & `qtealeaves-1.1.2/qtealeaves/tensors/tensor_backend.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/__init__.py` & `qtealeaves-1.1.2/qtealeaves/tooling/__init__.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/fortran_interfaces.py` & `qtealeaves-1.1.2/qtealeaves/tooling/fortran_interfaces.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/hilbert_curvature.py` & `qtealeaves-1.1.2/qtealeaves/tooling/hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/lattice_layout.py` & `qtealeaves-1.1.2/qtealeaves/tooling/lattice_layout.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/parameterized.py` & `qtealeaves-1.1.2/qtealeaves/tooling/parameterized.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/permutations.py` & `qtealeaves-1.1.2/qtealeaves/tooling/permutations.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/tooling/restrictedclasses.py` & `qtealeaves-1.1.2/qtealeaves/tooling/restrictedclasses.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/qtealeaves/version.py` & `qtealeaves-1.1.2/qtealeaves/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """
 Version string, e.g., for installation script.
 """
-__version__ = "1.1.1"
+__version__ = "1.1.2"
```

### Comparing `qtealeaves-1.1.1/qtealeaves.egg-info/PKG-INFO` & `qtealeaves-1.1.2/qtealeaves.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: qtealeaves
-Version: 1.1.1
+Version: 1.1.2
 Summary: Quantum TEA's python tensor network library
 Home-page: https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git
-Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Marco Rigobello, Nora Reinić, Simone Scarlatella
+Author: Marco Ballarin, Giovanni Cataldi, Aurora Costantini, Daniel Jaschke, Giuseppe Magnifico, Simone Notarnicola, Alice Pagano, Luka Pavesic, Davide Rattacaso, Marco Rigobello, Nora Reinić, Simone Scarlatella, Darvin Wanisch
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `qtealeaves-1.1.1/qtealeaves.egg-info/SOURCES.txt` & `qtealeaves-1.1.2/qtealeaves.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/setup.py` & `qtealeaves-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,19 @@
             "Giovanni Cataldi",
             "Aurora Costantini",
             "Daniel Jaschke",
             "Giuseppe Magnifico",
             "Simone Notarnicola",
             "Alice Pagano",
             "Luka Pavesic",
+            "Davide Rattacaso",
             "Marco Rigobello",
             "Nora Reinić",
             "Simone Scarlatella",
+            "Darvin Wanisch",
         ]
     ),
     author_email="",
     description="Quantum TEA's python tensor network library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://baltig.infn.it/quantum_tea_leaves/py_api_quantum_tea_leaves.git",
```

### Comparing `qtealeaves-1.1.1/tests/tests_formatting.py` & `qtealeaves-1.1.2/tests/tests_formatting.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_fortran_interface.py` & `qtealeaves-1.1.2/tests/tests_fortran_interface.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_hilbert_curvature.py` & `qtealeaves-1.1.2/tests/tests_hilbert_curvature.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_lattice_layout.py` & `qtealeaves-1.1.2/tests/tests_lattice_layout.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_linter.py` & `qtealeaves-1.1.2/tests/tests_linter.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_model_terms.py` & `qtealeaves-1.1.2/tests/tests_model_terms.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_observables.py` & `qtealeaves-1.1.2/tests/tests_observables.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_operators.py` & `qtealeaves-1.1.2/tests/tests_operators.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_quantum_trajectories.py` & `qtealeaves-1.1.2/tests/tests_quantum_trajectories.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_rydberg_model.py` & `qtealeaves-1.1.2/tests/tests_rydberg_model.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_simulation_setup.py` & `qtealeaves-1.1.2/tests/tests_simulation_setup.py`

 * *Files identical despite different names*

### Comparing `qtealeaves-1.1.1/tests/tests_tn_simulation.py` & `qtealeaves-1.1.2/tests/tests_tn_simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import tempfile
 from shutil import rmtree
 import numpy as np
 
 import qtealeaves as qtl
 from qtealeaves import modeling
 from qtealeaves.models import get_quantum_ising_1d
+from qtealeaves.operators import TNCombinedOperators
 
 
 class TestsTNsimulation(unittest.TestCase):
     def setUp(self):
         """
         Provide some default settings.
         """
@@ -334,7 +335,80 @@
 
             simulation.run(params)
 
             sim_status = simulation.status(params)
             self.assertEqual(
                 sim_status, (0, 0, 1), msg=f"Failed for TN {tn_type} & finished."
             )
+
+    def test_combined_operators(self):
+        """Test if the combined operator work in a simulation."""
+        self.conv.max_iter = 5
+        self.conv.sim_params["max_bond_dimension"] = 8
+
+        model, my_ops = get_quantum_ising_1d()
+
+        my_cops = TNCombinedOperators(my_ops, my_ops)
+
+        cmodel = modeling.QuantumModel(1, "L")
+        cmodel += modeling.LocalTerm("sz.id", strength="g", prefactor=-1)
+        cmodel += modeling.LocalTerm("id.sz", strength="g", prefactor=-1)
+        cmodel += modeling.LocalTerm("sx.sx", strength="J", prefactor=-1)
+        cmodel += modeling.TwoBodyTerm1D(
+            ["id.sx", "sx.id"], shift=1, strength="J", prefactor=-1
+        )
+
+        my_obs = qtl.observables.TNObservables()
+
+        for tn_type in self.ansatz.keys():
+            # ------------------------------------------------------------------
+            # Simulation without combined operators
+
+            in_folder = self.in_folder + f"TN{tn_type}"
+            out_folder = self.out_folder + f"TN{tn_type}"
+
+            simulation = qtl.QuantumGreenTeaSimulation(
+                model,
+                my_ops,
+                self.conv,
+                my_obs,
+                tn_type=tn_type,
+                tensor_backend=2,
+                folder_name_input=in_folder,
+                folder_name_output=out_folder,
+                has_log_file=True,
+                verbosity=False,
+            )
+
+            params = {"L": 16, "g": 0.5, "J": 1.0}
+            simulation.run(params)
+            results = simulation.get_static_obs(params)
+            energy = results["energy"]
+
+            # ------------------------------------------------------------------
+            # Simulation with combined operators
+
+            in_folder = self.in_folder + f"TN{tn_type}_c"
+            out_folder = self.out_folder + f"TN{tn_type}_c"
+
+            simulation = qtl.QuantumGreenTeaSimulation(
+                cmodel,
+                my_cops,
+                self.conv,
+                my_obs,
+                tn_type=tn_type,
+                tensor_backend=2,
+                folder_name_input=in_folder,
+                folder_name_output=out_folder,
+                has_log_file=True,
+                verbosity=False,
+            )
+
+            params = {"L": 8, "g": 0.5, "J": 1.0}
+            simulation.run(params)
+            results = simulation.get_static_obs(params)
+            energy_c = results["energy"]
+
+            # ------------------------------------------------------------------
+            # Test we get the same energy
+
+            self.assertAlmostEqual(energy, energy_c, 7)
```

