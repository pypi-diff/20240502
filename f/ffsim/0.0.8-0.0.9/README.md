# Comparing `tmp/ffsim-0.0.8.tar.gz` & `tmp/ffsim-0.0.9.tar.gz`

## Comparing `ffsim-0.0.8.tar` & `ffsim-0.0.9.tar`

### file list

```diff
@@ -1,102 +1,116 @@
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 ffsim-0.0.8/Cargo.toml
--rw-r--r--   0     1001      127     1500 2023-10-14 20:24:25.000000 ffsim-0.0.8/.github/workflows/build-and-release.yml
--rw-r--r--   0     1001      127     1873 2023-10-14 20:24:25.000000 ffsim-0.0.8/.github/workflows/check.yml
--rw-r--r--   0     1001      127      751 2023-10-14 20:24:25.000000 ffsim-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0     1001      127     1880 2023-10-14 20:24:25.000000 ffsim-0.0.8/.gitignore
--rw-r--r--   0     1001      127    11357 2023-10-14 20:24:25.000000 ffsim-0.0.8/LICENSE
--rw-r--r--   0     1001      127     2703 2023-10-14 20:24:25.000000 ffsim-0.0.8/README.md
--rw-r--r--   0     1001      127      904 2023-10-14 20:24:25.000000 ffsim-0.0.8/asv.conf.json
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/benchmarks/__init__.py
--rw-r--r--   0     1001      127     3754 2023-10-14 20:24:25.000000 ffsim-0.0.8/benchmarks/gates.py
--rw-r--r--   0     1001      127     3515 2023-10-14 20:24:25.000000 ffsim-0.0.8/benchmarks/rust.py
--rw-r--r--   0     1001      127      103 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/api/index.rst
--rw-r--r--   0     1001      127     1240 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/conf.py
--rw-r--r--   0     1001      127      270 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/index.rst
--rw-r--r--   0     1001      127     4148 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/tutorials/01-introduction.ipynb
--rw-r--r--   0     1001      127     8458 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/tutorials/02-orbital-rotation.ipynb
--rw-r--r--   0     1001      127    14878 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/tutorials/03-double-factorized.ipynb
--rw-r--r--   0     1001      127    11037 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/tutorials/04-lucj.ipynb
--rw-r--r--   0     1001      127      168 2023-10-14 20:24:25.000000 ffsim-0.0.8/docs/tutorials/index.rst
--rw-r--r--   0     1001      127     1302 2023-10-14 20:24:25.000000 ffsim-0.0.8/pyproject.toml
--rw-r--r--   0     1001      127     1756 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/__init__.py
--rw-r--r--   0     1001      127      755 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/contract/__init__.py
--rw-r--r--   0     1001      127     8840 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/contract/diag_coulomb.py
--rw-r--r--   0     1001      127     5069 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/contract/hamiltonian.py
--rw-r--r--   0     1001      127     5520 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/contract/num_op_sum.py
--rw-r--r--   0     1001      127      915 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/gates/__init__.py
--rw-r--r--   0     1001      127    13791 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/gates/basic_gates.py
--rw-r--r--   0     1001      127     6086 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/gates/diag_coulomb.py
--rw-r--r--   0     1001      127     4748 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/gates/num_op_sum.py
--rw-r--r--   0     1001      127    12874 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/gates/orbital_rotation.py
--rw-r--r--   0     1001      127      698 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/hamiltonians/__init__.py
--rw-r--r--   0     1001      127    11750 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/hamiltonians/double_factorized_hamiltonian.py
--rw-r--r--   0     1001      127     2220 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/hamiltonians/molecular_hamiltonian.py
--rw-r--r--   0     1001      127      910 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/linalg/__init__.py
--rw-r--r--   0     1001      127    20334 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/linalg/double_factorized.py
--rw-r--r--   0     1001      127     5373 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/linalg/givens.py
--rw-r--r--   0     1001      127     1401 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/linalg/linalg.py
--rw-r--r--   0     1001      127     3642 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/linalg/predicates.py
--rw-r--r--   0     1001      127     4370 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/molecular_data.py
--rw-r--r--   0     1001      127      602 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/protocols/__init__.py
--rw-r--r--   0     1001      127     1434 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/protocols/linear_operator.py
--rw-r--r--   0     1001      127     1228 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/protocols/trace.py
--rw-r--r--   0     1001      127     7191 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/random.py
--rw-r--r--   0     1001      127      509 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/__init__.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/contract/__init__.py
--rw-r--r--   0     1001      127     3260 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/contract/diag_coulomb.py
--rw-r--r--   0     1001      127      828 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/contract/num_op_sum.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/gates/__init__.py
--rw-r--r--   0     1001      127     4812 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/gates/diag_coulomb.py
--rw-r--r--   0     1001      127      835 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/gates/num_op_sum.py
--rw-r--r--   0     1001      127     2590 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/slow/gates/orbital_rotation.py
--rw-r--r--   0     1001      127     4498 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/states.py
--rw-r--r--   0     1001      127     1777 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/testing.py
--rw-r--r--   0     1001      127      640 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/trotter/__init__.py
--rw-r--r--   0     1001      127    24377 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/trotter/qdrift.py
--rw-r--r--   0     1001      127     6269 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/trotter/trotter.py
--rw-r--r--   0     1001      127      554 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/variational/__init__.py
--rw-r--r--   0     1001      127    13994 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/variational/lucj.py
--rw-r--r--   0     1001      127     3519 2023-10-14 20:24:25.000000 ffsim-0.0.8/python/ffsim/wick.py
--rw-r--r--   0     1001      127     5809 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/contract/diag_coulomb.rs
--rw-r--r--   0     1001      127      495 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/contract/mod.rs
--rw-r--r--   0     1001      127     1335 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/contract/num_op_sum.rs
--rw-r--r--   0     1001      127     6333 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/gates/diag_coulomb.rs
--rw-r--r--   0     1001      127      542 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/gates/mod.rs
--rw-r--r--   0     1001      127     1230 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/gates/num_op_sum.rs
--rw-r--r--   0     1001      127     6900 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/gates/orbital_rotation.rs
--rw-r--r--   0     1001      127     1375 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/gates/phase_shift.rs
--rw-r--r--   0     1001      127     1895 2023-10-14 20:24:25.000000 ffsim-0.0.8/src/lib.rs
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/contract/__init__.py
--rw-r--r--   0     1001      127     4563 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/contract/diag_coulomb_test.py
--rw-r--r--   0     1001      127     2630 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/contract/num_op_sum_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/gates/__init__.py
--rw-r--r--   0     1001      127    11830 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/gates/basic_gates_test.py
--rw-r--r--   0     1001      127     5713 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/gates/diag_coulomb_test.py
--rw-r--r--   0     1001      127     2907 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/gates/num_op_sum_test.py
--rw-r--r--   0     1001      127     6872 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/gates/orbital_rotation_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/hamiltonians/__init__.py
--rw-r--r--   0     1001      127     3546 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/hamiltonians/double_factorized_hamiltonian_test.py
--rw-r--r--   0     1001      127     2357 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/hamiltonians/molecular_hamiltonian_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/linalg/__init__.py
--rw-r--r--   0     1001      127    11009 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/linalg/double_factorized_test.py
--rw-r--r--   0     1001      127     1378 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/linalg/givens_test.py
--rw-r--r--   0     1001      127      864 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/linalg/linalg_test.py
--rw-r--r--   0     1001      127     3506 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/random_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/__init__.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/contract/__init__.py
--rw-r--r--   0     1001      127     3834 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/contract/diag_coulomb_test.py
--rw-r--r--   0     1001      127     1764 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/contract/num_op_sum_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/gates/__init__.py
--rw-r--r--   0     1001      127     5875 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/gates/diag_coulomb_test.py
--rw-r--r--   0     1001      127     1760 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/gates/num_op_sum_test.py
--rw-r--r--   0     1001      127     4885 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/slow/gates/orbital_rotation_test.py
--rw-r--r--   0     1001      127     1202 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/states_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/trotter/__init__.py
--rw-r--r--   0     1001      127    13401 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/trotter/qdrift_test.py
--rw-r--r--   0     1001      127     2842 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/trotter/trotter_test.py
--rw-r--r--   0     1001      127      444 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/variational/__init__.py
--rw-r--r--   0     1001      127     4314 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/variational/lucj_test.py
--rw-r--r--   0     1001      127     3863 2023-10-14 20:24:25.000000 ffsim-0.0.8/tests/wick_test.py
--rw-r--r--   0     1001      127     1246 2023-10-14 20:24:25.000000 ffsim-0.0.8/tox.ini
--rw-r--r--   0     1001      127    29724 2023-10-14 20:24:25.000000 ffsim-0.0.8/Cargo.lock
--rw-r--r--   0        0        0     3783 1970-01-01 00:00:00.000000 ffsim-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 ffsim-0.0.9/Cargo.toml
+-rw-r--r--   0     1001      127     1500 2023-10-20 17:45:55.000000 ffsim-0.0.9/.github/workflows/build-and-release.yml
+-rw-r--r--   0     1001      127     1873 2023-10-20 17:45:55.000000 ffsim-0.0.9/.github/workflows/check.yml
+-rw-r--r--   0     1001      127      751 2023-10-20 17:45:55.000000 ffsim-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0     1001      127     1880 2023-10-20 17:45:55.000000 ffsim-0.0.9/.gitignore
+-rw-r--r--   0     1001      127    11357 2023-10-20 17:45:55.000000 ffsim-0.0.9/LICENSE
+-rw-r--r--   0     1001      127     2908 2023-10-20 17:45:55.000000 ffsim-0.0.9/README.md
+-rw-r--r--   0     1001      127      851 2023-10-20 17:45:55.000000 ffsim-0.0.9/asv.conf.json
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/benchmarks/__init__.py
+-rw-r--r--   0     1001      127     1406 2023-10-20 17:45:55.000000 ffsim-0.0.9/benchmarks/fermion_operator.py
+-rw-r--r--   0     1001      127     3754 2023-10-20 17:45:55.000000 ffsim-0.0.9/benchmarks/gates.py
+-rw-r--r--   0     1001      127     3514 2023-10-20 17:45:55.000000 ffsim-0.0.9/benchmarks/rust.py
+-rw-r--r--   0     1001      127      103 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/api/index.rst
+-rw-r--r--   0     1001      127     1240 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/conf.py
+-rw-r--r--   0     1001      127      270 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/index.rst
+-rw-r--r--   0     1001      127     4173 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/01-introduction.ipynb
+-rw-r--r--   0     1001      127     8415 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/02-orbital-rotation.ipynb
+-rw-r--r--   0     1001      127    14983 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/03-double-factorized.ipynb
+-rw-r--r--   0     1001      127    11142 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/04-lucj.ipynb
+-rw-r--r--   0     1001      127     4542 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/05-entanglement-forging.ipynb
+-rw-r--r--   0     1001      127     6815 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/06-fermion-operator.ipynb
+-rw-r--r--   0     1001      127      218 2023-10-20 17:45:55.000000 ffsim-0.0.9/docs/tutorials/index.rst
+-rw-r--r--   0     1001      127     1300 2023-10-20 17:45:55.000000 ffsim-0.0.9/pyproject.toml
+-rw-r--r--   0     1001      127     1775 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/__init__.py
+-rw-r--r--   0     1001      127     3917 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_lib.pyi
+-rw-r--r--   0     1001      127      509 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/__init__.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/contract/__init__.py
+-rw-r--r--   0     1001      127     3260 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/contract/diag_coulomb.py
+-rw-r--r--   0     1001      127      828 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/contract/num_op_sum.py
+-rw-r--r--   0     1001      127     9940 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/fermion_operator.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/gates/__init__.py
+-rw-r--r--   0     1001      127     4812 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/gates/diag_coulomb.py
+-rw-r--r--   0     1001      127      835 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/gates/num_op_sum.py
+-rw-r--r--   0     1001      127     2590 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/_slow/gates/orbital_rotation.py
+-rw-r--r--   0     1001      127      749 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/contract/__init__.py
+-rw-r--r--   0     1001      127     8838 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/contract/diag_coulomb.py
+-rw-r--r--   0     1001      127     5518 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/contract/num_op_sum.py
+-rw-r--r--   0     1001      127     2703 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/contract/one_body.py
+-rw-r--r--   0     1001      127     2001 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/fermion_action.py
+-rw-r--r--   0     1001      127      915 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/gates/__init__.py
+-rw-r--r--   0     1001      127    13791 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/gates/basic_gates.py
+-rw-r--r--   0     1001      127     6084 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/gates/diag_coulomb.py
+-rw-r--r--   0     1001      127     4746 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/gates/num_op_sum.py
+-rw-r--r--   0     1001      127    12872 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/gates/orbital_rotation.py
+-rw-r--r--   0     1001      127      654 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/hamiltonians/__init__.py
+-rw-r--r--   0     1001      127    12313 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/hamiltonians/double_factorized_hamiltonian.py
+-rw-r--r--   0     1001      127     2718 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/hamiltonians/molecular_hamiltonian.py
+-rw-r--r--   0     1001      127      913 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/linalg/__init__.py
+-rw-r--r--   0     1001      127    20334 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/linalg/double_factorized.py
+-rw-r--r--   0     1001      127     5373 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/linalg/givens.py
+-rw-r--r--   0     1001      127     2018 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/linalg/linalg.py
+-rw-r--r--   0     1001      127     3642 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/linalg/predicates.py
+-rw-r--r--   0     1001      127     4362 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/molecular_data.py
+-rw-r--r--   0     1001      127      768 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/protocols/__init__.py
+-rw-r--r--   0     1001      127     2760 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/protocols/apply_unitary.py
+-rw-r--r--   0     1001      127     2364 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/protocols/approximate_equality.py
+-rw-r--r--   0     1001      127     3719 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/protocols/linear_operator.py
+-rw-r--r--   0     1001      127     1228 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/protocols/trace.py
+-rw-r--r--   0     1001      127        0 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/py.typed
+-rw-r--r--   0     1001      127     7191 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/random.py
+-rw-r--r--   0     1001      127     4498 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/states.py
+-rw-r--r--   0     1001      127     1777 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/testing.py
+-rw-r--r--   0     1001      127      640 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/trotter/__init__.py
+-rw-r--r--   0     1001      127    24377 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/trotter/qdrift.py
+-rw-r--r--   0     1001      127     6269 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/trotter/trotter.py
+-rw-r--r--   0     1001      127      647 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/variational/__init__.py
+-rw-r--r--   0     1001      127     1252 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/variational/hopgate.py
+-rw-r--r--   0     1001      127    13366 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/variational/lucj.py
+-rw-r--r--   0     1001      127     2183 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/variational/multireference.py
+-rw-r--r--   0     1001      127     3519 2023-10-20 17:45:55.000000 ffsim-0.0.9/python/ffsim/wick.py
+-rw-r--r--   0     1001      127     5809 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/contract/diag_coulomb.rs
+-rw-r--r--   0     1001      127      495 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/contract/mod.rs
+-rw-r--r--   0     1001      127     1335 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/contract/num_op_sum.rs
+-rw-r--r--   0     1001      127    13139 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/fermion_operator.rs
+-rw-r--r--   0     1001      127     6333 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/gates/diag_coulomb.rs
+-rw-r--r--   0     1001      127      542 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/gates/mod.rs
+-rw-r--r--   0     1001      127     1230 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/gates/num_op_sum.rs
+-rw-r--r--   0     1001      127     6900 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/gates/orbital_rotation.rs
+-rw-r--r--   0     1001      127     1375 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/gates/phase_shift.rs
+-rw-r--r--   0     1001      127     1972 2023-10-20 17:45:55.000000 ffsim-0.0.9/src/lib.rs
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/__init__.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/contract/__init__.py
+-rw-r--r--   0     1001      127     3833 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/contract/diag_coulomb_test.py
+-rw-r--r--   0     1001      127     1763 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/contract/num_op_sum_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/gates/__init__.py
+-rw-r--r--   0     1001      127     5874 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/gates/diag_coulomb_test.py
+-rw-r--r--   0     1001      127     1759 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/gates/num_op_sum_test.py
+-rw-r--r--   0     1001      127     4884 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/_slow/gates/orbital_rotation_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/contract/__init__.py
+-rw-r--r--   0     1001      127     4563 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/contract/diag_coulomb_test.py
+-rw-r--r--   0     1001      127     2630 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/contract/num_op_sum_test.py
+-rw-r--r--   0     1001      127     1213 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/fermion_action_test.py
+-rw-r--r--   0     1001      127    16184 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/fermion_operator_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/gates/__init__.py
+-rw-r--r--   0     1001      127    13107 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/gates/basic_gates_test.py
+-rw-r--r--   0     1001      127     5675 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/gates/diag_coulomb_test.py
+-rw-r--r--   0     1001      127     2866 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/gates/num_op_sum_test.py
+-rw-r--r--   0     1001      127     6815 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/gates/orbital_rotation_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/hamiltonians/__init__.py
+-rw-r--r--   0     1001      127     3596 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/hamiltonians/double_factorized_hamiltonian_test.py
+-rw-r--r--   0     1001      127     2356 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/hamiltonians/molecular_hamiltonian_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/linalg/__init__.py
+-rw-r--r--   0     1001      127    11004 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/linalg/double_factorized_test.py
+-rw-r--r--   0     1001      127     1378 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/linalg/givens_test.py
+-rw-r--r--   0     1001      127     1439 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/linalg/linalg_test.py
+-rw-r--r--   0     1001      127     3506 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/random_test.py
+-rw-r--r--   0     1001      127     1169 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/states_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/trotter/__init__.py
+-rw-r--r--   0     1001      127    13335 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/trotter/qdrift_test.py
+-rw-r--r--   0     1001      127     2867 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/trotter/trotter_test.py
+-rw-r--r--   0     1001      127      444 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/variational/__init__.py
+-rw-r--r--   0     1001      127     4309 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/variational/lucj_test.py
+-rw-r--r--   0     1001      127     3789 2023-10-20 17:45:55.000000 ffsim-0.0.9/tests/wick_test.py
+-rw-r--r--   0     1001      127     1246 2023-10-20 17:45:55.000000 ffsim-0.0.9/tox.ini
+-rw-r--r--   0     1001      127    29724 2023-10-20 17:45:55.000000 ffsim-0.0.9/Cargo.lock
+-rw-r--r--   0        0        0     3988 1970-01-01 00:00:00.000000 ffsim-0.0.9/PKG-INFO
```

### Comparing `ffsim-0.0.8/Cargo.toml` & `ffsim-0.0.9/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/.github/workflows/build-and-release.yml` & `ffsim-0.0.9/.github/workflows/build-and-release.yml`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/.github/workflows/check.yml` & `ffsim-0.0.9/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/.github/workflows/docs.yml` & `ffsim-0.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/.gitignore` & `ffsim-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/LICENSE` & `ffsim-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/README.md` & `ffsim-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -103,7 +103,19 @@
 ```
 
 You can also use `pytest` to run the tests directly. For example,
 
 ```bash
 pytest tests/
 ```
+
+## Cite ffsim
+
+You can cite ffsim using the following BibTeX:
+
+```bibtex
+@software{ffsim,
+  author = {{The ffsim developers}},
+  title = {ffsim},
+  url = {https://github.com/qiskit-community/ffsim}
+}
+```
```

### Comparing `ffsim-0.0.8/asv.conf.json` & `ffsim-0.0.9/asv.conf.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977678571428571%*

 * *Differences: {"'matrix'": "{'env_nobuild': {'RAYON_NUM_THREADS': '1'}}"}*

```diff
@@ -12,18 +12,15 @@
     "environment_type": "virtualenv",
     "html_dir": ".asv/html",
     "matrix": {
         "env_nobuild": {
             "MKL_NUM_THREADS": "1",
             "OMP_NUM_THREADS": "1",
             "OPENBLAS_NUM_THREADS": "1",
-            "RAYON_NUM_THREADS": [
-                "1",
-                "6"
-            ]
+            "RAYON_NUM_THREADS": "1"
         }
     },
     "project": "ffsim",
     "project_url": "https://github.com/qiskit-community/ffsim",
     "pythons": [
         "3.10"
     ],
```

### Comparing `ffsim-0.0.8/benchmarks/gates.py` & `ffsim-0.0.9/benchmarks/gates.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/benchmarks/rust.py` & `ffsim-0.0.9/benchmarks/rust.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 import numpy as np
 import scipy.linalg
 
 import ffsim
-from ffsim._ffsim import (
+from ffsim._lib import (
     apply_givens_rotation_in_place,
     apply_single_column_transformation_in_place,
 )
 from ffsim.gates.orbital_rotation import (
     _zero_one_subspace_indices,
     gen_orbital_rotation_index,
 )
-from ffsim.slow.gates.orbital_rotation import (
+from ffsim._slow.gates.orbital_rotation import (
     apply_givens_rotation_in_place_slow,
     apply_single_column_transformation_in_place_slow,
 )
 
 
 class RustBenchmark:
     """Benchmark Rust functions."""
```

### Comparing `ffsim-0.0.8/docs/conf.py` & `ffsim-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/docs/tutorials/01-introduction.ipynb` & `ffsim-0.0.9/docs/tutorials/01-introduction.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916071428571429%*

 * *Differences: {"'cells'": "{1: {'execution_count': None}, 3: {'execution_count': None, 'source': {insert: [(2, "*

 * *            "'dim_a, dim_b = ffsim.dims(norb, nelec)\\n'), (3, 'dim = ffsim.dim(norb, nelec)\\n'), "*

 * *            "(4, '\\n'), (5, 'assert dim_a == comb(norb, n_alpha, exact=True)\\n'), (6, 'assert "*

 * *            "dim_b == comb(norb, n_beta, exact=True)\\n'), (7, 'assert dim == dim_a * dim_b\\n'), "*

 * *            "(8, 'assert vec.shape == (dim,)')], delete: [7, 6, 5, 4, 3, 2]}}, 5: "*

 * *            "{'execution_count […]*

```diff
@@ -9,15 +9,15 @@
                 "ffsim is a software library for simulating fermionic quantum circuits that conserve particle number and the Z component of spin. By taking advantage of these symmetries, it can simulate these circuits much more efficiently than a generic quantum circuit simulator.\n",
                 "\n",
                 "ffsim is a rather \"low-level\" software library. It does not have a class for representing quantum circuits. The primary way of using ffsim is by calling functions that transform statevectors represented directly as NumPy arrays. As an example, the following code shows how to create a Slater determinant and apply an orbital rotation to it."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import ffsim\n",
                 "\n",
                 "# Set the number of orbitals and their occupancies\n",
                 "norb = 6\n",
@@ -48,38 +48,39 @@
                 "$$\n",
                 "\n",
                 "For convenience, ffsim includes functions to calculate these dimensions."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "from scipy.special import comb\n",
                 "\n",
-                "dim_a = comb(norb, n_alpha, exact=True)\n",
-                "dim_b = comb(norb, n_beta, exact=True)\n",
-                "dim = dim_a * dim_b\n",
-                "assert vec.shape == (dim,)\n",
-                "assert ffsim.dims(norb, nelec) == (dim_a, dim_b)\n",
-                "assert ffsim.dim(norb, nelec) == dim"
+                "dim_a, dim_b = ffsim.dims(norb, nelec)\n",
+                "dim = ffsim.dim(norb, nelec)\n",
+                "\n",
+                "assert dim_a == comb(norb, n_alpha, exact=True)\n",
+                "assert dim_b == comb(norb, n_beta, exact=True)\n",
+                "assert dim == dim_a * dim_b\n",
+                "assert vec.shape == (dim,)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "This representation of the statevector is the same as that used in standard full configuration interaction (FCI) routines. It is often convenient to represent the statevector as a matrix whose rows are indexed by \"$\\alpha$-strings\" describing the occupancies of the $\\alpha$ orbitals, and columns indexed by \"$\\beta$-strings\" describing the occupancies of the $\\beta$ orbitals. To convert the vector into this representation, simply reshape it:"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "reshaped_vec = vec.reshape((dim_a, dim_b))"
             ]
         },
         {
@@ -102,14 +103,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.10.13"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `ffsim-0.0.8/docs/tutorials/02-orbital-rotation.ipynb` & `ffsim-0.0.9/docs/tutorials/02-orbital-rotation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982278138528139%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(13, 'hamiltonian = "*

 * *            "ffsim.contract.one_body_linop(one_body_tensor, norb=norb, nelec=nelec)\\n')], delete: "*

 * *            '[15, 14, 13]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.13'}}"}*

```diff
@@ -114,17 +114,15 @@
                 "n_alpha, n_beta = nelec\n",
                 "occupied_orbitals = (range(n_alpha), range(n_beta))\n",
                 "\n",
                 "# Generate a random quadratic Hamiltonian\n",
                 "one_body_tensor = ffsim.random.random_hermitian(norb, seed=1234)\n",
                 "\n",
                 "# Convert the Hamiltonian to a LinearOperator\n",
-                "hamiltonian = ffsim.contract.hamiltonian_linop(\n",
-                "    one_body_tensor=one_body_tensor, norb=norb, nelec=nelec\n",
-                ")\n",
+                "hamiltonian = ffsim.contract.one_body_linop(one_body_tensor, norb=norb, nelec=nelec)\n",
                 "\n",
                 "# Get the ground state of the Hamiltonian\n",
                 "eigs, vecs = scipy.sparse.linalg.eigsh(hamiltonian, which=\"LA\", k=1)\n",
                 "eig = eigs[0]\n",
                 "vec = vecs[:, 0]"
             ]
         },
@@ -202,14 +200,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.10.13"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `ffsim-0.0.8/docs/tutorials/03-double-factorized.ipynb` & `ffsim-0.0.9/docs/tutorials/03-double-factorized.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997235863095238%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(5, \'mol.build(atom=[["H", (0, 0, 0)], ["H", (0, 0, '*

 * *            '1.8)]], basis="sto-6g", symmetry="d2h")\\n\'), (16, \'df_hamiltonian = '*

 * *            "ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(\\n'), (17, '    "*

 * *            "mol_hamiltonian\\n'), (18, ')')], delete: [19, 8, 7, 6, 5]}}, 2: {'source': ['Here, "*

 * *            '`mol_hamiltonian` is an instance of `MolecularHamiltonian`, a dataclass that stores '*

 * *            'the one- and two-body tenso […]*

```diff
@@ -45,36 +45,35 @@
             "outputs": [],
             "source": [
                 "import pyscf\n",
                 "import ffsim\n",
                 "\n",
                 "# Build an H2 molecule\n",
                 "mol = pyscf.gto.Mole()\n",
-                "mol.build(\n",
-                "    atom=[[\"H\", (0, 0, 0)], [\"H\", (0, 0, 1.8)]],\n",
-                "    basis=\"sto-6g\",\n",
-                ")\n",
+                "mol.build(atom=[[\"H\", (0, 0, 0)], [\"H\", (0, 0, 1.8)]], basis=\"sto-6g\", symmetry=\"d2h\")\n",
                 "hartree_fock = pyscf.scf.RHF(mol)\n",
                 "hartree_fock.kernel()\n",
                 "\n",
                 "# Get molecular data and molecular Hamiltonian (one- and two-body tensors)\n",
                 "mol_data = ffsim.MolecularData.from_hartree_fock(hartree_fock)\n",
                 "norb = mol_data.norb\n",
                 "nelec = mol_data.nelec\n",
                 "mol_hamiltonian = mol_data.hamiltonian\n",
                 "\n",
                 "# Get the Hamiltonian in the double-factorized representation\n",
-                "df_hamiltonian = ffsim.double_factorized_hamiltonian(mol_hamiltonian)"
+                "df_hamiltonian = ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(\n",
+                "    mol_hamiltonian\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The function `double_factorized_hamiltonian` returns an object of type `DoubleFactorizedHamiltonian` which is just a dataclass that stores the updated one-body-tensor, diagonal Coulomb matrices, and orbital rotations. In the cell below, we print out the tensors describing the original and double-factorized representations."
+                "Here, `mol_hamiltonian` is an instance of `MolecularHamiltonian`, a dataclass that stores the one- and two-body tensors, and `df_hamiltonian` is an instance of `DoubleFactorizedHamiltonian`, a dataclass that stores the updated one-body-tensor, diagonal Coulomb matrices, and orbital rotations. In the cell below, we print out the tensors describing the original and double-factorized representations."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -400,14 +399,14 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.10.13"
         },
         "orig_nbformat": 4
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `ffsim-0.0.8/docs/tutorials/04-lucj.ipynb` & `ffsim-0.0.9/docs/tutorials/04-lucj.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990024478471584%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'import pyscf.mcscf\\n'), (5, 'bond_distance = "*

 * *            '2.678\\n\'), (6, \'a = 0.5 * bond_distance\\n\'), (20, \'    symmetry="d2h",\\n\')], '*

 * *            'delete: [4]}}, 2: {\'source\': {insert: [(19, "In the code cell below, we run CCSD to '*

 * *            "get the t2 amplitudes for initializing the ansatz. We'll create an ansatz operator "*

 * *            "with 2 repetitions ($L = 2$). For our reference state, we'll use the Hartree-Fock "*

 * *            'state. Since […]*

```diff
@@ -12,31 +12,34 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pyscf\n",
+                "import pyscf.mcscf\n",
                 "import ffsim\n",
                 "\n",
                 "# Build a stretched ethene molecule\n",
-                "a = 1.339\n",
+                "bond_distance = 2.678\n",
+                "a = 0.5 * bond_distance\n",
                 "b = a + 0.5626\n",
                 "c = 0.9289\n",
                 "mol = pyscf.gto.Mole()\n",
                 "mol.build(\n",
                 "    atom=[\n",
                 "        [\"C\", (0, 0, a)],\n",
                 "        [\"C\", (0, 0, -a)],\n",
                 "        [\"H\", (0, c, b)],\n",
                 "        [\"H\", (0, -c, b)],\n",
                 "        [\"H\", (0, c, -b)],\n",
                 "        [\"H\", (0, -c, -b)],\n",
                 "    ],\n",
                 "    basis=\"sto-6g\",\n",
+                "    symmetry=\"d2h\",\n",
                 ")\n",
                 "hartree_fock = pyscf.scf.RHF(mol)\n",
                 "hartree_fock.kernel()\n",
                 "\n",
                 "# Define active space\n",
                 "active_space = range(mol.nelectron // 2 - 2, mol.nelectron // 2 + 2)\n",
                 "\n",
@@ -73,47 +76,45 @@
                 "    \\mathcal{J} = \\frac12\\sum_{ij,\\sigma \\tau} \\mathbf{J}^{\\sigma \\tau}_{ij} n_{i,\\sigma} n_{j,\\tau}.\n",
                 "$$\n",
                 "\n",
                 "Note that this expression for the diagonal Coulomb operator is more general than the one introduced in [the previous tutorial](./03-double-factorized.ipynb) because the matrices $\\mathbf{J}^{\\sigma \\tau}$ are indexed by the spins $\\sigma$ and $\\tau$. In order that the operator commutes with the total spin operator, we enforce that $\\mathbf{J}^{\\alpha\\alpha} = \\mathbf{J}^{\\beta\\beta}$ and $\\mathbf{J}^{\\alpha\\beta} = \\mathbf{J}^{\\beta\\alpha}$. As a result, we have two sets of matrices for describing the diagonal Coulomb operators: \"alpha-alpha\" matrices containing coefficients for terms involving the same spin, and \"alpha-beta\" matrices containing coefficients for terms involving different spins.\n",
                 "\n",
                 "In ffsim, the UCJ ansatz operator $\\prod_{k = 1}^L \\mathcal{W_k} e^{i \\mathcal{J}_k} \\mathcal{W_k^\\dagger}$ is represented by the `UCJOperator` class, which is just a dataclass that stores the diagonal Coulomb matrices and orbital rotations. A constructor method is provided to initialize the operator from a truncated double factorization of t2 amplitudes (e.g. from CCSD or MP2).\n",
                 "\n",
-                "In the code cell below, we run CCSD to get the t2 amplitudes for initializing the ansatz. We'll create an ansatz operator with 2 repetitions ($L = 2$). For our reference state, we'll use the Hartree-Fock state. We use the function `apply_ucj_operator` to apply the ansatz operator to the reference state to obtain the ansatz state. Finally, we compute the energy of the ansatz state."
+                "In the code cell below, we run CCSD to get the t2 amplitudes for initializing the ansatz. We'll create an ansatz operator with 2 repetitions ($L = 2$). For our reference state, we'll use the Hartree-Fock state. Since `UCJOperator` defines a unitary effect, we can use the function `apply_unitary` to apply the ansatz operator to the reference state to obtain the ansatz state. Finally, we compute the energy of the ansatz state."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from pyscf import cc\n",
                 "\n",
                 "# Get CCSD t2 amplitudes for initializing the ansatz\n",
                 "ccsd = cc.CCSD(\n",
                 "    hartree_fock,\n",
-                "    frozen=[i for i in range(hartree_fock.mo_coeff.shape[0]) if i not in active_space],\n",
+                "    frozen=[i for i in range(hartree_fock.mol.nao_nr()) if i not in active_space],\n",
                 ")\n",
                 "_, t1, t2 = ccsd.kernel()\n",
                 "\n",
                 "# Construct UCJ operator\n",
                 "n_reps = 2\n",
                 "operator = ffsim.UCJOperator.from_t_amplitudes(t2, n_reps=n_reps)\n",
                 "\n",
                 "# Construct the Hartree-Fock state to use as the reference state\n",
                 "n_alpha, n_beta = nelec\n",
                 "reference_state = ffsim.slater_determinant(\n",
                 "    norb=norb, occupied_orbitals=(range(n_alpha), range(n_beta))\n",
                 ")\n",
                 "\n",
                 "# Apply the operator to the reference state\n",
-                "ansatz_state = ffsim.apply_ucj_operator(\n",
-                "    reference_state, operator, norb=norb, nelec=nelec\n",
-                ")\n",
+                "ansatz_state = ffsim.apply_unitary(reference_state, operator, norb=norb, nelec=nelec)\n",
                 "\n",
                 "# Compute the energy \u27e8\u03c8|H|\u03c8\u27e9 of the ansatz state\n",
                 "hamiltonian = ffsim.linear_operator(mol_hamiltonian, norb=norb, nelec=nelec)\n",
                 "energy = np.real(np.vdot(ansatz_state, hamiltonian @ ansatz_state))\n",
                 "print(f\"Energy at initialialization: {energy}\")"
             ]
         },
@@ -135,15 +136,15 @@
                 "import scipy.optimize\n",
                 "\n",
                 "\n",
                 "def fun(x):\n",
                 "    # Initialize the ansatz operator from the parameter vector\n",
                 "    operator = ffsim.UCJOperator.from_parameters(x, norb=norb, n_reps=n_reps)\n",
                 "    # Apply the ansatz operator to the reference state\n",
-                "    final_state = ffsim.apply_ucj_operator(\n",
+                "    final_state = ffsim.apply_unitary(\n",
                 "        reference_state, operator, norb=norb, nelec=(n_alpha, n_beta)\n",
                 "    )\n",
                 "    # Return the energy \u27e8\u03c8|H|\u03c8\u27e9 of the ansatz state\n",
                 "    return np.real(np.vdot(final_state, hamiltonian @ final_state))\n",
                 "\n",
                 "\n",
                 "result = scipy.optimize.minimize(\n",
@@ -190,15 +191,15 @@
                 "    operator = ffsim.UCJOperator.from_parameters(\n",
                 "        x,\n",
                 "        norb=norb,\n",
                 "        n_reps=n_reps,\n",
                 "        alpha_alpha_indices=alpha_alpha_indices,\n",
                 "        alpha_beta_indices=alpha_beta_indices,\n",
                 "    )\n",
-                "    final_state = ffsim.apply_ucj_operator(\n",
+                "    final_state = ffsim.apply_unitary(\n",
                 "        reference_state, operator, norb=norb, nelec=(n_alpha, n_beta)\n",
                 "    )\n",
                 "    return np.real(np.vdot(final_state, hamiltonian @ final_state))\n",
                 "\n",
                 "\n",
                 "result = scipy.optimize.minimize(\n",
                 "    fun,\n",
```

### Comparing `ffsim-0.0.8/pyproject.toml` & `ffsim-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "ffsim"
 requires-python = ">=3.8"
-version = "0.0.8"
+version = "0.0.9"
 description = "Faster simulations of fermionic quantum circuits."
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
-dependencies = ["numpy", "opt_einsum>=3.3", "pyscf>=2.3.0", "scipy"]
+dependencies = ["numpy", "opt_einsum>=3.3", "pyscf==2.4.0", "scipy"]
 
 [project.urls]
 Homepage = "https://github.com/qiskit-community/ffsim"
 Documentation = "https://qiskit-community.github.io/ffsim/"
 
 [project.optional-dependencies]
 dev = [
@@ -33,15 +33,15 @@
     "sphinx",
     "sphinx-autodoc-typehints",
     "tox",
 ]
 
 [tool.maturin]
 python-source = "python"
-module-name = "ffsim._ffsim"
+module-name = "ffsim._lib"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.ruff]
 select = ["E", "F", "I"]
 src = ["python"]
```

### Comparing `ffsim-0.0.8/python/ffsim/__init__.py` & `ffsim-0.0.9/python/ffsim/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,51 +18,45 @@
     protocols,
     random,
     states,
     testing,
     trotter,
     variational,
 )
-from ffsim.contract import (
-    contract_diag_coulomb,
-    contract_num_op_sum,
-    diag_coulomb_linop,
-    hamiltonian_linop,
-    hamiltonian_trace,
-    num_op_sum_linop,
-)
+from ffsim._lib import FermionOperator
+from ffsim.fermion_action import FermionAction, cre, cre_a, cre_b, des, des_a, des_b
 from ffsim.gates import (
     apply_diag_coulomb_evolution,
     apply_fsim_gate,
     apply_givens_rotation,
     apply_hop_gate,
     apply_num_interaction,
     apply_num_num_interaction,
     apply_num_op_prod_interaction,
     apply_num_op_sum_evolution,
     apply_orbital_rotation,
     apply_tunneling_interaction,
 )
-from ffsim.hamiltonians import (
-    DoubleFactorizedHamiltonian,
-    MolecularHamiltonian,
-    double_factorized_hamiltonian,
-)
+from ffsim.hamiltonians import DoubleFactorizedHamiltonian, MolecularHamiltonian
 from ffsim.molecular_data import MolecularData
 from ffsim.protocols import (
+    SupportsApplyUnitary,
+    SupportsApproximateEquality,
     SupportsLinearOperator,
     SupportsTrace,
+    apply_unitary,
+    approx_eq,
     linear_operator,
     trace,
 )
 from ffsim.states import (
     dim,
     dims,
     one_hot,
     slater_determinant,
     slater_determinant_one_rdm,
 )
 from ffsim.trotter import (
     simulate_qdrift_double_factorized,
     simulate_trotter_double_factorized,
 )
-from ffsim.variational import UCJOperator, apply_ucj_operator
+from ffsim.variational import HopGateAnsatzOperator, UCJOperator, multireference_state
```

### Comparing `ffsim-0.0.8/python/ffsim/contract/__init__.py` & `ffsim-0.0.9/python/ffsim/hamiltonians/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,12 +4,11 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Functions for contracting tensors and constructing linear operators."""
+"""Classes for representing Hamiltonians."""
 
-from ffsim.contract.diag_coulomb import contract_diag_coulomb, diag_coulomb_linop
-from ffsim.contract.hamiltonian import hamiltonian_linop, hamiltonian_trace
-from ffsim.contract.num_op_sum import contract_num_op_sum, num_op_sum_linop
+from ffsim.hamiltonians.double_factorized_hamiltonian import DoubleFactorizedHamiltonian
+from ffsim.hamiltonians.molecular_hamiltonian import MolecularHamiltonian
```

### Comparing `ffsim-0.0.8/python/ffsim/contract/diag_coulomb.py` & `ffsim-0.0.9/python/ffsim/contract/diag_coulomb.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 
 import numpy as np
 import scipy.sparse.linalg
 from pyscf.fci import cistring
 from scipy.special import comb
 
-from ffsim._ffsim import (
+from ffsim._lib import (
     contract_diag_coulomb_into_buffer_num_rep,
     contract_diag_coulomb_into_buffer_z_rep,
 )
 from ffsim.gates.orbital_rotation import (
     apply_orbital_rotation,
     gen_orbital_rotation_index,
 )
```

### Comparing `ffsim-0.0.8/python/ffsim/contract/num_op_sum.py` & `ffsim-0.0.9/python/ffsim/contract/num_op_sum.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 
 import numpy as np
 import scipy.sparse.linalg
 from pyscf.fci import cistring
 from scipy.special import comb
 
-from ffsim._ffsim import (
+from ffsim._lib import (
     contract_num_op_sum_spin_into_buffer,
 )
 from ffsim.gates.orbital_rotation import (
     apply_orbital_rotation,
     gen_orbital_rotation_index,
 )
 from ffsim.states import dim
```

### Comparing `ffsim-0.0.8/python/ffsim/gates/__init__.py` & `ffsim-0.0.9/python/ffsim/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/gates/basic_gates.py` & `ffsim-0.0.9/python/ffsim/gates/basic_gates.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/gates/diag_coulomb.py` & `ffsim-0.0.9/python/ffsim/gates/diag_coulomb.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from typing import cast
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
-from ffsim._ffsim import (
+from ffsim._lib import (
     apply_diag_coulomb_evolution_in_place_num_rep,
     apply_diag_coulomb_evolution_in_place_z_rep,
 )
 from ffsim.gates.orbital_rotation import apply_orbital_rotation
 
 
 def apply_diag_coulomb_evolution(
```

### Comparing `ffsim-0.0.8/python/ffsim/gates/num_op_sum.py` & `ffsim-0.0.9/python/ffsim/gates/num_op_sum.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from __future__ import annotations
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
-from ffsim._ffsim import apply_num_op_sum_evolution_in_place
+from ffsim._lib import apply_num_op_sum_evolution_in_place
 from ffsim.gates.orbital_rotation import apply_orbital_rotation
 
 
 def apply_num_op_sum_evolution(
     vec: np.ndarray,
     coeffs: np.ndarray,
     time: float,
```

### Comparing `ffsim-0.0.8/python/ffsim/gates/orbital_rotation.py` & `ffsim-0.0.9/python/ffsim/gates/orbital_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from typing import Literal, overload
 
 import numpy as np
 import scipy.linalg
 from pyscf.fci import cistring
 from scipy.special import comb
 
-from ffsim._ffsim import (
+from ffsim._lib import (
     apply_givens_rotation_in_place,
     apply_phase_shift_in_place,
     apply_single_column_transformation_in_place,
     gen_orbital_rotation_index_in_place,
 )
 from ffsim.linalg import givens_decomposition, lup
```

### Comparing `ffsim-0.0.8/python/ffsim/hamiltonians/double_factorized_hamiltonian.py` & `ffsim-0.0.9/python/ffsim/hamiltonians/double_factorized_hamiltonian.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,171 @@
             one_body_tensor=self.one_body_tensor - one_body_correction,
             diag_coulomb_mats=self.diag_coulomb_mats,
             orbital_rotations=self.orbital_rotations,
             constant=self.constant - constant_correction,
             z_representation=False,
         )
 
+    @staticmethod
+    def from_molecular_hamiltonian(
+        hamiltonian: MolecularHamiltonian,
+        *,
+        z_representation: bool = False,
+        tol: float = 1e-8,
+        max_vecs: int | None = None,
+        optimize: bool = False,
+        method: str = "L-BFGS-B",
+        options: dict | None = None,
+        diag_coulomb_mask: np.ndarray | None = None,
+        cholesky: bool = True,
+    ) -> DoubleFactorizedHamiltonian:
+        r"""Double-factorized decomposition of a molecular Hamiltonian.
+
+        The double-factorized decomposition acts on a Hamiltonian of the form
+
+        .. math::
+
+            H = \sum_{pq, \sigma} h_{pq} a^\dagger_{p, \sigma} a_{q, \sigma}
+                + \frac12 \sum_{pqrs, \sigma \tau} h_{pqrs}
+                a^\dagger_{p, \sigma} a^\dagger_{r, \tau} a_{s, \tau} a_{q, \sigma}
+                + \text{constant}.
+
+        The Hamiltonian is decomposed into the double-factorized form
+
+        .. math::
+
+            H = \sum_{pq, \sigma} \kappa_{pq} a^\dagger_{p, \sigma} a_{q, \sigma}
+            + \frac12 \sum_t \sum_{ij, \sigma\tau}
+            Z^{(t)}_{ij} n^{(t)}_{i, \sigma} n^{(t)}_{j, \tau}
+            + \text{constant}'.
+
+        where
+
+        .. math::
+
+            n^{(t)}_{i, \sigma} = \sum_{pq} U^{(t)}_{pi}
+            a^\dagger_{p, \sigma} a^\dagger_{q, \sigma} U^{(t)}_{qi}.
+
+        Here :math:`U^{(t)}_{ij}` and :math:`Z^{(t)}_{ij}` are tensors that are output
+        by the decomposition, and :math:`\kappa_{pq}` is an updated one-body tensor.
+        Each matrix :math:`U^{(t)}` is guaranteed to be unitary so that the
+        :math:`n^{(t)}_{i, \sigma}` are number operators in a rotated basis, and
+        each :math:`Z^{(t)}` is a real symmetric matrix.
+        The number of terms :math:`t` in the decomposition depends on the allowed
+        error threshold. A larger error threshold leads to a smaller number of terms.
+        Furthermore, the `max_rank` parameter specifies an optional upper bound
+        on :math:`t`.
+
+        The default behavior of this routine is to perform a straightforward
+        "exact" factorization of the two-body tensor based on a nested
+        eigenvalue decomposition. Additionally, one can choose to optimize the
+        coefficients stored in the tensor to achieve a "compressed" factorization.
+        This option is enabled by setting the `optimize` parameter to `True`.
+        The optimization attempts to minimize a least-squares objective function
+        quantifying the error in the low rank decomposition.
+        It uses `scipy.optimize.minimize`, passing both the objective function
+        and its gradient. The diagonal coulomb matrices returned by the optimization
+        can be optionally constrained to have only certain elements allowed to be
+        nonzero. This is achieved by passing the `diag_coulomb_mask` parameter, which is
+        an :math:`N \times N` matrix of boolean values where :math:`N` is the number
+        of orbitals. The nonzero elements of this matrix indicate where the diagonal
+        Coulomb matrices are allowed to be nonzero. Only the upper triangular part of
+        the matrix is used because the diagonal Coulomb matrices are symmetric.
+
+        **"Z" representation**
+
+        The "Z" representation of the double factorization is an alternative
+        representation that sometimes yields simpler quantum circuits.
+
+        Under the Jordan-Wigner transformation, the number operators take the form
+
+        .. math::
+
+            n^{(t)}_{i, \sigma} = \frac{(1 - z^{(t)}_{i, \sigma})}{2}
+
+        where :math:`z^{(t)}_{i, \sigma}` is the Pauli Z operator in the rotated basis.
+        The "Z" representation is obtained by rewriting the two-body part in terms
+        of these Pauli Z operators and updating the one-body term as appropriate:
+
+        .. math::
+
+            H = \sum_{pq, \sigma} \kappa'_{pq} a^\dagger_{p, \sigma} a_{q, \sigma}
+            + \frac18 \sum_t \sum_{ij, \sigma\tau}^*
+            Z^{(t)}_{ij} z^{(t)}_{i, \sigma} z^{(t)}_{j, \tau}
+            + \text{constant}''
+
+        where the asterisk denotes summation over indices :math:`ij, \sigma\tau`
+        where :math:`i \neq j` or :math:`\sigma \neq \tau`.
+
+        Note: Currently, only real-valued two-body tensors are supported.
+
+        Args:
+            one_body_tensor: The one-body tensor of the Hamiltonian.
+            two_body_tensor: The two-body tensor of the Hamiltonian.
+            z_representation: Whether to use the "Z" representation of the
+                low rank decomposition.
+            tol: Tolerance for error in the decomposition.
+                The error is defined as the maximum absolute difference between
+                an element of the original tensor and the corresponding element of
+                the reconstructed tensor.
+            max_vecs: An optional limit on the number of terms to keep in the
+                decomposition of the two-body tensor. This argument overrides ``tol``.
+            optimize: Whether to optimize the tensors returned by the decomposition.
+            method: The optimization method. See the documentation of
+                `scipy.optimize.minimize`_ for possible values.
+            callback: Callback function for the optimization. See the documentation of
+                `scipy.optimize.minimize`_ for usage.
+            options: Options for the optimization. See the documentation of
+                `scipy.optimize.minimize`_ for usage.
+            diag_coulomb_mask: Diagonal Coulomb matrix mask to use in the optimization.
+                This is a matrix of boolean values where the nonzero elements indicate
+                where the diagonal Coulomb matrices returned by optimization are allowed
+                to be nonzero. This parameter is only used if `optimize` is set to
+                True, and only the upper triangular part of the matrix is used.
+            cholesky: Whether to perform the factorization using a modified Cholesky
+                decomposition. If False, a full eigenvalue decomposition is used
+                instead, which can be much more expensive. This argument is ignored if
+                ``optimize`` is set to True.
+
+        Returns:
+            The double-factorized Hamiltonian.
+
+        References:
+            - `arXiv:1808.02625`_
+            - `arXiv:2104.08957`_
+
+        .. _arXiv:1808.02625: https://arxiv.org/abs/1808.02625
+        .. _arXiv:2104.08957: https://arxiv.org/abs/2104.08957
+        .. _scipy.optimize.minimize: https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html
+        """
+        one_body_tensor = hamiltonian.one_body_tensor - 0.5 * np.einsum(
+            "prqr", hamiltonian.two_body_tensor
+        )
+
+        diag_coulomb_mats, orbital_rotations = double_factorized(
+            hamiltonian.two_body_tensor,
+            tol=tol,
+            max_vecs=max_vecs,
+            optimize=optimize,
+            method=method,
+            options=options,
+            diag_coulomb_mask=diag_coulomb_mask,
+            cholesky=cholesky,
+        )
+        df_hamiltonian = DoubleFactorizedHamiltonian(
+            one_body_tensor=one_body_tensor,
+            diag_coulomb_mats=diag_coulomb_mats,
+            orbital_rotations=orbital_rotations,
+        )
+
+        if z_representation:
+            df_hamiltonian = df_hamiltonian.to_z_representation()
+
+        return df_hamiltonian
+
 
 def _df_z_representation(
     diag_coulomb_mats: np.ndarray, orbital_rotations: np.ndarray
 ) -> tuple[np.ndarray, float]:
     one_body_correction = 0.5 * (
         np.einsum(
             "tij,tpi,tqi->pq",
@@ -136,163 +293,7 @@
             orbital_rotations.conj(),
         )
     )
     constant_correction = 0.25 * np.einsum("ijj->", diag_coulomb_mats) - 0.5 * np.sum(
         diag_coulomb_mats
     )
     return one_body_correction, constant_correction
-
-
-def double_factorized_hamiltonian(
-    hamiltonian: MolecularHamiltonian,
-    *,
-    z_representation: bool = False,
-    tol: float = 1e-8,
-    max_vecs: int | None = None,
-    optimize: bool = False,
-    method: str = "L-BFGS-B",
-    options: dict | None = None,
-    diag_coulomb_mask: np.ndarray | None = None,
-    cholesky: bool = True,
-) -> DoubleFactorizedHamiltonian:
-    r"""Double-factorized decomposition of a molecular Hamiltonian.
-
-    The double-factorized decomposition acts on a Hamiltonian of the form
-
-    .. math::
-
-        H = \sum_{pq, \sigma} h_{pq} a^\dagger_{p, \sigma} a_{q, \sigma}
-            + \frac12 \sum_{pqrs, \sigma \tau} h_{pqrs}
-            a^\dagger_{p, \sigma} a^\dagger_{r, \tau} a_{s, \tau} a_{q, \sigma}
-            + \text{constant}.
-
-    The Hamiltonian is decomposed into the double-factorized form
-
-    .. math::
-
-        H = \sum_{pq, \sigma} \kappa_{pq} a^\dagger_{p, \sigma} a_{q, \sigma}
-        + \frac12 \sum_t \sum_{ij, \sigma\tau}
-        Z^{(t)}_{ij} n^{(t)}_{i, \sigma} n^{(t)}_{j, \tau}
-        + \text{constant}'.
-
-    where
-
-    .. math::
-
-        n^{(t)}_{i, \sigma} = \sum_{pq} U^{(t)}_{pi}
-        a^\dagger_{p, \sigma} a^\dagger_{q, \sigma} U^{(t)}_{qi}.
-
-    Here :math:`U^{(t)}_{ij}` and :math:`Z^{(t)}_{ij}` are tensors that are output by
-    the decomposition, and :math:`\kappa_{pq}` is an updated one-body tensor.
-    Each matrix :math:`U^{(t)}` is guaranteed to be unitary so that the
-    :math:`n^{(t)}_{i, \sigma}` are number operators in a rotated basis, and
-    each :math:`Z^{(t)}` is a real symmetric matrix.
-    The number of terms :math:`t` in the decomposition depends on the allowed
-    error threshold. A larger error threshold leads to a smaller number of terms.
-    Furthermore, the `max_rank` parameter specifies an optional upper bound
-    on :math:`t`.
-
-    The default behavior of this routine is to perform a straightforward
-    "exact" factorization of the two-body tensor based on a nested
-    eigenvalue decomposition. Additionally, one can choose to optimize the
-    coefficients stored in the tensor to achieve a "compressed" factorization.
-    This option is enabled by setting the `optimize` parameter to `True`.
-    The optimization attempts to minimize a least-squares objective function
-    quantifying the error in the low rank decomposition.
-    It uses `scipy.optimize.minimize`, passing both the objective function
-    and its gradient. The core tensors returned by the optimization can be optionally
-    constrained to have only certain elements allowed to be nonzero. This is achieved by
-    passing the `diag_coulomb_mask` parameter, which is an :math:`N \times N` matrix of
-    boolean values where :math:`N` is the number of orbitals. The nonzero elements of
-    this matrix indicate where the core tensors are allowed to be nonzero. Only the
-    upper triangular part of the matrix is used because the core tensors are symmetric.
-
-    **"Z" representation**
-
-    The "Z" representation of the double factorization is an alternative
-    representation that sometimes yields simpler quantum circuits.
-
-    Under the Jordan-Wigner transformation, the number operators take the form
-
-    .. math::
-
-        n^{(t)}_{i, \sigma} = \frac{(1 - z^{(t)}_{i, \sigma})}{2}
-
-    where :math:`z^{(t)}_{i, \sigma}` is the Pauli Z operator in the rotated basis.
-    The "Z" representation is obtained by rewriting the two-body part in terms
-    of these Pauli Z operators and updating the one-body term as appropriate:
-
-    .. math::
-
-        H = \sum_{pq, \sigma} \kappa'_{pq} a^\dagger_{p, \sigma} a_{q, \sigma}
-        + \frac18 \sum_t \sum_{ij, \sigma\tau}^*
-        Z^{(t)}_{ij} z^{(t)}_{i, \sigma} z^{(t)}_{j, \tau}
-        + \text{constant}''
-
-    where the asterisk denotes summation over indices :math:`ij, \sigma\tau`
-    where :math:`i \neq j` or :math:`\sigma \neq \tau`.
-
-    Note: Currently, only real-valued two-body tensors are supported.
-
-    Args:
-        one_body_tensor: The one-body tensor of the Hamiltonian.
-        two_body_tensor: The two-body tensor of the Hamiltonian.
-        z_representation: Whether to use the "Z" representation of the
-            low rank decomposition.
-        tol: Tolerance for error in the decomposition.
-            The error is defined as the maximum absolute difference between
-            an element of the original tensor and the corresponding element of
-            the reconstructed tensor.
-        max_vecs: An optional limit on the number of terms to keep in the decomposition
-            of the two-body tensor. This argument overrides ``tol``.
-        optimize: Whether to optimize the tensors returned by the decomposition.
-        method: The optimization method. See the documentation of
-            `scipy.optimize.minimize`_ for possible values.
-        callback: Callback function for the optimization. See the documentation of
-            `scipy.optimize.minimize`_ for usage.
-        options: Options for the optimization. See the documentation of
-            `scipy.optimize.minimize`_ for usage.
-        diag_coulomb_mask: Diagonal Coulomb matrix mask to use in the optimization.
-            This is a matrix of boolean values where the nonzero elements indicate where
-            the diagonal coulomb matrices returned by optimization are allowed to be
-            nonzero. This parameter is only used if `optimize` is set to `True`, and
-            only the upper triangular part of the matrix is used.
-        cholesky: Whether to perform the factorization using a modified Cholesky
-            decomposition. If False, a full eigenvalue decomposition is used instead,
-            which can be much more expensive. This argument is ignored if ``optimize``
-            is set to True.
-
-    Returns:
-        The double-factorized Hamiltonian.
-
-    References:
-        - `arXiv:1808.02625`_
-        - `arXiv:2104.08957`_
-
-    .. _arXiv:1808.02625: https://arxiv.org/abs/1808.02625
-    .. _arXiv:2104.08957: https://arxiv.org/abs/2104.08957
-    .. _scipy.optimize.minimize: https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html
-    """
-    one_body_tensor = hamiltonian.one_body_tensor - 0.5 * np.einsum(
-        "prqr", hamiltonian.two_body_tensor
-    )
-
-    diag_coulomb_mats, orbital_rotations = double_factorized(
-        hamiltonian.two_body_tensor,
-        tol=tol,
-        max_vecs=max_vecs,
-        optimize=optimize,
-        method=method,
-        options=options,
-        diag_coulomb_mask=diag_coulomb_mask,
-        cholesky=cholesky,
-    )
-    df_hamiltonian = DoubleFactorizedHamiltonian(
-        one_body_tensor=one_body_tensor,
-        diag_coulomb_mats=diag_coulomb_mats,
-        orbital_rotations=orbital_rotations,
-    )
-
-    if z_representation:
-        df_hamiltonian = df_hamiltonian.to_z_representation()
-
-    return df_hamiltonian
```

### Comparing `ffsim-0.0.8/python/ffsim/linalg/__init__.py` & `ffsim-0.0.9/python/ffsim/linalg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,15 @@
 
 from ffsim.linalg.double_factorized import (
     double_factorized,
     double_factorized_t2,
     modified_cholesky,
 )
 from ffsim.linalg.givens import apply_matrix_to_slices, givens_decomposition
-from ffsim.linalg.linalg import (
-    expm_multiply_taylor,
-    lup,
-)
+from ffsim.linalg.linalg import expm_multiply_taylor, lup, reduced_matrix
 from ffsim.linalg.predicates import (
     is_antihermitian,
     is_hermitian,
     is_orthogonal,
     is_real_symmetric,
     is_special_orthogonal,
     is_unitary,
```

### Comparing `ffsim-0.0.8/python/ffsim/linalg/double_factorized.py` & `ffsim-0.0.9/python/ffsim/linalg/double_factorized.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/linalg/givens.py` & `ffsim-0.0.9/python/ffsim/linalg/givens.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/linalg/predicates.py` & `ffsim-0.0.9/python/ffsim/linalg/predicates.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/molecular_data.py` & `ffsim-0.0.9/python/ffsim/molecular_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,20 @@
         )
 
     @staticmethod
     def from_hartree_fock(
         hartree_fock: scf.hf.SCF, active_space: Iterable[int] | None = None
     ) -> "MolecularData":
         if active_space is None:
-            norb = hartree_fock.mo_coeff.shape[0]
+            norb = hartree_fock.mol.nao_nr()
             active_space = range(norb)
 
         active_space = list(active_space)
         norb = len(active_space)
-        n_electrons = int(np.sum(hartree_fock.mo_occ[active_space]))
+        n_electrons = int(sum(hartree_fock.mo_occ[active_space]))
         n_alpha = (n_electrons + hartree_fock.mol.spin) // 2
         n_beta = (n_electrons - hartree_fock.mol.spin) // 2
 
         cas = mcscf.CASCI(hartree_fock, norb, (n_alpha, n_beta))
         cas.mo_coeff = cas.sort_mo(active_space, base=0)
         one_body_tensor, core_energy = cas.get_h1cas()
         two_body_tensor = ao2mo.restore(1, cas.get_h2cas(), cas.ncas)
```

### Comparing `ffsim-0.0.8/python/ffsim/protocols/__init__.py` & `ffsim-0.0.9/python/ffsim/trotter/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,11 +4,11 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
-"""Protocols."""
+"""Hamiltonian simulation via Trotter-Suzuki formulas."""
 
-from ffsim.protocols.linear_operator import SupportsLinearOperator, linear_operator
-from ffsim.protocols.trace import SupportsTrace, trace
+from ffsim.trotter.qdrift import simulate_qdrift_double_factorized
+from ffsim.trotter.trotter import simulate_trotter_double_factorized
```

### Comparing `ffsim-0.0.8/python/ffsim/protocols/trace.py` & `ffsim-0.0.9/python/ffsim/protocols/trace.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/random.py` & `ffsim-0.0.9/python/ffsim/random.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/slow/contract/diag_coulomb.py` & `ffsim-0.0.9/python/ffsim/_slow/contract/diag_coulomb.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/slow/contract/num_op_sum.py` & `ffsim-0.0.9/python/ffsim/_slow/contract/num_op_sum.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/slow/gates/diag_coulomb.py` & `ffsim-0.0.9/python/ffsim/_slow/gates/diag_coulomb.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/slow/gates/num_op_sum.py` & `ffsim-0.0.9/python/ffsim/_slow/gates/num_op_sum.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/slow/gates/orbital_rotation.py` & `ffsim-0.0.9/python/ffsim/_slow/gates/orbital_rotation.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/states.py` & `ffsim-0.0.9/python/ffsim/states.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/testing.py` & `ffsim-0.0.9/python/ffsim/testing.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/trotter/qdrift.py` & `ffsim-0.0.9/python/ffsim/trotter/qdrift.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/trotter/trotter.py` & `ffsim-0.0.9/python/ffsim/trotter/trotter.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/python/ffsim/variational/__init__.py` & `ffsim-0.0.9/src/gates/mod.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# (C) Copyright IBM 2023.
-#
-# This code is licensed under the Apache License, Version 2.0. You may
-# obtain a copy of this license in the LICENSE.txt file in the root directory
-# of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
-#
-# Any modifications or derivative works of this code must retain this
-# copyright notice, and modified files need to carry a notice indicating
-# that they have been altered from the originals.
+// (C) Copyright IBM 2023
+//
+// This code is licensed under the Apache License, Version 2.0. You may
+// obtain a copy of this license in the LICENSE.txt file in the root directory
+// of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
+//
+// Any modifications or derivative works of this code must retain this
+// copyright notice, and modified files need to carry a notice indicating
+// that they have been altered from the originals.
 
-"""Variational ansatzes."""
-
-from ffsim.variational.lucj import (
-    UCJOperator,
-    apply_ucj_operator,
-)
+pub mod diag_coulomb;
+pub mod num_op_sum;
+pub mod orbital_rotation;
+pub mod phase_shift;
```

### Comparing `ffsim-0.0.8/python/ffsim/variational/lucj.py` & `ffsim-0.0.9/python/ffsim/variational/lucj.py`

 * *Files 13% similar despite different names*

```diff
@@ -296,57 +296,37 @@
 
         if self.final_orbital_rotation is None:
             return t2
 
         t1 = scipy.linalg.logm(self.final_orbital_rotation)[:nocc, nocc:]
         return t2, t1
 
-
-def apply_ucj_operator(
-    vec: np.ndarray,
-    operator: UCJOperator,
-    *,
-    norb: int,
-    nelec: tuple[int, int],
-    copy: bool = True,
-) -> np.ndarray:
-    """Apply a UCJ operator to a vector.
-
-    Args:
-        vec: The state vector to be transformed.
-        operator: The UCJ operator.
-        norb: The number of spatial orbitals.
-        nelec: The number of alpha and beta electrons.
-        copy: Whether to copy the vector before operating on it.
-            - If ``copy=True`` then this function always returns a newly allocated
-            vector and the original vector is left untouched.
-            - If ``copy=False`` then this function may still return a newly allocated
-            vector, but the original vector may have its data overwritten.
-            It is also possible that the original vector is returned,
-            modified in-place.
-    """
-    if copy:
-        vec = vec.copy()
-    for mat, mat_alpha_beta, orbital_rotation in zip(
-        operator.diag_coulomb_mats_alpha_alpha,
-        operator.diag_coulomb_mats_alpha_beta,
-        operator.orbital_rotations,
-    ):
-        vec = apply_diag_coulomb_evolution(
-            vec,
-            mat=mat,
-            time=-1.0,
-            norb=norb,
-            nelec=nelec,
-            mat_alpha_beta=mat_alpha_beta,
-            orbital_rotation=orbital_rotation,
-            copy=False,
-        )
-    if operator.final_orbital_rotation is not None:
-        vec = apply_orbital_rotation(
-            vec,
-            mat=operator.final_orbital_rotation,
-            norb=norb,
-            nelec=nelec,
-            copy=False,
-        )
-    return vec
+    def _apply_unitary_(
+        self, vec: np.ndarray, norb: int, nelec: tuple[int, int], copy: bool
+    ) -> np.ndarray:
+        """Apply the operator to a vector."""
+        if copy:
+            vec = vec.copy()
+        for mat, mat_alpha_beta, orbital_rotation in zip(
+            self.diag_coulomb_mats_alpha_alpha,
+            self.diag_coulomb_mats_alpha_beta,
+            self.orbital_rotations,
+        ):
+            vec = apply_diag_coulomb_evolution(
+                vec,
+                mat=mat,
+                time=-1.0,
+                norb=norb,
+                nelec=nelec,
+                mat_alpha_beta=mat_alpha_beta,
+                orbital_rotation=orbital_rotation,
+                copy=False,
+            )
+        if self.final_orbital_rotation is not None:
+            vec = apply_orbital_rotation(
+                vec,
+                mat=self.final_orbital_rotation,
+                norb=norb,
+                nelec=nelec,
+                copy=False,
+            )
+        return vec
```

### Comparing `ffsim-0.0.8/python/ffsim/wick.py` & `ffsim-0.0.9/python/ffsim/wick.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/contract/diag_coulomb.rs` & `ffsim-0.0.9/src/contract/diag_coulomb.rs`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/contract/num_op_sum.rs` & `ffsim-0.0.9/src/contract/num_op_sum.rs`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/gates/diag_coulomb.rs` & `ffsim-0.0.9/src/gates/diag_coulomb.rs`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/gates/num_op_sum.rs` & `ffsim-0.0.9/src/gates/num_op_sum.rs`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/gates/orbital_rotation.rs` & `ffsim-0.0.9/src/gates/orbital_rotation.rs`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/gates/phase_shift.rs` & `ffsim-0.0.9/src/gates/phase_shift.rs`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/src/lib.rs` & `ffsim-0.0.9/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 // Any modifications or derivative works of this code must retain this
 // copyright notice, and modified files need to carry a notice indicating
 // that they have been altered from the originals.
 
 use pyo3::prelude::*;
 
 mod contract;
+mod fermion_operator;
 mod gates;
 
 /// Python module exposing Rust extensions.
 #[pymodule]
-fn _ffsim(_py: Python, m: &PyModule) -> PyResult<()> {
+fn _lib(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(
         gates::phase_shift::apply_phase_shift_in_place,
         m
     )?)?;
     m.add_function(wrap_pyfunction!(
         gates::orbital_rotation::apply_givens_rotation_in_place,
         m
@@ -52,9 +53,10 @@
         contract::diag_coulomb::contract_diag_coulomb_into_buffer_z_rep,
         m
     )?)?;
     m.add_function(wrap_pyfunction!(
         contract::num_op_sum::contract_num_op_sum_spin_into_buffer,
         m
     )?)?;
+    m.add_class::<fermion_operator::FermionOperator>()?;
     Ok(())
 }
```

### Comparing `ffsim-0.0.8/tests/contract/diag_coulomb_test.py` & `ffsim-0.0.9/tests/contract/diag_coulomb_test.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/tests/contract/num_op_sum_test.py` & `ffsim-0.0.9/tests/contract/num_op_sum_test.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/tests/gates/basic_gates_test.py` & `ffsim-0.0.9/tests/gates/basic_gates_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,17 +92,15 @@
             result = ffsim.apply_givens_rotation(
                 vec, theta, target_orbs, norb=norb, nelec=nelec
             )
             generator = np.zeros((norb, norb))
             a, b = target_orbs
             generator[a, b] = theta
             generator[b, a] = -theta
-            linop = ffsim.contract.hamiltonian_linop(
-                one_body_tensor=generator, norb=norb, nelec=nelec
-            )
+            linop = ffsim.contract.one_body_linop(generator, norb=norb, nelec=nelec)
             expected = scipy.sparse.linalg.expm_multiply(
                 linop, vec, traceA=np.sum(np.abs(generator))
             )
             np.testing.assert_allclose(result, expected, atol=1e-8)
     np.testing.assert_allclose(vec, original_vec)
 
 
@@ -154,17 +152,15 @@
         for target_orbs in [(i, j), (j, i)]:
             result = ffsim.apply_tunneling_interaction(
                 vec, theta, target_orbs, norb=norb, nelec=nelec
             )
             generator = np.zeros((norb, norb))
             generator[i, j] = theta
             generator[j, i] = theta
-            linop = ffsim.contract.hamiltonian_linop(
-                one_body_tensor=generator, norb=norb, nelec=nelec
-            )
+            linop = ffsim.contract.one_body_linop(generator, norb=norb, nelec=nelec)
             expected = scipy.sparse.linalg.expm_multiply(
                 1j * linop, vec, traceA=np.sum(np.abs(generator))
             )
             np.testing.assert_allclose(result, expected, atol=1e-8)
 
 
 def test_apply_tunneling_interaction_matrix():
@@ -213,32 +209,70 @@
     theta = rng.uniform(-10, 10)
     for target_orb in range(norb):
         result = ffsim.apply_num_interaction(
             vec, theta, target_orb, norb=norb, nelec=nelec
         )
         generator = np.zeros((norb, norb))
         generator[target_orb, target_orb] = theta
-        linop = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=generator, norb=norb, nelec=nelec
-        )
+        linop = ffsim.contract.one_body_linop(generator, norb=norb, nelec=nelec)
         expected = scipy.sparse.linalg.expm_multiply(
             1j * linop, vec, traceA=np.sum(np.abs(generator))
         )
         np.testing.assert_allclose(result, expected, atol=1e-8)
 
 
 @pytest.mark.parametrize(
     "norb, nelec",
     [
         (2, (1, 1)),
+        (3, (2, 1)),
+    ],
+)
+def test_apply_num_num_interaction(norb: int, nelec: tuple[int, int]):
+    """Test applying number interaction."""
+    dim = ffsim.dim(norb, nelec)
+    rng = np.random.default_rng()
+    vec = np.array(ffsim.random.random_statevector(dim, seed=rng))
+    theta = rng.uniform(-10, 10)
+    for i, j in itertools.combinations(range(norb), 2):
+        for target_orbs in [(i, j), (j, i)]:
+            result = ffsim.apply_num_num_interaction(
+                vec, theta, target_orbs, norb=norb, nelec=nelec
+            )
+            m, n = target_orbs
+            generator = ffsim.FermionOperator(
+                {
+                    (
+                        ffsim.cre_a(m),
+                        ffsim.des_a(m),
+                        ffsim.cre_a(n),
+                        ffsim.des_a(n),
+                    ): theta,
+                    (
+                        ffsim.cre_b(m),
+                        ffsim.des_b(m),
+                        ffsim.cre_b(n),
+                        ffsim.des_b(n),
+                    ): theta,
+                }
+            )
+            linop = ffsim.linear_operator(generator, norb=norb, nelec=nelec)
+            expected = scipy.sparse.linalg.expm_multiply(1j * linop, vec, traceA=theta)
+            np.testing.assert_allclose(result, expected, atol=1e-8)
+
+
+@pytest.mark.parametrize(
+    "norb, nelec",
+    [
+        (2, (1, 1)),
         (4, (2, 2)),
         (5, (3, 2)),
     ],
 )
-def test_apply_num_num_interaction(norb: int, nelec: tuple[int, int]):
+def test_apply_num_num_interaction_eigenvalues(norb: int, nelec: tuple[int, int]):
     """Test applying number interaction."""
     rng = np.random.default_rng()
     occupied_orbitals = ffsim.testing.random_occupied_orbitals(norb, nelec)
     vec = ffsim.slater_determinant(norb, occupied_orbitals)
 
     theta = rng.uniform(-10, 10)
     for i, j in itertools.combinations(range(norb), 2):
```

### Comparing `ffsim-0.0.8/tests/gates/diag_coulomb_test.py` & `ffsim-0.0.9/tests/gates/diag_coulomb_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             orbital_rotation=orbital_rotation,
             z_representation=z_representation,
         )
 
         op = ffsim.contract.diag_coulomb_linop(
             mat, norb=norb, nelec=nelec, z_representation=z_representation
         )
-        orbital_op = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=scipy.linalg.logm(orbital_rotation), norb=norb, nelec=nelec
+        orbital_op = ffsim.contract.one_body_linop(
+            scipy.linalg.logm(orbital_rotation), norb=norb, nelec=nelec
         )
         expected = scipy.sparse.linalg.expm_multiply(
             -orbital_op, vec, traceA=np.sum(np.abs(orbital_rotation))
         )
         expected = scipy.sparse.linalg.expm_multiply(
             -1j * time * op, expected, traceA=np.sum(np.abs(mat))
         )
@@ -98,16 +98,16 @@
         op = ffsim.contract.diag_coulomb_linop(
             mat,
             norb=norb,
             nelec=nelec,
             mat_alpha_beta=mat_alpha_beta,
             z_representation=z_representation,
         )
-        orbital_op = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=scipy.linalg.logm(orbital_rotation), norb=norb, nelec=nelec
+        orbital_op = ffsim.contract.one_body_linop(
+            scipy.linalg.logm(orbital_rotation), norb=norb, nelec=nelec
         )
         expected = scipy.sparse.linalg.expm_multiply(
             -orbital_op, vec, traceA=np.sum(np.abs(orbital_rotation))
         )
         expected = scipy.sparse.linalg.expm_multiply(
             -1j * time * op, expected, traceA=np.sum(np.abs(mat))
         )
```

### Comparing `ffsim-0.0.8/tests/gates/num_op_sum_test.py` & `ffsim-0.0.9/tests/gates/num_op_sum_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,12 @@
         eigs, vecs = np.linalg.eigh(mat)
         vec = ffsim.random.random_statevector(dim, seed=rng)
 
         time = 0.6
         result = ffsim.apply_num_op_sum_evolution(
             vec, eigs, time, norb, nelec, orbital_rotation=vecs
         )
-        op = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=mat, norb=norb, nelec=nelec
-        )
+        op = ffsim.contract.one_body_linop(mat, norb=norb, nelec=nelec)
         expected = scipy.sparse.linalg.expm_multiply(
             -1j * time * op, vec, traceA=np.sum(np.abs(mat))
         )
         np.testing.assert_allclose(result, expected, atol=1e-8)
```

### Comparing `ffsim-0.0.8/tests/gates/orbital_rotation_test.py` & `ffsim-0.0.9/tests/gates/orbital_rotation_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         dim = ffsim.dim(norb, nelec)
 
         mat = ffsim.random.random_unitary(norb, seed=rng, dtype=dtype)
         vec = ffsim.random.random_statevector(dim, seed=rng, dtype=dtype)
         original_vec = vec.copy()
 
         result = ffsim.apply_orbital_rotation(vec, mat, norb, nelec)
-        op = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=scipy.linalg.logm(mat), norb=norb, nelec=nelec
+        op = ffsim.contract.one_body_linop(
+            scipy.linalg.logm(mat), norb=norb, nelec=nelec
         )
         expected = scipy.sparse.linalg.expm_multiply(op, original_vec, traceA=1)
         np.testing.assert_allclose(result, expected, atol=atol)
 
 
 def test_apply_orbital_rotation_no_side_effects():
     """Test applying orbital basis change doesn't modify the original vector."""
@@ -82,25 +82,25 @@
         vec = ffsim.random.random_statevector(dim, seed=rng, dtype=dtype)
         original_vec = vec.copy()
 
         result, perm = ffsim.apply_orbital_rotation(
             vec, mat, norb, nelec, allow_col_permutation=True, copy=True
         )
         np.testing.assert_allclose(np.linalg.norm(result), 1, atol=atol)
-        op = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=scipy.linalg.logm(mat @ perm), norb=norb, nelec=nelec
+        op = ffsim.contract.one_body_linop(
+            scipy.linalg.logm(mat @ perm), norb=norb, nelec=nelec
         )
         expected = scipy.sparse.linalg.expm_multiply(op, original_vec, traceA=1)
         np.testing.assert_allclose(result, expected, atol=atol)
 
         result, perm = ffsim.apply_orbital_rotation(
             vec, mat, norb, nelec, allow_row_permutation=True, copy=False
         )
-        op = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=scipy.linalg.logm(perm @ mat), norb=norb, nelec=nelec
+        op = ffsim.contract.one_body_linop(
+            scipy.linalg.logm(perm @ mat), norb=norb, nelec=nelec
         )
         expected = scipy.sparse.linalg.expm_multiply(op, original_vec, traceA=1)
         np.testing.assert_allclose(result, expected, atol=atol)
 
 
 def test_apply_orbital_rotation_eigenstates():
     """Test applying orbital basis change prepares eigenstates of one-body tensor."""
```

### Comparing `ffsim-0.0.8/tests/hamiltonians/double_factorized_hamiltonian_test.py` & `ffsim-0.0.9/tests/hamiltonians/double_factorized_hamiltonian_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     hamiltonian = ffsim.linear_operator(
         mol_hamiltonian,
         norb=norb,
         nelec=nelec,
     )
 
     # perform double factorization
-    df_hamiltonian = ffsim.double_factorized_hamiltonian(
+    df_hamiltonian = ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(
         mol_hamiltonian,
         z_representation=z_representation,
     )
 
     # generate random state
     dim = ffsim.dim(norb, nelec)
     state = ffsim.random.random_statevector(dim, seed=1360)
@@ -82,15 +82,15 @@
 
 def test_z_representation_round_trip():
     norb = 4
 
     one_body_tensor = ffsim.random.random_hermitian(norb, seed=2474)
     two_body_tensor = ffsim.random.random_two_body_tensor_real(norb, seed=7054)
 
-    df_hamiltonian = ffsim.double_factorized_hamiltonian(
+    df_hamiltonian = ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(
         ffsim.MolecularHamiltonian(one_body_tensor, two_body_tensor)
     )
     df_hamiltonian_num = df_hamiltonian.to_z_representation().to_number_representation()
 
     np.testing.assert_allclose(
         df_hamiltonian.one_body_tensor, df_hamiltonian_num.one_body_tensor
     )
```

### Comparing `ffsim-0.0.8/tests/hamiltonians/molecular_hamiltonian_test.py` & `ffsim-0.0.9/tests/hamiltonians/molecular_hamiltonian_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,14 @@
     mol_data = ffsim.MolecularData.from_hartree_fock(
         hartree_fock, active_space=active_space
     )
     norb = mol_data.norb
     nelec = mol_data.nelec
     mol_hamiltonian = mol_data.hamiltonian
 
-    # compute FCI energy from molecualar Hamiltonian
+    # compute FCI energy from molecular Hamiltonian
     hamiltonian = ffsim.linear_operator(mol_hamiltonian, norb=norb, nelec=nelec)
     eigs, _ = scipy.sparse.linalg.eigsh(hamiltonian, k=1, which="SA")
     eig = eigs[0]
 
     # Check that they match
     np.testing.assert_allclose(eig, energy_fci)
```

### Comparing `ffsim-0.0.8/tests/linalg/double_factorized_test.py` & `ffsim-0.0.9/tests/linalg/double_factorized_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     mol.build(
         verbose=0,
         atom=[["Li", (0, 0, 0)], ["H", (1.6, 0, 0)]],
         basis="sto-3g",
     )
     hartree_fock = scf.RHF(mol)
     hartree_fock.kernel()
-    norb, _ = hartree_fock.mo_coeff.shape
+    norb = hartree_fock.mol.nao_nr()
     mc = mcscf.CASCI(hartree_fock, norb, mol.nelec)
     two_body_tensor = ao2mo.restore(1, mc.get_h2cas(), mc.ncas)
 
     # test max_vecs
     max_vecs = 20
     diag_coulomb_mats, orbital_rotations = double_factorized(
         two_body_tensor, max_vecs=max_vecs, cholesky=cholesky
```

### Comparing `ffsim-0.0.8/tests/linalg/givens_test.py` & `ffsim-0.0.9/tests/linalg/givens_test.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/tests/random_test.py` & `ffsim-0.0.9/tests/random_test.py`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/tests/slow/contract/diag_coulomb_test.py` & `ffsim-0.0.9/tests/_slow/contract/diag_coulomb_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from __future__ import annotations
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
 import ffsim
-from ffsim._ffsim import (
+from ffsim._lib import (
     contract_diag_coulomb_into_buffer_num_rep,
     contract_diag_coulomb_into_buffer_z_rep,
 )
-from ffsim.slow.contract.diag_coulomb import (
+from ffsim._slow.contract.diag_coulomb import (
     contract_diag_coulomb_into_buffer_num_rep_slow,
     contract_diag_coulomb_into_buffer_z_rep_slow,
 )
 
 
 def test_contract_diag_coulomb_into_buffer_num_rep_slow():
     """Test contracting diag Coulomb operator."""
```

### Comparing `ffsim-0.0.8/tests/slow/contract/num_op_sum_test.py` & `ffsim-0.0.9/tests/_slow/contract/num_op_sum_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from __future__ import annotations
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
 import ffsim
-from ffsim._ffsim import contract_num_op_sum_spin_into_buffer
-from ffsim.slow.contract.num_op_sum import contract_num_op_sum_spin_into_buffer_slow
+from ffsim._lib import contract_num_op_sum_spin_into_buffer
+from ffsim._slow.contract.num_op_sum import contract_num_op_sum_spin_into_buffer_slow
 
 
 def test_contract_num_op_sum_spin_into_buffer_slow():
     """Test applying num op sum evolution."""
     norb = 5
     rng = np.random.default_rng()
     for _ in range(5):
```

### Comparing `ffsim-0.0.8/tests/slow/gates/diag_coulomb_test.py` & `ffsim-0.0.9/tests/_slow/gates/diag_coulomb_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from __future__ import annotations
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
 import ffsim
-from ffsim._ffsim import (
+from ffsim._lib import (
     apply_diag_coulomb_evolution_in_place_num_rep,
     apply_diag_coulomb_evolution_in_place_z_rep,
 )
-from ffsim.slow.gates.diag_coulomb import (
+from ffsim._slow.gates.diag_coulomb import (
     apply_diag_coulomb_evolution_in_place_num_rep_numpy,
     apply_diag_coulomb_evolution_in_place_num_rep_slow,
     apply_diag_coulomb_evolution_in_place_z_rep_slow,
 )
 
 
 def test_apply_diag_coulomb_evolution_num_rep_slow():
```

### Comparing `ffsim-0.0.8/tests/slow/gates/num_op_sum_test.py` & `ffsim-0.0.9/tests/_slow/gates/num_op_sum_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from __future__ import annotations
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
 import ffsim
-from ffsim._ffsim import apply_num_op_sum_evolution_in_place
-from ffsim.slow.gates.num_op_sum import apply_num_op_sum_evolution_in_place_slow
+from ffsim._lib import apply_num_op_sum_evolution_in_place
+from ffsim._slow.gates.num_op_sum import apply_num_op_sum_evolution_in_place_slow
 
 
 def test_apply_num_op_sum_evolution_in_place_slow():
     """Test applying num op sum evolution."""
     norb = 5
     rng = np.random.default_rng()
     for _ in range(5):
```

### Comparing `ffsim-0.0.8/tests/slow/gates/orbital_rotation_test.py` & `ffsim-0.0.9/tests/_slow/gates/orbital_rotation_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from __future__ import annotations
 
 import numpy as np
 from pyscf.fci import cistring
 from scipy.special import comb
 
 import ffsim
-from ffsim._ffsim import (
+from ffsim._lib import (
     apply_givens_rotation_in_place,
     apply_single_column_transformation_in_place,
     gen_orbital_rotation_index_in_place,
 )
-from ffsim.gates.orbital_rotation import (
-    _zero_one_subspace_indices,
-    gen_orbital_rotation_index,
-)
-from ffsim.slow.gates.orbital_rotation import (
+from ffsim._slow.gates.orbital_rotation import (
     apply_givens_rotation_in_place_slow,
     apply_single_column_transformation_in_place_slow,
     gen_orbital_rotation_index_in_place_slow,
 )
+from ffsim.gates.orbital_rotation import (
+    _zero_one_subspace_indices,
+    gen_orbital_rotation_index,
+)
 
 
 def test_apply_givens_rotation_in_place_slow():
     """Test applying Givens rotation."""
     norb = 5
     rng = np.random.default_rng()
     for _ in range(5):
```

### Comparing `ffsim-0.0.8/tests/states_test.py` & `ffsim-0.0.9/tests/states_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,11 +25,9 @@
     one_body_tensor = ffsim.random.random_hermitian(norb)
     eigs, orbital_rotation = np.linalg.eigh(one_body_tensor)
     eig = sum(eigs[occ_a]) + sum(eigs[occ_b])
     state = ffsim.slater_determinant(
         norb, occupied_orbitals, orbital_rotation=orbital_rotation
     )
 
-    hamiltonian = ffsim.contract.hamiltonian_linop(
-        one_body_tensor=one_body_tensor, norb=norb, nelec=nelec
-    )
+    hamiltonian = ffsim.contract.one_body_linop(one_body_tensor, norb=norb, nelec=nelec)
     np.testing.assert_allclose(hamiltonian @ state, eig * state)
```

### Comparing `ffsim-0.0.8/tests/trotter/qdrift_test.py` & `ffsim-0.0.9/tests/trotter/qdrift_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         (5, (1, 3)),
         (4, (3, 2)),
     ],
 )
 def test_spectral_norm_one_body_tensor(norb: int, nelec: tuple[int, int]):
     """Test spectral norm of one-body operator."""
     one_body_tensor = ffsim.random.random_hermitian(norb, seed=8034)
-    one_body_linop = ffsim.contract.hamiltonian_linop(
-        one_body_tensor=one_body_tensor, norb=norb, nelec=nelec
+    one_body_linop = ffsim.contract.one_body_linop(
+        one_body_tensor, norb=norb, nelec=nelec
     )
     actual = spectral_norm_one_body_tensor(one_body_tensor, nelec=nelec)
     singular_vals = scipy.sparse.linalg.svds(
         one_body_linop, k=1, which="LM", return_singular_vectors=False
     )
     np.testing.assert_allclose(actual, singular_vals[0], atol=1e-8)
 
@@ -123,18 +123,15 @@
             diag_coulomb_mat, orbital_rotation
         )
         zero = scipy.sparse.linalg.LinearOperator(
             shape=(dim, dim), matvec=lambda x: np.zeros_like(x)
         )
         actual = sum(
             [
-                ffsim.contract.hamiltonian_linop(
-                    one_body_tensor=tensor, norb=norb, nelec=nelec
-                )
-                ** 2
+                ffsim.contract.one_body_linop(tensor, norb=norb, nelec=nelec) ** 2
                 for tensor in one_body_tensors
             ],
             start=zero,
         )
         expected = ffsim.contract.diag_coulomb_linop(
             diag_coulomb_mat, norb=norb, nelec=nelec, orbital_rotation=orbital_rotation
         )
@@ -154,16 +151,16 @@
 )
 def test_variance_one_body_tensor(norb: int, nelec: tuple[int, int]):
     """Test variance of one-body tensor."""
     n_alpha, n_beta = nelec
     rng = np.random.default_rng()
 
     one_body_tensor = ffsim.random.random_hermitian(norb, seed=rng)
-    one_body_linop = ffsim.contract.hamiltonian_linop(
-        one_body_tensor=one_body_tensor, norb=norb, nelec=nelec
+    one_body_linop = ffsim.contract.one_body_linop(
+        one_body_tensor, norb=norb, nelec=nelec
     )
 
     # generate a random Slater determinant
     vecs = ffsim.random.random_unitary(norb, seed=rng)
     occupied_orbitals_a = vecs[:, :n_alpha]
     occupied_orbitals_b = vecs[:, :n_beta]
     one_rdm_a = occupied_orbitals_a.conj() @ occupied_orbitals_a.T
@@ -253,25 +250,25 @@
     mol.build(
         verbose=0,
         atom=[["H", (i * bond_distance, 0, 0)] for i in range(length)],
         basis=basis,
     )
     hartree_fock = scf.RHF(mol)
     hartree_fock.kernel()
-    norb, _ = hartree_fock.mo_coeff.shape
+    norb = hartree_fock.mol.nao_nr()
     mc = mcscf.CASCI(hartree_fock, norb, mol.nelec)
     one_body_tensor, _ = mc.get_h1cas()
     two_body_tensor = ao2mo.restore(1, mc.get_h2cas(), mc.ncas)
     norb, _ = one_body_tensor.shape
     nelec = mol.nelec
     mol_hamiltonian = ffsim.MolecularHamiltonian(one_body_tensor, two_body_tensor)
     hamiltonian = ffsim.linear_operator(mol_hamiltonian, norb=norb, nelec=nelec)
 
     # perform double factorization
-    df_hamiltonian = ffsim.double_factorized_hamiltonian(
+    df_hamiltonian = ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(
         mol_hamiltonian,
         z_representation=z_representation,
     )
 
     # generate initial state
     n_alpha, n_beta = nelec
     occupied_orbitals = (range(n_alpha), range(n_beta))
@@ -360,15 +357,15 @@
     two_body_tensor = ffsim.random.random_two_body_tensor_real(
         norb, rank=norb, seed=rng
     )
     mol_hamiltonian = ffsim.MolecularHamiltonian(one_body_tensor, two_body_tensor)
     hamiltonian = ffsim.linear_operator(mol_hamiltonian, norb=norb, nelec=nelec)
 
     # perform double factorization
-    df_hamiltonian = ffsim.double_factorized_hamiltonian(
+    df_hamiltonian = ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(
         mol_hamiltonian,
         optimize=optimize,
         z_representation=z_representation,
     )
 
     # generate initial state
     n_alpha, n_beta = nelec
```

### Comparing `ffsim-0.0.8/tests/trotter/trotter_test.py` & `ffsim-0.0.9/tests/trotter/trotter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     # https://github.com/qiskit-community/ffsim/issues/14
     one_body_tensor = np.real(ffsim.random.random_hermitian(norb, seed=2474))
     two_body_tensor = ffsim.random.random_two_body_tensor_real(norb, seed=7054)
     mol_hamiltonian = ffsim.MolecularHamiltonian(one_body_tensor, two_body_tensor)
     hamiltonian = ffsim.linear_operator(mol_hamiltonian, norb=norb, nelec=nelec)
 
     # perform double factorization
-    df_hamiltonian = ffsim.double_factorized_hamiltonian(
+    df_hamiltonian = ffsim.DoubleFactorizedHamiltonian.from_molecular_hamiltonian(
         mol_hamiltonian, z_representation=z_representation
     )
 
     # generate initial state
     dim = ffsim.dim(norb, nelec)
     initial_state = ffsim.random.random_statevector(dim, seed=1360)
     original_state = initial_state.copy()
```

### Comparing `ffsim-0.0.8/tests/variational/lucj_test.py` & `ffsim-0.0.9/tests/variational/lucj_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     # Construct the Hartree-Fock state to use as the reference state
     n_alpha, n_beta = nelec
     reference_state = ffsim.slater_determinant(
         norb=norb, occupied_orbitals=(range(n_alpha), range(n_beta))
     )
 
     # Apply the operator to the reference state
-    ansatz_state = ffsim.apply_ucj_operator(
+    ansatz_state = ffsim.apply_unitary(
         reference_state, operator, norb=norb, nelec=nelec
     )
 
     # Compute the energy ⟨ψ|H|ψ⟩ of the ansatz state
     hamiltonian = ffsim.linear_operator(mol_hamiltonian, norb=norb, nelec=nelec)
     energy = np.real(np.vdot(ansatz_state, hamiltonian @ ansatz_state))
     np.testing.assert_allclose(energy, -0.96962461, atol=1e-8)
```

### Comparing `ffsim-0.0.8/tests/wick_test.py` & `ffsim-0.0.9/tests/wick_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,17 +29,15 @@
     # generate random one-body tensors
     n_tensors = 6
     one_body_tensors = []
     linops = []
     for _ in range(n_tensors):
         one_body_tensor = rng.standard_normal((norb, norb)).astype(complex)
         one_body_tensor += 1j * rng.standard_normal((norb, norb))
-        linop = ffsim.contract.hamiltonian_linop(
-            one_body_tensor=one_body_tensor, norb=norb, nelec=nelec
-        )
+        linop = ffsim.contract.one_body_linop(one_body_tensor, norb=norb, nelec=nelec)
         one_body_tensors.append(one_body_tensor)
         linops.append(linop)
 
     # generate a random Slater determinant
     vecs = ffsim.random.random_unitary(norb, seed=rng)
     occupied_orbitals_a = vecs[:, :n_alpha]
     occupied_orbitals_b = vecs[:, :n_beta]
@@ -71,17 +69,15 @@
     n_alpha, n_beta = nelec
     dim = ffsim.dim(norb, nelec)
     rng = np.random.default_rng()
 
     # generate a random one-body tensor
     one_body_tensor = rng.standard_normal((norb, norb)).astype(complex)
     one_body_tensor += 1j * rng.standard_normal((norb, norb))
-    linop = ffsim.contract.hamiltonian_linop(
-        one_body_tensor=one_body_tensor, norb=norb, nelec=nelec
-    )
+    linop = ffsim.contract.one_body_linop(one_body_tensor, norb=norb, nelec=nelec)
 
     # generate a random Slater determinant
     vecs = ffsim.random.random_unitary(norb, seed=rng)
     occupied_orbitals_a = vecs[:, :n_alpha]
     occupied_orbitals_b = vecs[:, :n_beta]
     one_rdm_a = occupied_orbitals_a.conj() @ occupied_orbitals_a.T
     one_rdm_b = occupied_orbitals_b.conj() @ occupied_orbitals_b.T
```

### Comparing `ffsim-0.0.8/tox.ini` & `ffsim-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/Cargo.lock` & `ffsim-0.0.9/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ffsim-0.0.8/PKG-INFO` & `ffsim-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ffsim
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: numpy
 Requires-Dist: opt_einsum>=3.3
-Requires-Dist: pyscf>=2.3.0
+Requires-Dist: pyscf==2.4.0
 Requires-Dist: scipy
 Requires-Dist: black[jupyter]; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: jupyter-sphinx; extra == 'dev'
 Requires-Dist: maturin; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: nbmake; extra == 'dev'
@@ -20,16 +20,16 @@
 Requires-Dist: sphinx-autodoc-typehints; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Summary: Faster simulations of fermionic quantum circuits.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/qiskit-community/ffsim
 Project-URL: Documentation, https://qiskit-community.github.io/ffsim/
+Project-URL: Homepage, https://github.com/qiskit-community/ffsim
 
 # ffsim
 
 Faster simulations of fermionic quantum circuits.
 
 ## What is ffsim?
 
@@ -133,7 +133,19 @@
 
 You can also use `pytest` to run the tests directly. For example,
 
 ```bash
 pytest tests/
 ```
 
+## Cite ffsim
+
+You can cite ffsim using the following BibTeX:
+
+```bibtex
+@software{ffsim,
+  author = {{The ffsim developers}},
+  title = {ffsim},
+  url = {https://github.com/qiskit-community/ffsim}
+}
+```
+
```

