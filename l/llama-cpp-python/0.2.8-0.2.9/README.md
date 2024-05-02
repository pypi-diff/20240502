# Comparing `tmp/llama_cpp_python-0.2.8.tar.gz` & `tmp/llama_cpp_python-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_python-0.2.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "llama_cpp_python-0.2.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `llama_cpp_python-0.2.8.tar` & `llama_cpp_python-0.2.9.tar`

### file list

```diff
@@ -1,311 +1,447 @@
--rw-r--r--   0        0        0     3105 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.dockerignore
--rw-r--r--   0        0        0     3826 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1713 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/workflows/build-and-release.yaml
--rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/workflows/build-docker.yaml
--rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/workflows/publish-to-test.yaml
--rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/workflows/test-pypi.yaml
--rw-r--r--   0        0        0     1891 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.github/workflows/test.yaml
--rw-r--r--   0        0        0     3273 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.gitignore
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.gitmodules
--rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/.readthedocs.yaml
--rw-r--r--   0        0        0     6718 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/CHANGELOG.md
--rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/CMakeLists.txt
--rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/LICENSE.md
--rw-r--r--   0        0        0     1347 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/Makefile
--rw-r--r--   0        0        0     9613 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/README.md
--rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/README.md
--rw-r--r--   0        0        0      880 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/cuda_simple/Dockerfile
--rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/open_llama/Dockerfile
--rwxr-xr-x   0        0        0      341 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/open_llama/build.sh
--rw-r--r--   0        0        0     4944 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/open_llama/hug_model.py
--rwxr-xr-x   0        0        0      603 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/open_llama/start.sh
--rwxr-xr-x   0        0        0      338 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/open_llama/start_server.sh
--rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/openblas_simple/Dockerfile
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/simple/Dockerfile
--rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docker/simple/run.sh
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docs/api-reference.md
--rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docs/changelog.md
--rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docs/index.md
--rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docs/install/macos.md
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/docs/requirements.txt
--rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/high_level_api/fastapi_server.py
--rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/high_level_api/high_level_api_embedding.py
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/high_level_api/high_level_api_inference.py
--rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/high_level_api/high_level_api_streaming.py
--rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/high_level_api/langchain_custom_llm.py
--rw-r--r--   0        0        0     2780 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/Chat.py
--rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/Miku.py
--rw-r--r--   0        0        0     1397 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/ReasonAct.py
--rw-r--r--   0        0        0     8988 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/common.py
--rw-r--r--   0        0        0    21962 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/low_level_api_chat_cpp.py
--rw-r--r--   0        0        0     3489 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/low_level_api_llama_cpp.py
--rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/quantize.py
--rw-r--r--   0        0        0     2146 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/low_level_api/util.py
--rw-r--r--   0        0        0     2571 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/notebooks/Clients.ipynb
--rw-r--r--   0        0        0    10236 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/notebooks/Guidance.ipynb
--rw-r--r--   0        0        0   361229 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/examples/notebooks/PerformanceTuning.ipynb
--rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/__init__.py
--rw-r--r--   0        0        0    69486 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/llama.py
--rw-r--r--   0        0        0    10715 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/llama_chat_format.py
--rw-r--r--   0        0        0    61336 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/llama_cpp.py
--rw-r--r--   0        0        0    44450 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/llama_grammar.py
--rw-r--r--   0        0        0     3979 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/llama_types.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/py.typed
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/server/__init__.py
--rw-r--r--   0        0        0     2952 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/server/__main__.py
--rw-r--r--   0        0        0    29024 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/server/app.py
--rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/llama_cpp/utils.py
--rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/mkdocs.yml
--rw-r--r--   0        0        0     1819 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     5728 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/tests/test_llama.py
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.clang-tidy
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/cloud-v-pipeline
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/full-cuda.Dockerfile
--rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/full-rocm.Dockerfile
--rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/full.Dockerfile
--rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/main-cuda.Dockerfile
--rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/main-rocm.Dockerfile
--rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/main.Dockerfile
--rwxr-xr-x   0        0        0     1674 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/tools.sh
--rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.dockerignore
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.ecrc
--rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.editorconfig
--rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.flake8
--rw-r--r--   0        0        0     9985 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0    22781 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/build.yml
--rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/code-coverage.yml
--rw-r--r--   0        0        0     2744 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/docker.yml
--rw-r--r--   0        0        0      311 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/editorconfig.yml
--rw-r--r--   0        0        0     1183 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/gguf-publish.yml
--rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/tidy-post.yml
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/tidy-review.yml
--rw-r--r--   0        0        0     1032 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.gitignore
--rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/.pre-commit-config.yaml
--rw-r--r--   0        0        0    29688 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/CMakeLists.txt
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/LICENSE
--rw-r--r--   0        0        0    22633 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/Makefile
--rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/Package.swift
--rw-r--r--   0        0        0    49368 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/README.md
--rw-r--r--   0        0        0     3829 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/SHA256SUMS
--rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/build-info.h
--rw-r--r--   0        0        0     5188 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/build.zig
--rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ci/README.md
--rwxr-xr-x   0        0        0    26591 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ci/run.sh
--rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/codecov.yml
--rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/CMakeLists.txt
--rw-r--r--   0        0        0    57387 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/common.cpp
--rw-r--r--   0        0        0    10934 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/common.h
--rw-r--r--   0        0        0    16237 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/console.cpp
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/console.h
--rw-r--r--   0        0        0    17687 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/grammar-parser.cpp
--rw-r--r--   0        0        0      874 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/grammar-parser.h
--rw-r--r--   0        0        0    23698 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/log.h
--rw-r--r--   0        0        0    65376 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/train.cpp
--rw-r--r--   0        0        0     7828 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/common/train.h
--rwxr-xr-x   0        0        0     9555 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert-baichuan-hf-to-gguf.py
--rwxr-xr-x   0        0        0     9234 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert-falcon-hf-to-gguf.py
--rwxr-xr-x   0        0        0     8051 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert-gptneox-hf-to-gguf.py
--rwxr-xr-x   0        0        0    19527 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert-llama-ggml-to-gguf.py
--rwxr-xr-x   0        0        0     4306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert-lora-to-ggml.py
--rwxr-xr-x   0        0        0     8000 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert-starcoder-hf-to-gguf.py
--rwxr-xr-x   0        0        0    49891 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/convert.py
--rw-r--r--   0        0        0     1741 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/docs/BLIS.md
--rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/docs/token_generation_performance_tips.md
--rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/CMakeLists.txt
--rwxr-xr-x   0        0        0     2626 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/Miku.sh
--rwxr-xr-x   0        0        0      336 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/alpaca.sh
--rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/baby-llama/CMakeLists.txt
--rw-r--r--   0        0        0    62630 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/baby-llama/baby-llama.cpp
--rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/batched/CMakeLists.txt
--rw-r--r--   0        0        0     1406 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/batched/README.md
--rw-r--r--   0        0        0     7659 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/batched/batched.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/beam-search/CMakeLists.txt
--rw-r--r--   0        0        0     5887 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/beam-search/beam-search.cpp
--rw-r--r--   0        0        0      362 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/benchmark/CMakeLists.txt
--rw-r--r--   0        0        0     9759 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/benchmark/benchmark-matmult.cpp
--rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-13B.bat
--rwxr-xr-x   0        0        0     1339 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-13B.sh
--rwxr-xr-x   0        0        0     5020 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-persistent.sh
--rwxr-xr-x   0        0        0     1331 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-vicuna.sh
--rwxr-xr-x   0        0        0      344 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat.sh
--rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/convert-llama2c-to-ggml/CMakeLists.txt
--rw-r--r--   0        0        0     1344 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/convert-llama2c-to-ggml/README.md
--rw-r--r--   0        0        0    36407 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/convert-llama2c-to-ggml/convert-llama2c-to-ggml.cpp
--rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/.gitignore
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/CMakeLists.txt
--rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/README.md
--rw-r--r--   0        0        0     7362 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd-input-lib.cpp
--rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd-input-test.cpp
--rw-r--r--   0        0        0      639 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd-input.h
--rwxr-xr-x   0        0        0     2274 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd_input.py
--rwxr-xr-x   0        0        0     2834 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/llava.py
--rwxr-xr-x   0        0        0     4829 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/minigpt4.py
--rwxr-xr-x   0        0        0     3497 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/panda_gpt.py
--rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embedding/CMakeLists.txt
--rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embedding/README.md
--rw-r--r--   0        0        0     2868 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embedding/embedding.cpp
--rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/export-lora/CMakeLists.txt
--rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/export-lora/README.md
--rw-r--r--   0        0        0    15205 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/export-lora/export-lora.cpp
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/CMakeLists.txt
--rw-r--r--   0        0        0     4548 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/README.md
--rw-r--r--   0        0        0    27265 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/convert-finetune-checkpoint-to-gguf.py
--rw-r--r--   0        0        0    92852 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/finetune.cpp
--rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gguf/CMakeLists.txt
--rw-r--r--   0        0        0     7687 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gguf/gguf.cpp
--rwxr-xr-x   0        0        0      386 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gpt4all.sh
--rw-r--r--   0        0        0    79375 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gptneox-wip/cmpnct_gpt2bpe.hpp
--rw-r--r--   0        0        0    41762 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gptneox-wip/falcon-main.cpp
--rw-r--r--   0        0        0    40844 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gptneox-wip/gptneox-main.cpp
--rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/README.md
--rwxr-xr-x   0        0        0     1644 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/graph.py
--rwxr-xr-x   0        0        0      846 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/jeopardy.sh
--rw-r--r--   0        0        0    16674 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/qasheet.csv
--rw-r--r--   0        0        0    12308 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/questions.txt
--rwxr-xr-x   0        0        0     4930 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/json-schema-to-grammar.py
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama-bench/CMakeLists.txt
--rw-r--r--   0        0        0    13715 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama-bench/README.md
--rw-r--r--   0        0        0    37027 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama-bench/llama-bench.cpp
--rw-r--r--   0        0        0     5023 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama.vim
--rwxr-xr-x   0        0        0      323 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama2-13b.sh
--rwxr-xr-x   0        0        0      321 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama2.sh
--rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llm.vim
--rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main/CMakeLists.txt
--rw-r--r--   0        0        0    25244 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main/README.md
--rw-r--r--   0        0        0    33768 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main/main.cpp
--rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main-cmake-pkg/.gitignore
--rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main-cmake-pkg/CMakeLists.txt
--rw-r--r--   0        0        0     1717 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main-cmake-pkg/README.md
--rwxr-xr-x   0        0        0     5105 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/make-ggml.py
--rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/metal/CMakeLists.txt
--rw-r--r--   0        0        0     2896 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/metal/metal.cpp
--rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/parallel/CMakeLists.txt
--rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/parallel/README.md
--rw-r--r--   0        0        0    14183 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/parallel/parallel.cpp
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/perplexity/CMakeLists.txt
--rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/perplexity/README.md
--rw-r--r--   0        0        0    28505 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/perplexity/perplexity.cpp
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize/CMakeLists.txt
--rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize/README.md
--rw-r--r--   0        0        0     6906 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize/quantize.cpp
--rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize-stats/CMakeLists.txt
--rw-r--r--   0        0        0    16072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize-stats/quantize-stats.cpp
--rwxr-xr-x   0        0        0      350 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/reason-act.sh
--rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/save-load-state/CMakeLists.txt
--rw-r--r--   0        0        0     5230 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/save-load-state/save-load-state.cpp
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/CMakeLists.txt
--rw-r--r--   0        0        0    10244 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/README.md
--rwxr-xr-x   0        0        0     9780 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/api_like_OAI.py
--rwxr-xr-x   0        0        0     2516 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/chat-llama2.sh
--rw-r--r--   0        0        0     3499 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/chat.mjs
--rwxr-xr-x   0        0        0     1944 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/chat.sh
--rw-r--r--   0        0        0    31519 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/completion.js.hpp
--rwxr-xr-x   0        0        0      539 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/deps.sh
--rw-r--r--   0        0        0   288389 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/httplib.h
--rw-r--r--   0        0        0   172848 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/index.html.hpp
--rw-r--r--   0        0        0   138644 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/index.js.hpp
--rw-r--r--   0        0        0    22887 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/json-schema-to-grammar.mjs.hpp
--rw-r--r--   0        0        0   907858 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/json.hpp
--rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/completion.js
--rw-r--r--   0        0        0    28018 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/index.html
--rw-r--r--   0        0        0    22472 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/index.js
--rw-r--r--   0        0        0     3695 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/json-schema-to-grammar.mjs
--rw-r--r--   0        0        0    59274 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/server.cpp
--rwxr-xr-x   0        0        0      784 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server-llama2-13B.sh
--rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/simple/CMakeLists.txt
--rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/simple/README.md
--rw-r--r--   0        0        0     5332 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/simple/simple.cpp
--rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/speculative/CMakeLists.txt
--rw-r--r--   0        0        0    10440 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/speculative/speculative.cpp
--rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/CMakeLists.txt
--rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/README.md
--rw-r--r--   0        0        0    26389 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/convert-train-checkpoint-to-gguf.py
--rw-r--r--   0        0        0    59715 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/train-text-from-scratch.cpp
--rw-r--r--   0        0        0     1497 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/flake.lock
--rw-r--r--   0        0        0     4991 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/flake.nix
--rw-r--r--   0        0        0    23334 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-alloc.c
--rw-r--r--   0        0        0      971 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-alloc.h
--rw-r--r--   0        0        0   278510 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-cuda.cu
--rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-cuda.h
--rw-r--r--   0        0        0     3529 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-metal.h
--rw-r--r--   0        0        0    70413 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-metal.m
--rw-r--r--   0        0        0    89557 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-metal.metal
--rw-r--r--   0        0        0     6919 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-mpi.c
--rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-mpi.h
--rw-r--r--   0        0        0    68875 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-opencl.cpp
--rw-r--r--   0        0        0      845 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-opencl.h
--rw-r--r--   0        0        0   714034 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml.c
--rw-r--r--   0        0        0    76177 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/ggml.h
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/LICENSE
--rw-r--r--   0        0        0     1659 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/README.md
--rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/gguf/__init__.py
--rw-r--r--   0        0        0    32701 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/gguf/gguf.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/gguf/py.typed
--rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/pyproject.toml
--rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/tests/test_gguf.py
--rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/README.md
--rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/arithmetic.gbnf
--rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/c.gbnf
--rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/chess.gbnf
--rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/japanese.gbnf
--rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/json.gbnf
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/json_arr.gbnf
--rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/list.gbnf
--rw-r--r--   0        0        0   174427 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/k_quants.c
--rw-r--r--   0        0        0     7241 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/k_quants.h
--rw-r--r--   0        0        0   282388 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/llama.cpp
--rw-r--r--   0        0        0    32339 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/llama.h
--rw-r--r--   0        0        0   199945 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama-leader.jpeg
--rw-r--r--   0        0        0   144615 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama0-banner.png
--rw-r--r--   0        0        0   179940 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama0-logo.png
--rw-r--r--   0        0        0    33331 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama1-banner.png
--rw-r--r--   0        0        0    32494 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama1-logo.png
--rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/mypy.ini
--rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/pocs/CMakeLists.txt
--rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/pocs/vdot/CMakeLists.txt
--rw-r--r--   0        0        0     5330 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/pocs/vdot/q8dot.cpp
--rw-r--r--   0        0        0    13508 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/pocs/vdot/vdot.cpp
--rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/alpaca.txt
--rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/chat-with-baichuan.txt
--rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/chat-with-bob.txt
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/chat-with-vicuna-v0.txt
--rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/chat-with-vicuna-v1.txt
--rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/chat.txt
--rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/dan-modified.txt
--rw-r--r--   0        0        0     1663 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/dan.txt
--rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/reason-act.txt
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/requirements.txt
--rwxr-xr-x   0        0        0     5313 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/run_with_preset.py
--rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/LlamaConfig.cmake.in
--rw-r--r--   0        0        0     2363 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/build-info.cmake
--rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/build-info.h.in
--rwxr-xr-x   0        0        0      763 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/build-info.sh
--rwxr-xr-x   0        0        0     1384 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/convert-gg.sh
--rwxr-xr-x   0        0        0       95 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/get-wikitext-2.sh
--rwxr-xr-x   0        0        0      552 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/qnt-all.sh
--rwxr-xr-x   0        0        0      549 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/run-all-perf.sh
--rwxr-xr-x   0        0        0      548 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/run-all-ppl.sh
--rwxr-xr-x   0        0        0      756 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/sync-ggml.sh
--rwxr-xr-x   0        0        0     2359 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/verify-checksum-models.py
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/spm-headers/ggml.h -> ../ggml.h
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/spm-headers/llama.h -> ../llama.h
--rw-r--r--   0        0        0     2328 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/CMakeLists.txt
--rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-c.c
--rw-r--r--   0        0        0     1774 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-double-float.cpp
--rw-r--r--   0        0        0    56016 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-grad0.cpp
--rw-r--r--   0        0        0     8386 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-grammar-parser.cpp
--rw-r--r--   0        0        0    11119 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-llama-grammar.cpp
--rw-r--r--   0        0        0     5751 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-opt.cpp
--rw-r--r--   0        0        0     5689 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-quantize-fns.cpp
--rw-r--r--   0        0        0    14042 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-quantize-perf.cpp
--rw-r--r--   0        0        0     6285 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-rope.cpp
--rw-r--r--   0        0        0     7843 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-sampling.cpp
--rw-r--r--   0        0        0     6904 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-falcon.cpp
--rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-falcon.py
--rw-r--r--   0        0        0     7516 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-llama.cpp
--rw-r--r--   0        0        0     2856 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-llama.py
--rw-r--r--   0        0        0     4072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-1-llama.cpp
--rw-r--r--   0        0        0    11362 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     3105 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.dockerignore
+-rw-r--r--   0        0        0      132 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/FETCH_HEAD
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/HEAD
+-rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/config
+-rwxr-xr-x   0        0        0       73 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/description
+-rwxr-xr-x   0        0        0      478 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4726 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     2308 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0        0        0     3650 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/hooks/update.sample
+-rw-r--r--   0        0        0     6654 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/index
+-rwxr-xr-x   0        0        0      240 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/info/exclude
+-rw-r--r--   0        0        0      230 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/logs/HEAD
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/HEAD
+-rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/config
+-rwxr-xr-x   0        0        0       73 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/description
+-rwxr-xr-x   0        0        0      478 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/applypatch-msg.sample
+-rwxr-xr-x   0        0        0      896 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/commit-msg.sample
+-rwxr-xr-x   0        0        0     4726 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0        0        0      189 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/post-update.sample
+-rwxr-xr-x   0        0        0      424 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/pre-applypatch.sample
+-rwxr-xr-x   0        0        0     1643 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/pre-commit.sample
+-rwxr-xr-x   0        0        0      416 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0        0        0     1374 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/pre-push.sample
+-rwxr-xr-x   0        0        0     4898 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/pre-rebase.sample
+-rwxr-xr-x   0        0        0      544 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/pre-receive.sample
+-rwxr-xr-x   0        0        0     1492 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0        0        0     2783 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/push-to-checkout.sample
+-rwxr-xr-x   0        0        0     2308 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/sendemail-validate.sample
+-rwxr-xr-x   0        0        0     3650 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/hooks/update.sample
+-rw-r--r--   0        0        0    24651 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/index
+-rwxr-xr-x   0        0        0      240 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/info/exclude
+-rw-r--r--   0        0        0      490 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/logs/HEAD
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/logs/refs/heads/master
+-rw-r--r--   0        0        0      236 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0     9416 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/objects/pack/pack-c5c4a727e5070cbf5b2e9f3cb1f883616c9a1a05.idx
+-rw-r--r--   0        0        0  1665532 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/objects/pack/pack-c5c4a727e5070cbf5b2e9f3cb1f883616c9a1a05.pack
+-rw-r--r--   0        0        0     1244 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/objects/pack/pack-c5c4a727e5070cbf5b2e9f3cb1f883616c9a1a05.rev
+-rw-r--r--   0        0        0      114 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/packed-refs
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/refs/heads/master
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/refs/remotes/origin/HEAD
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/refs/tags/b1298
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/modules/vendor/llama.cpp/shallow
+-rw-r--r--   0        0        0     3996 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/04/5856ea2ffe697ec33db1c1c989bd45cde5bb3d
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/04/7bc14424303575f73af90611fec827334f54e8
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/06/1aed8b4a54f9aec500abc7a12a310aa66a2b57
+-rw-r--r--   0        0        0     3180 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/0f/ccf979fd8b95a7cfa3704815c3f91f0ae03737
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/11/2a0f7872fa9244bf38729a2722dc5c08dec20c
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/11/b6d5c26e3f7157658952b8ec353e985d522fac
+-rw-r--r--   0        0        0      296 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/12/90cad4931d6fc9b80e00baadecda4d45b1f005
+-rw-r--r--   0        0        0     1889 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/13/c5b6b0df5f67e80cbe584909b83777901265a1
+-rw-r--r--   0        0        0     3857 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/18/81af60185e2591a47c7156b7dc9be0c89e2ca3
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/19/9bd4ffbf88c68c98b52c05f388dfa92716f6b7
+-rw-r--r--   0        0        0      754 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/23/e37d4d40e5ec0bfd85b5e928834d58e2cf0da6
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/29/03e0146d304bcacbfabfe71f171a2edc03043e
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/2d/86e92443d200069a0fcee7cdb8b91bb802d77c
+-rw-r--r--   0        0        0    15446 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/30/e0de3ba25fa82c05f107ef6977f931a72717d0
+-rw-r--r--   0        0        0      593 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/31/6b9e7f4b18bf549bbe08b074b97b0f63da57b3
+-rw-r--r--   0        0        0      181 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/33/197007d97015ba62fb8fe835bf6eabe5bebd86
+-rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/36/10eaba65f7415c3ea07a4809c41f2ddf98eff7
+-rw-r--r--   0        0        0      645 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/3a/1d7180d508818fe957923e00dcd8950938632d
+-rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/3a/6457dcdfd47e764654bacae0ba8347976b645a
+-rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/41/cc68ea2402cf682807649d841e7c0f4175db01
+-rw-r--r--   0        0        0     7416 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/44/b6d4a35d3caf0c65aef0a1c77ff0ab4077d405
+-rw-r--r--   0        0        0     1247 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/47/4503fdfc554d8caabee4f321a80427f8c7d696
+-rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/4b/3189dd1a54be3bc416786ddf184dd047dc4b20
+-rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/4b/38dbacb6208ed2496e517018b0670beb21be65
+-rw-r--r--   0        0        0       67 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/4f/dbab4ed946c5c372edfc94aebccc91255cd83b
+-rw-r--r--   0        0        0     1628 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/51/f357200f8b998031f4be924e11ed2ae4bf3fea
+-rw-r--r--   0        0        0     3039 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/55/d08db5f514fb6847938e3d6489b99f737ba6e3
+-rw-r--r--   0        0        0     1869 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/5d/f12aaf53a0e85f55e1aa0e5167bc831ab32783
+-rw-r--r--   0        0        0       62 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/60/bc7aef42aac0409cfdca666ad2ff6f516d7b5b
+-rw-r--r--   0        0        0      200 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/66/0d6798c5615aa765347c461beb3aab2d502fb1
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/67/50769eef1992c7eaa624b9e602109a0ea77118
+-rw-r--r--   0        0        0     1055 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/6e/e7ef91468c1594e3c2244c13e1f3f561ecca89
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/73/f62293c40d7d7900a0f09e8054cefb4ed9dd76
+-rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/74/7c6130e3cb1479d20e2013b1dd3db3379c2266
+-rw-r--r--   0        0        0    88207 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/76/e26fbd106895fba52861f8ac1e11cc6ee2a307
+-rw-r--r--   0        0        0       58 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/77/8a7505c35756c11481cf2d6132c920af50f2f0
+-rw-r--r--   0        0        0      480 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/7d/6c970483161eaf43cfa9d50010c071d4953053
+-rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/7e/069b1903cc69a74e562a32ef8b0c1bd22d41d2
+-rw-r--r--   0        0        0       98 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/7e/df0975dc12ccc95ad14de085f07efe6d65c620
+-rw-r--r--   0        0        0      410 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/7e/e8f748eab47180cea09c0ad8e75c3b991b4af4
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/80/10fa0d9e0316327db4f15f0f04cf6fbef5e642
+-rw-r--r--   0        0        0      744 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/82/e5c4487e57d6d59c901a73bdd2a9bc172fee7c
+-rw-r--r--   0        0        0       52 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/87/c27df1134d4fcb8f98763d7be31d55cf99ffcb
+-rw-r--r--   0        0        0      402 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/8b/d03f88a1895cbf3ef249e13df79ee0efda779d
+-rw-r--r--   0        0        0      848 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/8c/52dffa2af040be62976560c72578ede27402bb
+-rw-r--r--   0        0        0      904 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/8f/0e9dbca8020193048f9711d5f1a28e433bdc1f
+-rw-r--r--   0        0        0    10951 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/8f/f15658e3841a564faa9378d0d38ef16fb33f64
+-rw-r--r--   0        0        0      307 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/91/abb11fdf507883caeeb2d2958e1c65fb6cbdc1
+-rw-r--r--   0        0        0       55 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/94/1a4eac8ffb4e7978bb8d6ef5108efdb06975bf
+-rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/99/32d6130f5552a9b85c8b15b4ac6bc26b1068ce
+-rw-r--r--   0        0        0      863 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/9d/0ec2f705618e591cfa8d6512cb9a96b3da75f1
+-rw-r--r--   0        0        0     8378 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/a0/6076e805ddf98a857c430cde79299e177861cf
+-rw-r--r--   0        0        0     1145 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/a2/94ebf8a4ed0b4dd705aaeaccd0df201e361c8b
+-rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/a9/e51cdc1672134ec9af66c9eccf09f6da4ceccd
+-rw-r--r--   0        0        0      379 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/ac/a743b7357e488562e9fac29a0cb641afb04328
+-rw-r--r--   0        0        0      772 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/b9/1632f5bc787c1404600c894a6a4126359747d8
+-rw-r--r--   0        0        0     1430 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/bb/2b42c13e6e499e759fc451af837551655249f7
+-rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/bb/cbbe7d61558adde3cbfd0c7a63a67c27ed6d30
+-rw-r--r--   0        0        0      169 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/bc/a965325d236fe68c64d8f063b1887b111d81d8
+-rw-r--r--   0        0        0     2763 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/bd/8110f2c91342802f63d13debe723e37a667249
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/be/b930d9e5ece4ce15ad886660607de5bac270dc
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/bf/f3d9756409c3d3c62f6db87b2e567bed0bb698
+-rw-r--r--   0        0        0      369 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/c1/4f53f61b04ac10f8489642dc840a4b3cde5daa
+-rw-r--r--   0        0        0      666 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/c6/33c0797f8d3c6e0e238793cece0fee5df49d76
+-rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/c8/5e73d2b657bb05ed99309615d67bac93d9f86e
+-rw-r--r--   0        0        0      947 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/ca/ebbb67fdb02a0a8897d4e4826ea046a9931f6f
+-rw-r--r--   0        0        0      364 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/cc/6a3a7252ea6e698614f0629d4bc040ab6ca717
+-rw-r--r--   0        0        0      133 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/ce/04d74a4af6b67d6e9ea2405b30661fd70413d0
+-rw-r--r--   0        0        0    15322 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/d2/a35c13fe399ff8786f2f5affc1f368620c5c7d
+-rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/d3/329eec3bac6ce7e54c76b77ac9bf99fab0fe3f
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/d4/888b448a6895f87411f7c52dc23f1ad5f0d8f6
+-rw-r--r--   0        0        0     1323 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/e3/cff3251c7fb6410937ee586b94f7b84331da2f
+-rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/e4/1f375774e6945e445bfb179502b128fe22dda7
+-rw-r--r--   0        0        0       15 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/e6/9de29bb2d1d6434b8b29ae775ad8c2e48c5391
+-rw-r--r--   0        0        0      556 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/e9/30609ff5c479a1d5e12a8f3993582d421a6326
+-rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/e9/48f8deb150039c6853e14537a8dd0cc9002b72
+-rw-r--r--   0        0        0     1339 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/eb/9a2cfa9167df02f136502af79738c71363abfd
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/fc/25ff5160028dee3570249abc40cd57780bcca9
+-rw-r--r--   0        0        0     1417 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/fc/ef8cd800ee8a265b146748d178cb56b5632bf3
+-rw-r--r--   0        0        0     1559 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/fd/64c09b37947c97e58903ce570785c657d56722
+-rw-r--r--   0        0        0      211 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/fe/b0ed68d94eac48b844fd587ddfb808649716a1
+-rw-r--r--   0        0        0      287 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/objects/ff/3e950cd1110fe552912cea4c268c4023d2b737
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/refs/tags/v0.2.9
+-rw-r--r--   0        0        0       41 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.git/shallow
+-rw-r--r--   0        0        0     3826 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      502 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     1713 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/workflows/build-and-release.yaml
+-rw-r--r--   0        0        0     1045 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/workflows/build-docker.yaml
+-rw-r--r--   0        0        0     1350 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/workflows/publish-to-test.yaml
+-rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/workflows/test-pypi.yaml
+-rw-r--r--   0        0        0     1891 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     3273 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.gitignore
+-rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.gitmodules
+-rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/.readthedocs.yaml
+-rw-r--r--   0        0        0     6848 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1858 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/CMakeLists.txt
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0     1347 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/Makefile
+-rw-r--r--   0        0        0     9613 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/README.md
+-rw-r--r--   0        0        0     2734 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/README.md
+-rw-r--r--   0        0        0      880 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/cuda_simple/Dockerfile
+-rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/open_llama/Dockerfile
+-rwxr-xr-x   0        0        0      341 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/open_llama/build.sh
+-rw-r--r--   0        0        0     4944 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/open_llama/hug_model.py
+-rwxr-xr-x   0        0        0      603 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/open_llama/start.sh
+-rwxr-xr-x   0        0        0      338 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/open_llama/start_server.sh
+-rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/openblas_simple/Dockerfile
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/simple/Dockerfile
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docker/simple/run.sh
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docs/api-reference.md
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docs/changelog.md
+-rw-r--r--   0        0        0       48 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docs/index.md
+-rw-r--r--   0        0        0     1685 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docs/install/macos.md
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/docs/requirements.txt
+-rw-r--r--   0        0        0      636 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/high_level_api/fastapi_server.py
+-rw-r--r--   0        0        0      291 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/high_level_api/high_level_api_embedding.py
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/high_level_api/high_level_api_inference.py
+-rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/high_level_api/high_level_api_streaming.py
+-rw-r--r--   0        0        0     1517 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/high_level_api/langchain_custom_llm.py
+-rw-r--r--   0        0        0     2780 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/Chat.py
+-rw-r--r--   0        0        0     2738 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/Miku.py
+-rw-r--r--   0        0        0     1397 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/ReasonAct.py
+-rw-r--r--   0        0        0     8988 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/common.py
+-rw-r--r--   0        0        0    21962 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/low_level_api_chat_cpp.py
+-rw-r--r--   0        0        0     3489 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/low_level_api_llama_cpp.py
+-rw-r--r--   0        0        0      906 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/quantize.py
+-rw-r--r--   0        0        0     2146 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/low_level_api/util.py
+-rw-r--r--   0        0        0     2571 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/notebooks/Clients.ipynb
+-rw-r--r--   0        0        0    10236 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/notebooks/Guidance.ipynb
+-rw-r--r--   0        0        0   361229 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/examples/notebooks/PerformanceTuning.ipynb
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/__init__.py
+-rw-r--r--   0        0        0    69486 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/llama.py
+-rw-r--r--   0        0        0    10715 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/llama_chat_format.py
+-rw-r--r--   0        0        0    61336 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/llama_cpp.py
+-rw-r--r--   0        0        0    44450 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/llama_grammar.py
+-rw-r--r--   0        0        0     3979 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/llama_types.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/py.typed
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/server/__init__.py
+-rw-r--r--   0        0        0     2952 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/server/__main__.py
+-rw-r--r--   0        0        0    29024 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/server/app.py
+-rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/llama_cpp/utils.py
+-rw-r--r--   0        0        0      476 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/mkdocs.yml
+-rw-r--r--   0        0        0     1819 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5728 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/tests/test_llama.py
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.clang-tidy
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/cloud-v-pipeline
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/full-cuda.Dockerfile
+-rw-r--r--   0        0        0      979 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/full-rocm.Dockerfile
+-rw-r--r--   0        0        0      371 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/full.Dockerfile
+-rw-r--r--   0        0        0      776 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/main-cuda.Dockerfile
+-rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/main-rocm.Dockerfile
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/main.Dockerfile
+-rwxr-xr-x   0        0        0     1674 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/tools.sh
+-rw-r--r--   0        0        0      121 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.dockerignore
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.ecrc
+-rw-r--r--   0        0        0      395 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.editorconfig
+-rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.flake8
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.git
+-rw-r--r--   0        0        0     9985 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0    22781 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/build.yml
+-rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/code-coverage.yml
+-rw-r--r--   0        0        0     2744 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/docker.yml
+-rw-r--r--   0        0        0      311 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/editorconfig.yml
+-rw-r--r--   0        0        0     1183 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/gguf-publish.yml
+-rw-r--r--   0        0        0      496 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/tidy-post.yml
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/tidy-review.yml
+-rw-r--r--   0        0        0     1032 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.gitignore
+-rw-r--r--   0        0        0      398 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29688 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/CMakeLists.txt
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/LICENSE
+-rw-r--r--   0        0        0    22633 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/Makefile
+-rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/Package.swift
+-rw-r--r--   0        0        0    49368 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/README.md
+-rw-r--r--   0        0        0     3829 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/SHA256SUMS
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/build-info.h
+-rw-r--r--   0        0        0     5188 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/build.zig
+-rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ci/README.md
+-rwxr-xr-x   0        0        0    26591 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ci/run.sh
+-rw-r--r--   0        0        0      210 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/codecov.yml
+-rw-r--r--   0        0        0      450 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/CMakeLists.txt
+-rw-r--r--   0        0        0    57387 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/common.cpp
+-rw-r--r--   0        0        0    10934 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/common.h
+-rw-r--r--   0        0        0    16237 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/console.cpp
+-rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/console.h
+-rw-r--r--   0        0        0    17687 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/grammar-parser.cpp
+-rw-r--r--   0        0        0      874 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/grammar-parser.h
+-rw-r--r--   0        0        0    23698 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/log.h
+-rw-r--r--   0        0        0    65376 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/train.cpp
+-rw-r--r--   0        0        0     7828 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/common/train.h
+-rwxr-xr-x   0        0        0     9555 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert-baichuan-hf-to-gguf.py
+-rwxr-xr-x   0        0        0     9234 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert-falcon-hf-to-gguf.py
+-rwxr-xr-x   0        0        0     8051 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert-gptneox-hf-to-gguf.py
+-rwxr-xr-x   0        0        0    19527 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert-llama-ggml-to-gguf.py
+-rwxr-xr-x   0        0        0     4306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert-lora-to-ggml.py
+-rwxr-xr-x   0        0        0     8000 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert-starcoder-hf-to-gguf.py
+-rwxr-xr-x   0        0        0    49891 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/convert.py
+-rw-r--r--   0        0        0     1741 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/docs/BLIS.md
+-rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/docs/token_generation_performance_tips.md
+-rw-r--r--   0        0        0      946 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/CMakeLists.txt
+-rwxr-xr-x   0        0        0     2626 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/Miku.sh
+-rwxr-xr-x   0        0        0      336 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/alpaca.sh
+-rw-r--r--   0        0        0      233 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/baby-llama/CMakeLists.txt
+-rw-r--r--   0        0        0    62630 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/baby-llama/baby-llama.cpp
+-rw-r--r--   0        0        0      227 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/batched/CMakeLists.txt
+-rw-r--r--   0        0        0     1406 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/batched/README.md
+-rw-r--r--   0        0        0     7659 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/batched/batched.cpp
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/beam-search/CMakeLists.txt
+-rw-r--r--   0        0        0     5887 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/beam-search/beam-search.cpp
+-rw-r--r--   0        0        0      362 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/benchmark/CMakeLists.txt
+-rw-r--r--   0        0        0     9759 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/benchmark/benchmark-matmult.cpp
+-rw-r--r--   0        0        0     2452 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-13B.bat
+-rwxr-xr-x   0        0        0     1339 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-13B.sh
+-rwxr-xr-x   0        0        0     5020 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-persistent.sh
+-rwxr-xr-x   0        0        0     1331 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-vicuna.sh
+-rwxr-xr-x   0        0        0      344 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat.sh
+-rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/convert-llama2c-to-ggml/CMakeLists.txt
+-rw-r--r--   0        0        0     1344 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/convert-llama2c-to-ggml/README.md
+-rw-r--r--   0        0        0    36407 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/convert-llama2c-to-ggml/convert-llama2c-to-ggml.cpp
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/.gitignore
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/CMakeLists.txt
+-rw-r--r--   0        0        0     2232 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/README.md
+-rw-r--r--   0        0        0     7362 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd-input-lib.cpp
+-rw-r--r--   0        0        0      969 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd-input-test.cpp
+-rw-r--r--   0        0        0      639 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd-input.h
+-rwxr-xr-x   0        0        0     2274 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd_input.py
+-rwxr-xr-x   0        0        0     2834 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/llava.py
+-rwxr-xr-x   0        0        0     4829 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/minigpt4.py
+-rwxr-xr-x   0        0        0     3497 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/panda_gpt.py
+-rw-r--r--   0        0        0      302 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embedding/CMakeLists.txt
+-rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embedding/README.md
+-rw-r--r--   0        0        0     2868 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embedding/embedding.cpp
+-rw-r--r--   0        0        0      235 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/export-lora/CMakeLists.txt
+-rw-r--r--   0        0        0      914 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/export-lora/README.md
+-rw-r--r--   0        0        0    15205 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/export-lora/export-lora.cpp
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/CMakeLists.txt
+-rw-r--r--   0        0        0     4548 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/README.md
+-rw-r--r--   0        0        0    27265 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/convert-finetune-checkpoint-to-gguf.py
+-rw-r--r--   0        0        0    92852 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/finetune.cpp
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gguf/CMakeLists.txt
+-rw-r--r--   0        0        0     7687 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gguf/gguf.cpp
+-rwxr-xr-x   0        0        0      386 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gpt4all.sh
+-rw-r--r--   0        0        0    79375 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gptneox-wip/cmpnct_gpt2bpe.hpp
+-rw-r--r--   0        0        0    41762 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gptneox-wip/falcon-main.cpp
+-rw-r--r--   0        0        0    40844 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gptneox-wip/gptneox-main.cpp
+-rw-r--r--   0        0        0     1023 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/README.md
+-rwxr-xr-x   0        0        0     1644 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/graph.py
+-rwxr-xr-x   0        0        0      846 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/jeopardy.sh
+-rw-r--r--   0        0        0    16674 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/qasheet.csv
+-rw-r--r--   0        0        0    12308 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/questions.txt
+-rwxr-xr-x   0        0        0     4930 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/json-schema-to-grammar.py
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama-bench/CMakeLists.txt
+-rw-r--r--   0        0        0    13715 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama-bench/README.md
+-rw-r--r--   0        0        0    37027 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama-bench/llama-bench.cpp
+-rw-r--r--   0        0        0     5023 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama.vim
+-rwxr-xr-x   0        0        0      323 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama2-13b.sh
+-rwxr-xr-x   0        0        0      321 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama2.sh
+-rw-r--r--   0        0        0      921 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llm.vim
+-rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main/CMakeLists.txt
+-rw-r--r--   0        0        0    25244 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main/README.md
+-rw-r--r--   0        0        0    33768 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main/main.cpp
+-rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main-cmake-pkg/.gitignore
+-rw-r--r--   0        0        0     1255 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main-cmake-pkg/CMakeLists.txt
+-rw-r--r--   0        0        0     1717 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main-cmake-pkg/README.md
+-rwxr-xr-x   0        0        0     5105 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/make-ggml.py
+-rw-r--r--   0        0        0      150 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/metal/CMakeLists.txt
+-rw-r--r--   0        0        0     2896 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/metal/metal.cpp
+-rw-r--r--   0        0        0      300 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/parallel/CMakeLists.txt
+-rw-r--r--   0        0        0       94 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/parallel/README.md
+-rw-r--r--   0        0        0    14183 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/parallel/parallel.cpp
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/perplexity/CMakeLists.txt
+-rw-r--r--   0        0        0      526 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/perplexity/README.md
+-rw-r--r--   0        0        0    28505 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/perplexity/perplexity.cpp
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize/CMakeLists.txt
+-rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize/README.md
+-rw-r--r--   0        0        0     6906 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize/quantize.cpp
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize-stats/CMakeLists.txt
+-rw-r--r--   0        0        0    16072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize-stats/quantize-stats.cpp
+-rwxr-xr-x   0        0        0      350 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/reason-act.sh
+-rw-r--r--   0        0        0      314 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/save-load-state/CMakeLists.txt
+-rw-r--r--   0        0        0     5230 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/save-load-state/save-load-state.cpp
+-rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/CMakeLists.txt
+-rw-r--r--   0        0        0    10244 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/README.md
+-rwxr-xr-x   0        0        0     9780 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/api_like_OAI.py
+-rwxr-xr-x   0        0        0     2516 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/chat-llama2.sh
+-rw-r--r--   0        0        0     3499 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/chat.mjs
+-rwxr-xr-x   0        0        0     1944 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/chat.sh
+-rw-r--r--   0        0        0    31519 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/completion.js.hpp
+-rwxr-xr-x   0        0        0      539 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/deps.sh
+-rw-r--r--   0        0        0   288389 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/httplib.h
+-rw-r--r--   0        0        0   172848 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/index.html.hpp
+-rw-r--r--   0        0        0   138644 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/index.js.hpp
+-rw-r--r--   0        0        0    22887 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/json-schema-to-grammar.mjs.hpp
+-rw-r--r--   0        0        0   907858 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/json.hpp
+-rw-r--r--   0        0        0     5099 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/completion.js
+-rw-r--r--   0        0        0    28018 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/index.html
+-rw-r--r--   0        0        0    22472 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/index.js
+-rw-r--r--   0        0        0     3695 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/json-schema-to-grammar.mjs
+-rw-r--r--   0        0        0    59274 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/server.cpp
+-rwxr-xr-x   0        0        0      784 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server-llama2-13B.sh
+-rw-r--r--   0        0        0      225 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/simple/CMakeLists.txt
+-rw-r--r--   0        0        0      903 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/simple/README.md
+-rw-r--r--   0        0        0     5332 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/simple/simple.cpp
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/speculative/CMakeLists.txt
+-rw-r--r--   0        0        0    10440 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/speculative/speculative.cpp
+-rw-r--r--   0        0        0      259 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/CMakeLists.txt
+-rw-r--r--   0        0        0      960 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/README.md
+-rw-r--r--   0        0        0    26389 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/convert-train-checkpoint-to-gguf.py
+-rw-r--r--   0        0        0    59715 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/train-text-from-scratch.cpp
+-rw-r--r--   0        0        0     1497 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/flake.lock
+-rw-r--r--   0        0        0     4991 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/flake.nix
+-rw-r--r--   0        0        0    23334 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-alloc.c
+-rw-r--r--   0        0        0      971 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-alloc.h
+-rw-r--r--   0        0        0   278510 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-cuda.cu
+-rw-r--r--   0        0        0     1788 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-cuda.h
+-rw-r--r--   0        0        0     3529 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-metal.h
+-rw-r--r--   0        0        0    70413 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-metal.m
+-rw-r--r--   0        0        0    89557 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-metal.metal
+-rw-r--r--   0        0        0     6919 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-mpi.c
+-rw-r--r--   0        0        0      911 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-mpi.h
+-rw-r--r--   0        0        0    68875 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-opencl.cpp
+-rw-r--r--   0        0        0      845 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-opencl.h
+-rw-r--r--   0        0        0   714034 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml.c
+-rw-r--r--   0        0        0    76177 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/ggml.h
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/LICENSE
+-rw-r--r--   0        0        0     1659 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/README.md
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/gguf/__init__.py
+-rw-r--r--   0        0        0    32701 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/gguf/gguf.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/gguf/py.typed
+-rw-r--r--   0        0        0      697 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/pyproject.toml
+-rw-r--r--   0        0        0       65 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/tests/test_gguf.py
+-rw-r--r--   0        0        0     4129 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/README.md
+-rw-r--r--   0        0        0      177 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/arithmetic.gbnf
+-rw-r--r--   0        0        0     1382 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/c.gbnf
+-rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/chess.gbnf
+-rw-r--r--   0        0        0      249 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/japanese.gbnf
+-rw-r--r--   0        0        0      595 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/json.gbnf
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/json_arr.gbnf
+-rw-r--r--   0        0        0      109 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/list.gbnf
+-rw-r--r--   0        0        0   174427 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/k_quants.c
+-rw-r--r--   0        0        0     7241 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/k_quants.h
+-rw-r--r--   0        0        0   282388 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/llama.cpp
+-rw-r--r--   0        0        0    32339 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/llama.h
+-rw-r--r--   0        0        0   199945 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama-leader.jpeg
+-rw-r--r--   0        0        0   144615 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama0-banner.png
+-rw-r--r--   0        0        0   179940 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama0-logo.png
+-rw-r--r--   0        0        0    33331 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama1-banner.png
+-rw-r--r--   0        0        0    32494 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama1-logo.png
+-rw-r--r--   0        0        0      103 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/mypy.ini
+-rw-r--r--   0        0        0      171 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/pocs/CMakeLists.txt
+-rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/pocs/vdot/CMakeLists.txt
+-rw-r--r--   0        0        0     5330 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/pocs/vdot/q8dot.cpp
+-rw-r--r--   0        0        0    13508 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/pocs/vdot/vdot.cpp
+-rw-r--r--   0        0        0      106 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/alpaca.txt
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/chat-with-baichuan.txt
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/chat-with-bob.txt
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/chat-with-vicuna-v0.txt
+-rw-r--r--   0        0        0      426 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/chat-with-vicuna-v1.txt
+-rw-r--r--   0        0        0     1837 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/chat.txt
+-rw-r--r--   0        0        0     1538 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/dan-modified.txt
+-rw-r--r--   0        0        0     1663 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/dan.txt
+-rw-r--r--   0        0        0      758 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/reason-act.txt
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/requirements.txt
+-rwxr-xr-x   0        0        0     5313 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/run_with_preset.py
+-rw-r--r--   0        0        0     1896 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/LlamaConfig.cmake.in
+-rw-r--r--   0        0        0     2363 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/build-info.cmake
+-rw-r--r--   0        0        0      221 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/build-info.h.in
+-rwxr-xr-x   0        0        0      763 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/build-info.sh
+-rwxr-xr-x   0        0        0     1384 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/convert-gg.sh
+-rwxr-xr-x   0        0        0       95 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/get-wikitext-2.sh
+-rwxr-xr-x   0        0        0      552 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/qnt-all.sh
+-rwxr-xr-x   0        0        0      549 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/run-all-perf.sh
+-rwxr-xr-x   0        0        0      548 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/run-all-ppl.sh
+-rwxr-xr-x   0        0        0      756 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/sync-ggml.sh
+-rwxr-xr-x   0        0        0     2359 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/verify-checksum-models.py
+lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/spm-headers/ggml.h -> ../ggml.h
+lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/spm-headers/llama.h -> ../llama.h
+-rw-r--r--   0        0        0     2328 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/CMakeLists.txt
+-rw-r--r--   0        0        0       38 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-c.c
+-rw-r--r--   0        0        0     1774 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-double-float.cpp
+-rw-r--r--   0        0        0    56016 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-grad0.cpp
+-rw-r--r--   0        0        0     8386 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-grammar-parser.cpp
+-rw-r--r--   0        0        0    11119 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-llama-grammar.cpp
+-rw-r--r--   0        0        0     5751 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-opt.cpp
+-rw-r--r--   0        0        0     5689 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-quantize-fns.cpp
+-rw-r--r--   0        0        0    14042 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-quantize-perf.cpp
+-rw-r--r--   0        0        0     6285 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-rope.cpp
+-rw-r--r--   0        0        0     7843 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-sampling.cpp
+-rw-r--r--   0        0        0     6904 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-falcon.cpp
+-rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-falcon.py
+-rw-r--r--   0        0        0     7516 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-llama.cpp
+-rw-r--r--   0        0        0     2856 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-llama.py
+-rw-r--r--   0        0        0     4072 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-1-llama.cpp
+-rw-r--r--   0        0        0    11362 2022-11-09 12:37:21.000000 llama_cpp_python-0.2.9/PKG-INFO
```

### Comparing `llama_cpp_python-0.2.8/.dockerignore` & `llama_cpp_python-0.2.9/.dockerignore`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `llama_cpp_python-0.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `llama_cpp_python-0.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/workflows/build-and-release.yaml` & `llama_cpp_python-0.2.9/.github/workflows/build-and-release.yaml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/workflows/build-docker.yaml` & `llama_cpp_python-0.2.9/.github/workflows/build-docker.yaml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/workflows/publish.yaml` & `llama_cpp_python-0.2.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/workflows/test-pypi.yaml` & `llama_cpp_python-0.2.9/.github/workflows/test-pypi.yaml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.github/workflows/test.yaml` & `llama_cpp_python-0.2.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/.gitignore` & `llama_cpp_python-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/CHANGELOG.md` & `llama_cpp_python-0.2.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.9]
+
+- Fix critical bug in pip installation of v0.2.8 due to `.git` directory in ac853e01e1a217a578080a4e1b851d2d08450adf
+
 ## [0.2.8]
 
 - Update llama.cpp to ggerganov/llama.cpp@40e07a60f9ce06e79f3ccd4c903eba300fb31b5e
 - Add configurable chat formats by @abetlen in #711
 - Fix rope scaling bug by @Josh-XT in #767
 - Fix missing numa parameter in server by @abetlen in d9bce17794d0dd6f7962d10aad768fedecf3ab89
```

### Comparing `llama_cpp_python-0.2.8/CMakeLists.txt` & `llama_cpp_python-0.2.9/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 cmake_minimum_required(VERSION 3.21)
 
 project(llama_cpp)
 
 option(LLAMA_BUILD "Build llama.cpp shared library and install alongside python package" ON)
 
-
 if (LLAMA_BUILD)
     set(BUILD_SHARED_LIBS "On")
     if (APPLE AND NOT CMAKE_SYSTEM_PROCESSOR MATCHES "arm64")
         # Need to disable these llama.cpp flags on Apple x86_64,
         # otherwise users may encounter invalid instruction errors
         set(LLAMA_AVX "Off" CACHE BOOL "llama: enable AVX" FORCE)
         set(LLAMA_AVX2 "Off" CACHE BOOL "llama: enable AVX2" FORCE)
```

### Comparing `llama_cpp_python-0.2.8/LICENSE.md` & `llama_cpp_python-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/Makefile` & `llama_cpp_python-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/README.md` & `llama_cpp_python-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/README.md` & `llama_cpp_python-0.2.9/docker/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/cuda_simple/Dockerfile` & `llama_cpp_python-0.2.9/docker/cuda_simple/Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/open_llama/Dockerfile` & `llama_cpp_python-0.2.9/docker/open_llama/Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/open_llama/hug_model.py` & `llama_cpp_python-0.2.9/docker/open_llama/hug_model.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/open_llama/start.sh` & `llama_cpp_python-0.2.9/docker/open_llama/start.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/openblas_simple/Dockerfile` & `llama_cpp_python-0.2.9/docker/openblas_simple/Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docker/simple/Dockerfile` & `llama_cpp_python-0.2.9/docker/simple/Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docs/api-reference.md` & `llama_cpp_python-0.2.9/docs/api-reference.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/docs/install/macos.md` & `llama_cpp_python-0.2.9/docs/install/macos.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/high_level_api/fastapi_server.py` & `llama_cpp_python-0.2.9/examples/high_level_api/fastapi_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/high_level_api/langchain_custom_llm.py` & `llama_cpp_python-0.2.9/examples/high_level_api/langchain_custom_llm.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/Chat.py` & `llama_cpp_python-0.2.9/examples/low_level_api/Chat.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/Miku.py` & `llama_cpp_python-0.2.9/examples/low_level_api/Miku.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/ReasonAct.py` & `llama_cpp_python-0.2.9/examples/low_level_api/ReasonAct.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/common.py` & `llama_cpp_python-0.2.9/examples/low_level_api/common.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/low_level_api_chat_cpp.py` & `llama_cpp_python-0.2.9/examples/low_level_api/low_level_api_chat_cpp.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/low_level_api_llama_cpp.py` & `llama_cpp_python-0.2.9/examples/low_level_api/low_level_api_llama_cpp.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/quantize.py` & `llama_cpp_python-0.2.9/examples/low_level_api/quantize.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/low_level_api/util.py` & `llama_cpp_python-0.2.9/examples/low_level_api/util.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/notebooks/Clients.ipynb` & `llama_cpp_python-0.2.9/examples/notebooks/Clients.ipynb`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/notebooks/Guidance.ipynb` & `llama_cpp_python-0.2.9/examples/notebooks/Guidance.ipynb`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/examples/notebooks/PerformanceTuning.ipynb` & `llama_cpp_python-0.2.9/examples/notebooks/PerformanceTuning.ipynb`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/llama.py` & `llama_cpp_python-0.2.9/llama_cpp/llama.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/llama_chat_format.py` & `llama_cpp_python-0.2.9/llama_cpp/llama_chat_format.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/llama_cpp.py` & `llama_cpp_python-0.2.9/llama_cpp/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/llama_grammar.py` & `llama_cpp_python-0.2.9/llama_cpp/llama_grammar.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/llama_types.py` & `llama_cpp_python-0.2.9/llama_cpp/llama_types.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/server/__main__.py` & `llama_cpp_python-0.2.9/llama_cpp/server/__main__.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/server/app.py` & `llama_cpp_python-0.2.9/llama_cpp/server/app.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/llama_cpp/utils.py` & `llama_cpp_python-0.2.9/llama_cpp/utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/pyproject.toml` & `llama_cpp_python-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 ]
 
 [tool.scikit-build]
 wheel.packages = ["llama_cpp"]
 cmake.verbose = true
 cmake.minimum-version = "3.21"
 minimum-version = "0.5.1"
-sdist.exclude = [".git", "vendor/llama.cpp/.git"]
+sdist.include = [".git", "vendor/llama.cpp/.git"]
 
 [tool.scikit-build.metadata.version]
 provider = "scikit_build_core.metadata.regex"
 input = "llama_cpp/__init__.py"
 
 [project.urls]
 Homepage = "https://github.com/abetlen/llama-cpp-python"
```

### Comparing `llama_cpp_python-0.2.8/tests/test_llama.py` & `llama_cpp_python-0.2.9/tests/test_llama.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.clang-tidy` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.clang-tidy`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/cloud-v-pipeline` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/cloud-v-pipeline`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/full-cuda.Dockerfile` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/full-cuda.Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/full-rocm.Dockerfile` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/full-rocm.Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/main-cuda.Dockerfile` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/main-cuda.Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/main-rocm.Dockerfile` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/main-rocm.Dockerfile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.devops/tools.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.devops/tools.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.github/ISSUE_TEMPLATE/custom.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.github/ISSUE_TEMPLATE/custom.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/build.yml` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/code-coverage.yml` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/code-coverage.yml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/docker.yml` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.github/workflows/gguf-publish.yml` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.github/workflows/gguf-publish.yml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/.gitignore` & `llama_cpp_python-0.2.9/vendor/llama.cpp/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/CMakeLists.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/LICENSE` & `llama_cpp_python-0.2.9/vendor/llama.cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/Makefile` & `llama_cpp_python-0.2.9/vendor/llama.cpp/Makefile`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/Package.swift` & `llama_cpp_python-0.2.9/vendor/llama.cpp/Package.swift`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/SHA256SUMS` & `llama_cpp_python-0.2.9/vendor/llama.cpp/SHA256SUMS`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/build.zig` & `llama_cpp_python-0.2.9/vendor/llama.cpp/build.zig`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ci/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ci/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ci/run.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ci/run.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/common.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/common.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/common.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/common.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/console.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/console.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/grammar-parser.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/grammar-parser.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/grammar-parser.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/grammar-parser.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/log.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/log.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/train.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/train.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/common/train.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/common/train.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert-baichuan-hf-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert-baichuan-hf-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert-falcon-hf-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert-falcon-hf-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert-gptneox-hf-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert-gptneox-hf-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert-llama-ggml-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert-llama-ggml-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert-lora-to-ggml.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert-lora-to-ggml.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert-starcoder-hf-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert-starcoder-hf-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/convert.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/convert.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/docs/BLIS.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/docs/BLIS.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/docs/token_generation_performance_tips.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/docs/token_generation_performance_tips.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/CMakeLists.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/Miku.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/Miku.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/baby-llama/baby-llama.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/baby-llama/baby-llama.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/batched/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/batched/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/batched/batched.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/batched/batched.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/beam-search/beam-search.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/beam-search/beam-search.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/benchmark/benchmark-matmult.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/benchmark/benchmark-matmult.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-13B.bat` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-13B.bat`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-13B.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-13B.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-persistent.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-persistent.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/chat-vicuna.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/chat-vicuna.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/convert-llama2c-to-ggml/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/convert-llama2c-to-ggml/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/convert-llama2c-to-ggml/convert-llama2c-to-ggml.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/convert-llama2c-to-ggml/convert-llama2c-to-ggml.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/CMakeLists.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd-input-lib.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd-input-lib.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd-input-test.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd-input-test.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd-input.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd-input.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/embd_input.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/embd_input.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/llava.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/llava.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/minigpt4.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/minigpt4.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embd-input/panda_gpt.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embd-input/panda_gpt.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embedding/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embedding/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/embedding/embedding.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/embedding/embedding.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/export-lora/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/export-lora/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/export-lora/export-lora.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/export-lora/export-lora.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/convert-finetune-checkpoint-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/convert-finetune-checkpoint-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/finetune/finetune.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/finetune/finetune.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gguf/gguf.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gguf/gguf.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gptneox-wip/cmpnct_gpt2bpe.hpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gptneox-wip/cmpnct_gpt2bpe.hpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gptneox-wip/falcon-main.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gptneox-wip/falcon-main.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/gptneox-wip/gptneox-main.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/gptneox-wip/gptneox-main.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/graph.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/graph.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/jeopardy.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/jeopardy.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/qasheet.csv` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/qasheet.csv`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/jeopardy/questions.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/jeopardy/questions.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/json-schema-to-grammar.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/json-schema-to-grammar.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama-bench/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama-bench/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama-bench/llama-bench.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama-bench/llama-bench.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llama.vim` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llama.vim`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/llm.vim` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/llm.vim`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main/main.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main/main.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main-cmake-pkg/CMakeLists.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main-cmake-pkg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/main-cmake-pkg/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/main-cmake-pkg/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/make-ggml.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/make-ggml.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/metal/metal.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/metal/metal.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/parallel/parallel.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/parallel/parallel.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/perplexity/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/perplexity/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/perplexity/perplexity.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/perplexity/perplexity.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize/quantize.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize/quantize.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/quantize-stats/quantize-stats.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/quantize-stats/quantize-stats.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/save-load-state/save-load-state.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/save-load-state/save-load-state.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/CMakeLists.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/api_like_OAI.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/api_like_OAI.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/chat-llama2.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/chat-llama2.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/chat.mjs` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/chat.mjs`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/chat.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/chat.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/completion.js.hpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/completion.js.hpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/deps.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/deps.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/httplib.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/httplib.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/index.html.hpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/index.html.hpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/index.js.hpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/index.js.hpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/json-schema-to-grammar.mjs.hpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/json-schema-to-grammar.mjs.hpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/json.hpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/json.hpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/completion.js` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/completion.js`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/index.html` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/index.html`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/index.js` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/index.js`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/public/json-schema-to-grammar.mjs` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/public/json-schema-to-grammar.mjs`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server/server.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server/server.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/server-llama2-13B.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/server-llama2-13B.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/simple/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/simple/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/simple/simple.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/simple/simple.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/speculative/speculative.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/speculative/speculative.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/convert-train-checkpoint-to-gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/convert-train-checkpoint-to-gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/examples/train-text-from-scratch/train-text-from-scratch.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/examples/train-text-from-scratch/train-text-from-scratch.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/flake.lock` & `llama_cpp_python-0.2.9/vendor/llama.cpp/flake.lock`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/flake.nix` & `llama_cpp_python-0.2.9/vendor/llama.cpp/flake.nix`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-alloc.c` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-alloc.c`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-alloc.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-alloc.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-cuda.cu` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-cuda.cu`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-cuda.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-cuda.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-metal.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-metal.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-metal.m` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-metal.m`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-metal.metal` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-metal.metal`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-mpi.c` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-mpi.c`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-mpi.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-mpi.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-opencl.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-opencl.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml-opencl.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml-opencl.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml.c` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml.c`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/ggml.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/ggml.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/LICENSE` & `llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/gguf/gguf.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/gguf/gguf.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/gguf-py/pyproject.toml` & `llama_cpp_python-0.2.9/vendor/llama.cpp/gguf-py/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/README.md` & `llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/c.gbnf` & `llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/c.gbnf`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/chess.gbnf` & `llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/chess.gbnf`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/json.gbnf` & `llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/grammars/json_arr.gbnf` & `llama_cpp_python-0.2.9/vendor/llama.cpp/grammars/json_arr.gbnf`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/k_quants.c` & `llama_cpp_python-0.2.9/vendor/llama.cpp/k_quants.c`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/k_quants.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/k_quants.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/llama.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/llama.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/llama.h` & `llama_cpp_python-0.2.9/vendor/llama.cpp/llama.h`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama-leader.jpeg` & `llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama-leader.jpeg`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama0-banner.png` & `llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama0-banner.png`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama0-logo.png` & `llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama0-logo.png`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama1-banner.png` & `llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama1-banner.png`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/media/llama1-logo.png` & `llama_cpp_python-0.2.9/vendor/llama.cpp/media/llama1-logo.png`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/pocs/vdot/q8dot.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/pocs/vdot/q8dot.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/pocs/vdot/vdot.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/pocs/vdot/vdot.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/chat.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/chat.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/dan-modified.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/dan-modified.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/dan.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/dan.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/prompts/reason-act.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/prompts/reason-act.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/run_with_preset.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/run_with_preset.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/LlamaConfig.cmake.in` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/LlamaConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/build-info.cmake` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/build-info.cmake`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/build-info.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/build-info.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/convert-gg.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/convert-gg.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/qnt-all.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/qnt-all.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/run-all-perf.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/run-all-perf.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/run-all-ppl.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/run-all-ppl.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/sync-ggml.sh` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/sync-ggml.sh`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/scripts/verify-checksum-models.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/scripts/verify-checksum-models.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/CMakeLists.txt` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-double-float.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-double-float.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-grad0.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-grad0.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-grammar-parser.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-grammar-parser.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-llama-grammar.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-llama-grammar.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-opt.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-opt.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-quantize-fns.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-quantize-fns.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-quantize-perf.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-quantize-perf.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-rope.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-rope.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-sampling.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-sampling.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-falcon.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-falcon.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-falcon.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-falcon.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-llama.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-llama.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-0-llama.py` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-0-llama.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/vendor/llama.cpp/tests/test-tokenizer-1-llama.cpp` & `llama_cpp_python-0.2.9/vendor/llama.cpp/tests/test-tokenizer-1-llama.cpp`

 * *Files identical despite different names*

### Comparing `llama_cpp_python-0.2.8/PKG-INFO` & `llama_cpp_python-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_cpp_python
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python bindings for the llama.cpp library
 Author-Email: Andrei Betlen <abetlen@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

