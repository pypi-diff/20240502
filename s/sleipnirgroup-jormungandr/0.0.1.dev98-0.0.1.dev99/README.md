# Comparing `tmp/sleipnirgroup_jormungandr-0.0.1.dev98.tar.gz` & `tmp/sleipnirgroup_jormungandr-0.0.1.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleipnirgroup_jormungandr-0.0.1.dev98.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sleipnirgroup_jormungandr-0.0.1.dev99.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sleipnirgroup_jormungandr-0.0.1.dev98.tar` & `sleipnirgroup_jormungandr-0.0.1.dev99.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    11689 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/CMakeLists.txt
--rw-r--r--   0        0        0     1465 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/LICENSE.txt
--rw-r--r--   0        0        0     8573 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/README.md
--rw-r--r--   0        0        0       68 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/SleipnirConfig.cmake.in
--rw-r--r--   0        0        0     1163 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/cmake/eigen-disable-fortran-support.patch
--rw-r--r--   0        0        0      991 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/Pybind11Mkdoc.cmake
--rw-r--r--   0        0        0      769 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/Pybind11Stubgen.cmake
--rw-r--r--   0        0        0     3848 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/SleipnirBuildTypes.cmake
--rw-r--r--   0        0        0      599 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/SleipnirCompilerFlags.cmake
--rw-r--r--   0        0        0      308 2024-04-02 04:30:42.432670 sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/SleipnirSubdirList.cmake
--rw-r--r--   0        0        0    33588 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Expression.hpp
--rw-r--r--   0        0        0     7555 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/ExpressionGraph.hpp
--rw-r--r--   0        0        0      536 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/ExpressionType.hpp
--rw-r--r--   0        0        0     1872 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Gradient.hpp
--rw-r--r--   0        0        0     2237 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Hessian.hpp
--rw-r--r--   0        0        0     4349 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Jacobian.hpp
--rw-r--r--   0        0        0     2165 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Profiler.hpp
--rw-r--r--   0        0        0    11634 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Variable.hpp
--rw-r--r--   0        0        0    15699 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/VariableBlock.hpp
--rw-r--r--   0        0        0    26943 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/VariableMatrix.hpp
--rw-r--r--   0        0        0    13118 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/control/OCPSolver.hpp
--rw-r--r--   0        0        0     7457 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/Constraints.hpp
--rw-r--r--   0        0        0    18482 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/OptimizationProblem.hpp
--rw-r--r--   0        0        0     1774 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverConfig.hpp
--rw-r--r--   0        0        0     2719 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverExitCondition.hpp
--rw-r--r--   0        0        0      763 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverIterationInfo.hpp
--rw-r--r--   0        0        0      904 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverStatus.hpp
--rw-r--r--   0        0        0     1778 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/solver/InteriorPoint.hpp
--rw-r--r--   0        0        0      843 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Assert.hpp
--rw-r--r--   0        0        0      743 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Concepts.hpp
--rw-r--r--   0        0        0     2773 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Formatters.hpp
--rw-r--r--   0        0        0     6089 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/IntrusiveSharedPtr.hpp
--rw-r--r--   0        0        0     4160 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Pool.hpp
--rw-r--r--   0        0        0     1290 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Print.hpp
--rw-r--r--   0        0        0     2198 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Spy.hpp
--rw-r--r--   0        0        0     7128 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/SymbolExports.hpp
--rw-r--r--   0        0        0      154 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/__init__.py
--rw-r--r--   0        0        0     1416 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/autodiff/__init__.py
--rw-r--r--   0        0        0      741 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/Binders.hpp
--rw-r--r--   0        0        0    70351 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/Docstrings.hpp
--rw-r--r--   0        0        0      899 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/Main.cpp
--rw-r--r--   0        0        0      483 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/NumPy.hpp
--rw-r--r--   0        0        0      959 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindExpressionType.cpp
--rw-r--r--   0        0        0      855 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindGradient.cpp
--rw-r--r--   0        0        0      641 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindHessian.cpp
--rw-r--r--   0        0        0      670 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindJacobian.cpp
--rw-r--r--   0        0        0     8942 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindVariable.cpp
--rw-r--r--   0        0        0    19493 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindVariableBlock.cpp
--rw-r--r--   0        0        0    22512 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindVariableMatrix.cpp
--rw-r--r--   0        0        0      972 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindConstraints.cpp
--rw-r--r--   0        0        0     3910 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindOptimizationProblem.cpp
--rw-r--r--   0        0        0     1944 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindSolverExitCondition.cpp
--rw-r--r--   0        0        0     1371 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindSolverIterationInfo.cpp
--rw-r--r--   0        0        0     1467 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindSolverStatus.cpp
--rw-r--r--   0        0        0       42 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/optimization/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/py.typed
--rw-r--r--   0        0        0    15046 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/gradient_test.py
--rw-r--r--   0        0        0     6144 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/hessian_test.py
--rw-r--r--   0        0        0     3531 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/jacobian_test.py
--rw-r--r--   0        0        0     4712 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/variable_matrix_test.py
--rw-r--r--   0        0        0      185 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/variable_test.py
--rw-r--r--   0        0        0     6029 2024-04-02 04:30:42.436670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/constraints_test.py
--rw-r--r--   0        0        0     2368 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/decision_variable_test.py
--rw-r--r--   0        0        0      969 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/linear_problem_test.py
--rw-r--r--   0        0        0     4213 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/nonlinear_problem_test.py
--rw-r--r--   0        0        0     3181 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py
--rw-r--r--   0        0        0     6874 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_cart_pole_test.py
--rw-r--r--   0        0        0     5452 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_differential_drive_test.py
--rw-r--r--   0        0        0     3791 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_double_integrator_test.py
--rw-r--r--   0        0        0     3247 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_flywheel_test.py
--rw-r--r--   0        0        0     3985 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/quadratic_problem_test.py
--rw-r--r--   0        0        0     4643 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/solver_exit_condition_test.py
--rw-r--r--   0        0        0     1624 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/trivial_problem_test.py
--rw-r--r--   0        0        0     1198 2024-04-02 04:30:42.732672 sleipnirgroup_jormungandr-0.0.1.dev98/pyproject.toml
--rw-r--r--   0        0        0      346 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/autodiff/Expression.cpp
--rw-r--r--   0        0        0     1406 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/Inertia.hpp
--rw-r--r--   0        0        0     5066 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/RegularizedLDLT.hpp
--rw-r--r--   0        0        0    30260 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/InteriorPoint.cpp
--rw-r--r--   0        0        0     2843 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/ErrorEstimate.hpp
--rw-r--r--   0        0        0     7944 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/FeasibilityRestoration.hpp
--rw-r--r--   0        0        0     4844 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/Filter.hpp
--rw-r--r--   0        0        0     1166 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/FractionToTheBoundaryRule.hpp
--rw-r--r--   0        0        0     1895 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/IsLocallyInfeasible.hpp
--rw-r--r--   0        0        0     1803 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/KKTError.hpp
--rw-r--r--   0        0        0      615 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/util/ScopeExit.hpp
--rw-r--r--   0        0        0      504 2024-04-02 04:30:42.440670 sleipnirgroup_jormungandr-0.0.1.dev98/src/util/ToMilliseconds.hpp
--rw-r--r--   0        0        0     8977 1970-01-01 00:00:00.000000 sleipnirgroup_jormungandr-0.0.1.dev98/PKG-INFO
+-rw-r--r--   0        0        0    11689 2024-04-02 04:50:20.272911 sleipnirgroup_jormungandr-0.0.1.dev99/CMakeLists.txt
+-rw-r--r--   0        0        0     1465 2024-04-02 04:50:20.272975 sleipnirgroup_jormungandr-0.0.1.dev99/LICENSE.txt
+-rw-r--r--   0        0        0     8573 2024-04-02 04:50:20.273061 sleipnirgroup_jormungandr-0.0.1.dev99/README.md
+-rw-r--r--   0        0        0       68 2024-04-02 04:50:20.273120 sleipnirgroup_jormungandr-0.0.1.dev99/SleipnirConfig.cmake.in
+-rw-r--r--   0        0        0     1163 2024-04-02 04:50:20.274881 sleipnirgroup_jormungandr-0.0.1.dev99/cmake/eigen-disable-fortran-support.patch
+-rw-r--r--   0        0        0      991 2024-04-02 04:50:20.274996 sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/Pybind11Mkdoc.cmake
+-rw-r--r--   0        0        0      769 2024-04-02 04:50:20.275087 sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/Pybind11Stubgen.cmake
+-rw-r--r--   0        0        0     3848 2024-04-02 04:50:20.275187 sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/SleipnirBuildTypes.cmake
+-rw-r--r--   0        0        0      599 2024-04-02 04:50:20.275262 sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/SleipnirCompilerFlags.cmake
+-rw-r--r--   0        0        0      308 2024-04-02 04:50:20.275454 sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/SleipnirSubdirList.cmake
+-rw-r--r--   0        0        0    33588 2024-04-02 04:50:20.279260 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Expression.hpp
+-rw-r--r--   0        0        0     7555 2024-04-02 04:50:20.279605 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/ExpressionGraph.hpp
+-rw-r--r--   0        0        0      536 2024-04-02 04:50:20.279673 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/ExpressionType.hpp
+-rw-r--r--   0        0        0     1872 2024-04-02 04:50:20.279734 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Gradient.hpp
+-rw-r--r--   0        0        0     2237 2024-04-02 04:50:20.279838 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Hessian.hpp
+-rw-r--r--   0        0        0     4349 2024-04-02 04:50:20.279938 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Jacobian.hpp
+-rw-r--r--   0        0        0     2165 2024-04-02 04:50:20.280059 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Profiler.hpp
+-rw-r--r--   0        0        0    11634 2024-04-02 04:50:20.280146 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Variable.hpp
+-rw-r--r--   0        0        0    15699 2024-04-02 04:50:20.280292 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/VariableBlock.hpp
+-rw-r--r--   0        0        0    26943 2024-04-02 04:50:20.280379 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/VariableMatrix.hpp
+-rw-r--r--   0        0        0    13118 2024-04-02 04:50:20.280499 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/control/OCPSolver.hpp
+-rw-r--r--   0        0        0     7457 2024-04-02 04:50:20.280593 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/Constraints.hpp
+-rw-r--r--   0        0        0    18482 2024-04-02 04:50:20.280676 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/OptimizationProblem.hpp
+-rw-r--r--   0        0        0     1774 2024-04-02 04:50:20.280809 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverConfig.hpp
+-rw-r--r--   0        0        0     2719 2024-04-02 04:50:20.280931 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverExitCondition.hpp
+-rw-r--r--   0        0        0      763 2024-04-02 04:50:20.281008 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverIterationInfo.hpp
+-rw-r--r--   0        0        0      904 2024-04-02 04:50:20.281086 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverStatus.hpp
+-rw-r--r--   0        0        0     1778 2024-04-02 04:50:20.281193 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/solver/InteriorPoint.hpp
+-rw-r--r--   0        0        0      843 2024-04-02 04:50:20.281302 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Assert.hpp
+-rw-r--r--   0        0        0      743 2024-04-02 04:50:20.281415 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Concepts.hpp
+-rw-r--r--   0        0        0     2773 2024-04-02 04:50:20.281504 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Formatters.hpp
+-rw-r--r--   0        0        0     6089 2024-04-02 04:50:20.281581 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/IntrusiveSharedPtr.hpp
+-rw-r--r--   0        0        0     4160 2024-04-02 04:50:20.281646 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Pool.hpp
+-rw-r--r--   0        0        0     1290 2024-04-02 04:50:20.281711 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Print.hpp
+-rw-r--r--   0        0        0     2198 2024-04-02 04:50:20.281776 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Spy.hpp
+-rw-r--r--   0        0        0     7128 2024-04-02 04:50:20.281861 sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/SymbolExports.hpp
+-rw-r--r--   0        0        0      154 2024-04-02 04:50:20.281959 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/__init__.py
+-rw-r--r--   0        0        0     1416 2024-04-02 04:50:20.282069 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/autodiff/__init__.py
+-rw-r--r--   0        0        0      741 2024-04-02 04:50:20.282177 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/Binders.hpp
+-rw-r--r--   0        0        0    70351 2024-04-02 04:50:20.282388 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/Docstrings.hpp
+-rw-r--r--   0        0        0      899 2024-04-02 04:50:20.282469 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/Main.cpp
+-rw-r--r--   0        0        0      483 2024-04-02 04:50:20.282531 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/NumPy.hpp
+-rw-r--r--   0        0        0      959 2024-04-02 04:50:20.282625 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindExpressionType.cpp
+-rw-r--r--   0        0        0      855 2024-04-02 04:50:20.282683 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindGradient.cpp
+-rw-r--r--   0        0        0      641 2024-04-02 04:50:20.282761 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindHessian.cpp
+-rw-r--r--   0        0        0      670 2024-04-02 04:50:20.282838 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindJacobian.cpp
+-rw-r--r--   0        0        0     8942 2024-04-02 04:50:20.282910 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindVariable.cpp
+-rw-r--r--   0        0        0    19493 2024-04-02 04:50:20.283022 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindVariableBlock.cpp
+-rw-r--r--   0        0        0    22512 2024-04-02 04:50:20.283107 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindVariableMatrix.cpp
+-rw-r--r--   0        0        0      972 2024-04-02 04:50:20.283235 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindConstraints.cpp
+-rw-r--r--   0        0        0     3910 2024-04-02 04:50:20.283301 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindOptimizationProblem.cpp
+-rw-r--r--   0        0        0     1944 2024-04-02 04:50:20.283364 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindSolverExitCondition.cpp
+-rw-r--r--   0        0        0     1371 2024-04-02 04:50:20.283445 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindSolverIterationInfo.cpp
+-rw-r--r--   0        0        0     1467 2024-04-02 04:50:20.283504 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindSolverStatus.cpp
+-rw-r--r--   0        0        0       42 2024-04-02 04:50:20.283583 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/optimization/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 04:50:20.283609 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/py.typed
+-rw-r--r--   0        0        0    15046 2024-04-02 04:50:20.283733 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/gradient_test.py
+-rw-r--r--   0        0        0     6144 2024-04-02 04:50:20.283801 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/hessian_test.py
+-rw-r--r--   0        0        0     3531 2024-04-02 04:50:20.283869 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/jacobian_test.py
+-rw-r--r--   0        0        0     4712 2024-04-02 04:50:20.283930 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/variable_matrix_test.py
+-rw-r--r--   0        0        0      185 2024-04-02 04:50:20.284084 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/variable_test.py
+-rw-r--r--   0        0        0     6029 2024-04-02 04:50:20.284194 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/constraints_test.py
+-rw-r--r--   0        0        0     2368 2024-04-02 04:50:20.284273 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/decision_variable_test.py
+-rw-r--r--   0        0        0      969 2024-04-02 04:50:20.284354 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/linear_problem_test.py
+-rw-r--r--   0        0        0     4213 2024-04-02 04:50:20.284434 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/nonlinear_problem_test.py
+-rw-r--r--   0        0        0     3181 2024-04-02 04:50:20.284526 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py
+-rw-r--r--   0        0        0     6874 2024-04-02 04:50:20.284620 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_cart_pole_test.py
+-rw-r--r--   0        0        0     5452 2024-04-02 04:50:20.284714 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_differential_drive_test.py
+-rw-r--r--   0        0        0     3791 2024-04-02 04:50:20.284816 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_double_integrator_test.py
+-rw-r--r--   0        0        0     3247 2024-04-02 04:50:20.284902 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_flywheel_test.py
+-rw-r--r--   0        0        0     3985 2024-04-02 04:50:20.284987 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/quadratic_problem_test.py
+-rw-r--r--   0        0        0     4643 2024-04-02 04:50:20.285067 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/solver_exit_condition_test.py
+-rw-r--r--   0        0        0     1624 2024-04-02 04:50:20.285136 sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/trivial_problem_test.py
+-rw-r--r--   0        0        0     1198 2024-04-02 04:50:36.253545 sleipnirgroup_jormungandr-0.0.1.dev99/pyproject.toml
+-rw-r--r--   0        0        0      346 2024-04-02 04:50:20.286730 sleipnirgroup_jormungandr-0.0.1.dev99/src/autodiff/Expression.cpp
+-rw-r--r--   0        0        0     1406 2024-04-02 04:50:20.286863 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/Inertia.hpp
+-rw-r--r--   0        0        0     5066 2024-04-02 04:50:20.286956 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/RegularizedLDLT.hpp
+-rw-r--r--   0        0        0    30260 2024-04-02 04:50:20.287131 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/InteriorPoint.cpp
+-rw-r--r--   0        0        0     2843 2024-04-02 04:50:20.287251 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/ErrorEstimate.hpp
+-rw-r--r--   0        0        0     7944 2024-04-02 04:50:20.287352 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/FeasibilityRestoration.hpp
+-rw-r--r--   0        0        0     4844 2024-04-02 04:50:20.287448 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/Filter.hpp
+-rw-r--r--   0        0        0     1166 2024-04-02 04:50:20.287522 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/FractionToTheBoundaryRule.hpp
+-rw-r--r--   0        0        0     1895 2024-04-02 04:50:20.287594 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/IsLocallyInfeasible.hpp
+-rw-r--r--   0        0        0     1803 2024-04-02 04:50:20.287662 sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/KKTError.hpp
+-rw-r--r--   0        0        0      615 2024-04-02 04:50:20.287752 sleipnirgroup_jormungandr-0.0.1.dev99/src/util/ScopeExit.hpp
+-rw-r--r--   0        0        0      504 2024-04-02 04:50:20.287817 sleipnirgroup_jormungandr-0.0.1.dev99/src/util/ToMilliseconds.hpp
+-rw-r--r--   0        0        0     8977 1970-01-01 00:00:00.000000 sleipnirgroup_jormungandr-0.0.1.dev99/PKG-INFO
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/CMakeLists.txt` & `sleipnirgroup_jormungandr-0.0.1.dev99/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/LICENSE.txt` & `sleipnirgroup_jormungandr-0.0.1.dev99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/README.md` & `sleipnirgroup_jormungandr-0.0.1.dev99/README.md`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/cmake/eigen-disable-fortran-support.patch` & `sleipnirgroup_jormungandr-0.0.1.dev99/cmake/eigen-disable-fortran-support.patch`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/Pybind11Mkdoc.cmake` & `sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/Pybind11Mkdoc.cmake`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/Pybind11Stubgen.cmake` & `sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/Pybind11Stubgen.cmake`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/SleipnirBuildTypes.cmake` & `sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/SleipnirBuildTypes.cmake`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/cmake/modules/SleipnirCompilerFlags.cmake` & `sleipnirgroup_jormungandr-0.0.1.dev99/cmake/modules/SleipnirCompilerFlags.cmake`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Expression.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Expression.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/ExpressionGraph.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/ExpressionGraph.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/ExpressionType.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/ExpressionType.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Gradient.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Gradient.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Hessian.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Hessian.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Jacobian.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Jacobian.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Profiler.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Profiler.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/Variable.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/Variable.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/VariableBlock.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/VariableBlock.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/autodiff/VariableMatrix.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/autodiff/VariableMatrix.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/control/OCPSolver.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/control/OCPSolver.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/Constraints.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/Constraints.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/OptimizationProblem.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/OptimizationProblem.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverConfig.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverConfig.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverExitCondition.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverExitCondition.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverIterationInfo.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverIterationInfo.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/SolverStatus.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/SolverStatus.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/optimization/solver/InteriorPoint.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/optimization/solver/InteriorPoint.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Assert.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Assert.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Concepts.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Concepts.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Formatters.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Formatters.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/IntrusiveSharedPtr.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/IntrusiveSharedPtr.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Pool.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Pool.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Print.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Print.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/Spy.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/Spy.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/include/sleipnir/util/SymbolExports.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/include/sleipnir/util/SymbolExports.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/autodiff/__init__.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/autodiff/__init__.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/Binders.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/Binders.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/Docstrings.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/Docstrings.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/Main.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/Main.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindExpressionType.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindExpressionType.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindGradient.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindGradient.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindHessian.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindHessian.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindJacobian.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindJacobian.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindVariable.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindVariable.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindVariableBlock.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindVariableBlock.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/autodiff/BindVariableMatrix.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/autodiff/BindVariableMatrix.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindConstraints.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindConstraints.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindOptimizationProblem.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindOptimizationProblem.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindSolverExitCondition.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindSolverExitCondition.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindSolverIterationInfo.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindSolverIterationInfo.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/cpp/optimization/BindSolverStatus.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/cpp/optimization/BindSolverStatus.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/gradient_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/gradient_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/hessian_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/hessian_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/jacobian_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/jacobian_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/autodiff/variable_matrix_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/autodiff/variable_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/constraints_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/constraints_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/decision_variable_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/decision_variable_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/linear_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/linear_problem_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/nonlinear_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/nonlinear_problem_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_arm_on_elevator_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_cart_pole_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_cart_pole_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_differential_drive_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_differential_drive_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_double_integrator_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_double_integrator_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/optimization_problem_flywheel_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/optimization_problem_flywheel_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/quadratic_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/quadratic_problem_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/solver_exit_condition_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/solver_exit_condition_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/jormungandr/test/optimization/trivial_problem_test.py` & `sleipnirgroup_jormungandr-0.0.1.dev99/jormungandr/test/optimization/trivial_problem_test.py`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/pyproject.toml` & `sleipnirgroup_jormungandr-0.0.1.dev99/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "sleipnirgroup-jormungandr"
 description = "A linearity-exploiting sparse nonlinear constrained optimization problem solver that uses the interior-point method."
-version = "0.0.1.dev98"
+version = "0.0.1.dev99"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [ "matplotlib", "numpy", "scipy" ]
 
   [project.license]
   file = "LICENSE.txt"
```

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/Inertia.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/Inertia.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/RegularizedLDLT.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/RegularizedLDLT.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/InteriorPoint.cpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/InteriorPoint.cpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/ErrorEstimate.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/ErrorEstimate.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/FeasibilityRestoration.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/FeasibilityRestoration.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/Filter.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/Filter.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/FractionToTheBoundaryRule.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/FractionToTheBoundaryRule.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/IsLocallyInfeasible.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/IsLocallyInfeasible.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/optimization/solver/util/KKTError.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/optimization/solver/util/KKTError.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/src/util/ScopeExit.hpp` & `sleipnirgroup_jormungandr-0.0.1.dev99/src/util/ScopeExit.hpp`

 * *Files identical despite different names*

### Comparing `sleipnirgroup_jormungandr-0.0.1.dev98/PKG-INFO` & `sleipnirgroup_jormungandr-0.0.1.dev99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleipnirgroup-jormungandr
-Version: 0.0.1.dev98
+Version: 0.0.1.dev99
 Summary: A linearity-exploiting sparse nonlinear constrained optimization problem solver that uses the interior-point method.
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Project-URL: Documentation, https://sleipnirgroup.github.io/Sleipnir/
```

