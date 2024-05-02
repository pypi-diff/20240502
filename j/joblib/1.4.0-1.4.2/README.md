# Comparing `tmp/joblib-1.4.0.tar.gz` & `tmp/joblib-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joblib-1.4.0.tar", last modified: Mon Apr  8 15:06:26 2024, max compression
+gzip compressed data, was "joblib-1.4.2.tar", last modified: Thu May  2 12:12:05 2024, max compression
```

## Comparing `joblib-1.4.0.tar` & `joblib-1.4.2.tar`

### file list

```diff
@@ -1,520 +1,520 @@
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.276729 joblib-1.4.0/
--rw-r--r--   0 tom       (1000) users      (984)      218 2024-04-08 12:26:43.000000 joblib-1.4.0/.codecov.yml
--rw-r--r--   0 tom       (1000) users      (984)      696 2024-04-08 12:26:43.000000 joblib-1.4.0/.gitignore
--rw-r--r--   0 tom       (1000) users      (984)      467 2024-04-03 09:55:41.000000 joblib-1.4.0/.mailmap
--rw-r--r--   0 tom       (1000) users      (984)       99 2024-04-08 12:26:43.000000 joblib-1.4.0/.readthedocs-requirements.txt
--rw-r--r--   0 tom       (1000) users      (984)      321 2024-04-08 12:26:43.000000 joblib-1.4.0/.readthedocs.yaml
--rw-r--r--   0 tom       (1000) users      (984)    40004 2024-04-08 15:05:17.000000 joblib-1.4.0/CHANGES.rst
--rw-r--r--   0 tom       (1000) users      (984)     1527 2024-04-08 12:26:43.000000 joblib-1.4.0/LICENSE.txt
--rw-r--r--   0 tom       (1000) users      (984)      128 2024-04-03 09:55:41.000000 joblib-1.4.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) users      (984)      363 2024-04-03 09:55:41.000000 joblib-1.4.0/Makefile
--rw-r--r--   0 tom       (1000) users      (984)     5370 2024-04-08 15:06:26.276729 joblib-1.4.0/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (984)     4218 2024-04-08 12:26:43.000000 joblib-1.4.0/README.rst
--rw-r--r--   0 tom       (1000) users      (984)     1711 2024-04-08 12:26:43.000000 joblib-1.4.0/TODO.rst
--rw-r--r--   0 tom       (1000) users      (984)     5110 2024-04-08 12:26:43.000000 joblib-1.4.0/azure-pipelines.yml
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.070062 joblib-1.4.0/benchmarks/
--rw-r--r--   0 tom       (1000) users      (984)     4331 2024-04-03 09:55:41.000000 joblib-1.4.0/benchmarks/bench_auto_batching.py
--rw-r--r--   0 tom       (1000) users      (984)     8560 2024-04-08 12:26:43.000000 joblib-1.4.0/benchmarks/bench_compression.py
--rw-r--r--   0 tom       (1000) users      (984)     3276 2024-04-08 12:26:43.000000 joblib-1.4.0/benchmarks/bench_grid_search_scaling.py
--rwxr-xr-x   0 tom       (1000) users      (984)    17244 2024-04-08 12:26:43.000000 joblib-1.4.0/benchmarks/bench_pickle.py
--rw-r--r--   0 tom       (1000) users      (984)     3228 2024-04-08 12:26:43.000000 joblib-1.4.0/benchmarks/bench_sequential_fast_tasks.py
--rw-r--r--   0 tom       (1000) users      (984)     2885 2024-04-08 12:26:43.000000 joblib-1.4.0/conftest.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.070062 joblib-1.4.0/continuous_integration/
--rwxr-xr-x   0 tom       (1000) users      (984)     2258 2024-04-08 12:29:25.000000 joblib-1.4.0/continuous_integration/install.sh
--rwxr-xr-x   0 tom       (1000) users      (984)     2171 2024-04-08 12:29:25.000000 joblib-1.4.0/continuous_integration/run_tests.sh
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.073396 joblib-1.4.0/doc/
--rw-r--r--   0 tom       (1000) users      (984)    39978 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/CHANGES.rst
--rw-r--r--   0 tom       (1000) users      (984)      535 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/Makefile
--rw-r--r--   0 tom       (1000) users      (984)     4218 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/README.rst
--rw-r--r--   0 tom       (1000) users      (984)       95 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.063396 joblib-1.4.0/doc/_build/
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.093396 joblib-1.4.0/doc/_build/html/
--rw-r--r--   0 tom       (1000) users      (984)      230 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/.buildinfo
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.120062 joblib-1.4.0/doc/_build/html/.doctrees/
--rw-r--r--   0 tom       (1000) users      (984)   212003 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/CHANGES.doctree
--rw-r--r--   0 tom       (1000) users      (984)    23583 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/README.doctree
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.130062 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    41328 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree
--rw-r--r--   0 tom       (1000) users      (984)    20104 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/index.doctree
--rw-r--r--   0 tom       (1000) users      (984)    27373 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree
--rw-r--r--   0 tom       (1000) users      (984)    27845 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.130062 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)    17457 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree
--rw-r--r--   0 tom       (1000) users      (984)     5902 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree
--rw-r--r--   0 tom       (1000) users      (984)     5383 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree
--rw-r--r--   0 tom       (1000) users      (984)    44080 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree
--rw-r--r--   0 tom       (1000) users      (984)    36427 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree
--rw-r--r--   0 tom       (1000) users      (984)    29227 2024-04-08 06:49:52.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree
--rw-r--r--   0 tom       (1000) users      (984)    35543 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree
--rw-r--r--   0 tom       (1000) users      (984)    12583 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree
--rw-r--r--   0 tom       (1000) users      (984)   237494 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/developing.doctree
--rw-r--r--   0 tom       (1000) users      (984)  5607833 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/environment.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.133396 joblib-1.4.0/doc/_build/html/.doctrees/generated/
--rw-r--r--   0 tom       (1000) users      (984)    53079 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.Memory.doctree
--rw-r--r--   0 tom       (1000) users      (984)    72422 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree
--rw-r--r--   0 tom       (1000) users      (984)    22222 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.dump.doctree
--rw-r--r--   0 tom       (1000) users      (984)     7876 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.hash.doctree
--rw-r--r--   0 tom       (1000) users      (984)    17533 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.load.doctree
--rw-r--r--   0 tom       (1000) users      (984)    20713 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.parallel_backend.doctree
--rw-r--r--   0 tom       (1000) users      (984)    50167 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree
--rw-r--r--   0 tom       (1000) users      (984)     7589 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree
--rw-r--r--   0 tom       (1000) users      (984)    35435 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/index.doctree
--rw-r--r--   0 tom       (1000) users      (984)    10914 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/installing.doctree
--rw-r--r--   0 tom       (1000) users      (984)   168597 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/.doctrees/memory.doctree
--rw-r--r--   0 tom       (1000) users      (984)   234009 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/parallel.doctree
--rw-r--r--   0 tom       (1000) users      (984)    28059 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/parallel_numpy.doctree
--rw-r--r--   0 tom       (1000) users      (984)    33378 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/persistence.doctree
--rw-r--r--   0 tom       (1000) users      (984)    10538 2024-04-08 06:49:53.000000 joblib-1.4.0/doc/_build/html/.doctrees/why.doctree
--rw-r--r--   0 tom       (1000) users      (984)    76111 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/CHANGES.html
--rw-r--r--   0 tom       (1000) users      (984)    13140 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/README.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.063396 joblib-1.4.0/doc/_build/html/_downloads/
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.133396 joblib-1.4.0/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/
--rw-r--r--   0 tom       (1000) users      (984)    48989 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.133396 joblib-1.4.0/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/
--rw-r--r--   0 tom       (1000) users      (984)     5723 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.133396 joblib-1.4.0/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/
--rw-r--r--   0 tom       (1000) users      (984)    11044 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.136729 joblib-1.4.0/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/
--rw-r--r--   0 tom       (1000) users      (984)     9044 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.136729 joblib-1.4.0/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/
--rw-r--r--   0 tom       (1000) users      (984)     7302 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.136729 joblib-1.4.0/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/
--rw-r--r--   0 tom       (1000) users      (984)    68782 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.136729 joblib-1.4.0/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/
--rw-r--r--   0 tom       (1000) users      (984)     7913 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.136729 joblib-1.4.0/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/
--rw-r--r--   0 tom       (1000) users      (984)     7520 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.136729 joblib-1.4.0/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/
--rw-r--r--   0 tom       (1000) users      (984)     6406 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/
--rw-r--r--   0 tom       (1000) users      (984)     4695 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/
--rw-r--r--   0 tom       (1000) users      (984)     1984 2024-04-08 06:45:46.000000 joblib-1.4.0/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/
--rw-r--r--   0 tom       (1000) users      (984)     8458 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/
--rw-r--r--   0 tom       (1000) users      (984)     5092 2024-04-08 06:43:09.000000 joblib-1.4.0/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/
--rw-r--r--   0 tom       (1000) users      (984)    13695 2024-04-08 06:45:46.000000 joblib-1.4.0/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/
--rw-r--r--   0 tom       (1000) users      (984)     4787 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.140062 joblib-1.4.0/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/
--rw-r--r--   0 tom       (1000) users      (984)    13465 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.143396 joblib-1.4.0/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/
--rw-r--r--   0 tom       (1000) users      (984)     5588 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.143396 joblib-1.4.0/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/
--rw-r--r--   0 tom       (1000) users      (984)     2943 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.146729 joblib-1.4.0/doc/_build/html/_images/
--rw-r--r--   0 tom       (1000) users      (984)    14175 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png
--rw-r--r--   0 tom       (1000) users      (984)     7869 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png
--rw-r--r--   0 tom       (1000) users      (984)    13475 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    20475 2024-04-08 06:47:56.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_generator_001.png
--rw-r--r--   0 tom       (1000) users      (984)    14279 2024-04-08 06:48:35.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.153396 joblib-1.4.0/doc/_build/html/_sources/
--rw-r--r--   0 tom       (1000) users      (984)    39978 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/CHANGES.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     4218 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/README.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.156729 joblib-1.4.0/doc/_build/html/_sources/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    13175 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     4940 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/index.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     7558 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     7412 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.156729 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)     4448 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      789 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      569 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    12861 2024-04-08 06:48:35.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    10852 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     8467 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    10133 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1976 2024-04-08 06:47:55.000000 joblib-1.4.0/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)       97 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/developing.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.163396 joblib-1.4.0/doc/_build/html/_sources/generated/
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.Memory.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      197 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.Parallel.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.dump.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.hash.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.load.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      239 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.parallel_backend.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      234 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.parallel_config.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)      247 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/_build/html/_sources/generated/joblib.register_compressor.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1268 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/index.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1839 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/installing.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    18015 2024-04-08 06:50:46.000000 joblib-1.4.0/doc/_build/html/_sources/memory.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)    19093 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/parallel.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     6328 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/parallel_numpy.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     7247 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/persistence.rst.txt
--rw-r--r--   0 tom       (1000) users      (984)     1680 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_sources/why.rst.txt
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.180062 joblib-1.4.0/doc/_build/html/_static/
--rw-r--r--   0 tom       (1000) users      (984)    11230 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/_static/alabaster.css
--rw-r--r--   0 tom       (1000) users      (984)    14692 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/_static/basic.css
--rw-r--r--   0 tom       (1000) users      (984)     3380 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/binder_badge_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    21404 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/broken_example.png
--rw-r--r--   0 tom       (1000) users      (984)     1302 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_static/custom.css
--rw-r--r--   0 tom       (1000) users      (984)    10766 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/doctools.js
--rw-r--r--   0 tom       (1000) users      (984)      422 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/_static/documentation_options.js
--rw-r--r--   0 tom       (1000) users      (984)   268286 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_static/favicon.ico
--rw-r--r--   0 tom       (1000) users      (984)      286 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/file.png
--rw-r--r--   0 tom       (1000) users      (984)    15594 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_static/joblib_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    27703 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_build/html/_static/joblib_logo_examples.png
--rw-r--r--   0 tom       (1000) users      (984)   287630 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 tom       (1000) users      (984)    89476 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/jquery.js
--rw-r--r--   0 tom       (1000) users      (984)     6936 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/jupyterlite_badge_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    10854 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/_static/language_data.js
--rw-r--r--   0 tom       (1000) users      (984)       90 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/minus.png
--rw-r--r--   0 tom       (1000) users      (984)     4315 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/no_image.png
--rw-r--r--   0 tom       (1000) users      (984)       90 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/plus.png
--rw-r--r--   0 tom       (1000) users      (984)     4929 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/_static/pygments.css
--rw-r--r--   0 tom       (1000) users      (984)    16634 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/searchtools.js
--rw-r--r--   0 tom       (1000) users      (984)      167 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/sg_gallery-binder.css
--rw-r--r--   0 tom       (1000) users      (984)     1137 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/sg_gallery-dataframe.css
--rw-r--r--   0 tom       (1000) users      (984)     4330 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/sg_gallery-rendered-html.css
--rw-r--r--   0 tom       (1000) users      (984)     9530 2023-04-18 19:56:48.000000 joblib-1.4.0/doc/_build/html/_static/sg_gallery.css
--rw-r--r--   0 tom       (1000) users      (984)    68420 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 tom       (1000) users      (984)    19530 2023-09-05 22:32:59.000000 joblib-1.4.0/doc/_build/html/_static/underscore.js
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.186729 joblib-1.4.0/doc/_build/html/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    61440 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/compressors_comparison.html
--rw-r--r--   0 tom       (1000) users      (984)    11116 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/index.html
--rw-r--r--   0 tom       (1000) users      (984)    38535 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/memory_basic_usage.html
--rw-r--r--   0 tom       (1000) users      (984)    35688 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/nested_parallel_memory.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.186729 joblib-1.4.0/doc/_build/html/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)    14623 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html
--rw-r--r--   0 tom       (1000) users      (984)     6185 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/parallel/index.html
--rw-r--r--   0 tom       (1000) users      (984)     5698 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/parallel/sg_execution_times.html
--rw-r--r--   0 tom       (1000) users      (984)    41580 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/parallel_generator.html
--rw-r--r--   0 tom       (1000) users      (984)    44464 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/parallel_memmap.html
--rw-r--r--   0 tom       (1000) users      (984)    36621 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/parallel_random_state.html
--rw-r--r--   0 tom       (1000) users      (984)    33549 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/serialization_and_wrappers.html
--rw-r--r--   0 tom       (1000) users      (984)     7794 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/auto_examples/sg_execution_times.html
--rw-r--r--   0 tom       (1000) users      (984)    86206 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/developing.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.190062 joblib-1.4.0/doc/_build/html/generated/
--rw-r--r--   0 tom       (1000) users      (984)    18604 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.Memory.html
--rw-r--r--   0 tom       (1000) users      (984)    31096 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.Parallel.html
--rw-r--r--   0 tom       (1000) users      (984)    10213 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.dump.html
--rw-r--r--   0 tom       (1000) users      (984)     6452 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.hash.html
--rw-r--r--   0 tom       (1000) users      (984)     9144 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.load.html
--rw-r--r--   0 tom       (1000) users      (984)    14807 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.parallel_backend.html
--rw-r--r--   0 tom       (1000) users      (984)    19630 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.parallel_config.html
--rw-r--r--   0 tom       (1000) users      (984)     6327 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/generated/joblib.register_compressor.html
--rw-r--r--   0 tom       (1000) users      (984)    10542 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/genindex.html
--rw-r--r--   0 tom       (1000) users      (984)    23348 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/index.html
--rw-r--r--   0 tom       (1000) users      (984)     9384 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/installing.html
--rw-r--r--   0 tom       (1000) users      (984)    78141 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/memory.html
--rw-r--r--   0 tom       (1000) users      (984)     1805 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/objects.inv
--rw-r--r--   0 tom       (1000) users      (984)   110008 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/parallel.html
--rw-r--r--   0 tom       (1000) users      (984)    21579 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/parallel_numpy.html
--rw-r--r--   0 tom       (1000) users      (984)    30768 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/persistence.html
--rw-r--r--   0 tom       (1000) users      (984)     4958 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/py-modindex.html
--rw-r--r--   0 tom       (1000) users      (984)     5197 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/search.html
--rw-r--r--   0 tom       (1000) users      (984)    49550 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/searchindex.js
--rw-r--r--   0 tom       (1000) users      (984)     7853 2024-04-08 06:50:49.000000 joblib-1.4.0/doc/_build/html/why.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.193395 joblib-1.4.0/doc/_static/
--rw-r--r--   0 tom       (1000) users      (984)     1302 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/_static/custom.css
--rw-r--r--   0 tom       (1000) users      (984)   268286 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_static/favicon.ico
--rw-r--r--   0 tom       (1000) users      (984)    15594 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_static/joblib_logo.svg
--rw-r--r--   0 tom       (1000) users      (984)    27703 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_static/joblib_logo_examples.png
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.193395 joblib-1.4.0/doc/_templates/
--rw-r--r--   0 tom       (1000) users      (984)      208 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/_templates/class.rst
--rw-r--r--   0 tom       (1000) users      (984)      226 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/_templates/function.rst
--rw-r--r--   0 tom       (1000) users      (984)      480 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/_templates/layout.html
--rw-r--r--   0 tom       (1000) users      (984)      323 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/_templates/navigation.html
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.213395 joblib-1.4.0/doc/auto_examples/
--rw-r--r--   0 tom       (1000) users      (984)    68782 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/auto_examples_jupyter.zip
--rw-r--r--   0 tom       (1000) users      (984)    48989 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/auto_examples_python.zip
--rw-r--r--   0 tom       (1000) users      (984)    13465 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/compressors_comparison.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     9044 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/auto_examples/compressors_comparison.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/compressors_comparison.py.md5
--rw-r--r--   0 tom       (1000) users      (984)    13175 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/compressors_comparison.rst
--rw-r--r--   0 tom       (1000) users      (984)     3434 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/compressors_comparison_codeobj.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.216729 joblib-1.4.0/doc/auto_examples/images/
--rw-r--r--   0 tom       (1000) users      (984)    14175 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png
--rw-r--r--   0 tom       (1000) users      (984)     7869 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png
--rw-r--r--   0 tom       (1000) users      (984)    20475 2024-04-08 06:47:41.000000 joblib-1.4.0/doc/auto_examples/images/sphx_glr_parallel_generator_001.png
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.216729 joblib-1.4.0/doc/auto_examples/images/thumb/
--rw-r--r--   0 tom       (1000) users      (984)    13475 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    14279 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)     4940 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/index.rst
--rw-r--r--   0 tom       (1000) users      (984)     6406 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/auto_examples/memory_basic_usage.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     4695 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/auto_examples/memory_basic_usage.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/auto_examples/memory_basic_usage.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     7558 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/auto_examples/memory_basic_usage.rst
--rw-r--r--   0 tom       (1000) users      (984)     2516 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/auto_examples/memory_basic_usage_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     7302 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/auto_examples/nested_parallel_memory.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     5092 2024-04-08 06:43:09.000000 joblib-1.4.0/doc/auto_examples/nested_parallel_memory.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/auto_examples/nested_parallel_memory.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     7412 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/auto_examples/nested_parallel_memory.rst
--rw-r--r--   0 tom       (1000) users      (984)     2729 2024-04-08 06:43:21.000000 joblib-1.4.0/doc/auto_examples/nested_parallel_memory_codeobj.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.220062 joblib-1.4.0/doc/auto_examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)     2943 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     1984 2024-04-08 06:45:46.000000 joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     4448 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.rst
--rw-r--r--   0 tom       (1000) users      (984)     2457 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.063396 joblib-1.4.0/doc/auto_examples/parallel/images/
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.220062 joblib-1.4.0/doc/auto_examples/parallel/images/thumb/
--rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png
--rw-r--r--   0 tom       (1000) users      (984)      789 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/index.rst
--rw-r--r--   0 tom       (1000) users      (984)      569 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/auto_examples/parallel/sg_execution_times.rst
--rw-r--r--   0 tom       (1000) users      (984)    13695 2024-04-08 06:45:46.000000 joblib-1.4.0/doc/auto_examples/parallel_generator.ipynb
--rw-r--r--   0 tom       (1000) users      (984)    11044 2024-04-08 06:45:12.000000 joblib-1.4.0/doc/auto_examples/parallel_generator.py
--rw-r--r--   0 tom       (1000) users      (984)    12861 2024-04-08 06:48:35.000000 joblib-1.4.0/doc/auto_examples/parallel_generator.rst
--rw-r--r--   0 tom       (1000) users      (984)     1263 2024-04-08 06:50:48.000000 joblib-1.4.0/doc/auto_examples/parallel_generator_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     8458 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/auto_examples/parallel_memmap.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     5588 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/parallel_memmap.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/auto_examples/parallel_memmap.py.md5
--rw-r--r--   0 tom       (1000) users      (984)    10852 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/auto_examples/parallel_memmap.rst
--rw-r--r--   0 tom       (1000) users      (984)     2644 2024-04-08 06:43:40.000000 joblib-1.4.0/doc/auto_examples/parallel_memmap_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     7520 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/parallel_random_state.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     4787 2024-04-08 06:43:36.000000 joblib-1.4.0/doc/auto_examples/parallel_random_state.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/parallel_random_state.py.md5
--rw-r--r--   0 tom       (1000) users      (984)     8467 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/parallel_random_state.rst
--rw-r--r--   0 tom       (1000) users      (984)     1503 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/parallel_random_state_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-08 06:48:37.000000 joblib-1.4.0/doc/auto_examples/searchindex.bak
--rw-r--r--   0 tom       (1000) users      (984)    73632 2024-04-08 06:48:37.000000 joblib-1.4.0/doc/auto_examples/searchindex.dat
--rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-08 06:48:37.000000 joblib-1.4.0/doc/auto_examples/searchindex.dir
--rw-r--r--   0 tom       (1000) users      (984)     7913 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.ipynb
--rw-r--r--   0 tom       (1000) users      (984)     5723 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.py
--rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.py.md5
--rw-r--r--   0 tom       (1000) users      (984)    10133 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.rst
--rw-r--r--   0 tom       (1000) users      (984)     1619 2024-04-08 06:43:37.000000 joblib-1.4.0/doc/auto_examples/serialization_and_wrappers_codeobj.pickle
--rw-r--r--   0 tom       (1000) users      (984)     1976 2024-04-08 06:47:55.000000 joblib-1.4.0/doc/auto_examples/sg_execution_times.rst
--rw-r--r--   0 tom       (1000) users      (984)     7882 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/conf.py
--rw-r--r--   0 tom       (1000) users      (984)      624 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/conftest.py
--rw-r--r--   0 tom       (1000) users      (984)       97 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/developing.rst
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.233396 joblib-1.4.0/doc/generated/
--rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.Logger.cache.examples
--rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.Logger.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)      706 2024-04-08 06:47:55.000000 joblib-1.4.0/doc/generated/joblib.Logger.examples
--rw-r--r--   0 tom       (1000) users      (984)     1235 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.MemorizedFunc.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Memory.__init__.examples
--rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.Memory.cache.examples
--rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.Memory.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Memory.eval.examples
--rw-r--r--   0 tom       (1000) users      (984)     1221 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.Memory.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Memory.format.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Memory.reduce_size.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.Memory.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Parallel.dispatch_next.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Parallel.dispatch_one_batch.examples
--rw-r--r--   0 tom       (1000) users      (984)      710 2024-04-08 06:47:55.000000 joblib-1.4.0/doc/generated/joblib.Parallel.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Parallel.format.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.Parallel.print_progress.examples
--rw-r--r--   0 tom       (1000) users      (984)      197 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.Parallel.rst
--rw-r--r--   0 tom       (1000) users      (984)      708 2024-04-08 06:47:55.000000 joblib-1.4.0/doc/generated/joblib.delayed.examples
--rw-r--r--   0 tom       (1000) users      (984)     1210 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.dump.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.dump.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.expires_after.examples
--rw-r--r--   0 tom       (1000) users      (984)      763 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.externals.loky.set_loky_pickler.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.hash.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.hash.rst
--rw-r--r--   0 tom       (1000) users      (984)     1210 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.load.examples
--rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.load.rst
--rw-r--r--   0 tom       (1000) users      (984)     1247 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.logger.Logger.cache.examples
--rw-r--r--   0 tom       (1000) users      (984)     1247 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.logger.Logger.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.memory.MemorizedFunc.__init__.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.memory.MemorizedFunc.call.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.memory.MemorizedFunc.check_call_in_cache.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.memory.MemorizedFunc.clear.examples
--rw-r--r--   0 tom       (1000) users      (984)     1249 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.memory.MemorizedFunc.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.parallel.AutoBatchingMixin.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.parallel.ParallelBackendBase.examples
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.parallel_backend.examples
--rw-r--r--   0 tom       (1000) users      (984)      239 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.parallel_backend.rst
--rw-r--r--   0 tom       (1000) users      (984)     1295 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.parallel_config.examples
--rw-r--r--   0 tom       (1000) users      (984)      234 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.parallel_config.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.register_compressor.examples
--rw-r--r--   0 tom       (1000) users      (984)      247 2024-04-08 06:43:01.000000 joblib-1.4.0/doc/generated/joblib.register_compressor.rst
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.0/doc/generated/joblib.register_parallel_backend.examples
--rw-r--r--   0 tom       (1000) users      (984)      753 2024-04-08 06:45:48.000000 joblib-1.4.0/doc/generated/joblib.wrap_non_picklable_objects.examples
--rw-r--r--   0 tom       (1000) users      (984)     1268 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/index.rst
--rw-r--r--   0 tom       (1000) users      (984)     1839 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/installing.rst
--rw-r--r--   0 tom       (1000) users      (984)    17989 2024-04-08 12:29:30.000000 joblib-1.4.0/doc/memory.rst
--rw-r--r--   0 tom       (1000) users      (984)    19093 2024-04-08 12:29:20.000000 joblib-1.4.0/doc/parallel.rst
--rw-r--r--   0 tom       (1000) users      (984)     6328 2024-04-08 12:26:43.000000 joblib-1.4.0/doc/parallel_numpy.rst
--rw-r--r--   0 tom       (1000) users      (984)     7247 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/persistence.rst
--rw-r--r--   0 tom       (1000) users      (984)     1680 2024-04-03 09:55:41.000000 joblib-1.4.0/doc/why.rst
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.233396 joblib-1.4.0/examples/
--rw-r--r--   0 tom       (1000) users      (984)      131 2024-04-03 09:55:41.000000 joblib-1.4.0/examples/README.txt
--rw-r--r--   0 tom       (1000) users      (984)     9044 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/compressors_comparison.py
--rw-r--r--   0 tom       (1000) users      (984)     4695 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/memory_basic_usage.py
--rw-r--r--   0 tom       (1000) users      (984)     5092 2024-04-03 09:55:41.000000 joblib-1.4.0/examples/nested_parallel_memory.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.233396 joblib-1.4.0/examples/parallel/
--rw-r--r--   0 tom       (1000) users      (984)      111 2024-04-03 09:55:41.000000 joblib-1.4.0/examples/parallel/README.txt
--rw-r--r--   0 tom       (1000) users      (984)     1984 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/parallel/distributed_backend_simple.py
--rw-r--r--   0 tom       (1000) users      (984)    11044 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/parallel_generator.py
--rw-r--r--   0 tom       (1000) users      (984)     5588 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/parallel_memmap.py
--rw-r--r--   0 tom       (1000) users      (984)     4787 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/parallel_random_state.py
--rw-r--r--   0 tom       (1000) users      (984)     5723 2024-04-08 12:26:43.000000 joblib-1.4.0/examples/serialization_and_wrappers.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.236729 joblib-1.4.0/joblib/
--rw-r--r--   0 tom       (1000) users      (984)     5132 2024-04-08 15:05:17.000000 joblib-1.4.0/joblib/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)      417 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/_cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)    13313 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/_dask.py
--rw-r--r--   0 tom       (1000) users      (984)    28092 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/_memmapping_reducer.py
--rw-r--r--   0 tom       (1000) users      (984)     1925 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/_multiprocessing_helpers.py
--rw-r--r--   0 tom       (1000) users      (984)    25489 2024-04-08 12:29:20.000000 joblib-1.4.0/joblib/_parallel_backends.py
--rw-r--r--   0 tom       (1000) users      (984)    16683 2024-04-08 12:29:25.000000 joblib-1.4.0/joblib/_store_backends.py
--rw-r--r--   0 tom       (1000) users      (984)     2076 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/_utils.py
--rw-r--r--   0 tom       (1000) users      (984)     5361 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/backports.py
--rw-r--r--   0 tom       (1000) users      (984)    19768 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/compressor.py
--rw-r--r--   0 tom       (1000) users      (984)     4389 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/disk.py
--rw-r--r--   0 tom       (1000) users      (984)     5136 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/executor.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.240062 joblib-1.4.0/joblib/externals/
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/externals/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.240062 joblib-1.4.0/joblib/externals/cloudpickle/
--rw-r--r--   0 tom       (1000) users      (984)      308 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/cloudpickle/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)    55283 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/cloudpickle/cloudpickle.py
--rw-r--r--   0 tom       (1000) users      (984)      322 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/cloudpickle/cloudpickle_fast.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.240062 joblib-1.4.0/joblib/externals/loky/
--rw-r--r--   0 tom       (1000) users      (984)     1104 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     1057 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/_base.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.243396 joblib-1.4.0/joblib/externals/loky/backend/
--rw-r--r--   0 tom       (1000) users      (984)      312 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     1776 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/_posix_reduction.py
--rw-r--r--   0 tom       (1000) users      (984)      683 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/_win_reduction.py
--rw-r--r--   0 tom       (1000) users      (984)    13654 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/context.py
--rw-r--r--   0 tom       (1000) users      (984)     1186 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/fork_exec.py
--rw-r--r--   0 tom       (1000) users      (984)     5580 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/popen_loky_posix.py
--rw-r--r--   0 tom       (1000) users      (984)     5325 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/popen_loky_win32.py
--rw-r--r--   0 tom       (1000) users      (984)     2018 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/process.py
--rw-r--r--   0 tom       (1000) users      (984)     7322 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/queues.py
--rw-r--r--   0 tom       (1000) users      (984)     7063 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/reduction.py
--rw-r--r--   0 tom       (1000) users      (984)    14498 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/resource_tracker.py
--rw-r--r--   0 tom       (1000) users      (984)     8962 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/spawn.py
--rw-r--r--   0 tom       (1000) users      (984)    11768 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/synchronize.py
--rw-r--r--   0 tom       (1000) users      (984)     5757 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/backend/utils.py
--rw-r--r--   0 tom       (1000) users      (984)     3608 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)     2567 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/initializers.py
--rw-r--r--   0 tom       (1000) users      (984)    51050 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/process_executor.py
--rw-r--r--   0 tom       (1000) users      (984)    10305 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/loky/reusable_executor.py
--rw-r--r--   0 tom       (1000) users      (984)      671 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/externals/vendor_cloudpickle.sh
--rwxr-xr-x   0 tom       (1000) users      (984)      965 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/externals/vendor_loky.sh
--rw-r--r--   0 tom       (1000) users      (984)    14204 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/func_inspect.py
--rw-r--r--   0 tom       (1000) users      (984)    10535 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/hashing.py
--rw-r--r--   0 tom       (1000) users      (984)     5463 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/logger.py
--rw-r--r--   0 tom       (1000) users      (984)    45990 2024-04-08 12:29:25.000000 joblib-1.4.0/joblib/memory.py
--rw-r--r--   0 tom       (1000) users      (984)    26886 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/numpy_pickle.py
--rw-r--r--   0 tom       (1000) users      (984)     8547 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/numpy_pickle_compat.py
--rw-r--r--   0 tom       (1000) users      (984)     8723 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/numpy_pickle_utils.py
--rw-r--r--   0 tom       (1000) users      (984)    84579 2024-04-08 12:29:25.000000 joblib-1.4.0/joblib/parallel.py
--rw-r--r--   0 tom       (1000) users      (984)    14411 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/pool.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.250062 joblib-1.4.0/joblib/test/
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/__init__.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.250062 joblib-1.4.0/joblib/test/_openmp_test_helper/
--rw-r--r--   0 tom       (1000) users      (984)       16 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/_openmp_test_helper/.gitignore
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/_openmp_test_helper/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)      390 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/_openmp_test_helper/parallel_sum.pyx
--rw-r--r--   0 tom       (1000) users      (984)      749 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/_openmp_test_helper/setup.py
--rw-r--r--   0 tom       (1000) users      (984)     2336 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/common.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.276729 joblib-1.4.0/joblib/test/data/
--rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     3460 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/data/create_numpy_pickle.py
--rwxr-xr-x   0 tom       (1000) users      (984)      514 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/generate_data.sh
--rw-r--r--   0 tom       (1000) users      (984)      769 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz
--rw-r--r--   0 tom       (1000) users      (984)      757 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz
--rw-r--r--   0 tom       (1000) users      (984)      792 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz
--rw-r--r--   0 tom       (1000) users      (984)      794 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      790 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      986 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl
--rw-r--r--   0 tom       (1000) users      (984)      997 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      798 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      660 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      712 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl
--rw-r--r--   0 tom       (1000) users      (984)     1000 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      831 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      694 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)     1021 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      831 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      697 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)     1005 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      833 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      701 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)      800 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz
--rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl
--rw-r--r--   0 tom       (1000) users      (984)      991 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2
--rw-r--r--   0 tom       (1000) users      (984)      800 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip
--rw-r--r--   0 tom       (1000) users      (984)      715 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma
--rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz
--rw-r--r--   0 tom       (1000) users      (984)      849 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.12.2_pickle_py36_np114.pkl.lz4
--rw-r--r--   0 tom       (1000) users      (984)      659 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz
--rw-r--r--   0 tom       (1000) users      (984)      658 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz
--rw-r--r--   0 tom       (1000) users      (984)      658 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz
--rw-r--r--   0 tom       (1000) users      (984)      673 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      673 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)      670 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      670 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      691 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      307 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      691 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      307 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      691 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_01.npy
--rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_02.npy
--rw-r--r--   0 tom       (1000) users      (984)      307 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_03.npy
--rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_04.npy
--rw-r--r--   0 tom       (1000) users      (984)      802 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz
--rw-r--r--   0 tom       (1000) users      (984)       43 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_01.npy.z
--rw-r--r--   0 tom       (1000) users      (984)       43 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_02.npy.z
--rw-r--r--   0 tom       (1000) users      (984)       37 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_03.npy.z
--rw-r--r--   0 tom       (1000) users      (984)     1175 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/test_backports.py
--rw-r--r--   0 tom       (1000) users      (984)      751 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)     5284 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_config.py
--rw-r--r--   0 tom       (1000) users      (984)    18418 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_dask.py
--rw-r--r--   0 tom       (1000) users      (984)     2205 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/test_disk.py
--rw-r--r--   0 tom       (1000) users      (984)     9488 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_func_inspect.py
--rw-r--r--   0 tom       (1000) users      (984)      145 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_func_inspect_special_encoding.py
--rw-r--r--   0 tom       (1000) users      (984)    16054 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_hashing.py
--rw-r--r--   0 tom       (1000) users      (984)      422 2024-04-03 09:55:41.000000 joblib-1.4.0/joblib/test/test_init.py
--rw-r--r--   0 tom       (1000) users      (984)      984 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_logger.py
--rw-r--r--   0 tom       (1000) users      (984)    43298 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_memmapping.py
--rw-r--r--   0 tom       (1000) users      (984)    49419 2024-04-08 12:29:25.000000 joblib-1.4.0/joblib/test/test_memory.py
--rw-r--r--   0 tom       (1000) users      (984)     4807 2024-04-08 12:29:25.000000 joblib-1.4.0/joblib/test/test_memory_async.py
--rw-r--r--   0 tom       (1000) users      (984)     1123 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_missing_multiprocessing.py
--rw-r--r--   0 tom       (1000) users      (984)     1936 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_module.py
--rw-r--r--   0 tom       (1000) users      (984)    42485 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_numpy_pickle.py
--rw-r--r--   0 tom       (1000) users      (984)      609 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_numpy_pickle_compat.py
--rw-r--r--   0 tom       (1000) users      (984)      383 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_numpy_pickle_utils.py
--rw-r--r--   0 tom       (1000) users      (984)    73523 2024-04-08 12:29:20.000000 joblib-1.4.0/joblib/test/test_parallel.py
--rw-r--r--   0 tom       (1000) users      (984)     3121 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_store_backends.py
--rw-r--r--   0 tom       (1000) users      (984)     2570 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_testing.py
--rw-r--r--   0 tom       (1000) users      (984)      584 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/test_utils.py
--rw-r--r--   0 tom       (1000) users      (984)      251 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/test/testutils.py
--rw-r--r--   0 tom       (1000) users      (984)     3093 2024-04-08 12:26:43.000000 joblib-1.4.0/joblib/testing.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-04-08 15:06:26.236729 joblib-1.4.0/joblib.egg-info/
--rw-r--r--   0 tom       (1000) users      (984)     5370 2024-04-08 15:06:25.000000 joblib-1.4.0/joblib.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (984)    21285 2024-04-08 15:06:26.000000 joblib-1.4.0/joblib.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) users      (984)        1 2024-04-08 15:06:25.000000 joblib-1.4.0/joblib.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) users      (984)        7 2024-04-08 15:06:25.000000 joblib-1.4.0/joblib.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) users      (984)     2390 2024-04-08 12:26:43.000000 joblib-1.4.0/pyproject.toml
--rw-r--r--   0 tom       (1000) users      (984)      172 2024-04-08 15:06:26.276729 joblib-1.4.0/setup.cfg
--rwxr-xr-x   0 tom       (1000) users      (984)       92 2024-04-08 12:26:43.000000 joblib-1.4.0/setup.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.793951 joblib-1.4.2/
+-rw-r--r--   0 tom       (1000) users      (984)      218 2024-04-08 12:26:43.000000 joblib-1.4.2/.codecov.yml
+-rw-r--r--   0 tom       (1000) users      (984)      696 2024-04-08 12:26:43.000000 joblib-1.4.2/.gitignore
+-rw-r--r--   0 tom       (1000) users      (984)      467 2024-04-03 09:55:41.000000 joblib-1.4.2/.mailmap
+-rw-r--r--   0 tom       (1000) users      (984)       99 2024-04-08 12:26:43.000000 joblib-1.4.2/.readthedocs-requirements.txt
+-rw-r--r--   0 tom       (1000) users      (984)      321 2024-04-08 12:26:43.000000 joblib-1.4.2/.readthedocs.yaml
+-rw-r--r--   0 tom       (1000) users      (984)    40387 2024-05-02 12:11:23.000000 joblib-1.4.2/CHANGES.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1527 2024-04-08 12:26:43.000000 joblib-1.4.2/LICENSE.txt
+-rw-r--r--   0 tom       (1000) users      (984)      128 2024-04-03 09:55:41.000000 joblib-1.4.2/MANIFEST.in
+-rw-r--r--   0 tom       (1000) users      (984)      363 2024-04-03 09:55:41.000000 joblib-1.4.2/Makefile
+-rw-r--r--   0 tom       (1000) users      (984)     5364 2024-05-02 12:12:05.793951 joblib-1.4.2/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (984)     4212 2024-04-09 07:52:44.000000 joblib-1.4.2/README.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1711 2024-04-08 12:26:43.000000 joblib-1.4.2/TODO.rst
+-rw-r--r--   0 tom       (1000) users      (984)     5106 2024-04-09 07:51:51.000000 joblib-1.4.2/azure-pipelines.yml
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.697284 joblib-1.4.2/benchmarks/
+-rw-r--r--   0 tom       (1000) users      (984)     4331 2024-04-03 09:55:41.000000 joblib-1.4.2/benchmarks/bench_auto_batching.py
+-rw-r--r--   0 tom       (1000) users      (984)     8560 2024-04-08 12:26:43.000000 joblib-1.4.2/benchmarks/bench_compression.py
+-rw-r--r--   0 tom       (1000) users      (984)     3276 2024-04-08 12:26:43.000000 joblib-1.4.2/benchmarks/bench_grid_search_scaling.py
+-rwxr-xr-x   0 tom       (1000) users      (984)    17244 2024-04-08 12:26:43.000000 joblib-1.4.2/benchmarks/bench_pickle.py
+-rw-r--r--   0 tom       (1000) users      (984)     3228 2024-04-08 12:26:43.000000 joblib-1.4.2/benchmarks/bench_sequential_fast_tasks.py
+-rw-r--r--   0 tom       (1000) users      (984)     3107 2024-05-02 08:05:25.000000 joblib-1.4.2/conftest.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.697284 joblib-1.4.2/continuous_integration/
+-rwxr-xr-x   0 tom       (1000) users      (984)     2258 2024-04-08 12:29:25.000000 joblib-1.4.2/continuous_integration/install.sh
+-rwxr-xr-x   0 tom       (1000) users      (984)     2171 2024-04-08 12:29:25.000000 joblib-1.4.2/continuous_integration/run_tests.sh
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.697284 joblib-1.4.2/doc/
+-rw-r--r--   0 tom       (1000) users      (984)    39978 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/CHANGES.rst
+-rw-r--r--   0 tom       (1000) users      (984)      535 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/Makefile
+-rw-r--r--   0 tom       (1000) users      (984)     4218 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/README.rst
+-rw-r--r--   0 tom       (1000) users      (984)       95 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/__init__.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.687284 joblib-1.4.2/doc/_build/
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.700617 joblib-1.4.2/doc/_build/html/
+-rw-r--r--   0 tom       (1000) users      (984)      230 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/.buildinfo
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.713951 joblib-1.4.2/doc/_build/html/.doctrees/
+-rw-r--r--   0 tom       (1000) users      (984)   212003 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/CHANGES.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    23583 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/README.doctree
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    41328 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    20104 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/index.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    27373 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    27845 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)    17457 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     5902 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     5383 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    44080 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    36427 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    29227 2024-04-08 06:49:52.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    35543 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    12583 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree
+-rw-r--r--   0 tom       (1000) users      (984)   237494 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/developing.doctree
+-rw-r--r--   0 tom       (1000) users      (984)  5607833 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/environment.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/.doctrees/generated/
+-rw-r--r--   0 tom       (1000) users      (984)    53079 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.Memory.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    72422 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    22222 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.dump.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     7876 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.hash.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    17533 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.load.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    20713 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.parallel_backend.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    50167 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree
+-rw-r--r--   0 tom       (1000) users      (984)     7589 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    35435 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    10914 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/installing.doctree
+-rw-r--r--   0 tom       (1000) users      (984)   168597 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/.doctrees/memory.doctree
+-rw-r--r--   0 tom       (1000) users      (984)   234009 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/parallel.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    28059 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/parallel_numpy.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    33378 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/persistence.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    10538 2024-04-08 06:49:53.000000 joblib-1.4.2/doc/_build/html/.doctrees/why.doctree
+-rw-r--r--   0 tom       (1000) users      (984)    76111 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/CHANGES.html
+-rw-r--r--   0 tom       (1000) users      (984)    13140 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/README.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.687284 joblib-1.4.2/doc/_build/html/_downloads/
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/
+-rw-r--r--   0 tom       (1000) users      (984)    48989 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/
+-rw-r--r--   0 tom       (1000) users      (984)     5723 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/
+-rw-r--r--   0 tom       (1000) users      (984)    11044 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.717284 joblib-1.4.2/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/
+-rw-r--r--   0 tom       (1000) users      (984)     9044 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/
+-rw-r--r--   0 tom       (1000) users      (984)     7302 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/
+-rw-r--r--   0 tom       (1000) users      (984)    68782 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/
+-rw-r--r--   0 tom       (1000) users      (984)     7913 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/
+-rw-r--r--   0 tom       (1000) users      (984)     7520 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/
+-rw-r--r--   0 tom       (1000) users      (984)     6406 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/
+-rw-r--r--   0 tom       (1000) users      (984)     4695 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/
+-rw-r--r--   0 tom       (1000) users      (984)     1984 2024-04-08 06:45:46.000000 joblib-1.4.2/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/
+-rw-r--r--   0 tom       (1000) users      (984)     8458 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/
+-rw-r--r--   0 tom       (1000) users      (984)     5092 2024-04-08 06:43:09.000000 joblib-1.4.2/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/
+-rw-r--r--   0 tom       (1000) users      (984)    13695 2024-04-08 06:45:46.000000 joblib-1.4.2/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/
+-rw-r--r--   0 tom       (1000) users      (984)     4787 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/
+-rw-r--r--   0 tom       (1000) users      (984)    13465 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/
+-rw-r--r--   0 tom       (1000) users      (984)     5588 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.720617 joblib-1.4.2/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/
+-rw-r--r--   0 tom       (1000) users      (984)     2943 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.723951 joblib-1.4.2/doc/_build/html/_images/
+-rw-r--r--   0 tom       (1000) users      (984)    14175 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png
+-rw-r--r--   0 tom       (1000) users      (984)     7869 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png
+-rw-r--r--   0 tom       (1000) users      (984)    13475 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    20475 2024-04-08 06:47:56.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_generator_001.png
+-rw-r--r--   0 tom       (1000) users      (984)    14279 2024-04-08 06:48:35.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.723951 joblib-1.4.2/doc/_build/html/_sources/
+-rw-r--r--   0 tom       (1000) users      (984)    39978 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/CHANGES.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     4218 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/README.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.727284 joblib-1.4.2/doc/_build/html/_sources/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    13175 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     4940 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/index.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     7558 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     7412 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.727284 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)     4448 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      789 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      569 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    12861 2024-04-08 06:48:35.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    10852 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     8467 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    10133 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1976 2024-04-08 06:47:55.000000 joblib-1.4.2/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)       97 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/developing.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.727284 joblib-1.4.2/doc/_build/html/_sources/generated/
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.Memory.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      197 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.Parallel.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.dump.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.hash.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.load.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      239 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.parallel_backend.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      234 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.parallel_config.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)      247 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/_build/html/_sources/generated/joblib.register_compressor.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1268 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1839 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/installing.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    18015 2024-04-08 06:50:46.000000 joblib-1.4.2/doc/_build/html/_sources/memory.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)    19093 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/parallel.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     6328 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/parallel_numpy.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     7247 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/persistence.rst.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1680 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_sources/why.rst.txt
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.733951 joblib-1.4.2/doc/_build/html/_static/
+-rw-r--r--   0 tom       (1000) users      (984)    11230 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/_static/alabaster.css
+-rw-r--r--   0 tom       (1000) users      (984)    14692 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/_static/basic.css
+-rw-r--r--   0 tom       (1000) users      (984)     3380 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/binder_badge_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    21404 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/broken_example.png
+-rw-r--r--   0 tom       (1000) users      (984)     1302 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_static/custom.css
+-rw-r--r--   0 tom       (1000) users      (984)    10766 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/doctools.js
+-rw-r--r--   0 tom       (1000) users      (984)      422 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/_static/documentation_options.js
+-rw-r--r--   0 tom       (1000) users      (984)   268286 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_static/favicon.ico
+-rw-r--r--   0 tom       (1000) users      (984)      286 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/file.png
+-rw-r--r--   0 tom       (1000) users      (984)    15594 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_static/joblib_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    27703 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_build/html/_static/joblib_logo_examples.png
+-rw-r--r--   0 tom       (1000) users      (984)   287630 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 tom       (1000) users      (984)    89476 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/jquery.js
+-rw-r--r--   0 tom       (1000) users      (984)     6936 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/jupyterlite_badge_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    10854 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/_static/language_data.js
+-rw-r--r--   0 tom       (1000) users      (984)       90 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/minus.png
+-rw-r--r--   0 tom       (1000) users      (984)     4315 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/no_image.png
+-rw-r--r--   0 tom       (1000) users      (984)       90 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/plus.png
+-rw-r--r--   0 tom       (1000) users      (984)     4929 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/_static/pygments.css
+-rw-r--r--   0 tom       (1000) users      (984)    16634 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/searchtools.js
+-rw-r--r--   0 tom       (1000) users      (984)      167 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/sg_gallery-binder.css
+-rw-r--r--   0 tom       (1000) users      (984)     1137 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/sg_gallery-dataframe.css
+-rw-r--r--   0 tom       (1000) users      (984)     4330 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/sg_gallery-rendered-html.css
+-rw-r--r--   0 tom       (1000) users      (984)     9530 2023-04-18 19:56:48.000000 joblib-1.4.2/doc/_build/html/_static/sg_gallery.css
+-rw-r--r--   0 tom       (1000) users      (984)    68420 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 tom       (1000) users      (984)    19530 2023-09-05 22:32:59.000000 joblib-1.4.2/doc/_build/html/_static/underscore.js
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.733951 joblib-1.4.2/doc/_build/html/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    61440 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/compressors_comparison.html
+-rw-r--r--   0 tom       (1000) users      (984)    11116 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/index.html
+-rw-r--r--   0 tom       (1000) users      (984)    38535 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/memory_basic_usage.html
+-rw-r--r--   0 tom       (1000) users      (984)    35688 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/nested_parallel_memory.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.733951 joblib-1.4.2/doc/_build/html/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)    14623 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html
+-rw-r--r--   0 tom       (1000) users      (984)     6185 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/parallel/index.html
+-rw-r--r--   0 tom       (1000) users      (984)     5698 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/parallel/sg_execution_times.html
+-rw-r--r--   0 tom       (1000) users      (984)    41580 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/parallel_generator.html
+-rw-r--r--   0 tom       (1000) users      (984)    44464 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/parallel_memmap.html
+-rw-r--r--   0 tom       (1000) users      (984)    36621 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/parallel_random_state.html
+-rw-r--r--   0 tom       (1000) users      (984)    33549 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/serialization_and_wrappers.html
+-rw-r--r--   0 tom       (1000) users      (984)     7794 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/auto_examples/sg_execution_times.html
+-rw-r--r--   0 tom       (1000) users      (984)    86206 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/developing.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.737284 joblib-1.4.2/doc/_build/html/generated/
+-rw-r--r--   0 tom       (1000) users      (984)    18604 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.Memory.html
+-rw-r--r--   0 tom       (1000) users      (984)    31096 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.Parallel.html
+-rw-r--r--   0 tom       (1000) users      (984)    10213 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.dump.html
+-rw-r--r--   0 tom       (1000) users      (984)     6452 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.hash.html
+-rw-r--r--   0 tom       (1000) users      (984)     9144 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.load.html
+-rw-r--r--   0 tom       (1000) users      (984)    14807 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.parallel_backend.html
+-rw-r--r--   0 tom       (1000) users      (984)    19630 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.parallel_config.html
+-rw-r--r--   0 tom       (1000) users      (984)     6327 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/generated/joblib.register_compressor.html
+-rw-r--r--   0 tom       (1000) users      (984)    10542 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/genindex.html
+-rw-r--r--   0 tom       (1000) users      (984)    23348 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/index.html
+-rw-r--r--   0 tom       (1000) users      (984)     9384 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/installing.html
+-rw-r--r--   0 tom       (1000) users      (984)    78141 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/memory.html
+-rw-r--r--   0 tom       (1000) users      (984)     1805 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/objects.inv
+-rw-r--r--   0 tom       (1000) users      (984)   110008 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/parallel.html
+-rw-r--r--   0 tom       (1000) users      (984)    21579 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/parallel_numpy.html
+-rw-r--r--   0 tom       (1000) users      (984)    30768 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/persistence.html
+-rw-r--r--   0 tom       (1000) users      (984)     4958 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/py-modindex.html
+-rw-r--r--   0 tom       (1000) users      (984)     5197 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/search.html
+-rw-r--r--   0 tom       (1000) users      (984)    49550 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/searchindex.js
+-rw-r--r--   0 tom       (1000) users      (984)     7853 2024-04-08 06:50:49.000000 joblib-1.4.2/doc/_build/html/why.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.737284 joblib-1.4.2/doc/_static/
+-rw-r--r--   0 tom       (1000) users      (984)     1302 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/_static/custom.css
+-rw-r--r--   0 tom       (1000) users      (984)   268286 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_static/favicon.ico
+-rw-r--r--   0 tom       (1000) users      (984)    15594 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_static/joblib_logo.svg
+-rw-r--r--   0 tom       (1000) users      (984)    27703 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_static/joblib_logo_examples.png
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.737284 joblib-1.4.2/doc/_templates/
+-rw-r--r--   0 tom       (1000) users      (984)      208 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/_templates/class.rst
+-rw-r--r--   0 tom       (1000) users      (984)      226 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/_templates/function.rst
+-rw-r--r--   0 tom       (1000) users      (984)      480 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/_templates/layout.html
+-rw-r--r--   0 tom       (1000) users      (984)      323 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/_templates/navigation.html
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.747284 joblib-1.4.2/doc/auto_examples/
+-rw-r--r--   0 tom       (1000) users      (984)    68782 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/auto_examples_jupyter.zip
+-rw-r--r--   0 tom       (1000) users      (984)    48989 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/auto_examples_python.zip
+-rw-r--r--   0 tom       (1000) users      (984)    13465 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/compressors_comparison.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     9044 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/auto_examples/compressors_comparison.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/compressors_comparison.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)    13175 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/compressors_comparison.rst
+-rw-r--r--   0 tom       (1000) users      (984)     3434 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/compressors_comparison_codeobj.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.747284 joblib-1.4.2/doc/auto_examples/images/
+-rw-r--r--   0 tom       (1000) users      (984)    14175 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png
+-rw-r--r--   0 tom       (1000) users      (984)     7869 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png
+-rw-r--r--   0 tom       (1000) users      (984)    20475 2024-04-08 06:47:41.000000 joblib-1.4.2/doc/auto_examples/images/sphx_glr_parallel_generator_001.png
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.747284 joblib-1.4.2/doc/auto_examples/images/thumb/
+-rw-r--r--   0 tom       (1000) users      (984)    13475 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    14279 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)     4940 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/index.rst
+-rw-r--r--   0 tom       (1000) users      (984)     6406 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/auto_examples/memory_basic_usage.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     4695 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/auto_examples/memory_basic_usage.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/auto_examples/memory_basic_usage.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     7558 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/auto_examples/memory_basic_usage.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2516 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/auto_examples/memory_basic_usage_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     7302 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/auto_examples/nested_parallel_memory.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     5092 2024-04-08 06:43:09.000000 joblib-1.4.2/doc/auto_examples/nested_parallel_memory.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/auto_examples/nested_parallel_memory.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     7412 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/auto_examples/nested_parallel_memory.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2729 2024-04-08 06:43:21.000000 joblib-1.4.2/doc/auto_examples/nested_parallel_memory_codeobj.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.747284 joblib-1.4.2/doc/auto_examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)     2943 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     1984 2024-04-08 06:45:46.000000 joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     4448 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2457 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.690617 joblib-1.4.2/doc/auto_examples/parallel/images/
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.747284 joblib-1.4.2/doc/auto_examples/parallel/images/thumb/
+-rw-r--r--   0 tom       (1000) users      (984)    16874 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png
+-rw-r--r--   0 tom       (1000) users      (984)      789 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/index.rst
+-rw-r--r--   0 tom       (1000) users      (984)      569 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/auto_examples/parallel/sg_execution_times.rst
+-rw-r--r--   0 tom       (1000) users      (984)    13695 2024-04-08 06:45:46.000000 joblib-1.4.2/doc/auto_examples/parallel_generator.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)    11044 2024-04-08 06:45:12.000000 joblib-1.4.2/doc/auto_examples/parallel_generator.py
+-rw-r--r--   0 tom       (1000) users      (984)    12861 2024-04-08 06:48:35.000000 joblib-1.4.2/doc/auto_examples/parallel_generator.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1263 2024-04-08 06:50:48.000000 joblib-1.4.2/doc/auto_examples/parallel_generator_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     8458 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/auto_examples/parallel_memmap.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     5588 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/parallel_memmap.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/auto_examples/parallel_memmap.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)    10852 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/auto_examples/parallel_memmap.rst
+-rw-r--r--   0 tom       (1000) users      (984)     2644 2024-04-08 06:43:40.000000 joblib-1.4.2/doc/auto_examples/parallel_memmap_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     7520 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/parallel_random_state.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     4787 2024-04-08 06:43:36.000000 joblib-1.4.2/doc/auto_examples/parallel_random_state.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/parallel_random_state.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)     8467 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/parallel_random_state.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1503 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/parallel_random_state_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-08 06:48:37.000000 joblib-1.4.2/doc/auto_examples/searchindex.bak
+-rw-r--r--   0 tom       (1000) users      (984)    73632 2024-04-08 06:48:37.000000 joblib-1.4.2/doc/auto_examples/searchindex.dat
+-rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-08 06:48:37.000000 joblib-1.4.2/doc/auto_examples/searchindex.dir
+-rw-r--r--   0 tom       (1000) users      (984)     7913 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.ipynb
+-rw-r--r--   0 tom       (1000) users      (984)     5723 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.py
+-rw-r--r--   0 tom       (1000) users      (984)       32 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.py.md5
+-rw-r--r--   0 tom       (1000) users      (984)    10133 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1619 2024-04-08 06:43:37.000000 joblib-1.4.2/doc/auto_examples/serialization_and_wrappers_codeobj.pickle
+-rw-r--r--   0 tom       (1000) users      (984)     1976 2024-04-08 06:47:55.000000 joblib-1.4.2/doc/auto_examples/sg_execution_times.rst
+-rw-r--r--   0 tom       (1000) users      (984)     7882 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/conf.py
+-rw-r--r--   0 tom       (1000) users      (984)      624 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/conftest.py
+-rw-r--r--   0 tom       (1000) users      (984)       97 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/developing.rst
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.760617 joblib-1.4.2/doc/generated/
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.Logger.cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.Logger.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)      706 2024-04-08 06:47:55.000000 joblib-1.4.2/doc/generated/joblib.Logger.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1235 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.MemorizedFunc.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Memory.__init__.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.Memory.cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1233 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.Memory.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Memory.eval.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1221 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.Memory.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Memory.format.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Memory.reduce_size.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.Memory.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Parallel.dispatch_next.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Parallel.dispatch_one_batch.examples
+-rw-r--r--   0 tom       (1000) users      (984)      710 2024-04-08 06:47:55.000000 joblib-1.4.2/doc/generated/joblib.Parallel.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Parallel.format.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.Parallel.print_progress.examples
+-rw-r--r--   0 tom       (1000) users      (984)      197 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.Parallel.rst
+-rw-r--r--   0 tom       (1000) users      (984)      708 2024-04-08 06:47:55.000000 joblib-1.4.2/doc/generated/joblib.delayed.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1210 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.dump.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.dump.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.expires_after.examples
+-rw-r--r--   0 tom       (1000) users      (984)      763 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.externals.loky.set_loky_pickler.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.hash.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.hash.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1210 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.load.examples
+-rw-r--r--   0 tom       (1000) users      (984)      187 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.load.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1247 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.logger.Logger.cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1247 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.logger.Logger.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.memory.MemorizedFunc.__init__.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.memory.MemorizedFunc.call.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.memory.MemorizedFunc.check_call_in_cache.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.memory.MemorizedFunc.clear.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1249 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.memory.MemorizedFunc.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.parallel.AutoBatchingMixin.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.parallel.ParallelBackendBase.examples
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.parallel_backend.examples
+-rw-r--r--   0 tom       (1000) users      (984)      239 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.parallel_backend.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1295 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.parallel_config.examples
+-rw-r--r--   0 tom       (1000) users      (984)      234 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.parallel_config.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.register_compressor.examples
+-rw-r--r--   0 tom       (1000) users      (984)      247 2024-04-08 06:43:01.000000 joblib-1.4.2/doc/generated/joblib.register_compressor.rst
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 06:45:49.000000 joblib-1.4.2/doc/generated/joblib.register_parallel_backend.examples
+-rw-r--r--   0 tom       (1000) users      (984)      753 2024-04-08 06:45:48.000000 joblib-1.4.2/doc/generated/joblib.wrap_non_picklable_objects.examples
+-rw-r--r--   0 tom       (1000) users      (984)     1268 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/index.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1839 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/installing.rst
+-rw-r--r--   0 tom       (1000) users      (984)    17989 2024-04-08 12:29:30.000000 joblib-1.4.2/doc/memory.rst
+-rw-r--r--   0 tom       (1000) users      (984)    19092 2024-05-02 08:05:25.000000 joblib-1.4.2/doc/parallel.rst
+-rw-r--r--   0 tom       (1000) users      (984)     6328 2024-04-08 12:26:43.000000 joblib-1.4.2/doc/parallel_numpy.rst
+-rw-r--r--   0 tom       (1000) users      (984)     7247 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/persistence.rst
+-rw-r--r--   0 tom       (1000) users      (984)     1680 2024-04-03 09:55:41.000000 joblib-1.4.2/doc/why.rst
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.763951 joblib-1.4.2/examples/
+-rw-r--r--   0 tom       (1000) users      (984)      131 2024-04-03 09:55:41.000000 joblib-1.4.2/examples/README.txt
+-rw-r--r--   0 tom       (1000) users      (984)     9044 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/compressors_comparison.py
+-rw-r--r--   0 tom       (1000) users      (984)     4695 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/memory_basic_usage.py
+-rw-r--r--   0 tom       (1000) users      (984)     5092 2024-04-03 09:55:41.000000 joblib-1.4.2/examples/nested_parallel_memory.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.763951 joblib-1.4.2/examples/parallel/
+-rw-r--r--   0 tom       (1000) users      (984)      111 2024-04-03 09:55:41.000000 joblib-1.4.2/examples/parallel/README.txt
+-rw-r--r--   0 tom       (1000) users      (984)     1984 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/parallel/distributed_backend_simple.py
+-rw-r--r--   0 tom       (1000) users      (984)    11044 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/parallel_generator.py
+-rw-r--r--   0 tom       (1000) users      (984)     5588 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/parallel_memmap.py
+-rw-r--r--   0 tom       (1000) users      (984)     4787 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/parallel_random_state.py
+-rw-r--r--   0 tom       (1000) users      (984)     5723 2024-04-08 12:26:43.000000 joblib-1.4.2/examples/serialization_and_wrappers.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.767284 joblib-1.4.2/joblib/
+-rw-r--r--   0 tom       (1000) users      (984)     5132 2024-05-02 12:11:23.000000 joblib-1.4.2/joblib/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)      417 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/_cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)    13313 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/_dask.py
+-rw-r--r--   0 tom       (1000) users      (984)    28092 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/_memmapping_reducer.py
+-rw-r--r--   0 tom       (1000) users      (984)     1925 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/_multiprocessing_helpers.py
+-rw-r--r--   0 tom       (1000) users      (984)    25489 2024-04-08 12:29:20.000000 joblib-1.4.2/joblib/_parallel_backends.py
+-rw-r--r--   0 tom       (1000) users      (984)    16683 2024-04-08 12:29:25.000000 joblib-1.4.2/joblib/_store_backends.py
+-rw-r--r--   0 tom       (1000) users      (984)     2076 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)     5361 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/backports.py
+-rw-r--r--   0 tom       (1000) users      (984)    19768 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/compressor.py
+-rw-r--r--   0 tom       (1000) users      (984)     4389 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/disk.py
+-rw-r--r--   0 tom       (1000) users      (984)     5136 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/executor.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.770617 joblib-1.4.2/joblib/externals/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/externals/__init__.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.770617 joblib-1.4.2/joblib/externals/cloudpickle/
+-rw-r--r--   0 tom       (1000) users      (984)      308 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/cloudpickle/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)    55283 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/cloudpickle/cloudpickle.py
+-rw-r--r--   0 tom       (1000) users      (984)      322 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/cloudpickle/cloudpickle_fast.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.770617 joblib-1.4.2/joblib/externals/loky/
+-rw-r--r--   0 tom       (1000) users      (984)     1104 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     1057 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/_base.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.773951 joblib-1.4.2/joblib/externals/loky/backend/
+-rw-r--r--   0 tom       (1000) users      (984)      312 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     1776 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/_posix_reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)      683 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/_win_reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)    13654 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/context.py
+-rw-r--r--   0 tom       (1000) users      (984)     1186 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/fork_exec.py
+-rw-r--r--   0 tom       (1000) users      (984)     5580 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/popen_loky_posix.py
+-rw-r--r--   0 tom       (1000) users      (984)     5325 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/popen_loky_win32.py
+-rw-r--r--   0 tom       (1000) users      (984)     2018 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/process.py
+-rw-r--r--   0 tom       (1000) users      (984)     7322 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/queues.py
+-rw-r--r--   0 tom       (1000) users      (984)     7063 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)    14498 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/resource_tracker.py
+-rw-r--r--   0 tom       (1000) users      (984)     8962 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/spawn.py
+-rw-r--r--   0 tom       (1000) users      (984)    11768 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/synchronize.py
+-rw-r--r--   0 tom       (1000) users      (984)     5757 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/backend/utils.py
+-rw-r--r--   0 tom       (1000) users      (984)     3608 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)     2567 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/initializers.py
+-rw-r--r--   0 tom       (1000) users      (984)    51048 2024-04-09 07:53:52.000000 joblib-1.4.2/joblib/externals/loky/process_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)    10305 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/loky/reusable_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)      671 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/externals/vendor_cloudpickle.sh
+-rwxr-xr-x   0 tom       (1000) users      (984)      965 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/externals/vendor_loky.sh
+-rw-r--r--   0 tom       (1000) users      (984)    14204 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/func_inspect.py
+-rw-r--r--   0 tom       (1000) users      (984)    10535 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/hashing.py
+-rw-r--r--   0 tom       (1000) users      (984)     5463 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/logger.py
+-rw-r--r--   0 tom       (1000) users      (984)    46539 2024-05-02 12:11:23.000000 joblib-1.4.2/joblib/memory.py
+-rw-r--r--   0 tom       (1000) users      (984)    26886 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/numpy_pickle.py
+-rw-r--r--   0 tom       (1000) users      (984)     8547 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/numpy_pickle_compat.py
+-rw-r--r--   0 tom       (1000) users      (984)     8723 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/numpy_pickle_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)    84583 2024-04-15 15:26:47.000000 joblib-1.4.2/joblib/parallel.py
+-rw-r--r--   0 tom       (1000) users      (984)    14415 2024-04-09 07:53:33.000000 joblib-1.4.2/joblib/pool.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.780617 joblib-1.4.2/joblib/test/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/__init__.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.780617 joblib-1.4.2/joblib/test/_openmp_test_helper/
+-rw-r--r--   0 tom       (1000) users      (984)       16 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/_openmp_test_helper/.gitignore
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/_openmp_test_helper/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)      390 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/_openmp_test_helper/parallel_sum.pyx
+-rw-r--r--   0 tom       (1000) users      (984)      749 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/_openmp_test_helper/setup.py
+-rw-r--r--   0 tom       (1000) users      (984)     2336 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/common.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.793951 joblib-1.4.2/joblib/test/data/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     3460 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/data/create_numpy_pickle.py
+-rwxr-xr-x   0 tom       (1000) users      (984)      514 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/generate_data.sh
+-rw-r--r--   0 tom       (1000) users      (984)      769 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz
+-rw-r--r--   0 tom       (1000) users      (984)      757 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz
+-rw-r--r--   0 tom       (1000) users      (984)      792 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz
+-rw-r--r--   0 tom       (1000) users      (984)      794 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      790 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      986 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      997 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      798 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      660 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      712 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl
+-rw-r--r--   0 tom       (1000) users      (984)     1000 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      831 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      694 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)     1021 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      831 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      697 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)     1005 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      833 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      701 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)      800 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz
+-rw-r--r--   0 tom       (1000) users      (984)     1068 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      991 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2
+-rw-r--r--   0 tom       (1000) users      (984)      800 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip
+-rw-r--r--   0 tom       (1000) users      (984)      715 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma
+-rw-r--r--   0 tom       (1000) users      (984)      752 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz
+-rw-r--r--   0 tom       (1000) users      (984)      849 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.12.2_pickle_py36_np114.pkl.lz4
+-rw-r--r--   0 tom       (1000) users      (984)      659 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz
+-rw-r--r--   0 tom       (1000) users      (984)      658 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz
+-rw-r--r--   0 tom       (1000) users      (984)      658 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz
+-rw-r--r--   0 tom       (1000) users      (984)      673 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      673 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)      670 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      670 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      236 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      691 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      307 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      691 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      307 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      691 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_01.npy
+-rw-r--r--   0 tom       (1000) users      (984)      120 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_02.npy
+-rw-r--r--   0 tom       (1000) users      (984)      307 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_03.npy
+-rw-r--r--   0 tom       (1000) users      (984)      104 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl_04.npy
+-rw-r--r--   0 tom       (1000) users      (984)      802 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz
+-rw-r--r--   0 tom       (1000) users      (984)       43 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_01.npy.z
+-rw-r--r--   0 tom       (1000) users      (984)       43 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_02.npy.z
+-rw-r--r--   0 tom       (1000) users      (984)       37 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz_03.npy.z
+-rw-r--r--   0 tom       (1000) users      (984)     1175 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/test_backports.py
+-rw-r--r--   0 tom       (1000) users      (984)      751 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)     5284 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_config.py
+-rw-r--r--   0 tom       (1000) users      (984)    18418 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_dask.py
+-rw-r--r--   0 tom       (1000) users      (984)     2205 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/test_disk.py
+-rw-r--r--   0 tom       (1000) users      (984)     9488 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_func_inspect.py
+-rw-r--r--   0 tom       (1000) users      (984)      145 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_func_inspect_special_encoding.py
+-rw-r--r--   0 tom       (1000) users      (984)    16054 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_hashing.py
+-rw-r--r--   0 tom       (1000) users      (984)      422 2024-04-03 09:55:41.000000 joblib-1.4.2/joblib/test/test_init.py
+-rw-r--r--   0 tom       (1000) users      (984)      984 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_logger.py
+-rw-r--r--   0 tom       (1000) users      (984)    43298 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_memmapping.py
+-rw-r--r--   0 tom       (1000) users      (984)    50353 2024-05-02 12:11:23.000000 joblib-1.4.2/joblib/test/test_memory.py
+-rw-r--r--   0 tom       (1000) users      (984)     5347 2024-05-02 08:05:25.000000 joblib-1.4.2/joblib/test/test_memory_async.py
+-rw-r--r--   0 tom       (1000) users      (984)     1123 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_missing_multiprocessing.py
+-rw-r--r--   0 tom       (1000) users      (984)     1936 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_module.py
+-rw-r--r--   0 tom       (1000) users      (984)    42485 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_numpy_pickle.py
+-rw-r--r--   0 tom       (1000) users      (984)      609 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_numpy_pickle_compat.py
+-rw-r--r--   0 tom       (1000) users      (984)      383 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_numpy_pickle_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)    74168 2024-04-09 10:38:57.000000 joblib-1.4.2/joblib/test/test_parallel.py
+-rw-r--r--   0 tom       (1000) users      (984)     3121 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_store_backends.py
+-rw-r--r--   0 tom       (1000) users      (984)     2570 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_testing.py
+-rw-r--r--   0 tom       (1000) users      (984)      584 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/test_utils.py
+-rw-r--r--   0 tom       (1000) users      (984)      251 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/test/testutils.py
+-rw-r--r--   0 tom       (1000) users      (984)     3093 2024-04-08 12:26:43.000000 joblib-1.4.2/joblib/testing.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2024-05-02 12:12:05.770617 joblib-1.4.2/joblib.egg-info/
+-rw-r--r--   0 tom       (1000) users      (984)     5364 2024-05-02 12:12:05.000000 joblib-1.4.2/joblib.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (984)    21285 2024-05-02 12:12:05.000000 joblib-1.4.2/joblib.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) users      (984)        1 2024-05-02 12:12:05.000000 joblib-1.4.2/joblib.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) users      (984)        7 2024-05-02 12:12:05.000000 joblib-1.4.2/joblib.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) users      (984)     2390 2024-04-08 12:26:43.000000 joblib-1.4.2/pyproject.toml
+-rw-r--r--   0 tom       (1000) users      (984)      172 2024-05-02 12:12:05.793951 joblib-1.4.2/setup.cfg
+-rwxr-xr-x   0 tom       (1000) users      (984)       92 2024-04-08 12:26:43.000000 joblib-1.4.2/setup.py
```

### Comparing `joblib-1.4.0/.gitignore` & `joblib-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/CHANGES.rst` & `joblib-1.4.2/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 Latest changes
 ==============
 
+Release 1.4.2 -- 2024/05/02
+---------------------------
+
+Due to maintenance issues, 1.4.1 was not valid and we bumped the version to 1.4.2
+
+
+- Fix a backward incompatible change in ``MemorizedFunc.call`` which needs to
+  return the metadata. Also make sure that ``NotMemorizedFunc.call`` return
+  an empty dict for metadata for consistency.
+  https://github.com/joblib/joblib/pull/1576
+
+
 Release 1.4.0 -- 2024/04/08
 ---------------------------
 
 - Allow caching co-routines with `Memory.cache`.
   https://github.com/joblib/joblib/pull/894
-  
+
 - Try to cast ``n_jobs`` to int in parallel and raise an error if
   it fails. This means that ``n_jobs=2.3`` will now result in
   ``effective_n_jobs=2`` instead of failing.
   https://github.com/joblib/joblib/pull/1539
-  
+
 - Ensure that errors in the task generator given to Parallel's call
   are raised in the results consumming thread.
   https://github.com/joblib/joblib/pull/1491
 
 - Adjust codebase to NumPy 2.0 by changing ``np.NaN`` to ``np.nan``
   and importing ``byte_bounds`` from ``np.lib.array_utils``.
   https://github.com/joblib/joblib/pull/1501
@@ -24,15 +36,15 @@
   ``generator_unordered``. In this case the results will be returned in the
   order of task completion rather than the order of submission.
   https://github.com/joblib/joblib/pull/1463
 
 - dask backend now supports ``return_as=generator`` and
   ``return_as=generator_unordered``.
   https://github.com/joblib/joblib/pull/1520
-  
+
 - Vendor cloudpickle 3.0.0 and end support for Python 3.7 which has
   reached end of life.
   https://github.com/joblib/joblib/pull/1487
   https://github.com/joblib/joblib/pull/1515
 
 Release 1.3.2 -- 2023/08/08
 ---------------------------
@@ -74,15 +86,15 @@
 - Fix temporary folder creation in `joblib.Parallel` on Linux subsystems on Windows
   which do have `/dev/shm` but don't have the `os.statvfs` function
   https://github.com/joblib/joblib/issues/1353
 
 - Drop runtime dependency on ``distutils``. ``distutils`` is going away
   in Python 3.12 and is deprecated from Python 3.10 onwards. This import
   was kept around to avoid breaking scikit-learn, however it's now been
-  long enough since scikit-learn deployed a fixed (verion 1.1 was released
+  long enough since scikit-learn deployed a fixed (version 1.1 was released
   in May 2022) that it should be safe to remove this.
   https://github.com/joblib/joblib/pull/1361
 
 - A warning is raised when a pickling error occurs during caching operations.
   In version 1.5, this warning will be turned into an error. For all other
   errors, a new warning has been introduced: ``joblib.memory.CacheWarning``.
   https://github.com/joblib/joblib/pull/1359
```

### Comparing `joblib-1.4.0/LICENSE.txt` & `joblib-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/PKG-INFO` & `joblib-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joblib
-Version: 1.4.0
+Version: 1.4.2
 Summary: Lightweight pipelining with Python functions
 Author-email: Gael Varoquaux <gael.varoquaux@normalesup.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://joblib.readthedocs.io
 Project-URL: Source, https://github.com/joblib/joblib
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,23 +29,23 @@
 
 |PyPi| |Azure| |ReadTheDocs| |Codecov| 
 
 .. |PyPi| image:: https://badge.fury.io/py/joblib.svg
    :target: https://badge.fury.io/py/joblib
    :alt: Joblib version
 
-.. |Azure| image:: https://dev.azure.com/joblib/joblib/_apis/build/status/joblib.joblib?branchName=master
+.. |Azure| image:: https://dev.azure.com/joblib/joblib/_apis/build/status/joblib.joblib?branchName=main
    :target: https://dev.azure.com/joblib/joblib/_build?definitionId=3&_a=summary&branchFilter=40
    :alt: Azure CI status
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/joblib/badge/?version=latest
     :target: https://joblib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |Codecov| image:: https://codecov.io/gh/joblib/joblib/branch/master/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/joblib/joblib/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/joblib/joblib
    :alt: Codecov coverage
 
 
 The homepage of joblib with user documentation is located on:
 
 https://joblib.readthedocs.io
@@ -54,15 +54,15 @@
 =======================
 
 To get the latest code using git, simply type::
 
     git clone https://github.com/joblib/joblib.git
 
 If you don't have git installed, you can download a zip
-of the latest code: https://github.com/joblib/joblib/archive/refs/heads/master.zip
+of the latest code: https://github.com/joblib/joblib/archive/refs/heads/main.zip
 
 Installing
 ==========
 
 You can use `pip` to install joblib::
 
     pip install joblib
```

### Comparing `joblib-1.4.0/README.rst` & `joblib-1.4.2/doc/README.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/TODO.rst` & `joblib-1.4.2/TODO.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/azure-pipelines.yml` & `joblib-1.4.2/azure-pipelines.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # https://docs.microsoft.com/azure/devops/pipelines/languages/python
 
 schedules:
 - cron: "0 9 * * *"
   displayName: Daily build
   branches:
     include:
-    - master
+    - main
 
 trigger:
-- master
+- main
 
 jobs:
 - job: linting
   displayName: Linting
   pool:
     vmImage: ubuntu-latest
   steps:
```

### Comparing `joblib-1.4.0/benchmarks/bench_auto_batching.py` & `joblib-1.4.2/benchmarks/bench_auto_batching.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/benchmarks/bench_compression.py` & `joblib-1.4.2/benchmarks/bench_compression.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/benchmarks/bench_grid_search_scaling.py` & `joblib-1.4.2/benchmarks/bench_grid_search_scaling.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/benchmarks/bench_pickle.py` & `joblib-1.4.2/benchmarks/bench_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/benchmarks/bench_sequential_fast_tasks.py` & `joblib-1.4.2/benchmarks/bench_sequential_fast_tasks.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/conftest.py` & `joblib-1.4.2/conftest.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import faulthandler
 
 import pytest
 from _pytest.doctest import DoctestItem
 
 from joblib.parallel import mp
 from joblib.backports import LooseVersion
+from joblib import Memory
 try:
     import lz4
 except ImportError:
     lz4 = None
 try:
     from distributed.utils_test import loop, loop_in_thread
 except ImportError:
@@ -80,7 +81,15 @@
     # should be disabled. Note that we cancel the global dump_traceback_later
     # to waiting for too long.
     faulthandler.cancel_dump_traceback_later()
 
     # Note that we also use a shorter timeout for the per-test callback
     # configured via the pytest-timeout extension.
     faulthandler.dump_traceback_later(60, exit=True)
+
+
+@pytest.fixture(scope='function')
+def memory(tmp_path):
+    "Fixture to get an independent and self-cleaning Memory"
+    mem = Memory(location=tmp_path, verbose=0)
+    yield mem
+    mem.clear()
```

### Comparing `joblib-1.4.0/continuous_integration/install.sh` & `joblib-1.4.2/continuous_integration/install.sh`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/continuous_integration/run_tests.sh` & `joblib-1.4.2/continuous_integration/run_tests.sh`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/CHANGES.rst` & `joblib-1.4.2/doc/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/Makefile` & `joblib-1.4.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/README.rst` & `joblib-1.4.2/doc/_build/html/_sources/README.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/CHANGES.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/CHANGES.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/README.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/compressors_comparison.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/index.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/index.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/memory_basic_usage.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/nested_parallel_memory.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/distributed_backend_simple.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/index.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel/sg_execution_times.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel_generator.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel_memmap.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/parallel_random_state.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/serialization_and_wrappers.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/auto_examples/sg_execution_times.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/developing.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/developing.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/environment.pickle` & `joblib-1.4.2/doc/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.Memory.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.Memory.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.Parallel.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.dump.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.dump.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.hash.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.hash.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.load.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.load.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.parallel_backend.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.parallel_backend.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.parallel_config.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/generated/joblib.register_compressor.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/index.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/installing.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/installing.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/memory.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/memory.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/parallel.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/parallel.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/parallel_numpy.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/parallel_numpy.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/persistence.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/persistence.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/.doctrees/why.doctree` & `joblib-1.4.2/doc/_build/html/.doctrees/why.doctree`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/CHANGES.html` & `joblib-1.4.2/doc/_build/html/CHANGES.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/README.html` & `joblib-1.4.2/doc/_build/html/README.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip` & `joblib-1.4.2/doc/_build/html/_downloads/07fcc19ba03226cd3d83d4e40ec44385/auto_examples_python.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py` & `joblib-1.4.2/doc/_build/html/_downloads/13c28a3486775ce7013bf819ce88d3d8/serialization_and_wrappers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py` & `joblib-1.4.2/doc/_build/html/_downloads/3fa10e137733c0c23e90dca9a693a9e7/parallel_generator.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py` & `joblib-1.4.2/doc/_build/html/_downloads/4ac6cfb8777b2242df320ff920ecbafd/compressors_comparison.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/58796f572e8ca7b503da779777847d75/nested_parallel_memory.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip` & `joblib-1.4.2/doc/_build/html/_downloads/6f1e7a639e0699d6164445b55e6c116d/auto_examples_jupyter.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/6f54ccb28e994a64c34b08c8f124a046/serialization_and_wrappers.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/715d8eefe44aa2b912e10d4c21fb08de/parallel_random_state.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/7be5f3fad7e3c26454929e6071a20924/memory_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py` & `joblib-1.4.2/doc/_build/html/_downloads/7dab825b78538857a35613f772624938/memory_basic_usage.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py` & `joblib-1.4.2/doc/_build/html/_downloads/857637eaee8f6564825e4c32dddf9581/distributed_backend_simple.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/a0562d33325f994d06f0e84c36489eb6/parallel_memmap.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py` & `joblib-1.4.2/doc/_build/html/_downloads/b808e89441bc95f4a6531c96f76aa6b5/nested_parallel_memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/db658a25107c199addf4f0b83d7dc5ac/parallel_generator.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py` & `joblib-1.4.2/doc/_build/html/_downloads/e41e7e8dec6d8bd0e6a8790b4e1f1e1e/parallel_random_state.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/eb580176dbb28422a2948502cec12406/compressors_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py` & `joblib-1.4.2/doc/_build/html/_downloads/eeebf825310c36181bb48faf49b207dd/parallel_memmap.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb` & `joblib-1.4.2/doc/_build/html/_downloads/fec4ba264e936c334617fdc79f61159e/distributed_backend_simple.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_compressors_comparison_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_compressors_comparison_002.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_compressors_comparison_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_distributed_backend_simple_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_memory_basic_usage_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_nested_parallel_memory_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_generator_001.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_generator_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_generator_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_memmap_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_parallel_random_state_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png` & `joblib-1.4.2/doc/_build/html/_images/sphx_glr_serialization_and_wrappers_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/CHANGES.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/CHANGES.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/README.rst.txt` & `joblib-1.4.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 |PyPi| |Azure| |ReadTheDocs| |Codecov| 
 
 .. |PyPi| image:: https://badge.fury.io/py/joblib.svg
    :target: https://badge.fury.io/py/joblib
    :alt: Joblib version
 
-.. |Azure| image:: https://dev.azure.com/joblib/joblib/_apis/build/status/joblib.joblib?branchName=master
+.. |Azure| image:: https://dev.azure.com/joblib/joblib/_apis/build/status/joblib.joblib?branchName=main
    :target: https://dev.azure.com/joblib/joblib/_build?definitionId=3&_a=summary&branchFilter=40
    :alt: Azure CI status
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/joblib/badge/?version=latest
     :target: https://joblib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |Codecov| image:: https://codecov.io/gh/joblib/joblib/branch/master/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/joblib/joblib/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/joblib/joblib
    :alt: Codecov coverage
 
 
 The homepage of joblib with user documentation is located on:
 
 https://joblib.readthedocs.io
@@ -25,15 +25,15 @@
 =======================
 
 To get the latest code using git, simply type::
 
     git clone https://github.com/joblib/joblib.git
 
 If you don't have git installed, you can download a zip
-of the latest code: https://github.com/joblib/joblib/archive/refs/heads/master.zip
+of the latest code: https://github.com/joblib/joblib/archive/refs/heads/main.zip
 
 Installing
 ==========
 
 You can use `pip` to install joblib::
 
     pip install joblib
```

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/compressors_comparison.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/index.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/index.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/memory_basic_usage.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/nested_parallel_memory.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/distributed_backend_simple.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/index.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel/sg_execution_times.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel_generator.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel_memmap.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/parallel_random_state.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/serialization_and_wrappers.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/auto_examples/sg_execution_times.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/index.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/installing.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/installing.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/memory.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/memory.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/parallel.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/parallel.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/parallel_numpy.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/parallel_numpy.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/persistence.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/persistence.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_sources/why.rst.txt` & `joblib-1.4.2/doc/_build/html/_sources/why.rst.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/alabaster.css` & `joblib-1.4.2/doc/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/basic.css` & `joblib-1.4.2/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/binder_badge_logo.svg` & `joblib-1.4.2/doc/_build/html/_static/binder_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/broken_example.png` & `joblib-1.4.2/doc/_build/html/_static/broken_example.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/custom.css` & `joblib-1.4.2/doc/_build/html/_static/custom.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/doctools.js` & `joblib-1.4.2/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/favicon.ico` & `joblib-1.4.2/doc/_build/html/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/joblib_logo.svg` & `joblib-1.4.2/doc/_build/html/_static/joblib_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/joblib_logo_examples.png` & `joblib-1.4.2/doc/_build/html/_static/joblib_logo_examples.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/jquery-3.5.1.js` & `joblib-1.4.2/doc/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/jquery.js` & `joblib-1.4.2/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/jupyterlite_badge_logo.svg` & `joblib-1.4.2/doc/_build/html/_static/jupyterlite_badge_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/language_data.js` & `joblib-1.4.2/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/no_image.png` & `joblib-1.4.2/doc/_build/html/_static/no_image.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/pygments.css` & `joblib-1.4.2/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/searchtools.js` & `joblib-1.4.2/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/sg_gallery-dataframe.css` & `joblib-1.4.2/doc/_build/html/_static/sg_gallery-dataframe.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/sg_gallery-rendered-html.css` & `joblib-1.4.2/doc/_build/html/_static/sg_gallery-rendered-html.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/sg_gallery.css` & `joblib-1.4.2/doc/_build/html/_static/sg_gallery.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/underscore-1.13.1.js` & `joblib-1.4.2/doc/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/_static/underscore.js` & `joblib-1.4.2/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/compressors_comparison.html` & `joblib-1.4.2/doc/_build/html/auto_examples/compressors_comparison.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/index.html` & `joblib-1.4.2/doc/_build/html/auto_examples/index.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/memory_basic_usage.html` & `joblib-1.4.2/doc/_build/html/auto_examples/memory_basic_usage.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/nested_parallel_memory.html` & `joblib-1.4.2/doc/_build/html/auto_examples/nested_parallel_memory.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html` & `joblib-1.4.2/doc/_build/html/auto_examples/parallel/distributed_backend_simple.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/parallel/index.html` & `joblib-1.4.2/doc/_build/html/auto_examples/parallel/index.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/parallel/sg_execution_times.html` & `joblib-1.4.2/doc/_build/html/auto_examples/parallel/sg_execution_times.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/parallel_generator.html` & `joblib-1.4.2/doc/_build/html/auto_examples/parallel_generator.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/parallel_memmap.html` & `joblib-1.4.2/doc/_build/html/auto_examples/parallel_memmap.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/parallel_random_state.html` & `joblib-1.4.2/doc/_build/html/auto_examples/parallel_random_state.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/serialization_and_wrappers.html` & `joblib-1.4.2/doc/_build/html/auto_examples/serialization_and_wrappers.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/auto_examples/sg_execution_times.html` & `joblib-1.4.2/doc/_build/html/auto_examples/sg_execution_times.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/developing.html` & `joblib-1.4.2/doc/_build/html/developing.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.Memory.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.Memory.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.Parallel.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.Parallel.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.dump.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.dump.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.hash.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.hash.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.load.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.load.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.parallel_backend.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.parallel_backend.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.parallel_config.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.parallel_config.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/generated/joblib.register_compressor.html` & `joblib-1.4.2/doc/_build/html/generated/joblib.register_compressor.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/genindex.html` & `joblib-1.4.2/doc/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/index.html` & `joblib-1.4.2/doc/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/installing.html` & `joblib-1.4.2/doc/_build/html/installing.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/memory.html` & `joblib-1.4.2/doc/_build/html/memory.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/objects.inv` & `joblib-1.4.2/doc/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/parallel.html` & `joblib-1.4.2/doc/_build/html/parallel.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/parallel_numpy.html` & `joblib-1.4.2/doc/_build/html/parallel_numpy.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/persistence.html` & `joblib-1.4.2/doc/_build/html/persistence.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/py-modindex.html` & `joblib-1.4.2/doc/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/search.html` & `joblib-1.4.2/doc/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/searchindex.js` & `joblib-1.4.2/doc/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_build/html/why.html` & `joblib-1.4.2/doc/_build/html/why.html`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_static/custom.css` & `joblib-1.4.2/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_static/favicon.ico` & `joblib-1.4.2/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_static/joblib_logo.svg` & `joblib-1.4.2/doc/_static/joblib_logo.svg`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/_static/joblib_logo_examples.png` & `joblib-1.4.2/doc/_static/joblib_logo_examples.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/auto_examples_jupyter.zip` & `joblib-1.4.2/doc/auto_examples/auto_examples_jupyter.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/auto_examples_python.zip` & `joblib-1.4.2/doc/auto_examples/auto_examples_python.zip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/compressors_comparison.ipynb` & `joblib-1.4.2/doc/auto_examples/compressors_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/compressors_comparison.py` & `joblib-1.4.2/doc/auto_examples/compressors_comparison.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/compressors_comparison.rst` & `joblib-1.4.2/doc/auto_examples/compressors_comparison.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/compressors_comparison_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/compressors_comparison_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png` & `joblib-1.4.2/doc/auto_examples/images/sphx_glr_compressors_comparison_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png` & `joblib-1.4.2/doc/auto_examples/images/sphx_glr_compressors_comparison_002.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/sphx_glr_parallel_generator_001.png` & `joblib-1.4.2/doc/auto_examples/images/sphx_glr_parallel_generator_001.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_compressors_comparison_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_memory_basic_usage_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_nested_parallel_memory_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_parallel_generator_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_parallel_memmap_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_parallel_random_state_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png` & `joblib-1.4.2/doc/auto_examples/images/thumb/sphx_glr_serialization_and_wrappers_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/index.rst` & `joblib-1.4.2/doc/auto_examples/index.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/memory_basic_usage.ipynb` & `joblib-1.4.2/doc/auto_examples/memory_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/memory_basic_usage.py` & `joblib-1.4.2/doc/auto_examples/memory_basic_usage.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/memory_basic_usage.rst` & `joblib-1.4.2/doc/auto_examples/memory_basic_usage.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/memory_basic_usage_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/memory_basic_usage_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/nested_parallel_memory.ipynb` & `joblib-1.4.2/doc/auto_examples/nested_parallel_memory.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/nested_parallel_memory.py` & `joblib-1.4.2/doc/auto_examples/nested_parallel_memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/nested_parallel_memory.rst` & `joblib-1.4.2/doc/auto_examples/nested_parallel_memory.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/nested_parallel_memory_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/nested_parallel_memory_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.ipynb` & `joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.py` & `joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple.rst` & `joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/parallel/distributed_backend_simple_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png` & `joblib-1.4.2/doc/auto_examples/parallel/images/thumb/sphx_glr_distributed_backend_simple_thumb.png`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/index.rst` & `joblib-1.4.2/doc/auto_examples/parallel/index.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel/sg_execution_times.rst` & `joblib-1.4.2/doc/auto_examples/parallel/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_generator.ipynb` & `joblib-1.4.2/doc/auto_examples/parallel_generator.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_generator.py` & `joblib-1.4.2/doc/auto_examples/parallel_generator.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_generator.rst` & `joblib-1.4.2/doc/auto_examples/parallel_generator.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_generator_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/parallel_generator_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_memmap.ipynb` & `joblib-1.4.2/doc/auto_examples/parallel_memmap.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_memmap.py` & `joblib-1.4.2/doc/auto_examples/parallel_memmap.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_memmap.rst` & `joblib-1.4.2/doc/auto_examples/parallel_memmap.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_memmap_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/parallel_memmap_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_random_state.ipynb` & `joblib-1.4.2/doc/auto_examples/parallel_random_state.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_random_state.py` & `joblib-1.4.2/doc/auto_examples/parallel_random_state.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_random_state.rst` & `joblib-1.4.2/doc/auto_examples/parallel_random_state.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/parallel_random_state_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/parallel_random_state_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/searchindex.dat` & `joblib-1.4.2/doc/auto_examples/searchindex.dat`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.ipynb` & `joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.ipynb`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.py` & `joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/serialization_and_wrappers.rst` & `joblib-1.4.2/doc/auto_examples/serialization_and_wrappers.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/serialization_and_wrappers_codeobj.pickle` & `joblib-1.4.2/doc/auto_examples/serialization_and_wrappers_codeobj.pickle`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/auto_examples/sg_execution_times.rst` & `joblib-1.4.2/doc/auto_examples/sg_execution_times.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/conf.py` & `joblib-1.4.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/conftest.py` & `joblib-1.4.2/doc/conftest.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Logger.cache.examples` & `joblib-1.4.2/doc/generated/joblib.Logger.cache.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Logger.clear.examples` & `joblib-1.4.2/doc/generated/joblib.Logger.clear.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Logger.examples` & `joblib-1.4.2/doc/generated/joblib.Logger.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.MemorizedFunc.examples` & `joblib-1.4.2/doc/generated/joblib.MemorizedFunc.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Memory.cache.examples` & `joblib-1.4.2/doc/generated/joblib.Memory.cache.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Memory.clear.examples` & `joblib-1.4.2/doc/generated/joblib.Memory.clear.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Memory.examples` & `joblib-1.4.2/doc/generated/joblib.Memory.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.Parallel.examples` & `joblib-1.4.2/doc/generated/joblib.Parallel.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.delayed.examples` & `joblib-1.4.2/doc/generated/joblib.delayed.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.dump.examples` & `joblib-1.4.2/doc/generated/joblib.dump.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.externals.loky.set_loky_pickler.examples` & `joblib-1.4.2/doc/generated/joblib.externals.loky.set_loky_pickler.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.load.examples` & `joblib-1.4.2/doc/generated/joblib.load.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.logger.Logger.cache.examples` & `joblib-1.4.2/doc/generated/joblib.logger.Logger.cache.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.logger.Logger.clear.examples` & `joblib-1.4.2/doc/generated/joblib.logger.Logger.clear.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.memory.MemorizedFunc.examples` & `joblib-1.4.2/doc/generated/joblib.memory.MemorizedFunc.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.parallel_config.examples` & `joblib-1.4.2/doc/generated/joblib.parallel_config.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/generated/joblib.wrap_non_picklable_objects.examples` & `joblib-1.4.2/doc/generated/joblib.wrap_non_picklable_objects.examples`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/index.rst` & `joblib-1.4.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/installing.rst` & `joblib-1.4.2/doc/installing.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/memory.rst` & `joblib-1.4.2/doc/memory.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/parallel.rst` & `joblib-1.4.2/doc/parallel.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 This generator enables reducing the memory footprint of
 :class:`joblib.Parallel` calls in case the results can benefit from on-the-fly
 aggregation, as illustrated in
 :ref:`sphx_glr_auto_examples_parallel_generator.py`.
 
 Future releases are planned to also support returning a generator that yields
 the results in the order of completion rather than the order of submission, by
-using ``return_as="unordered_generator"`` instead of ``return_as="generator"``.
+using ``return_as="generator_unordered"`` instead of ``return_as="generator"``.
 In this case the order of the outputs will depend on the concurrency of workers
 and will not be guaranteed to be deterministic, meaning the results can be
 yielded with a different order every time the code is executed.
 
 Thread-based parallelism vs process-based parallelism
 =====================================================
 
@@ -256,15 +256,15 @@
 registered with the :func:`joblib.register_parallel_backend` function by
 passing a name and a backend factory.
 
 The backend factory can be any callable that returns an instance of
 ``ParallelBackendBase``. Please refer to the `default backends source code`_ as
 a reference if you want to implement your own custom backend.
 
-.. _`default backends source code`: https://github.com/joblib/joblib/blob/master/joblib/_parallel_backends.py
+.. _`default backends source code`: https://github.com/joblib/joblib/blob/main/joblib/_parallel_backends.py
 
 Note that it is possible to register a backend class that has some mandatory
 constructor parameters such as the network address and connection credentials
 for a remote cluster computing service::
 
     class MyCustomBackend(ParallelBackendBase):
 
@@ -414,8 +414,8 @@
 
 .. autofunction:: joblib.wrap_non_picklable_objects
 
 .. autofunction:: joblib.register_parallel_backend
 
 .. autoclass:: joblib.parallel.ParallelBackendBase
 
-.. autoclass:: joblib.parallel.AutoBatchingMixin
+.. autoclass:: joblib.parallel.AutoBatchingMixin
```

### Comparing `joblib-1.4.0/doc/parallel_numpy.rst` & `joblib-1.4.2/doc/parallel_numpy.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/persistence.rst` & `joblib-1.4.2/doc/persistence.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/doc/why.rst` & `joblib-1.4.2/doc/why.rst`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/compressors_comparison.py` & `joblib-1.4.2/examples/compressors_comparison.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/memory_basic_usage.py` & `joblib-1.4.2/examples/memory_basic_usage.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/nested_parallel_memory.py` & `joblib-1.4.2/examples/nested_parallel_memory.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/parallel/distributed_backend_simple.py` & `joblib-1.4.2/examples/parallel/distributed_backend_simple.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/parallel_generator.py` & `joblib-1.4.2/examples/parallel_generator.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/parallel_memmap.py` & `joblib-1.4.2/examples/parallel_memmap.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/parallel_random_state.py` & `joblib-1.4.2/examples/parallel_random_state.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/examples/serialization_and_wrappers.py` & `joblib-1.4.2/examples/serialization_and_wrappers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/__init__.py` & `joblib-1.4.2/joblib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '1.4.0'
+__version__ = '1.4.2'
 
 
 import os
 
 from .memory import Memory
 from .memory import MemorizedResult
 from .memory import register_store_backend
```

### Comparing `joblib-1.4.0/joblib/_dask.py` & `joblib-1.4.2/joblib/_dask.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/_memmapping_reducer.py` & `joblib-1.4.2/joblib/_memmapping_reducer.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/_multiprocessing_helpers.py` & `joblib-1.4.2/joblib/_multiprocessing_helpers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/_parallel_backends.py` & `joblib-1.4.2/joblib/_parallel_backends.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/_store_backends.py` & `joblib-1.4.2/joblib/_store_backends.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/_utils.py` & `joblib-1.4.2/joblib/_utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/backports.py` & `joblib-1.4.2/joblib/backports.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/compressor.py` & `joblib-1.4.2/joblib/compressor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/disk.py` & `joblib-1.4.2/joblib/disk.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/executor.py` & `joblib-1.4.2/joblib/executor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/cloudpickle/cloudpickle.py` & `joblib-1.4.2/joblib/externals/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/__init__.py` & `joblib-1.4.2/joblib/externals/loky/__init__.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/_base.py` & `joblib-1.4.2/joblib/externals/loky/_base.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/_posix_reduction.py` & `joblib-1.4.2/joblib/externals/loky/backend/_posix_reduction.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/_win_reduction.py` & `joblib-1.4.2/joblib/externals/loky/backend/_win_reduction.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/context.py` & `joblib-1.4.2/joblib/externals/loky/backend/context.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/fork_exec.py` & `joblib-1.4.2/joblib/externals/loky/backend/fork_exec.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/popen_loky_posix.py` & `joblib-1.4.2/joblib/externals/loky/backend/popen_loky_posix.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/popen_loky_win32.py` & `joblib-1.4.2/joblib/externals/loky/backend/popen_loky_win32.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/process.py` & `joblib-1.4.2/joblib/externals/loky/backend/process.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/queues.py` & `joblib-1.4.2/joblib/externals/loky/backend/queues.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/reduction.py` & `joblib-1.4.2/joblib/externals/loky/backend/reduction.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/resource_tracker.py` & `joblib-1.4.2/joblib/externals/loky/backend/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/spawn.py` & `joblib-1.4.2/joblib/externals/loky/backend/spawn.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/synchronize.py` & `joblib-1.4.2/joblib/externals/loky/backend/synchronize.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/backend/utils.py` & `joblib-1.4.2/joblib/externals/loky/backend/utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/cloudpickle_wrapper.py` & `joblib-1.4.2/joblib/externals/loky/cloudpickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/initializers.py` & `joblib-1.4.2/joblib/externals/loky/initializers.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/loky/process_executor.py` & `joblib-1.4.2/joblib/externals/loky/process_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
                 # cycles.
                 mem_usage = _get_memory_usage(pid, force_gc=True)
                 _last_memory_leak_check = time()
                 if mem_usage - _process_reference_size < _MAX_MEMORY_LEAK_SIZE:
                     # The GC managed to free the memory: everything is fine.
                     continue
 
-                # The process is leaking memory: let the master process
+                # The process is leaking memory: let the main process
                 # know that we need to start a new worker.
                 mp.util.info("Memory leak detected: shutting down worker")
                 result_queue.put(pid)
                 with worker_exit_lock:
                     mp.util.debug("Exit due to memory leak")
                     return
         else:
```

### Comparing `joblib-1.4.0/joblib/externals/loky/reusable_executor.py` & `joblib-1.4.2/joblib/externals/loky/reusable_executor.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/vendor_cloudpickle.sh` & `joblib-1.4.2/joblib/externals/vendor_cloudpickle.sh`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/externals/vendor_loky.sh` & `joblib-1.4.2/joblib/externals/vendor_loky.sh`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/func_inspect.py` & `joblib-1.4.2/joblib/func_inspect.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/hashing.py` & `joblib-1.4.2/joblib/hashing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/logger.py` & `joblib-1.4.2/joblib/logger.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/memory.py` & `joblib-1.4.2/joblib/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         return '{0}(func={1})'.format(self.__class__.__name__, self.func)
 
     def clear(self, warn=True):
         # Argument "warn" is for compatibility with MemorizedFunc.clear
         pass
 
     def call(self, *args, **kwargs):
-        return self.func(*args, **kwargs)
+        return self.func(*args, **kwargs), {}
 
     def check_call_in_cache(self, *args, **kwargs):
         return False
 
 
 ###############################################################################
 # class `AsyncNotMemorizedFunc`
@@ -472,16 +472,17 @@
 
         shelving: bool
             True when called via the call_and_shelve function.
 
 
         Returns
         -------
-        Output of the wrapped function if shelving is false, or a
-        MemorizedResult reference to the value if shelving is true.
+        output: Output of the wrapped function if shelving is false, or a
+            MemorizedResult reference to the value if shelving is true.
+        metadata: dict containing the metadata associated with the call.
         """
         args_id = self._get_args_id(*args, **kwargs)
         call_id = (self.func_id, args_id)
         _, func_name = get_func_name(self.func)
         func_info = self.store_backend.get_cached_func_info([self.func_id])
         location = func_info['location']
 
@@ -502,35 +503,36 @@
             )
 
         # Compare the function code with the previous to see if the
         # function code has changed and check if the results are present in
         # the cache.
         if self._is_in_cache_and_valid(call_id):
             if shelving:
-                return self._get_memorized_result(call_id)
+                return self._get_memorized_result(call_id), {}
 
             try:
                 start_time = time.time()
                 output = self._load_item(call_id)
                 if self._verbose > 4:
                     self._print_duration(time.time() - start_time,
                                          context='cache loaded ')
-                return output
+                return output, {}
             except Exception:
                 # XXX: Should use an exception logger
                 _, signature = format_signature(self.func, *args, **kwargs)
                 self.warn('Exception while loading results for '
                           '{}\n {}'.format(signature, traceback.format_exc()))
 
         if self._verbose > 10:
             self.warn(
                 f"Computing func {func_name}, argument hash {args_id} "
                 f"in location {location}"
             )
 
+        # Returns the output but not the metadata
         return self._call(call_id, args, kwargs, shelving)
 
     @property
     def func_code_info(self):
         # 3-tuple property containing: the function source code, source file,
         # and first line of the code inside the source file
         if hasattr(self.func, '__code__'):
@@ -563,18 +565,20 @@
         Returns
         -------
         cached_result: MemorizedResult or NotMemorizedResult
             reference to the value returned by the wrapped function. The
             class "NotMemorizedResult" is used when there is no cache
             activated (e.g. location=None in Memory).
         """
-        return self._cached_call(args, kwargs, shelving=True)
+        # Return the wrapped output, without the metadata
+        return self._cached_call(args, kwargs, shelving=True)[0]
 
     def __call__(self, *args, **kwargs):
-        return self._cached_call(args, kwargs, shelving=False)
+        # Return the output, without the metadata
+        return self._cached_call(args, kwargs, shelving=False)[0]
 
     def __getstate__(self):
         # Make sure self.func's source is introspected prior to being pickled -
         # code introspection utilities typically do not work inside child
         # processes
         _ = self.func_code_info
 
@@ -748,19 +752,24 @@
         **kwargs: keyword arguments
             Keyword arguments.
 
         Returns
         -------
         output : object
             The output of the function call.
+        metadata : dict
+            The metadata associated with the call.
         """
         call_id = (self.func_id, self._get_args_id(*args, **kwargs))
+
+        # Return the output and the metadata
         return self._call(call_id, args, kwargs)
 
     def _call(self, call_id, args, kwargs, shelving=False):
+        # Return the output and the metadata
         self._before_call(args, kwargs)
         start_time = time.time()
         output = self.func(*args, **kwargs)
         return self._after_call(call_id, args, kwargs, shelving,
                                 output, start_time)
 
     def _before_call(self, args, kwargs):
@@ -770,21 +779,21 @@
     def _after_call(self, call_id, args, kwargs, shelving, output, start_time):
         self.store_backend.dump_item(call_id, output, verbose=self._verbose)
         duration = time.time() - start_time
         if self._verbose > 0:
             self._print_duration(duration)
         metadata = self._persist_input(duration, call_id, args, kwargs)
         if shelving:
-            return self._get_memorized_result(call_id, metadata)
+            return self._get_memorized_result(call_id, metadata), metadata
 
         if self.mmap_mode is not None:
             # Memmap the output at the first call to be consistent with
             # later calls
             output = self._load_item(call_id, metadata)
-        return output
+        return output, metadata
 
     def _persist_input(self, duration, call_id, args, kwargs,
                        this_duration_limit=0.5):
         """ Save a small summary of the call using json format in the
             output directory.
 
             output_dir: string
@@ -857,31 +866,34 @@
 
 
 ###############################################################################
 # class `AsyncMemorizedFunc`
 ###############################################################################
 class AsyncMemorizedFunc(MemorizedFunc):
     async def __call__(self, *args, **kwargs):
-        out = super().__call__(*args, **kwargs)
-        return await out if asyncio.iscoroutine(out) else out
+        out = self._cached_call(args, kwargs, shelving=False)
+        out = await out if asyncio.iscoroutine(out) else out
+        return out[0]  # Don't return metadata
 
     async def call_and_shelve(self, *args, **kwargs):
-        out = super().call_and_shelve(*args, **kwargs)
-        return await out if asyncio.iscoroutine(out) else out
+        out = self._cached_call(args, kwargs, shelving=True)
+        out = await out if asyncio.iscoroutine(out) else out
+        return out[0]  # Don't return metadata
 
     async def call(self, *args, **kwargs):
         out = super().call(*args, **kwargs)
         return await out if asyncio.iscoroutine(out) else out
 
     async def _call(self, call_id, args, kwargs, shelving=False):
         self._before_call(args, kwargs)
         start_time = time.time()
         output = await self.func(*args, **kwargs)
-        return self._after_call(call_id, args, kwargs, shelving,
-                                output, start_time)
+        return self._after_call(
+            call_id, args, kwargs, shelving, output, start_time
+        )
 
 
 ###############################################################################
 # class `Memory`
 ###############################################################################
 class Memory(Logger):
     """ A context object for caching a function's return value each time it
```

### Comparing `joblib-1.4.0/joblib/numpy_pickle.py` & `joblib-1.4.2/joblib/numpy_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/numpy_pickle_compat.py` & `joblib-1.4.2/joblib/numpy_pickle_compat.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/numpy_pickle_utils.py` & `joblib-1.4.2/joblib/numpy_pickle_utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/parallel.py` & `joblib-1.4.2/joblib/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 def _get_config_param(param, context_config, key):
     """Return the value of a parallel config parameter
 
     Explicitly setting it in Parallel has priority over setting in a
     parallel_(config/backend) context manager.
     """
     if param is not default_parallel_config[key]:
-        # param is explicitely set, return it
+        # param is explicitly set, return it
         return param
 
     if context_config[key] is not default_parallel_config[key]:
         # there's a context manager and the key is set, return it
         return context_config[key]
 
     # Otherwise, we are in the default_parallel_config,
@@ -182,28 +182,28 @@
 
     # Try to use the backend set by the user with the context manager.
 
     nesting_level = backend.nesting_level
     uses_threads = getattr(backend, 'uses_threads', False)
     supports_sharedmem = getattr(backend, 'supports_sharedmem', False)
     # Force to use thread-based backend if the provided backend does not
-    # match the shared memory constraint or if the backend is not explicitely
-    # given and threads are prefered.
+    # match the shared memory constraint or if the backend is not explicitly
+    # given and threads are preferred.
     force_threads = (require == 'sharedmem' and not supports_sharedmem)
     force_threads |= (
         not explicit_backend and prefer == 'threads' and not uses_threads
     )
     if force_threads:
         # This backend does not match the shared memory constraint:
         # fallback to the default thead-based backend.
         sharedmem_backend = BACKENDS[DEFAULT_THREAD_BACKEND](
             nesting_level=nesting_level
         )
         # Warn the user if we forced the backend to thread-based, while the
-        # user explicitely specified a non-thread-based backend.
+        # user explicitly specified a non-thread-based backend.
         if verbose >= 10 and explicit_backend:
             print(
                 f"Using {sharedmem_backend.__class__.__name__} as "
                 f"joblib backend instead of {backend.__class__.__name__} "
                 "as the latter does not provide shared memory semantics."
             )
         # Force to n_jobs=1 by default
@@ -1469,15 +1469,15 @@
                     islice = list(itertools.islice(iterator, big_batch_size))
                 except Exception as e:
                     # Handle the fact that the generator of task raised an
                     # exception. As this part of the code can be executed in
                     # a thread internal to the backend, register a task with
                     # an error that will be raised in the user's thread.
                     if isinstance(e.__context__, queue.Empty):
-                        # Supress the cause of the exception if it is
+                        # Suppress the cause of the exception if it is
                         # queue.Empty to avoid cluttered traceback. Only do it
                         # if the __context__ is really empty to avoid messing
                         # with causes of the original error.
                         e.__cause__ = None
                     batch_tracker = BatchCompletionCallBack(
                         0, batch_size, self
                     )
@@ -1713,18 +1713,18 @@
         while len(_remaining_outputs) > 0:
             batched_results = _remaining_outputs.popleft()
             batched_results = batched_results.get_result(self.timeout)
             for result in batched_results:
                 yield result
 
     def _wait_retrieval(self):
-        """Return True if we need to continue retriving some tasks."""
+        """Return True if we need to continue retrieving some tasks."""
 
         # If the input load is still being iterated over, it means that tasks
-        # are still on the dispatch wait list and their results will need to
+        # are still on the dispatch waitlist and their results will need to
         # be retrieved later on.
         if self._iterating:
             return True
 
         # If some of the dispatched tasks are still being processed by the
         # workers, wait for the compute to finish before starting retrieval
         if self.n_completed_tasks < self.n_dispatched_tasks:
@@ -1778,15 +1778,15 @@
         """If we are aborting, raise if a job caused an error."""
 
         # Find the first job whose status is TASK_ERROR if it exists.
         with self._lock:
             error_job = next((job for job in self._jobs
                               if job.status == TASK_ERROR), None)
 
-        # If this error job exists, immediatly raise the error by
+        # If this error job exists, immediately raise the error by
         # calling get_result. This job might not exists if abort has been
         # called directly or if the generator is gc'ed.
         if error_job is not None:
             error_job.get_result(self.timeout)
 
     def _warn_exit_early(self):
         """Warn the user if the generator is gc'ed before being consumned."""
@@ -1908,15 +1908,15 @@
         if not self._managed_backend:
             n_jobs = self._initialize_backend()
         else:
             n_jobs = self._effective_n_jobs()
 
         if n_jobs == 1:
             # If n_jobs==1, run the computation sequentially and return
-            # immediatly to avoid overheads.
+            # immediately to avoid overheads.
             output = self._get_sequential_output(iterable)
             next(output)
             return output if self.return_generator else list(output)
 
         # Let's create an ID that uniquely identifies the current call. If the
         # call is interrupted early and that the same instance is immediately
         # re-used, this id will be used to prevent workers that were
@@ -1930,15 +1930,15 @@
         self._cached_effective_n_jobs = n_jobs
 
         if isinstance(self._backend, LokyBackend):
             # For the loky backend, we add a callback executed when reducing
             # BatchCalls, that makes the loky executor use a temporary folder
             # specific to this Parallel object when pickling temporary memmaps.
             # This callback is necessary to ensure that several Parallel
-            # objects using the same resuable executor don't use the same
+            # objects using the same reusable executor don't use the same
             # temporary resources.
 
             def _batched_calls_reducer_callback():
                 # Relevant implementation detail: the following lines, called
                 # when reducing BatchedCalls, are called in a thread-safe
                 # situation, meaning that the context of the temporary folder
                 # manager will not be changed in between the callback execution
@@ -1996,15 +1996,15 @@
         self._pickle_cache = dict()
 
         output = self._get_outputs(iterator, pre_dispatch)
         self._call_ref = weakref.ref(output)
 
         # The first item from the output is blank, but it makes the interpreter
         # progress until it enters the Try/Except block of the generator and
-        # reach the first `yield` statement. This starts the aynchronous
+        # reaches the first `yield` statement. This starts the asynchronous
         # dispatch of the tasks to the workers.
         next(output)
 
         return output if self.return_generator else list(output)
 
     def __repr__(self):
         return '%s(n_jobs=%s)' % (self.__class__.__name__, self.n_jobs)
```

### Comparing `joblib-1.4.0/joblib/pool.py` & `joblib-1.4.2/joblib/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,19 +261,19 @@
         Threshold on the size of arrays passed to the workers that
         triggers automated memory mapping in temp_folder.
         Use None to disable memmapping of large arrays.
     mmap_mode: {'r+', 'r', 'w+', 'c'}
         Memmapping mode for numpy arrays passed to workers.
         See 'max_nbytes' parameter documentation for more details.
     forward_reducers: dictionary, optional
-        Reducers used to pickle objects passed from master to worker
+        Reducers used to pickle objects passed from main process to worker
         processes: see below.
     backward_reducers: dictionary, optional
         Reducers used to pickle return values from workers back to the
-        master process.
+        main process.
     verbose: int, optional
         Make it possible to monitor how the communication of numpy arrays
         with the subprocess is handled (pickling or memmapping)
     prewarm: bool or str, optional, "auto" by default.
         If True, force a read on newly memmapped array to make sure that OS
         pre-cache it in memory. This can be useful to avoid concurrent disk
         access when the same data array is passed to different worker
```

### Comparing `joblib-1.4.0/joblib/test/_openmp_test_helper/setup.py` & `joblib-1.4.2/joblib/test/_openmp_test_helper/setup.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/common.py` & `joblib-1.4.2/joblib/test/common.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/create_numpy_pickle.py` & `joblib-1.4.2/joblib/test/data/create_numpy_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/generate_data.sh` & `joblib-1.4.2/joblib/test/data/generate_data.sh`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np16.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py27_np17.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py33_np18.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py34_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_compressed_pickle_py35_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py27_np17.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py33_np18.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py34_np19.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz` & `joblib-1.4.2/joblib/test/data/joblib_0.10.0_pickle_py35_np19.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.11.0_compressed_pickle_py36_np111.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2` & `joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.bz2`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip` & `joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.gzip`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma` & `joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.lzma`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz` & `joblib-1.4.2/joblib/test/data/joblib_0.11.0_pickle_py36_np111.pkl.xz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.12.2_pickle_py36_np114.pkl.lz4` & `joblib-1.4.2/joblib/test/data/joblib_0.12.2_pickle_py36_np114.pkl.lz4`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.8.4_compressed_pickle_py27_np17.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np16.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py27_np17.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py34_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_compressed_pickle_py35_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np16.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py27_np17.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py33_np18.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py34_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl` & `joblib-1.4.2/joblib/test/data/joblib_0.9.2_pickle_py35_np19.pkl`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz` & `joblib-1.4.2/joblib/test/data/joblib_0.9.4.dev0_compressed_cache_size_pickle_py35_np19.gz`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_backports.py` & `joblib-1.4.2/joblib/test/test_backports.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_cloudpickle_wrapper.py` & `joblib-1.4.2/joblib/test/test_cloudpickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_config.py` & `joblib-1.4.2/joblib/test/test_config.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_dask.py` & `joblib-1.4.2/joblib/test/test_dask.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_disk.py` & `joblib-1.4.2/joblib/test/test_disk.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_func_inspect.py` & `joblib-1.4.2/joblib/test/test_func_inspect.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_hashing.py` & `joblib-1.4.2/joblib/test/test_hashing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_logger.py` & `joblib-1.4.2/joblib/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_memmapping.py` & `joblib-1.4.2/joblib/test/test_memmapping.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_memory.py` & `joblib-1.4.2/joblib/test/test_memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1408,20 +1408,14 @@
     with pytest.warns(DeprecationWarning, match="bytes_limit"):
         _ = Memory(location=tmpdir.strpath, bytes_limit='1K')
 
 
 class TestCacheValidationCallback:
     "Tests on parameter `cache_validation_callback`"
 
-    @pytest.fixture()
-    def memory(self, tmp_path):
-        mem = Memory(location=tmp_path)
-        yield mem
-        mem.clear()
-
     def foo(self, x, d, delay=None):
         d["run"] = True
         if delay is not None:
             time.sleep(delay)
         return x * 2
 
     def test_invalid_cache_validation_callback(self, memory):
@@ -1487,7 +1481,46 @@
         assert f(2, d2) == 4
         time.sleep(.5)
         assert f(2, d3) == 4
 
         assert d1["run"]
         assert not d2["run"]
         assert d3["run"]
+
+
+class TestMemorizedFunc:
+    "Tests for the MemorizedFunc and NotMemorizedFunc classes"
+
+    @staticmethod
+    def f(x, counter):
+        counter[x] = counter.get(x, 0) + 1
+        return counter[x]
+
+    def test_call_method_memorized(self, memory):
+        "Test calling the function"
+
+        f = memory.cache(self.f, ignore=['counter'])
+
+        counter = {}
+        assert f(2, counter) == 1
+        assert f(2, counter) == 1
+
+        x, meta = f.call(2, counter)
+        assert x == 2, "f has not been called properly"
+        assert isinstance(meta, dict), (
+            "Metadata are not returned by MemorizedFunc.call."
+        )
+
+    def test_call_method_not_memorized(self, memory):
+        "Test calling the function"
+
+        f = NotMemorizedFunc(self.f)
+
+        counter = {}
+        assert f(2, counter) == 1
+        assert f(2, counter) == 2
+
+        x, meta = f.call(2, counter)
+        assert x == 3, "f has not been called properly"
+        assert isinstance(meta, dict), (
+            "Metadata are not returned by MemorizedFunc.call."
+        )
```

### Comparing `joblib-1.4.0/joblib/test/test_memory_async.py` & `joblib-1.4.2/joblib/test/test_memory_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,7 +143,28 @@
             assert isinstance(result, Result)
             assert result.get() == 5
 
         result.clear()
         with raises(KeyError):
             result.get()
         result.clear()  # Do nothing if there is no cache.
+
+
+@pytest.mark.asyncio
+async def test_memorized_func_call_async(memory):
+
+    async def ff(x, counter):
+        await asyncio.sleep(0.1)
+        counter[x] = counter.get(x, 0) + 1
+        return counter[x]
+
+    gg = memory.cache(ff, ignore=['counter'])
+
+    counter = {}
+    assert await gg(2, counter) == 1
+    assert await gg(2, counter) == 1
+
+    x, meta = await gg.call(2, counter)
+    assert x == 2, "f has not been called properly"
+    assert isinstance(meta, dict), (
+        "Metadata are not returned by MemorizedFunc.call."
+    )
```

### Comparing `joblib-1.4.0/joblib/test/test_missing_multiprocessing.py` & `joblib-1.4.2/joblib/test/test_missing_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_module.py` & `joblib-1.4.2/joblib/test/test_module.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_numpy_pickle.py` & `joblib-1.4.2/joblib/test/test_numpy_pickle.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_numpy_pickle_compat.py` & `joblib-1.4.2/joblib/test/test_numpy_pickle_compat.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_parallel.py` & `joblib-1.4.2/joblib/test/test_parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,14 +358,36 @@
             raise RuntimeError('123')
 
     with raises(PicklingError, match=r"the task to send"):
         Parallel(n_jobs=2, backend='loky')(delayed(id)(
             UnpicklableObject()) for _ in range(10))
 
 
+@with_numpy
+@with_multiprocessing
+@parametrize('byteorder', ['<', '>', '='])
+def test_parallel_byteorder_corruption(byteorder):
+
+    def inspect_byteorder(x):
+        return x, x.dtype.byteorder
+
+    x = np.arange(6).reshape((2, 3)).view(f'{byteorder}i4')
+
+    initial_np_byteorder = x.dtype.byteorder
+
+    result = Parallel(n_jobs=2, backend='loky')(
+        delayed(inspect_byteorder)(x) for _ in range(3)
+    )
+
+    for x_returned, byteorder_in_worker in result:
+        assert byteorder_in_worker == initial_np_byteorder
+        assert byteorder_in_worker == x_returned.dtype.byteorder
+        np.testing.assert_array_equal(x, x_returned)
+
+
 @parametrize('backend', PARALLEL_BACKENDS)
 def test_parallel_timeout_success(backend):
     # Check that timeout isn't thrown when function is fast enough
     assert len(Parallel(n_jobs=2, backend=backend, timeout=30)(
         delayed(sleep)(0.001) for x in range(10))) == 10
```

### Comparing `joblib-1.4.0/joblib/test/test_store_backends.py` & `joblib-1.4.2/joblib/test/test_store_backends.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_testing.py` & `joblib-1.4.2/joblib/test/test_testing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/test/test_utils.py` & `joblib-1.4.2/joblib/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib/testing.py` & `joblib-1.4.2/joblib/testing.py`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/joblib.egg-info/PKG-INFO` & `joblib-1.4.2/joblib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joblib
-Version: 1.4.0
+Version: 1.4.2
 Summary: Lightweight pipelining with Python functions
 Author-email: Gael Varoquaux <gael.varoquaux@normalesup.org>
 License: BSD 3-Clause
 Project-URL: Homepage, https://joblib.readthedocs.io
 Project-URL: Source, https://github.com/joblib/joblib
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -29,23 +29,23 @@
 
 |PyPi| |Azure| |ReadTheDocs| |Codecov| 
 
 .. |PyPi| image:: https://badge.fury.io/py/joblib.svg
    :target: https://badge.fury.io/py/joblib
    :alt: Joblib version
 
-.. |Azure| image:: https://dev.azure.com/joblib/joblib/_apis/build/status/joblib.joblib?branchName=master
+.. |Azure| image:: https://dev.azure.com/joblib/joblib/_apis/build/status/joblib.joblib?branchName=main
    :target: https://dev.azure.com/joblib/joblib/_build?definitionId=3&_a=summary&branchFilter=40
    :alt: Azure CI status
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/joblib/badge/?version=latest
     :target: https://joblib.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. |Codecov| image:: https://codecov.io/gh/joblib/joblib/branch/master/graph/badge.svg
+.. |Codecov| image:: https://codecov.io/gh/joblib/joblib/branch/main/graph/badge.svg
    :target: https://codecov.io/gh/joblib/joblib
    :alt: Codecov coverage
 
 
 The homepage of joblib with user documentation is located on:
 
 https://joblib.readthedocs.io
@@ -54,15 +54,15 @@
 =======================
 
 To get the latest code using git, simply type::
 
     git clone https://github.com/joblib/joblib.git
 
 If you don't have git installed, you can download a zip
-of the latest code: https://github.com/joblib/joblib/archive/refs/heads/master.zip
+of the latest code: https://github.com/joblib/joblib/archive/refs/heads/main.zip
 
 Installing
 ==========
 
 You can use `pip` to install joblib::
 
     pip install joblib
```

### Comparing `joblib-1.4.0/joblib.egg-info/SOURCES.txt` & `joblib-1.4.2/joblib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joblib-1.4.0/pyproject.toml` & `joblib-1.4.2/pyproject.toml`

 * *Files identical despite different names*

