# Comparing `tmp/ansys_optislang_core-0.7.0.tar.gz` & `tmp/ansys_optislang_core-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_optislang_core-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_optislang_core-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_optislang_core-0.7.0.tar` & `ansys_optislang_core-0.7.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1089 2024-04-29 09:33:35.871300 ansys_optislang_core-0.7.0/LICENSE
--rw-r--r--   0        0        0     7471 2024-04-29 09:33:35.871300 ansys_optislang_core-0.7.0/README.rst
--rw-r--r--   0        0        0     2253 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2198 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/__init__.py
--rw-r--r--   0        0        0     7292 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/application.py
--rw-r--r--   0        0        0     3328 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/encoding.py
--rw-r--r--   0        0        0     2100 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/errors.py
--rw-r--r--   0        0        0     2250 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp
--rw-r--r--   0        0        0   235264 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb
--rw-r--r--   0        0        0     3813 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py
--rw-r--r--   0        0        0    28174 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf
--rw-r--r--   0        0        0    73304 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf
--rw-r--r--   0        0        0    25280 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf
--rw-r--r--   0        0        0    47797 2024-04-29 09:33:35.879300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf
--rw-r--r--   0        0        0   146518 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf
--rw-r--r--   0        0        0   212239 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf
--rw-r--r--   0        0        0      299 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.bat
--rw-r--r--   0        0        0     2966 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py
--rw-r--r--   0        0        0     4438 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s
--rw-r--r--   0        0        0      194 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.sh
--rw-r--r--   0        0        0     1401 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt
--rw-r--r--   0        0        0     1989 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt
--rw-r--r--   0        0        0     4596 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py
--rw-r--r--   0        0        0     4081 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py
--rw-r--r--   0        0        0     5483 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py
--rw-r--r--   0        0        0     5002 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py
--rw-r--r--   0        0        0     4428 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py
--rw-r--r--   0        0        0     4992 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py
--rw-r--r--   0        0        0    10784 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py
--rw-r--r--   0        0        0     7325 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py
--rw-r--r--   0        0        0     1629 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py
--rw-r--r--   0        0        0     3755 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py
--rw-r--r--   0        0        0     2405 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py
--rw-r--r--   0        0        0     1906 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py
--rw-r--r--   0        0        0     2521 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py
--rw-r--r--   0        0        0     1780 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py
--rw-r--r--   0        0        0     5243 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py
--rw-r--r--   0        0        0     2872 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac
--rw-r--r--   0        0        0      686 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out
--rw-r--r--   0        0        0    10909 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s
--rw-r--r--   0        0        0      686 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out
--rw-r--r--   0        0        0    10785 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s
--rw-r--r--   0        0        0    34914 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz
--rw-r--r--   0        0        0     3222 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py
--rw-r--r--   0        0        0     6443 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py
--rw-r--r--   0        0        0     2164 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py
--rw-r--r--   0        0        0     5697 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py
--rw-r--r--   0        0        0     1240 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/__init__.py
--rw-r--r--   0        0        0     3090 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/downloads.py
--rw-r--r--   0        0        0     7119 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/examples.py
--rw-r--r--   0        0        0     7808 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/io.py
--rw-r--r--   0        0        0    10077 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/logging.py
--rw-r--r--   0        0        0    12455 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/managers.py
--rw-r--r--   0        0        0    30303 2024-04-29 09:33:35.883300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/node_types.py
--rw-r--r--   0        0        0    52843 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/nodes.py
--rw-r--r--   0        0        0    36959 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/optislang.py
--rw-r--r--   0        0        0    42928 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_process.py
--rw-r--r--   0        0        0     5738 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_server.py
--rw-r--r--   0        0        0    13918 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/project.py
--rw-r--r--   0        0        0   132646 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/project_parametric.py
--rw-r--r--   0        0        0     8922 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/application.py
--rw-r--r--   0        0        0    20317 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/managers.py
--rw-r--r--   0        0        0   116145 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/nodes.py
--rw-r--r--   0        0        0   178734 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/osl_server.py
--rw-r--r--   0        0        0    20093 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/project.py
--rw-r--r--   0        0        0    59114 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_commands.py
--rw-r--r--   0        0        0    25617 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_queries.py
--rw-r--r--   0        0        0    16155 2024-04-29 09:33:35.887300 ansys_optislang_core-0.7.0/src/ansys/optislang/core/utils.py
--rw-r--r--   0        0        0     9157 1970-01-01 00:00:00.000000 ansys_optislang_core-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-05-02 10:35:08.077622 ansys_optislang_core-0.7.1/LICENSE
+-rw-r--r--   0        0        0     7471 2024-05-02 10:35:08.077622 ansys_optislang_core-0.7.1/README.rst
+-rw-r--r--   0        0        0     2253 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2198 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/__init__.py
+-rw-r--r--   0        0        0     7292 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/application.py
+-rw-r--r--   0        0        0     3328 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/encoding.py
+-rw-r--r--   0        0        0     2100 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/errors.py
+-rw-r--r--   0        0        0     2250 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp
+-rw-r--r--   0        0        0   235264 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb
+-rw-r--r--   0        0        0     3813 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py
+-rw-r--r--   0        0        0    28174 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf
+-rw-r--r--   0        0        0    73304 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf
+-rw-r--r--   0        0        0    25280 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf
+-rw-r--r--   0        0        0    47797 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf
+-rw-r--r--   0        0        0   146518 2024-05-02 10:35:08.089622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf
+-rw-r--r--   0        0        0   212239 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf
+-rw-r--r--   0        0        0      299 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.bat
+-rw-r--r--   0        0        0     2966 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py
+-rw-r--r--   0        0        0     4438 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s
+-rw-r--r--   0        0        0      194 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.sh
+-rw-r--r--   0        0        0     1401 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt
+-rw-r--r--   0        0        0     1989 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt
+-rw-r--r--   0        0        0     4596 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py
+-rw-r--r--   0        0        0     4081 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py
+-rw-r--r--   0        0        0     5483 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py
+-rw-r--r--   0        0        0     5002 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py
+-rw-r--r--   0        0        0     4428 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py
+-rw-r--r--   0        0        0     4992 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py
+-rw-r--r--   0        0        0    10784 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py
+-rw-r--r--   0        0        0     7325 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py
+-rw-r--r--   0        0        0     1629 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py
+-rw-r--r--   0        0        0     3755 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py
+-rw-r--r--   0        0        0     2405 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py
+-rw-r--r--   0        0        0     1906 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py
+-rw-r--r--   0        0        0     2521 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py
+-rw-r--r--   0        0        0     1780 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py
+-rw-r--r--   0        0        0     5243 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py
+-rw-r--r--   0        0        0     2872 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac
+-rw-r--r--   0        0        0      686 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out
+-rw-r--r--   0        0        0    10909 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s
+-rw-r--r--   0        0        0      686 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out
+-rw-r--r--   0        0        0    10785 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s
+-rw-r--r--   0        0        0    34914 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz
+-rw-r--r--   0        0        0     3222 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py
+-rw-r--r--   0        0        0     6443 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py
+-rw-r--r--   0        0        0     2164 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py
+-rw-r--r--   0        0        0     5697 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py
+-rw-r--r--   0        0        0     1240 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/__init__.py
+-rw-r--r--   0        0        0     3090 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/downloads.py
+-rw-r--r--   0        0        0     7119 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/examples.py
+-rw-r--r--   0        0        0     7808 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/io.py
+-rw-r--r--   0        0        0    10077 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/logging.py
+-rw-r--r--   0        0        0    12455 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/managers.py
+-rw-r--r--   0        0        0    30303 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/node_types.py
+-rw-r--r--   0        0        0    52843 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/nodes.py
+-rw-r--r--   0        0        0    36959 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/optislang.py
+-rw-r--r--   0        0        0    42928 2024-05-02 10:35:08.093622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/osl_process.py
+-rw-r--r--   0        0        0     5738 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/osl_server.py
+-rw-r--r--   0        0        0    13918 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/project.py
+-rw-r--r--   0        0        0   132646 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/project_parametric.py
+-rw-r--r--   0        0        0     8922 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/application.py
+-rw-r--r--   0        0        0    20317 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/managers.py
+-rw-r--r--   0        0        0   116145 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/nodes.py
+-rw-r--r--   0        0        0   178622 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/osl_server.py
+-rw-r--r--   0        0        0    20093 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/project.py
+-rw-r--r--   0        0        0    59114 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/server_commands.py
+-rw-r--r--   0        0        0    25617 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/server_queries.py
+-rw-r--r--   0        0        0    16155 2024-05-02 10:35:08.097622 ansys_optislang_core-0.7.1/src/ansys/optislang/core/utils.py
+-rw-r--r--   0        0        0     9157 1970-01-01 00:00:00.000000 ansys_optislang_core-0.7.1/PKG-INFO
```

### Comparing `ansys_optislang_core-0.7.0/LICENSE` & `ansys_optislang_core-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/README.rst` & `ansys_optislang_core-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/pyproject.toml` & `ansys_optislang_core-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-optislang-core"
-version = "0.7.0"
+version = "0.7.1"
 description = "A Python wrapper for Ansys optiSLang application."
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/__init__.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/application.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/application.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/encoding.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/encoding.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/errors.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/errors.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.inp`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/files/oscillator.odb`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/etk_abaqus/scripts/etk_abaqus.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/calculator.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/calculator_with_params.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/connect_nodes.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/nested_systems.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/omdb_files.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/files/ten_bar_truss.opf`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_reference.txt`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/files/oscillator_signal.txt`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/_create_oscillator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_ea.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_optimization_on_mop.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_robustness_arsm.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_sensitivity_mop.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillator_system_python.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_ascii.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/oscillator/scripts/oscillatorcalibration_system_python.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_help.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/python/scripts/python_node.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/ansys_workbench_portscan.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/create_all_possible_nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/optimizer_settings.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/sensitivity_settings.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/scripts/simple_calculator.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ansys_link.mac`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.out`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.out`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss2.s`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/files/ten_bar_truss_apdl.wbpz`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ansys_workbench_ten_bar_truss.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/arsm_ten_bar_truss.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_modify_parameters.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/00_run_script/ten_bar_truss/scripts/ten_bar_truss_lc2.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/__init__.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/downloads.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/examples/examples.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/examples/examples.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/io.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/io.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/logging.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/managers.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/managers.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/node_types.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/node_types.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/nodes.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/optislang.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/optislang.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_process.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/osl_process.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/osl_server.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/osl_server.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/project.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/project.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/project_parametric.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/project_parametric.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/application.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/application.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/managers.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/managers.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/nodes.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/nodes.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/osl_server.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/osl_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -3016,17 +3016,14 @@
             Raised when the command or query fails.
         TimeoutError
             Raised when the timeout float value expires.
         """
         file_path = self.__cast_to_path(file_path=file_path)
         self.__validate_path(file_path=file_path)
 
-        if not file_path.is_file():
-            raise FileNotFoundError(f'File "{file_path}" doesn\'t exist.')
-
         current_func_name = self.open.__name__
 
         if self.__osl_version[0] < 24:
             self._logger.error(
                 f"Command ``open`` doesn't work correctly in version {self.__osl_version_string}."
                 " Please use at least version 24.1."
             )
```

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/project.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/project.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_commands.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/server_commands.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/tcp/server_queries.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/tcp/server_queries.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/src/ansys/optislang/core/utils.py` & `ansys_optislang_core-0.7.1/src/ansys/optislang/core/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_optislang_core-0.7.0/PKG-INFO` & `ansys_optislang_core-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-optislang-core
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python wrapper for Ansys optiSLang application.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

