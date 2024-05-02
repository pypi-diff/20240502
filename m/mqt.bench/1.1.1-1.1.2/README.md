# Comparing `tmp/mqt.bench-1.1.1.tar.gz` & `tmp/mqt_bench-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.bench-1.1.1.tar", last modified: Thu Apr 11 12:11:54 2024, max compression
+gzip compressed data, was "mqt_bench-1.1.2.tar", last modified: Thu May  2 14:39:07 2024, max compression
```

## Comparing `mqt.bench-1.1.1.tar` & `mqt_bench-1.1.2.tar`

### file list

```diff
@@ -1,166 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.795949 mqt.bench-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.755949 mqt.bench-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.755949 mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.755949 mqt.bench-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/test_pregenerated_zip.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-11 12:11:54.795949 mqt.bench-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.759949 mqt.bench-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Abstraction_levels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Benchmark_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/DevelopmentGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Parameter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/References.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Support.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.763949 mqt.bench-1.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/arch.png
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)   100569 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/erc_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)   102052 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/erc_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40262 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    84500 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    76051 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_3.png
--rw-r--r--   0 runner    (1001) docker     (127)   112485 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_4.png
--rw-r--r--   0 runner    (1001) docker     (127)   184498 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/logo-bavaria.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/logo-mqv.svg
--rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    57266 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/mqt_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   196044 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/mqtbench.png
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/tum_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/tum_light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.763949 mqt.bench-1.1.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:11:54.795949 mqt.bench-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.751949 mqt.bench-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.751949 mqt.bench-1.1.1/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.763949 mqt.bench-1.1.1/src/mqt/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18948 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmark_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/ae.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/dj.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/graphstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/grover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qft.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qftentangled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_nature/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeexact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeinexact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qwalk.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/realamprandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/shor.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/su2random.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/twolocalrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/vqe.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/wstate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/calibration_files/
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_montreal_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)    58070 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_washington_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_aria1_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_harmony_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/oqc_lucy_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)    55310 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.771949 mqt.bench-1.1.1/src/mqt/bench/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/ionq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/oqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/quantinuum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/rigetti.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.787949 mqt.bench-1.1.1/src/mqt/bench/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127) 15925096 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_data.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/pie.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/qubit_dist.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    24774 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/violins.pdf
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/qiskit_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/tket_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26385 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/MQTBench_all.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/qasm_output/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/qasm_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/tum_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/benchmark_description.html
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/description.html
--rw-r--r--   0 runner    (1001) docker     (127)    28601 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/legal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_ibm_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_ionq_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_oqc_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_quantinuum_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_rigetti_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    30958 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    15211 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/test_benchviewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/test_pregenerated_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.075947 mqt_bench-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.031947 mqt_bench-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.031947 mqt_bench-1.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.031947 mqt_bench-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-05-02 14:39:07.075947 mqt_bench-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.035947 mqt_bench-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Abstraction_levels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Benchmark_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/DevelopmentGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Parameter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/References.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/Usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.039947 mqt_bench-1.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/arch.png
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)   100569 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/erc_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   102052 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/erc_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40262 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/level_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84500 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/level_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76051 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/level_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112485 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/level_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   184498 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/logo-bavaria.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/logo-mqv.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57266 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   196044 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/mqtbench.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/tum_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_static/tum_light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.039947 mqt_bench-1.1.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:39:07.075947 mqt_bench-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.027947 mqt_bench-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.027947 mqt_bench-1.1.2/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.039947 mqt_bench-1.1.2/src/mqt/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19064 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmark_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.043947 mqt_bench-1.1.2/src/mqt/bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/dj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/graphstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qftentangled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.043947 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.043947 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.043947 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_nature/
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.047947 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qpeexact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qpeinexact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/qwalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/realamprandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/shor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/su2random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/twolocalrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/vqe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/benchmarks/wstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.047947 mqt_bench-1.1.2/src/mqt/bench/calibration_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/ibm_montreal_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58070 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/ibm_washington_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/ionq_aria1_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/ionq_harmony_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/oqc_lucy_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    55310 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.047947 mqt_bench-1.1.2/src/mqt/bench/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/ionq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/oqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/quantinuum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/devices/rigetti.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.067947 mqt_bench-1.1.2/src/mqt/bench/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127) 15925096 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/evaluation_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/evaluation_visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.067947 mqt_bench-1.1.2/src/mqt/bench/evaluation/results/
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/results/pie.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/results/qubit_dist.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    24774 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/evaluation/results/violins.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/qiskit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/tket_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.067947 mqt_bench-1.1.2/src/mqt/bench/viewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26319 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/src/mqt/bench/viewer/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/src/mqt/bench/viewer/static/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/static/files/MQTBench_all.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/src/mqt/bench/viewer/static/files/qasm_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/static/files/qasm_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/static/tum_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/src/mqt/bench/viewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/templates/benchmark_description.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/templates/description.html
+-rw-r--r--   0 runner    (1001) docker     (127)    29071 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/src/mqt/bench/viewer/templates/legal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/src/mqt.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-05-02 14:39:06.000000 mqt_bench-1.1.2/src/mqt.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-02 14:39:07.000000 mqt_bench-1.1.2/src/mqt.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:39:06.000000 mqt_bench-1.1.2/src/mqt.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-02 14:39:06.000000 mqt_bench-1.1.2/src/mqt.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-02 14:39:06.000000 mqt_bench-1.1.2/src/mqt.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 14:39:06.000000 mqt_bench-1.1.2/src/mqt.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:39:07.071947 mqt_bench-1.1.2/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/devices/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/devices/test_ibm_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/devices/test_ionq_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/devices/test_oqc_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/devices/test_quantinuum_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/devices/test_rigetti_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30664 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/test_benchviewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-02 14:39:01.000000 mqt_bench-1.1.2/tests/test_pregenerated_zip.py
```

### Comparing `mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/bug-report.yml` & `mqt_bench-1.1.2/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `mqt_bench-1.1.2/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.github/contributing.rst` & `mqt_bench-1.1.2/.github/contributing.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.github/dependabot.yml` & `mqt_bench-1.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.github/release-drafter.yml` & `mqt_bench-1.1.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.github/support.rst` & `mqt_bench-1.1.2/.github/support.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.github/workflows/deploy.yml` & `mqt_bench-1.1.2/.github/workflows/cd.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,90 +1,49 @@
-name: Deploy to PyPI
-
+name: CD
 on:
   release:
     types: [published]
-  push:
-    branches: [main]
-  pull_request:
   workflow_dispatch:
 
-concurrency:
-  group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
-  cancel-in-progress: true
-
-env:
-  DEPLOY_KEY: ${{ secrets.DEPLOY_KEY }}
-  KNOWN_HOSTS: ${{ secrets.KNOWN_HOSTS }}
-  CDA_HOST_NAME: tueicda-cda.srv.mwn.de
-  CDA_USER_NAME: web-user
-  CDA_TARGET_DIR: /var/www/cda/app/mqtbench/
-
 jobs:
-  build_wheel:
-    name: Build wheel
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-        with:
-          fetch-depth: 0
-      - uses: actions/setup-python@v5
-        with:
-          python-version: "3.10"
-        name: Install Python
-      - name: Build wheel
-        run: pipx run build --wheel
-      - name: Install wheel
-        run: python -m pip install --verbose dist/*.whl
-      - uses: actions/upload-artifact@v4
-        with:
-          name: cibw-wheel
-          path: dist/*.whl
-
-  build_sdist:
-    name: Build source distribution
-    runs-on: ubuntu-latest
-    steps:
-      - uses: actions/checkout@v4
-        with:
-          fetch-depth: 0
-      - uses: actions/setup-python@v5
-        with:
-          python-version: "3.10"
-        name: Install Python
-      - name: Build sdist
-        run: pipx run build --sdist
-      - name: Install sdist
-        run: python -m pip install --verbose dist/*.tar.gz
-      - uses: actions/upload-artifact@v4
-        with:
-          name: cibw-sdist
-          path: dist/*.tar.gz
+  python-packaging:
+    name: 🐍 Packaging
+    uses: cda-tum/mqt-core/.github/workflows/reusable-python-packaging.yml@v2.4.1
+    with:
+      pure-python: true
 
-  upload_pypi:
-    needs: [build_wheel, build_sdist]
-    runs-on: ubuntu-latest
+  deploy:
     if: github.event_name == 'release' && github.event.action == 'published'
+    name: 🚀 Deploy to PyPI
+    runs-on: ubuntu-latest
     environment:
       name: pypi
       url: https://pypi.org/p/mqt.bench
     permissions:
       id-token: write
+    needs: [python-packaging]
     steps:
       - uses: actions/download-artifact@v4
         with:
           pattern: cibw-*
           path: dist
           merge-multiple: true
       - uses: pypa/gh-action-pypi-publish@release/v1
 
   upload_webserver:
-    needs: upload_pypi
-    runs-on: ubuntu-latest
     if: github.event_name == 'release' && github.event.action == 'published'
+    name: 🚀 Deploy to Webserver
+    needs: deploy
+    runs-on: ubuntu-latest
+    env:
+      DEPLOY_KEY: ${{ secrets.DEPLOY_KEY }}
+      KNOWN_HOSTS: ${{ secrets.KNOWN_HOSTS }}
+      CDA_HOST_NAME: tueicda-cda.srv.mwn.de
+      CDA_USER_NAME: web-user
+      CDA_TARGET_DIR: /var/www/cda/app/mqtbench/
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Create version file
         run: |
           echo "version = \"$(git describe --tags --always)\"" > mqtbench_version.txt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mqt.bench-1.1.1/.gitignore` & `mqt_bench-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/.pre-commit-config.yaml` & `mqt_bench-1.1.2/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -50,25 +50,25 @@
       - id: nb-clean
   # Check for spelling
   - repo: https://github.com/codespell-project/codespell
     rev: "v2.2.6"
     hooks:
       - id: codespell
         args: ["-L", "wille,linz,fro"]
-        exclude: "mqt/benchviewer/templates/legal.html"
+        exclude: "mqt/bench/viewer/templates/legal.html"
 
   # Format configuration files with prettier
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.2
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
@@ -76,15 +76,15 @@
   - repo: https://github.com/adamchainz/blacken-docs
     rev: 1.16.0
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==23.*]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: mypy
         files: ^(src|tests)
         args: []
         additional_dependencies:
           - pytket_qiskit
           - qiskit_optimization
@@ -104,11 +104,11 @@
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest|Mqt|Tum
         exclude: .pre-commit-config.yaml
 
   # Check best practices for scientific Python code
   - repo: https://github.com/scientific-python/cookie
-    rev: 2024.03.10
+    rev: 2024.04.23
     hooks:
       - id: sp-repo-review
         additional_dependencies: ["repo-review[cli]"]
```

### Comparing `mqt.bench-1.1.1/.readthedocs.yaml` & `mqt_bench-1.1.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/LICENSE` & `mqt_bench-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/PKG-INFO` & `mqt_bench-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.1.1
+Version: 1.1.2
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@tum.de>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,32 +42,30 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket-qiskit<0.53.0,>=0.50.0
-Requires-Dist: qiskit_optimization
-Requires-Dist: qiskit_nature
-Requires-Dist: qiskit_finance
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: flask>=2.0.0
-Requires-Dist: networkx>=2.0.0
-Requires-Dist: pyscf>=2.3.0
+Requires-Dist: pytket-qiskit<0.54.0,>=0.53.0
+Requires-Dist: qiskit_optimization>=0.6
+Requires-Dist: qiskit_nature[pyscf]>=0.7
+Requires-Dist: qiskit_finance>=0.4.1
+Requires-Dist: pandas>=2.1.2
+Requires-Dist: flask>=2.3.0
+Requires-Dist: networkx>=2.8.8
 Requires-Dist: packaging>=21.0
-Requires-Dist: tqdm>=4.0.0
+Requires-Dist: tqdm>=4.29.0
 Requires-Dist: joblib>=1.3.0
-Requires-Dist: importlib_metadata>=3.6; python_version < "3.10"
-Requires-Dist: importlib_resources>=5.9; python_version < "3.10"
 Provides-Extra: test
 Requires-Dist: pytest>=7.2; extra == "test"
+Requires-Dist: pytest-console-scripts>=1.4; extra == "test"
 Provides-Extra: coverage
 Requires-Dist: mqt.bench[test]; extra == "coverage"
-Requires-Dist: pytest-cov[toml]; extra == "coverage"
+Requires-Dist: pytest-cov>=4; extra == "coverage"
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == "docs"
 Requires-Dist: sphinx~=7.0; extra == "docs"
 Requires-Dist: setuptools-scm>=7; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.4.2; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-hoverxref; extra == "docs"
@@ -78,31 +76,35 @@
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: qiskit[visualization]; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mqt.bench[coverage,docs]; extra == "dev"
 
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)](https://pypi.org/project/mqt.bench/)
+![OS](https://img.shields.io/badge/os-linux%20%7C%20macos%20%7C%20windows-blue?style=flat-square)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
-[![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/coverage.yml?branch=main&style=flat-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/actions/workflows/coverage.yml)
-[![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/workflows/deploy.yml)
+[![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-bench/ci.yml?branch=main&style=flat-square&logo=github&label=ci)](https://github.com/cda-tum/mqt-bench/actions/workflows/ci.yml)
+[![CD](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-bench/cd.yml?style=flat-square&logo=github&label=cd)](https://github.com/cda-tum/mqt-bench/actions/workflows/cd.yml)
+[![Documentation](https://img.shields.io/readthedocs/bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/bench)
 [![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-bench)
-[![Documentation](https://img.shields.io/readthedocs/mqt-bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/bench)
 
 <p align="center">
 <picture>
+<a href="https://mqt.readthedocs.io/projects/bench">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/mqt_light.png" width="60%">
   <img src="https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/mqt_dark.png" width="60%">
+</a>
 </picture>
 </p>
 
 # MQT Bench: Benchmarking Software and Design Automation Tools for Quantum Computing
 
 MQT Bench is a quantum circuit benchmark suite with cross-level support, i.e., providing the same benchmark algorithms for different abstraction levels throughout the quantum computing
 software stack.
+MQT Bench is part of the [_Munich Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io) developed by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/).
 
 <p align="center">
   <a href="https://mqt.readthedocs.io/projects/bench">
   <img width=30% src="https://img.shields.io/badge/documentation-blue?style=for-the-badge&logo=read%20the%20docs" alt="Documentation" />
   </a>
 </p>
 
@@ -130,22 +132,17 @@
 
 # draw the circuit
 print(qc_algorithmic_level.draw())
 ```
 
 **Detailed documentation and examples are available at [ReadTheDocs](https://mqt.readthedocs.io/projects/bench).**
 
-# Repository Structure
+## Availability as a PennyLane Dataset
 
-- src/mqt/: main source directory
-  - bench: Directory for the MQT Bench package
-  - bench/benchmarks: Directory for the benchmarks
-  - benchviewer: Directory for the webpage (which can be started locally and is also hosted at
-    [https://www.cda.cit.tum.de/mqtbench/](https://www.cda.cit.tum.de/mqtbench/))
-- tests: Directory for the tests for MQT Bench
+MQT Bench is also available as a [Pennylane dataset](https://pennylane.ai/datasets/other/mqt-bench).
 
 ## Acknowledgements
 
 The Munich Quantum Toolkit has been supported by the European
 Research Council (ERC) under the European Union's Horizon 2020 research and innovation program (grant agreement
 No. 101001318), the Bavarian State Ministry for Science and Arts through the Distinguished Professorship Program, as well as the
 Munich Quantum Valley, which is supported by the Bavarian state government with funds from the Hightech Agenda Bayern Plus.
```

### Comparing `mqt.bench-1.1.1/README.md` & `mqt_bench-1.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)](https://pypi.org/project/mqt.bench/)
+![OS](https://img.shields.io/badge/os-linux%20%7C%20macos%20%7C%20windows-blue?style=flat-square)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
-[![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/coverage.yml?branch=main&style=flat-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/actions/workflows/coverage.yml)
-[![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/workflows/deploy.yml)
+[![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-bench/ci.yml?branch=main&style=flat-square&logo=github&label=ci)](https://github.com/cda-tum/mqt-bench/actions/workflows/ci.yml)
+[![CD](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-bench/cd.yml?style=flat-square&logo=github&label=cd)](https://github.com/cda-tum/mqt-bench/actions/workflows/cd.yml)
+[![Documentation](https://img.shields.io/readthedocs/bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/bench)
 [![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-bench)
-[![Documentation](https://img.shields.io/readthedocs/mqt-bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/bench)
 
 <p align="center">
 <picture>
+<a href="https://mqt.readthedocs.io/projects/bench">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/mqt_light.png" width="60%">
   <img src="https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/mqt_dark.png" width="60%">
+</a>
 </picture>
 </p>
 
 # MQT Bench: Benchmarking Software and Design Automation Tools for Quantum Computing
 
 MQT Bench is a quantum circuit benchmark suite with cross-level support, i.e., providing the same benchmark algorithms for different abstraction levels throughout the quantum computing
 software stack.
+MQT Bench is part of the [_Munich Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io) developed by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/).
 
 <p align="center">
   <a href="https://mqt.readthedocs.io/projects/bench">
   <img width=30% src="https://img.shields.io/badge/documentation-blue?style=for-the-badge&logo=read%20the%20docs" alt="Documentation" />
   </a>
 </p>
 
@@ -47,22 +51,17 @@
 
 # draw the circuit
 print(qc_algorithmic_level.draw())
 ```
 
 **Detailed documentation and examples are available at [ReadTheDocs](https://mqt.readthedocs.io/projects/bench).**
 
-# Repository Structure
+## Availability as a PennyLane Dataset
 
-- src/mqt/: main source directory
-  - bench: Directory for the MQT Bench package
-  - bench/benchmarks: Directory for the benchmarks
-  - benchviewer: Directory for the webpage (which can be started locally and is also hosted at
-    [https://www.cda.cit.tum.de/mqtbench/](https://www.cda.cit.tum.de/mqtbench/))
-- tests: Directory for the tests for MQT Bench
+MQT Bench is also available as a [Pennylane dataset](https://pennylane.ai/datasets/other/mqt-bench).
 
 ## Acknowledgements
 
 The Munich Quantum Toolkit has been supported by the European
 Research Council (ERC) under the European Union's Horizon 2020 research and innovation program (grant agreement
 No. 101001318), the Bavarian State Ministry for Science and Arts through the Distinguished Professorship Program, as well as the
 Munich Quantum Valley, which is supported by the Bavarian state government with funds from the Hightech Agenda Bayern Plus.
```

#### html2text {}

```diff
@@ -1,27 +1,30 @@
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)]
-(https://pypi.org/project/mqt.bench/) [![License: MIT](https://img.shields.io/
-badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/
-MIT) [![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/
-MQTBench/coverage.yml?branch=main&style=flat-
-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/
-actions/workflows/coverage.yml) [![Bindings](https://img.shields.io/github/
-actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-
-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/
-workflows/deploy.yml) [![codecov](https://img.shields.io/codecov/c/github/cda-
-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/
-mqt-bench) [![Documentation](https://img.shields.io/readthedocs/mqt-
-bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/
-bench)
-    [https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/
-                                 mqt_dark.png]
+(https://pypi.org/project/mqt.bench/) ![OS](https://img.shields.io/badge/os-
+linux%20%7C%20macos%20%7C%20windows-blue?style=flat-square) [![License: MIT]
+(https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://
+opensource.org/licenses/MIT) [![CI](https://img.shields.io/github/actions/
+workflow/status/cda-tum/mqt-bench/ci.yml?branch=main&style=flat-
+square&logo=github&label=ci)](https://github.com/cda-tum/mqt-bench/actions/
+workflows/ci.yml) [![CD](https://img.shields.io/github/actions/workflow/status/
+cda-tum/mqt-bench/cd.yml?style=flat-square&logo=github&label=cd)](https://
+github.com/cda-tum/mqt-bench/actions/workflows/cd.yml) [![Documentation](https:
+//img.shields.io/readthedocs/bench?logo=readthedocs&style=flat-square)](https:/
+/mqt.readthedocs.io/projects/bench) [![codecov](https://img.shields.io/codecov/
+c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/
+gh/cda-tum/mqt-bench)
+    _[_h_t_t_p_s_:_/_/_r_a_w_._g_i_t_h_u_b_u_s_e_r_c_o_n_t_e_n_t_._c_o_m_/_c_d_a_-_t_u_m_/_m_q_t_b_e_n_c_h_/_m_a_i_n_/_d_o_c_s_/___s_t_a_t_i_c_/
+                                 _m_q_t___d_a_r_k_._p_n_g_]
 # MQT Bench: Benchmarking Software and Design Automation Tools for Quantum
 Computing MQT Bench is a quantum circuit benchmark suite with cross-level
 support, i.e., providing the same benchmark algorithms for different
-abstraction levels throughout the quantum computing software stack.
+abstraction levels throughout the quantum computing software stack. MQT Bench
+is part of the [_Munich Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io)
+developed by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at
+the [Technical University of Munich](https://www.tum.de/).
                                 _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
 If you have any questions, feel free to create a [discussion](https://
 github.com/cda-tum/mqt-bench/discussions) or an [issue](https://github.com/cda-
 tum/mqt-bench/issues) on [GitHub](https://github.com/cda-tum/mqt-bench). MQT
 Bench is part of the Munich Quantum Toolkit (MQT) developed by the [Chair for
 Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of
 Munich](https://www.tum.de/) and is hosted at [https://www.cda.cit.tum.de/
@@ -31,23 +34,20 @@
 available via [PyPI](https://pypi.org/project/mqt.bench/). ```console (venv) $
 pip install mqt.bench ``` The following code gives an example on the usage:
 ```python3 from mqt.bench import get_benchmark # get a benchmark circuit on
 algorithmic level representing the GHZ state with 5 qubits qc_algorithmic_level
 = get_benchmark(benchmark_name="dj", level="alg", circuit_size=5) # draw the
 circuit print(qc_algorithmic_level.draw()) ``` **Detailed documentation and
 examples are available at [ReadTheDocs](https://mqt.readthedocs.io/projects/
-bench).** # Repository Structure - src/mqt/: main source directory - bench:
-Directory for the MQT Bench package - bench/benchmarks: Directory for the
-benchmarks - benchviewer: Directory for the webpage (which can be started
-locally and is also hosted at [https://www.cda.cit.tum.de/mqtbench/](https://
-www.cda.cit.tum.de/mqtbench/)) - tests: Directory for the tests for MQT Bench
-## Acknowledgements The Munich Quantum Toolkit has been supported by the
-European Research Council (ERC) under the European Union's Horizon 2020
-research and innovation program (grant agreement No. 101001318), the Bavarian
-State Ministry for Science and Arts through the Distinguished Professorship
-Program, as well as the Munich Quantum Valley, which is supported by the
-Bavarian state government with funds from the Hightech Agenda Bayern Plus.
+bench).** ## Availability as a PennyLane Dataset MQT Bench is also available as
+a [Pennylane dataset](https://pennylane.ai/datasets/other/mqt-bench). ##
+Acknowledgements The Munich Quantum Toolkit has been supported by the European
+Research Council (ERC) under the European Union's Horizon 2020 research and
+innovation program (grant agreement No. 101001318), the Bavarian State Ministry
+for Science and Arts through the Distinguished Professorship Program, as well
+as the Munich Quantum Valley, which is supported by the Bavarian state
+government with funds from the Hightech Agenda Bayern Plus.
     [https://raw.githubusercontent.com/cda-tum/mqt-bench/main/docs/_static/
  tum_light.svg][https://raw.githubusercontent.com/cda-tum/mqt-bench/main/docs/
 _static/logo-bavaria.svg][https://raw.githubusercontent.com/cda-tum/mqt-bench/
 main/docs/_static/erc_light.svg][https://raw.githubusercontent.com/cda-tum/mqt-
                      bench/main/docs/_static/logo-mqv.svg]
```

### Comparing `mqt.bench-1.1.1/docs/Abstraction_levels.rst` & `mqt_bench-1.1.2/docs/Abstraction_levels.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/Benchmark_selection.rst` & `mqt_bench-1.1.2/docs/Benchmark_selection.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/DevelopmentGuide.rst` & `mqt_bench-1.1.2/docs/DevelopmentGuide.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/Parameter.rst` & `mqt_bench-1.1.2/docs/Parameter.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/Quickstart.ipynb` & `mqt_bench-1.1.2/docs/Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/Usage.rst` & `mqt_bench-1.1.2/docs/Usage.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/arch.png` & `mqt_bench-1.1.2/docs/_static/arch.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/erc_dark.svg` & `mqt_bench-1.1.2/docs/_static/erc_dark.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/erc_light.svg` & `mqt_bench-1.1.2/docs/_static/erc_light.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/level_1.png` & `mqt_bench-1.1.2/docs/_static/level_1.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/level_2.png` & `mqt_bench-1.1.2/docs/_static/level_2.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/level_3.png` & `mqt_bench-1.1.2/docs/_static/level_3.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/level_4.png` & `mqt_bench-1.1.2/docs/_static/level_4.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/logo-bavaria.svg` & `mqt_bench-1.1.2/docs/_static/logo-bavaria.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/logo-mqv.svg` & `mqt_bench-1.1.2/docs/_static/logo-mqv.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/mqt_dark.png` & `mqt_bench-1.1.2/docs/_static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/mqt_light.png` & `mqt_bench-1.1.2/docs/_static/mqt_light.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/mqtbench.png` & `mqt_bench-1.1.2/docs/_static/mqtbench.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/tum_dark.svg` & `mqt_bench-1.1.2/docs/_static/tum_dark.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_static/tum_light.svg` & `mqt_bench-1.1.2/docs/_static/tum_light.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/_templates/page.html` & `mqt_bench-1.1.2/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/conf.py` & `mqt_bench-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/docs/index.rst` & `mqt_bench-1.1.2/docs/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Welcome to MQT Bench's documentation!
 =====================================
 
 MQT Bench is a tool for benchmarking quantum software tools developed as part of the `Munich Quantum Toolkit <https://mqt.readthedocs.io>`_ (*MQT*) by the `Chair for Design Automation <https://www.cda.cit.tum.de/>`_ at the `Technical University of Munich <https://www.tum.de>`_.
 
 We recommend you to start with the :doc:`quickstart guide <Quickstart>`.
 If you are interested in the theory behind MQT Bench, have a look at the publication :cite:labelpar:`quetschlich2023mqtbench`.
+Furthermore, MQT Bench is also available as a `PennyLane dataset <https://pennylane.ai/datasets/other/mqt-bench>`_.
 
 We appreciate any feedback and contributions to the project. If you want to contribute, you can find more information in the :doc:`Contribution <Contributing>` guide. If you are having trouble with the installation or the usage of MQT Bench, please let us know at our :doc:`Support <Support>` page.
 
 ----
 
  .. toctree::
     :hidden:
```

### Comparing `mqt.bench-1.1.1/docs/refs.bib` & `mqt_bench-1.1.2/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/noxfile.py` & `mqt_bench-1.1.2/noxfile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """Nox sessions."""
 
 from __future__ import annotations
 
 import argparse
 import os
+from typing import TYPE_CHECKING
 
 import nox
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+
 nox.needs_version = ">=2024.3.2"
 nox.options.default_venv_backend = "uv|virtualenv"
 
+
 PYTHON_ALL_VERSIONS = ["3.10", "3.11", "3.12"]
 
 BUILD_REQUIREMENTS = [
-    "setuptools>=61",
+    "setuptools>=66.1",
     "setuptools_scm>=7",
+    "wheel>=0.40",
 ]
 
 if os.environ.get("CI", None):
     nox.options.error_on_missing_interpreters = True
 
 
 @nox.session(reuse_venv=True)
@@ -27,14 +34,52 @@
 
     Simply execute `nox -rs lint` to run all configured hooks.
     """
     session.install("pre-commit")
     session.run("pre-commit", "run", "--all-files", *session.posargs)
 
 
+def _run_tests(
+    session: nox.Session,
+    *,
+    install_args: Sequence[str] = (),
+    run_args: Sequence[str] = (),
+    extras: Sequence[str] = (),
+) -> None:
+    posargs = list(session.posargs)
+    env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
+
+    _extras = ["test", *extras]
+    if "--cov" in posargs:
+        _extras.append("coverage")
+        posargs.append("--cov-config=pyproject.toml")
+
+    session.install(*BUILD_REQUIREMENTS, *install_args, env=env)
+    install_arg = f"-ve.[{','.join(_extras)}]"
+    session.install("--no-build-isolation", install_arg, *install_args, env=env)
+    session.run("pytest", *run_args, *posargs, env=env)
+
+
+@nox.session(reuse_venv=True, python=PYTHON_ALL_VERSIONS)
+def tests(session: nox.Session) -> None:
+    """Run the test suite."""
+    _run_tests(session)
+
+
+@nox.session(reuse_venv=True, venv_backend="uv", python=PYTHON_ALL_VERSIONS)
+def minimums(session: nox.Session) -> None:
+    """Test the minimum versions of dependencies."""
+    _run_tests(
+        session,
+        install_args=["--resolution=lowest-direct"],
+        run_args=["-Wdefault"],
+    )
+    session.run("uv", "pip", "list")
+
+
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """Build the docs. Use "--non-interactive" to avoid serving. Pass "-b linkcheck" to check links."""
     parser = argparse.ArgumentParser()
     parser.add_argument("-b", dest="builder", default="html", help="Build target (default: html)")
     args, posargs = parser.parse_known_args(session.posargs)
 
@@ -54,10 +99,10 @@
         f"-b={args.builder}",
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
 
     if serve:
-        session.run("sphinx-autobuild", *shared_args)
+        session.run("sphinx-autobuild", "--ignore", "**jupyter**", *shared_args)
     else:
         session.run("sphinx-build", "--keep-going", *shared_args)
```

### Comparing `mqt.bench-1.1.1/pyproject.toml` & `mqt_bench-1.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools>=61",
+    "setuptools>=66.1",
     "setuptools_scm>=7",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mqt.bench"
 description = "MQT Bench - A MQT tool for Benchmarking Quantum Software Tools"
@@ -15,29 +15,27 @@
 ]
 keywords = ["MQT",  "quantum computing", "benchmarking", "performance", "testing"]
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 dynamic = ["version"]
 
 dependencies = [
-    "pytket-qiskit>=0.50.0,<0.53.0",  #  manages the dependencies for qiskit and tket in a combined fashion
-    "qiskit_optimization",
-    "qiskit_nature",
-    "qiskit_finance",
-    "pandas>=1.0.0",
-    "flask>=2.0.0",
-    "networkx>=2.0.0",
-    "pyscf>=2.3.0",
+    "pytket-qiskit>=0.53.0,<0.54.0",  #  manages the dependencies for qiskit and tket in a combined fashion
+    "qiskit_optimization>=0.6",
+    "qiskit_nature[pyscf]>=0.7",
+    "qiskit_finance>=0.4.1",
+    "pandas>=2.1.2",
+    "flask>=2.3.0",
+    "networkx>=2.8.8",
     "packaging>=21.0",
-    "tqdm>=4.0.0",
+    "tqdm>=4.29.0",
     "joblib>=1.3.0",
-    "importlib_metadata>=3.6; python_version < '3.10'",
-    "importlib_resources>=5.9; python_version < '3.10'",
 ]
 
+
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS",
     "Operating System :: POSIX :: Linux",
@@ -47,16 +45,16 @@
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Science/Research",
     "Natural Language :: English",
     "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
 ]
 
 [project.optional-dependencies]
-test = ["pytest>=7.2"]
-coverage = ["mqt.bench[test]", "pytest-cov[toml]"]
+test = ["pytest>=7.2", "pytest-console-scripts>=1.4"]
+coverage = ["mqt.bench[test]", "pytest-cov>=4"]
 docs = [
     "furo>=2023.08.17",
     "sphinx~=7.0",
     "setuptools-scm>=7",
     "sphinxcontrib-bibtex>=2.4.2",
     "sphinx-copybutton",
     "sphinx-hoverxref",
@@ -67,17 +65,18 @@
     "sphinxext-opengraph",
     "sphinx-autodoc-typehints",
     "qiskit[visualization]",
 ]
 dev = ["mqt.bench[coverage, docs]"]
 
 [project.scripts]
-"mqt.bench" = "mqt.benchviewer.main:start_server"
+"mqt.bench" = "mqt.bench.viewer.main:start_server"
 "create_mqt_bench_zip" = "mqt.bench.utils:create_zip_file"
 "generate_mqt_bench" = "mqt.bench.benchmark_generator:generate"
+"mqt.bench.cli" = "mqt.bench.cli:main"
 
 [project.urls]
 Homepage = "https://github.com/cda-tum/mqtbench"
 "Bug Tracker" = "https://github.com/cda-tum/mqtbench/issues"
 Discussions = "https://github.com/cda-tum/mqtbench/discussions"
 Research = "https://www.cda.cit.tum.de/research/quantum/"
 
@@ -91,45 +90,49 @@
 xfail_strict = true
 filterwarnings = [
     "error",
     "ignore:.*pkg_resources.*:DeprecationWarning:",
     "ignore:.*sre_.*:DeprecationWarning:",
     "ignore:.*Rigetti.*:UserWarning:",
     "ignore:.*Values in x.*:RuntimeWarning:",
+    "ignore:.*divide by zero encountered in det.*:RuntimeWarning:",
+    "ignore:.*invalid value encountered in det.*:RuntimeWarning:",
+    "ignore::DeprecationWarning:.*(docplex).*",
+    "ignore::SyntaxWarning:.*(docplex).*",
 ]
 
 [tool.coverage]
-run.source = ["mqt.bench", "mqt.benchviewer"]
+run.source = ["mqt.bench"]
 report.exclude_also = [
     '\.\.\.',
     'if TYPE_CHECKING:',
     'raise AssertionError',
     'raise NotImplementedError',
 ]
 
 show_missing = true
 skip_empty = true
 precision = 1
 
 [tool.mypy]
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
-files = ["src", "tests", "setup.py"]
+files = ["src", "tests"]
 python_version = "3.10"
 strict = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 explicit_package_bases = true
 pretty = true
 
 [[tool.mypy.overrides]]
 module = ["pytket.*", "qiskit_finance.*"]
 implicit_reexport = true
 
 [[tool.mypy.overrides]]
-module = ["qiskit.*", "qiskit_finance.*", "joblib.*", "networkx.*", "pandas.*", "qiskit_algorithms.*", "qiskit_ibm_runtime.*"]
+module = ["qiskit.*", "qiskit_finance.*", "joblib.*", "networkx.*", "pandas.*", "qiskit_algorithms.*", "qiskit_ibm_runtime.*", "pytest_console_scripts.*"]
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 120
 extend-include = ["*.ipynb"]
 src = ["src"]
 preview = true
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmark_generator.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmark_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         if cfg_path is None:
             cfg_path = utils.get_default_config_path()
         with Path(cfg_path).open() as jsonfile:
             self.cfg = json.load(jsonfile)
             print("Read config successful")
         self.timeout = self.cfg["timeout"]
         if qasm_output_path is None:
-            self.qasm_output_path = str(resources.files("mqt.benchviewer") / "static" / "files" / "qasm_output")
+            self.qasm_output_path = str(resources.files("mqt.bench") / "viewer" / "static" / "files" / "qasm_output")
         else:
             self.qasm_output_path = qasm_output_path
 
         Path(self.qasm_output_path).mkdir(exist_ok=True, parents=True)
 
     def create_benchmarks_from_config(self, num_jobs: int) -> bool:
         benchmarks = [Benchmark(benchmark) for benchmark in self.cfg["benchmarks"]]  # type: ignore[misc]
@@ -389,16 +389,14 @@
 
     if compiler_settings is None:
         compiler_settings = CompilerSettings(QiskitSettings(), TKETSettings())
     elif not isinstance(compiler_settings, CompilerSettings):
         msg = "compiler_settings must be of type CompilerSettings or None."  # type: ignore[unreachable]
         raise ValueError(msg)
 
-    assert (compiler_settings.tket is not None) or (compiler_settings.qiskit is not None)
-
     independent_level = 1
     if level in ("indep", independent_level):
         if compiler == "qiskit":
             return qiskit_helper.get_indep_level(qc, circuit_size, False, True)
         if compiler == "tket":
             return tket_helper.get_indep_level(qc, circuit_size, False, True)
 
@@ -461,14 +459,18 @@
 
 
 def timeout_watcher(
     func: Callable[..., bool | QuantumCircuit],
     timeout: int,
     args: list[Any] | int | tuple[int, str] | str,
 ) -> bool | QuantumCircuit | Circuit:
+    if sys.platform == "win32":
+        warn("Timeout is not supported on Windows.", category=RuntimeWarning, stacklevel=2)
+        return func(*args) if isinstance(args, tuple | list) else func(args)
+
     class TimeoutExceptionError(Exception):  # Custom exception class
         pass
 
     def timeout_handler(_signum: int, _frame: Any) -> None:  # noqa: ANN401
         raise TimeoutExceptionError
 
     # Change the behavior of SIGALRM
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/__init__.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/ae.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/ae.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/dj.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/dj.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/ghz.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/ghz.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/graphstate.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/graphstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/grover.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/grover.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qaoa.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qaoa.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qft.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qft.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qftentangled.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qftentangled.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
     # set number of assets (= number of qubits)
     num_assets = num_qubits
 
     # Generate expected return and covariance matrix from (random) time-series
-    stocks = [("TICKER%s" % i) for i in range(num_assets)]
+    stocks = [(f"TICKER{i}") for i in range(num_assets)]
     data = RandomDataProvider(
         tickers=stocks,
         start=datetime.datetime(2016, 1, 1),
         end=datetime.datetime(2016, 1, 30),
     )
     data.run()
     mu = data.get_period_return_mean_vector()
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
     # set number of assets (= number of qubits)
     num_assets = num_qubits
 
     # Generate expected return and covariance matrix from (random) time-series
-    stocks = [("TICKER%s" % i) for i in range(num_assets)]
+    stocks = [(f"TICKER{i}") for i in range(num_assets)]
     data = RandomDataProvider(
         tickers=stocks,
         start=datetime.datetime(2016, 1, 1),
         end=datetime.datetime(2016, 1, 30),
     )
     data.run()
     mu = data.get_period_return_mean_vector()
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from qiskit.circuit.library import TwoLocal
+from qiskit.exceptions import MissingOptionalLibraryError
 from qiskit.primitives import Estimator
 from qiskit_algorithms.minimum_eigensolvers import VQE
 from qiskit_algorithms.optimizers import COBYLA
 from qiskit_nature.second_q.drivers import PySCFDriver
 from qiskit_nature.second_q.mappers import JordanWignerMapper
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -18,18 +19,27 @@
 
 def create_circuit(choice: str) -> QuantumCircuit:
     """Returns a quantum circuit implementing Ground State Estimation.
 
     Keyword Arguments:
     molecule -- Molecule for which the ground state shall be estimated.
     """
+
     molecule = get_molecule(choice)
-    driver = PySCFDriver(atom=molecule)
-    es_problem = driver.run()
 
+    try:
+        driver = PySCFDriver(atom=molecule)
+    except MissingOptionalLibraryError:
+        msg = (
+            "PySCF is not installed (most likely because you are on a Windows system)."
+            "Please either download benchmark from https://www.cda.cit.tum.de/mqtbench/ or try to manually install PySCF."
+        )
+        raise ImportError(msg) from None
+
+    es_problem = driver.run()
     mapper = JordanWignerMapper()
     second_q_op = es_problem.second_q_ops()
     operator = mapper.map(second_q_op[0])
 
     tl_circuit = TwoLocal(
         rotation_blocks=["h", "rx"],
         entanglement_blocks="cz",
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeexact.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qpeexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeinexact.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qpeinexact.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qwalk.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/qwalk.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/random.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/realamprandom.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/realamprandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/shor.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/shor.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/su2random.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/su2random.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/twolocalrandom.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/twolocalrandom.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/vqe.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/vqe.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/benchmarks/wstate.py` & `mqt_bench-1.1.2/src/mqt/bench/benchmarks/wstate.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_montreal_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/ibm_montreal_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_washington_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/ibm_washington_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_aria1_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/ionq_aria1_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_harmony_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/ionq_harmony_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/oqc_lucy_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/oqc_lucy_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json` & `mqt_bench-1.1.2/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/config.json` & `mqt_bench-1.1.2/src/mqt/bench/config.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/__init__.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/calibration.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/calibration.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/device.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/device.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/ibm.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/ibm.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/ionq.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/ionq.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/oqc.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/oqc.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/provider.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         """Get a list of all available basis gates."""
         unique_basis_gates = {tuple(device.basis_gates) for device in cls.get_available_devices()}
         return [list(basis_gates) for basis_gates in unique_basis_gates]
 
     @classmethod
     def get_max_qubits(cls) -> int:
         """Get the maximum number of qubits offered by a device from the provider."""
-        return max([device.num_qubits for device in cls.get_available_devices()])
+        return max(device.num_qubits for device in cls.get_available_devices())
 
     @classmethod
     @abstractmethod
     def import_backend(cls, path: Path) -> Device:
         """Import a device from a file containing calibration data."""
 
     @classmethod
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/quantinuum.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/quantinuum.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/devices/rigetti.py` & `mqt_bench-1.1.2/src/mqt/bench/devices/rigetti.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation.py` & `mqt_bench-1.1.2/src/mqt/bench/evaluation/evaluation.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,12 +54,12 @@
         num_gates=sum(qc.count_ops().values()),
         num_multiple_qubit_gates=qc.num_nonlocal_gates(),
         supermarq_features=utils.calc_supermarq_features(qc),
     )
 
 
 def count_occurrences(filenames: list[str], search_str: str) -> int:
-    return sum([search_str in filename for filename in filenames])
+    return sum(search_str in filename for filename in filenames)
 
 
 def count_qubit_numbers_per_compiler(filenames: list[str], compiler: str) -> list[int]:
     return [int(str(filename).split("_")[-1].split(".")[0]) for filename in filenames if compiler in filename]
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_data.pkl` & `mqt_bench-1.1.2/src/mqt/bench/evaluation/evaluation_data.pkl`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_visualization.ipynb` & `mqt_bench-1.1.2/src/mqt/bench/evaluation/evaluation_visualization.ipynb`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/evaluation/results/pie.pdf` & `mqt_bench-1.1.2/src/mqt/bench/evaluation/results/pie.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/evaluation/results/qubit_dist.pdf` & `mqt_bench-1.1.2/src/mqt/bench/evaluation/results/qubit_dist.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/evaluation/results/violins.pdf` & `mqt_bench-1.1.2/src/mqt/bench/evaluation/results/violins.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/bench/qiskit_helper.py` & `mqt_bench-1.1.2/src/mqt/bench/qiskit_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-    filename_indep = target_filename if target_filename else qc.name + "_indep_qiskit_" + str(num_qubits)
+    filename_indep = target_filename or qc.name + "_indep_qiskit_" + str(num_qubits)
 
     path = Path(target_directory, filename_indep + ".qasm")
     if file_precheck and path.is_file():
         return True
     openqasm_gates = utils.get_openqasm_gates()
     target_independent = transpile(qc, basis_gates=openqasm_gates, optimization_level=1, seed_transpiler=10)
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/tket_helper.py` & `mqt_bench-1.1.2/src/mqt/bench/tket_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-    filename_indep = target_filename if target_filename else qc.name + "_indep_tket_" + str(num_qubits)
+    filename_indep = target_filename or qc.name + "_indep_tket_" + str(num_qubits)
 
     path = Path(target_directory, filename_indep + ".qasm")
     if file_precheck and path.is_file():
         return True
     try:
         gates = list(set(utils.get_openqasm_gates()) - {"rccx"})
         qc = transpile(
```

### Comparing `mqt.bench-1.1.1/src/mqt/bench/utils.py` & `mqt_bench-1.1.2/src/mqt/bench/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import subprocess
 import sys
 from datetime import date
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:  # pragma: no cover
     from types import ModuleType
@@ -15,16 +14,14 @@
 import numpy as np
 from pytket import __version__ as __tket_version__
 from qiskit import QuantumCircuit
 from qiskit import __version__ as __qiskit_version__
 from qiskit.converters import circuit_to_dag
 from qiskit_optimization.applications import Maxcut
 
-from mqt.bench.devices import OQCProvider
-
 if TYPE_CHECKING or sys.version_info >= (3, 10, 0):  # pragma: no cover
     from importlib import metadata, resources
 else:
     import importlib_metadata as metadata
     import importlib_resources as resources
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -38,17 +35,14 @@
     program_communication: float
     critical_depth: float
     entanglement_ratio: float
     parallelism: float
     liveness: float
 
 
-qasm_path = str(resources.files("mqt.benchviewer") / "static/files/qasm_output/")
-
-
 def get_supported_benchmarks() -> list[str]:
     return [
         "ae",
         "dj",
         "grover-noancilla",
         "grover-v-chain",
         "ghz",
@@ -88,25 +82,25 @@
 
 def get_default_config_path() -> str:
     return str(resources.files("mqt.bench") / "config.json")
 
 
 def get_default_qasm_output_path() -> str:
     """Returns the path where all .qasm files are stored."""
-    return str(resources.files("mqt.benchviewer") / "static" / "files" / "qasm_output")
+    return str(resources.files("mqt.bench") / "viewer" / "static" / "files" / "qasm_output")
 
 
 def get_default_evaluation_output_path() -> str:
     """Returns the path where all .qasm files are stored."""
     return str(resources.files("mqt.bench") / "evaluation")
 
 
-def get_zip_file_path() -> str:
+def get_zip_folder_path() -> str:
     """Returns the path where the zip file is stored."""
-    return str(resources.files("mqt.benchviewer") / "static/files/MQTBench_all.zip")
+    return str(resources.files("mqt.bench") / "viewer" / "static" / "files")
 
 
 def get_examplary_max_cut_qp(n_nodes: int, degree: int = 2) -> QuadraticProgram:
     """Returns a quadratic problem formulation of a max cut problem of a random graph.
 
     Keyword Arguments:
     n_nodes -- number of graph nodes (and also number of qubits)
@@ -206,52 +200,31 @@
             f.write("// Used Gate Set: " + str(gate_set) + "\n")
         if mapped:
             f.write("// Coupling List: " + str(c_map) + "\n")
         f.write("\n")
         f.write(qc_str)
     f.close()
 
-    if gate_set == OQCProvider.get_native_gates():
-        postprocess_single_oqc_file(str(file))
     return True
 
 
-def postprocess_single_oqc_file(filename: str) -> None:
-    with Path(filename).open() as f:
-        lines = f.readlines()
-    with Path(filename).open("w") as f:
-        for line in lines:
-            if not ("gate rzx" in line.strip("\n") or "gate ecr" in line.strip("\n")):
-                f.write(line)
-            if 'include "qelib1.inc"' in line.strip("\n"):
-                f.write("opaque ecr q0,q1;\n")
-
-
-def create_zip_file(zip_path: str | None = None, qasm_path: str | None = None) -> int:
-    if zip_path is None:
-        zip_path = get_zip_file_path()
-    if qasm_path is None:
-        qasm_path = get_default_qasm_output_path()
-    return subprocess.call(f"zip -rj {zip_path} {qasm_path}", shell=True)
-
-
 def calc_supermarq_features(
     qc: QuantumCircuit,
 ) -> SupermarqFeatures:
     """Calculates the Supermarq features for a given quantum circuit. Code adapted from https://github.com/Infleqtion/client-superstaq/blob/91d947f8cc1d99f90dca58df5248d9016e4a5345/supermarq-benchmarks/supermarq/converters.py."""
     num_qubits = qc.num_qubits
     dag = circuit_to_dag(qc)
     dag.remove_all_ops_named("barrier")
 
     # Program communication = circuit's average qubit degree / degree of a complete graph.
     graph = nx.Graph()
     for op in dag.two_qubit_ops():
         q1, q2 = op.qargs
         graph.add_edge(qc.find_bit(q1).index, qc.find_bit(q2).index)
-    degree_sum = sum([graph.degree(n) for n in graph.nodes])
+    degree_sum = sum(graph.degree(n) for n in graph.nodes)
     program_communication = degree_sum / (num_qubits * (num_qubits - 1)) if num_qubits > 1 else 0
 
     # Liveness feature = sum of all entries in the liveness matrix / (num_qubits * depth).
     activity_matrix = np.zeros((num_qubits, dag.depth()))
     for i, layer in enumerate(dag.layers()):
         for op in layer["partition"]:
             for qubit in op:
@@ -266,15 +239,15 @@
     )
 
     # Entanglement-ratio = ratio between # of 2-qubit gates and total number of gates in the circuit.
     entanglement_ratio = len(dag.two_qubit_ops()) / len(dag.gate_nodes()) if len(dag.gate_nodes()) > 0 else 0
 
     # Critical depth = # of 2-qubit gates along the critical path / total # of 2-qubit gates.
     longest_paths = dag.count_ops_longest_path()
-    n_ed = sum([longest_paths[name] for name in {op.name for op in dag.two_qubit_ops()} if name in longest_paths])
+    n_ed = sum(longest_paths[name] for name in {op.name for op in dag.two_qubit_ops()} if name in longest_paths)
     n_e = len(dag.two_qubit_ops())
     critical_depth = n_ed / n_e if n_e != 0 else 0
 
     assert 0 <= program_communication <= 1
     assert 0 <= critical_depth <= 1
     assert 0 <= entanglement_ratio <= 1
     assert 0 <= parallelism <= 1
```

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/backend.py` & `mqt_bench-1.1.2/src/mqt/bench/viewer/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,14 @@
         with (
             Path(fname).open("wb") as f,
             tqdm(
                 desc=fname,
                 total=total_length,
                 unit="iB",
                 unit_scale=True,
-                unit_divisor=1024,
             ) as bar,
         ):
             for data in r.iter_content(chunk_size=1024):
                 size = f.write(data)
                 bar.update(size)
         print(f"Download completed to {fname}. Server is starting now.")
 
@@ -651,15 +650,14 @@
     with (
         Path(fname).open("wb") as f,
         tqdm(
             desc=fname,
             total=total_length,
             unit="iB",
             unit_scale=True,
-            unit_divisor=1024,
         ) as bar,
     ):
         for data in r.iter_content(chunk_size=1024):
             size = f.write(data)
             bar.update(size)
     print(f"Download completed to {fname}. Server is starting now.")
```

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/main.py` & `mqt_bench-1.1.2/src/mqt/bench/viewer/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from __future__ import annotations
 
 import logging
 import os
-import sys
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 from flask import Flask, cli, jsonify, render_template, request, send_from_directory
 
-from mqt.benchviewer.backend import Backend
-
-if TYPE_CHECKING or sys.version_info < (3, 10, 0):  # pragma: no cover
-    import importlib_resources as resources
-else:
-    from importlib import resources
+from mqt.bench import utils
+from mqt.bench.viewer.backend import Backend
 
 if TYPE_CHECKING:  # pragma: no cover
     from flask import Response
 
 
 class Server:
     def __init__(
@@ -156,15 +151,15 @@
 def start_server(
     skip_question: bool = False,
     activate_logging: bool = False,
     target_location: str | None = None,
     debug_flag: bool = False,
 ) -> None:
     if not target_location:
-        target_location = str(resources.files("mqt.benchviewer") / "static" / "files")
+        target_location = utils.get_zip_folder_path()
 
     Server(
         target_location=target_location,
         skip_question=skip_question,
         activate_logging=activate_logging,
     )
     print(
```

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/static/favicon.ico` & `mqt_bench-1.1.2/src/mqt/bench/viewer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/static/mqt_dark.png` & `mqt_bench-1.1.2/src/mqt/bench/viewer/static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/static/tum_logo.svg` & `mqt_bench-1.1.2/src/mqt/bench/viewer/static/tum_logo.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/templates/benchmark_description.html` & `mqt_bench-1.1.2/src/mqt/bench/viewer/templates/benchmark_description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/templates/description.html` & `mqt_bench-1.1.2/src/mqt/bench/viewer/templates/description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/templates/index.html` & `mqt_bench-1.1.2/src/mqt/bench/viewer/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,18 @@
         algorithms on different levels of abstractions. At the moment, MQT Bench
         comprises around 70,000 benchmark circuits ranging from 2 up to 130
         qubits on four abstraction levels.
       </p>
 
       <p>
         In order to create a benchmark set according to your needs, simply fill
-        out the form below.
+        out the form below. Furthermore, MQT Bench is also available as a
+        <a href="https://pennylane.ai/datasets/other/mqt-bench" target="_blank"
+          >PennyLane dataset</a
+        >.
       </p>
     </div>
     <form
       method="POST"
       class="form-inline"
       role="form"
       action="download"
@@ -623,14 +626,24 @@
             class="btn btn-primary btn-lg mx-auto text-center"
             id="downloadButton"
             disabled
             value="submit"
           >
             Download selected Benchmarks
           </button>
+          <div class="d-flex">
+            <p>
+              MQT Bench is also available as a
+              <a
+                href="https://pennylane.ai/datasets/other/mqt-bench"
+                target="_blank"
+                >PennyLane dataset</a
+              >.
+            </p>
+          </div>
         </div>
       </div>
     </form>
 
     <div class="col-md-12" style="height: 20px"></div>
 
     <div class="container">
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 operate on and across different levels of abstraction, it is beneficial having
 benchmarks consistently available across those levels. The MQT Benchmark
 Library (MQT Bench) provides a single benchmark suite which offers the same
 benchmark algorithms on different levels of abstractions. At the moment, MQT
 Bench comprises around 70,000 benchmark circuits ranging from 2 up to 130
 qubits on four abstraction levels.
 In order to create a benchmark set according to your needs, simply fill out the
-form below.
+form below. Furthermore, MQT Bench is also available as a _P_e_n_n_y_L_a_n_e_ _d_a_t_a_s_e_t.
 ****** BBeenncchhmmaarrkk SSeelleeccttiioonn ******
 Please select the desired benchmarks from the set of all available ones or
 select all (??). For details, see the _b_e_n_c_h_m_a_r_k_ _d_e_s_c_r_i_p_t_i_o_n_.
 ** SSccaallaabbllee BBeenncchhmmaarrkkss:: **
 TThhee nnuummbbeerr ooff qquubbiittss ffoorr tthhee ffoolllloowwiinngg bbeenncchhmmaarrkkss iiss aaddjjuussttaabbllee..
 {% for benchmark in benchmarks %}
 ??{{ benchmark.name }}
@@ -76,14 +76,15 @@
 ****** DDoowwnnllooaadd ******
 Number of selected benchmarks:  
 0
 After the download button is clicked, all benchmarks provided as ..qqaassmm files
 are downloaded as a ..zziipp archive. Details of the _f_i_l_e_ _f_o_r_m_a_t are provided.
 Alternatively, a pre-generated archive with aallll benchmarks can be _d_o_w_n_l_o_a_d_e_d.
 Download selected Benchmarks
+MQT Bench is also available as a _P_e_n_n_y_L_a_n_e_ _d_a_t_a_s_e_t.
 ****** RReeffeerreennccee ******
 For a more detailed description of MQT Bench, we are referring to the
 corresponding paper _"_M_Q_T_ _B_e_n_c_h_:_ _B_e_n_c_h_m_a_r_k_i_n_g_ _S_o_f_t_w_a_r_e_ _a_n_d_ _D_e_s_i_g_n_ _A_u_t_o_m_a_t_i_o_n
 _T_o_o_l_s_ _f_o_r_ _Q_u_a_n_t_u_m_ _C_o_m_p_u_t_i_n_g_". Our implementation is available on _G_i_t_H_u_b. IInn
 ccaassee yyoouu aarree uussiinngg MMQQTT BBeenncchh iinn yyoouurr wwoorrkk,, wwee wwoouulldd bbee tthhaannkkffuull iiff yyoouu rreeffeerrrreedd
 ttoo iitt bbyy cciittiinngg tthhee ffoolllloowwiinngg ppuubblliiccaattiioonn::
 @article{quetschlich2023mqtbench,
```

### Comparing `mqt.bench-1.1.1/src/mqt/benchviewer/templates/legal.html` & `mqt_bench-1.1.2/src/mqt/bench/viewer/templates/legal.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/src/mqt.bench.egg-info/PKG-INFO` & `mqt_bench-1.1.2/src/mqt.bench.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.1.1
+Version: 1.1.2
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@tum.de>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,32 +42,30 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket-qiskit<0.53.0,>=0.50.0
-Requires-Dist: qiskit_optimization
-Requires-Dist: qiskit_nature
-Requires-Dist: qiskit_finance
-Requires-Dist: pandas>=1.0.0
-Requires-Dist: flask>=2.0.0
-Requires-Dist: networkx>=2.0.0
-Requires-Dist: pyscf>=2.3.0
+Requires-Dist: pytket-qiskit<0.54.0,>=0.53.0
+Requires-Dist: qiskit_optimization>=0.6
+Requires-Dist: qiskit_nature[pyscf]>=0.7
+Requires-Dist: qiskit_finance>=0.4.1
+Requires-Dist: pandas>=2.1.2
+Requires-Dist: flask>=2.3.0
+Requires-Dist: networkx>=2.8.8
 Requires-Dist: packaging>=21.0
-Requires-Dist: tqdm>=4.0.0
+Requires-Dist: tqdm>=4.29.0
 Requires-Dist: joblib>=1.3.0
-Requires-Dist: importlib_metadata>=3.6; python_version < "3.10"
-Requires-Dist: importlib_resources>=5.9; python_version < "3.10"
 Provides-Extra: test
 Requires-Dist: pytest>=7.2; extra == "test"
+Requires-Dist: pytest-console-scripts>=1.4; extra == "test"
 Provides-Extra: coverage
 Requires-Dist: mqt.bench[test]; extra == "coverage"
-Requires-Dist: pytest-cov[toml]; extra == "coverage"
+Requires-Dist: pytest-cov>=4; extra == "coverage"
 Provides-Extra: docs
 Requires-Dist: furo>=2023.08.17; extra == "docs"
 Requires-Dist: sphinx~=7.0; extra == "docs"
 Requires-Dist: setuptools-scm>=7; extra == "docs"
 Requires-Dist: sphinxcontrib-bibtex>=2.4.2; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: sphinx-hoverxref; extra == "docs"
@@ -78,31 +76,35 @@
 Requires-Dist: sphinxext-opengraph; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: qiskit[visualization]; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: mqt.bench[coverage,docs]; extra == "dev"
 
 [![PyPI](https://img.shields.io/pypi/v/mqt.bench?logo=pypi&style=flat-square)](https://pypi.org/project/mqt.bench/)
+![OS](https://img.shields.io/badge/os-linux%20%7C%20macos%20%7C%20windows-blue?style=flat-square)
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://opensource.org/licenses/MIT)
-[![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/coverage.yml?branch=main&style=flat-square&logo=github&label=coverage)](https://github.com/cda-tum/MQTBench/actions/workflows/coverage.yml)
-[![Bindings](https://img.shields.io/github/actions/workflow/status/cda-tum/MQTBench/deploy.yml?branch=main&style=flat-square&logo=github&label=python)](https://github.com/cda-tum/MQTBench/actions/workflows/deploy.yml)
+[![CI](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-bench/ci.yml?branch=main&style=flat-square&logo=github&label=ci)](https://github.com/cda-tum/mqt-bench/actions/workflows/ci.yml)
+[![CD](https://img.shields.io/github/actions/workflow/status/cda-tum/mqt-bench/cd.yml?style=flat-square&logo=github&label=cd)](https://github.com/cda-tum/mqt-bench/actions/workflows/cd.yml)
+[![Documentation](https://img.shields.io/readthedocs/bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/bench)
 [![codecov](https://img.shields.io/codecov/c/github/cda-tum/mqt-bench?style=flat-square&logo=codecov)](https://codecov.io/gh/cda-tum/mqt-bench)
-[![Documentation](https://img.shields.io/readthedocs/mqt-bench?logo=readthedocs&style=flat-square)](https://mqt.readthedocs.io/projects/bench)
 
 <p align="center">
 <picture>
+<a href="https://mqt.readthedocs.io/projects/bench">
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/mqt_light.png" width="60%">
   <img src="https://raw.githubusercontent.com/cda-tum/mqtbench/main/docs/_static/mqt_dark.png" width="60%">
+</a>
 </picture>
 </p>
 
 # MQT Bench: Benchmarking Software and Design Automation Tools for Quantum Computing
 
 MQT Bench is a quantum circuit benchmark suite with cross-level support, i.e., providing the same benchmark algorithms for different abstraction levels throughout the quantum computing
 software stack.
+MQT Bench is part of the [_Munich Quantum Toolkit_ (_MQT_)](https://mqt.readthedocs.io) developed by the [Chair for Design Automation](https://www.cda.cit.tum.de/) at the [Technical University of Munich](https://www.tum.de/).
 
 <p align="center">
   <a href="https://mqt.readthedocs.io/projects/bench">
   <img width=30% src="https://img.shields.io/badge/documentation-blue?style=for-the-badge&logo=read%20the%20docs" alt="Documentation" />
   </a>
 </p>
 
@@ -130,22 +132,17 @@
 
 # draw the circuit
 print(qc_algorithmic_level.draw())
 ```
 
 **Detailed documentation and examples are available at [ReadTheDocs](https://mqt.readthedocs.io/projects/bench).**
 
-# Repository Structure
+## Availability as a PennyLane Dataset
 
-- src/mqt/: main source directory
-  - bench: Directory for the MQT Bench package
-  - bench/benchmarks: Directory for the benchmarks
-  - benchviewer: Directory for the webpage (which can be started locally and is also hosted at
-    [https://www.cda.cit.tum.de/mqtbench/](https://www.cda.cit.tum.de/mqtbench/))
-- tests: Directory for the tests for MQT Bench
+MQT Bench is also available as a [Pennylane dataset](https://pennylane.ai/datasets/other/mqt-bench).
 
 ## Acknowledgements
 
 The Munich Quantum Toolkit has been supported by the European
 Research Council (ERC) under the European Union's Horizon 2020 research and innovation program (grant agreement
 No. 101001318), the Bavarian State Ministry for Science and Arts through the Distinguished Professorship Program, as well as the
 Munich Quantum Valley, which is supported by the Bavarian state government with funds from the Hightech Agenda Bayern Plus.
```

### Comparing `mqt.bench-1.1.1/src/mqt.bench.egg-info/SOURCES.txt` & `mqt_bench-1.1.2/src/mqt.bench.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -12,20 +12,17 @@
 .github/codecov.yml
 .github/contributing.rst
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/support.rst
 .github/ISSUE_TEMPLATE/bug-report.yml
 .github/ISSUE_TEMPLATE/feature-request.yml
-.github/workflows/codeql.yml
-.github/workflows/coverage.yml
-.github/workflows/deploy.yml
-.github/workflows/mypy.yml
+.github/workflows/cd.yml
+.github/workflows/ci.yml
 .github/workflows/release-drafter.yml
-.github/workflows/test_pregenerated_zip.yml
 docs/Abstraction_levels.rst
 docs/Benchmark_selection.rst
 docs/Contributing.rst
 docs/DevelopmentGuide.rst
 docs/Parameter.rst
 docs/Quickstart.ipynb
 docs/References.rst
@@ -54,14 +51,15 @@
 src/mqt.bench.egg-info/SOURCES.txt
 src/mqt.bench.egg-info/dependency_links.txt
 src/mqt.bench.egg-info/entry_points.txt
 src/mqt.bench.egg-info/requires.txt
 src/mqt.bench.egg-info/top_level.txt
 src/mqt/bench/__init__.py
 src/mqt/bench/benchmark_generator.py
+src/mqt/bench/cli.py
 src/mqt/bench/config.json
 src/mqt/bench/py.typed
 src/mqt/bench/qiskit_helper.py
 src/mqt/bench/tket_helper.py
 src/mqt/bench/utils.py
 src/mqt/bench/benchmarks/__init__.py
 src/mqt/bench/benchmarks/ae.py
@@ -109,29 +107,29 @@
 src/mqt/bench/evaluation/__init__.py
 src/mqt/bench/evaluation/evaluation.py
 src/mqt/bench/evaluation/evaluation_data.pkl
 src/mqt/bench/evaluation/evaluation_visualization.ipynb
 src/mqt/bench/evaluation/results/pie.pdf
 src/mqt/bench/evaluation/results/qubit_dist.pdf
 src/mqt/bench/evaluation/results/violins.pdf
-src/mqt/benchviewer/__init__.py
-src/mqt/benchviewer/backend.py
-src/mqt/benchviewer/main.py
-src/mqt/benchviewer/py.typed
-src/mqt/benchviewer/static/favicon.ico
-src/mqt/benchviewer/static/mqt_dark.png
-src/mqt/benchviewer/static/tum_logo.svg
-src/mqt/benchviewer/static/files/MQTBench_all.zip
-src/mqt/benchviewer/static/files/qasm_output/.gitignore
-src/mqt/benchviewer/templates/benchmark_description.html
-src/mqt/benchviewer/templates/description.html
-src/mqt/benchviewer/templates/index.html
-src/mqt/benchviewer/templates/legal.html
+src/mqt/bench/viewer/__init__.py
+src/mqt/bench/viewer/backend.py
+src/mqt/bench/viewer/main.py
+src/mqt/bench/viewer/static/favicon.ico
+src/mqt/bench/viewer/static/mqt_dark.png
+src/mqt/bench/viewer/static/tum_logo.svg
+src/mqt/bench/viewer/static/files/MQTBench_all.zip
+src/mqt/bench/viewer/static/files/qasm_output/.gitignore
+src/mqt/bench/viewer/templates/benchmark_description.html
+src/mqt/bench/viewer/templates/description.html
+src/mqt/bench/viewer/templates/index.html
+src/mqt/bench/viewer/templates/legal.html
 tests/test_bench.py
 tests/test_benchviewer.py
+tests/test_cli.py
 tests/test_pregenerated_zip.py
 tests/devices/test_devices.py
 tests/devices/test_ibm_device_support.py
 tests/devices/test_ionq_device_support.py
 tests/devices/test_oqc_device_support.py
 tests/devices/test_quantinuum_device_support.py
 tests/devices/test_rigetti_device_support.py
```

### Comparing `mqt.bench-1.1.1/tests/devices/test_devices.py` & `mqt_bench-1.1.2/tests/devices/test_devices.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/tests/devices/test_ibm_device_support.py` & `mqt_bench-1.1.2/tests/devices/test_ibm_device_support.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/tests/devices/test_ionq_device_support.py` & `mqt_bench-1.1.2/tests/devices/test_ionq_device_support.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/tests/devices/test_oqc_device_support.py` & `mqt_bench-1.1.2/tests/devices/test_oqc_device_support.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/tests/devices/test_quantinuum_device_support.py` & `mqt_bench-1.1.2/tests/devices/test_quantinuum_device_support.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/tests/devices/test_rigetti_device_support.py` & `mqt_bench-1.1.2/tests/devices/test_rigetti_device_support.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.1/tests/test_bench.py` & `mqt_bench-1.1.2/tests/test_bench.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import json
 import pickle
+import sys
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytket
 from qiskit.qasm2 import dump
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -82,38 +83,38 @@
         "dj_mapped_quantinuum_h2_qiskit_opt3_23.qasm",
     ]
 
 
 @pytest.mark.parametrize(
     ("benchmark", "input_value", "scalable"),
     [
-        (ae, 8, True),
-        (ghz, 5, True),
+        (ae, 3, True),
+        (ghz, 2, True),  # the generated GHZ benchmarks are later used in test_benchviewer.py::test_streaming_zip
         (dj, 3, True),
-        (graphstate, 8, True),
-        (grover, 5, False),
-        (qaoa, 5, True),
-        (qft, 8, True),
-        (qftentangled, 8, True),
-        (qnn, 8, True),
-        (qpeexact, 8, True),
-        (qpeinexact, 8, True),
+        (graphstate, 3, True),
+        (grover, 3, False),
+        (qaoa, 3, True),
+        (qft, 3, True),
+        (qftentangled, 3, True),
+        (qnn, 3, True),
+        (qpeexact, 3, True),
+        (qpeinexact, 3, True),
         (tsp, 3, False),
-        (qwalk, 5, False),
-        (vqe, 5, True),
-        (random, 9, True),
-        (realamprandom, 9, True),
-        (su2random, 7, True),
-        (twolocalrandom, 8, True),
-        (wstate, 8, True),
-        (portfolioqaoa, 5, True),
-        (shor, 9, False),
-        (portfoliovqe, 5, True),
-        (pricingcall, 5, False),
-        (pricingput, 5, False),
+        (qwalk, 3, False),
+        (vqe, 3, True),
+        (random, 3, True),
+        (realamprandom, 3, True),
+        (su2random, 3, True),
+        (twolocalrandom, 3, True),
+        (wstate, 3, True),
+        (portfolioqaoa, 3, True),
+        (shor, 3, False),
+        (portfoliovqe, 3, True),
+        (pricingcall, 3, False),
+        (pricingput, 3, False),
     ],
 )
 def test_quantumcircuit_indep_level(
     benchmark: types.ModuleType, input_value: int, scalable: bool, output_path: str
 ) -> None:
     if benchmark in (grover, qwalk):
         qc = benchmark.create_circuit(input_value, ancillary_mode="noancilla")
@@ -157,37 +158,37 @@
     )
     assert res
 
 
 @pytest.mark.parametrize(
     ("benchmark", "input_value", "scalable"),
     [
-        (ae, 8, True),
-        (ghz, 5, True),
+        (ae, 3, True),
+        (ghz, 3, True),
         (dj, 3, True),
-        (graphstate, 8, True),
-        (grover, 5, False),
-        (qaoa, 5, True),
-        (qft, 8, True),
-        (qftentangled, 8, True),
-        (qnn, 5, True),
-        (qpeexact, 8, True),
-        (qpeinexact, 8, True),
+        (graphstate, 3, True),
+        (grover, 3, False),
+        (qaoa, 3, True),
+        (qft, 3, True),
+        (qftentangled, 3, True),
+        (qnn, 3, True),
+        (qpeexact, 3, True),
+        (qpeinexact, 3, True),
         (tsp, 3, False),
-        (qwalk, 5, False),
-        (vqe, 5, True),
-        (random, 9, True),
+        (qwalk, 3, False),
+        (vqe, 3, True),
+        (random, 3, True),
         (realamprandom, 3, True),
-        (su2random, 7, True),
-        (twolocalrandom, 5, True),
-        (wstate, 8, True),
-        (portfolioqaoa, 5, True),
-        (portfoliovqe, 5, True),
-        (pricingcall, 5, False),
-        (pricingput, 5, False),
+        (su2random, 3, True),
+        (twolocalrandom, 3, True),
+        (wstate, 3, True),
+        (portfolioqaoa, 3, True),
+        (portfoliovqe, 3, True),
+        (pricingcall, 3, False),
+        (pricingput, 3, False),
     ],
 )
 def test_quantumcircuit_native_and_mapped_levels(
     benchmark: types.ModuleType, input_value: int, scalable: bool, output_path: str
 ) -> None:
     if benchmark in (grover, qwalk):
         qc = benchmark.create_circuit(input_value, ancillary_mode="noancilla")
@@ -304,19 +305,14 @@
 
 
 def test_dj_constant_oracle() -> None:
     qc = dj.create_circuit(5, False)
     assert qc.depth() > 0
 
 
-def test_groundstate() -> None:
-    qc = groundstate.create_circuit("small")
-    assert qc.depth() > 0
-
-
 def test_routing() -> None:
     qc = routing.create_circuit(4, 2)
     assert qc.depth() > 0
 
 
 def test_get_benchmark_deprecation_warning() -> None:
     with pytest.warns(
@@ -406,15 +402,14 @@
             4,
             None,
             "tket",
             None,
             "",
             "",
         ),
-        ("groundstate", 1, 4, "small", "qiskit", None, "", ""),
         (
             "dj",
             "nativegates",
             5,
             None,
             "qiskit",
             CompilerSettings(qiskit=QiskitSettings(optimization_level=2)),
@@ -823,44 +818,33 @@
             "qiskit",
             CompilerSettings(qiskit=QiskitSettings(optimization_level=1)),
             "rigetti",
             "wrong_device",
         )
 
 
-def test_create_benchmarks_from_config(output_path: str) -> None:
+def test_create_benchmarks_from_config_and_evaluation(output_path: str) -> None:
     config = {
         "timeout": 1,
         "benchmarks": [
             {
                 "name": "ghz",
                 "include": True,
-                "min_qubits": 2,
-                "max_qubits": 3,
+                "min_qubits": 20,
+                "max_qubits": 21,
                 "stepsize": 1,
                 "precheck_possible": True,
             },
             {
-                "name": "grover",
+                "name": "graphstate",
                 "include": True,
-                "min_qubits": 2,
-                "max_qubits": 3,
+                "min_qubits": 20,
+                "max_qubits": 21,
                 "stepsize": 1,
-                "ancillary_mode": ["noancilla"],
-                "precheck_possible": False,
-            },
-            {"name": "shor", "include": True, "instances": ["small"], "precheck_possible": False},
-            {"name": "routing", "include": True, "min_nodes": 2, "max_nodes": 3, "precheck_possible": False},
-            {"name": "groundstate", "include": True, "instances": ["small"], "precheck_possible": False},
-            {
-                "name": "pricingput",
-                "include": True,
-                "min_uncertainty": 2,
-                "max_uncertainty": 3,
-                "precheck_possible": False,
+                "precheck_possible": True,
             },
         ],
     }
     file = Path("test_config.json")
     with file.open("w") as f:
         json.dump(config, f)
 
@@ -871,25 +855,14 @@
     evaluation.create_statistics(source_directory=Path(output_path), target_directory=Path(output_path))
 
     with (Path(output_path) / "evaluation_data.pkl").open("rb") as f:
         res_dicts = pickle.load(f)
     assert len(res_dicts) > 0
 
 
-def test_zip_creation() -> None:
-    """Test the creation of the overall zip file."""
-    zip_path = str(Path("./tests/MQTBench_all.zip").resolve())
-    qasm_path = str(Path("./tests/test_output/").resolve())
-    retcode = utils.create_zip_file(zip_path, qasm_path)
-    assert retcode == 0
-
-    zip_file = Path(utils.get_zip_file_path())
-    assert zip_file.is_file()
-
-
 def test_configure_end(output_path: str) -> None:
     # delete all files in the test directory and the directory itself
     for f in Path(output_path).iterdir():
         f.unlink()
     Path(output_path).rmdir()
 
 
@@ -938,15 +911,15 @@
     )
     assert res
     path = Path(directory) / Path(filename).with_suffix(".qasm")
     assert path.is_file()
     path.unlink()
 
 
-def test_oqc_postprocessing() -> None:
+def test_oqc_benchmarks() -> None:
     qc = get_benchmark("ghz", 1, 5)
     directory = "."
     filename = "ghz_oqc"
     path = Path(directory) / Path(filename).with_suffix(".qasm")
 
     tket_helper.get_native_gates_level(
         qc,
@@ -1107,33 +1080,56 @@
 class SampleObject:
     def __init__(self, name: str) -> None:
         self.name = name
 
 
 def test_timeout_watchers() -> None:
     timeout = 1
-    assert not timeout_watcher(endless_loop, timeout, [SampleObject("test"), True])
-    assert timeout_watcher(endless_loop, timeout, [SampleObject("test"), False])
+    if sys.platform == "win32":
+        with pytest.warns(RuntimeWarning, match="Timeout is not supported on Windows."):
+            timeout_watcher(endless_loop, timeout, [SampleObject("test"), False])
+    else:
+        assert not timeout_watcher(endless_loop, timeout, [SampleObject("test"), True])
+        assert timeout_watcher(endless_loop, timeout, [SampleObject("test"), False])
 
 
 def test_get_module_for_benchmark() -> None:
     for benchmark in utils.get_supported_benchmarks():
         assert utils.get_module_for_benchmark(benchmark.split("-")[0]) is not None
 
 
-def test_benchmark_helper() -> None:
+def test_benchmark_helper_shor() -> None:
     shor_instances = ["xsmall", "small", "medium", "large", "xlarge"]
     for elem in shor_instances:
         res_shor = shor.get_instance(elem)
         assert res_shor
+
+
+@pytest.mark.skipif(
+    sys.platform == "win32",
+    reason="PySCF is not available on Windows.",
+)
+def test_benchmark_groundstate_non_windows() -> None:
     groundstate_instances = ["small", "medium", "large"]
     for elem in groundstate_instances:
         res_groundstate = groundstate.get_molecule(elem)
         assert res_groundstate
 
+    qc = groundstate.create_circuit("small")
+    assert qc.depth() > 0
+
+
+@pytest.mark.skipif(
+    sys.platform != "win32",
+    reason="Windows-specific test.",
+)
+def test_benchmark_groundstate_windows() -> None:
+    with pytest.raises(ImportError, match=r"PySCF is not installed"):
+        groundstate.create_circuit("small")
+
 
 def test_tket_mapped_circuit_qubit_number() -> None:
     qc = get_benchmark("ghz", 1, 5)
     res = tket_helper.get_mapped_level(
         qc,
         qc.num_qubits,
         IBMProvider().get_device("ibm_washington"),
```

### Comparing `mqt.bench-1.1.1/tests/test_benchviewer.py` & `mqt_bench-1.1.2/tests/test_benchviewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 
-from mqt.benchviewer import Backend, BenchmarkConfiguration, Server, backend
-from mqt.benchviewer.main import app
+from mqt.bench.viewer import Backend, BenchmarkConfiguration, Server, backend
+from mqt.bench.viewer.main import app
 
 if TYPE_CHECKING or sys.version_info >= (3, 10, 0):  # pragma: no cover
     from importlib import resources
 else:
     import importlib_resources as resources
 
 
@@ -274,15 +274,15 @@
             "quantinuum_h2",
         ],
     )
     backend = Backend()
     assert backend.prepare_form_input(form_data) == expected_res
 
 
-benchviewer = resources.files("mqt.benchviewer")
+benchviewer = resources.files("mqt.bench.viewer")
 
 
 def test_read_mqtbench_all_zip() -> None:
     backend = Backend()
     with resources.as_file(benchviewer):
         target_location = str(Path("./tests").resolve())
     assert backend.read_mqtbench_all_zip(skip_question=True, target_location=target_location)
```

### Comparing `mqt.bench-1.1.1/tests/test_pregenerated_zip.py` & `mqt_bench-1.1.2/tests/test_pregenerated_zip.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import os
 import sys
 from typing import TYPE_CHECKING
 
 import pytest
 
 from mqt.bench import utils
-from mqt.benchviewer import Server
-from mqt.benchviewer.main import app
+from mqt.bench.viewer import Server
+from mqt.bench.viewer.main import app
 
 if TYPE_CHECKING or sys.version_info >= (3, 10, 0):  # pragma: no cover
     from importlib import resources
 else:
     import importlib_resources as resources
 
 # only run test when executed on GitHub runner
 IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
 
 
 @pytest.mark.skipif(not IN_GITHUB_ACTIONS, reason="Only run this test on GitHub runner")
 def test_flask_server_with_pregenerated_zip() -> None:
-    benchviewer = resources.files("mqt.benchviewer")
+    benchviewer = resources.files("mqt.bench.viewer")
     with resources.as_file(benchviewer) as benchviewer_path:
         benchviewer_location = benchviewer_path
 
     Server(
         skip_question=True,
         activate_logging=False,
-        target_location=str(utils.get_zip_file_path()),
+        target_location=str(utils.get_zip_folder_path()),
     )
 
     paths_to_check = [
         "static/files/MQTBench_all.zip",
         "templates/benchmark_description.html",
         "templates/index.html",
         "templates/legal.html",
```

