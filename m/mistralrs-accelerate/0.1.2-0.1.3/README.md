# Comparing `tmp/mistralrs_accelerate-0.1.2.tar.gz` & `tmp/mistralrs_accelerate-0.1.3.tar.gz`

## Comparing `mistralrs_accelerate-0.1.2.tar` & `mistralrs_accelerate-0.1.3.tar`

### file list

```diff
@@ -1,76 +1,75 @@
--rw-r--r--   0     1000     1000      794 2024-04-26 00:59:23.000000 mistralrs_accelerate-0.1.2/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs_accelerate-0.1.2/mistralrs-lora/README.md
--rw-r--r--   0     1000     1000     2395 2024-04-26 13:56:27.000000 mistralrs_accelerate-0.1.2/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1000     1000     5818 2024-04-28 01:11:39.000000 mistralrs_accelerate-0.1.2/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1000     1000     9472 2024-04-28 22:09:55.000000 mistralrs_accelerate-0.1.2/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1000     1000     9961 2024-04-28 22:10:05.000000 mistralrs_accelerate-0.1.2/mistralrs-lora/src/qloralinear.rs
--rw-------   0     1000     1000     1974 2024-04-30 09:44:59.000000 mistralrs_accelerate-0.1.2/mistralrs-core/Cargo.toml
--rw-r--r--   0     1000     1000        0 2024-04-26 16:25:02.000000 mistralrs_accelerate-0.1.2/mistralrs-core/README.md
--rw-r--r--   0     1000     1000      133 2024-04-11 10:11:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1000     1000     6567 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1000     1000      320 2024-04-11 10:11:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1000     1000    15114 2024-04-11 10:11:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1000     1000     9819 2024-04-11 10:11:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1000     1000      179 2024-04-11 10:11:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1000     1000     2447 2024-04-19 18:01:00.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1000     1000     1696 2024-04-12 01:34:41.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1000     1000     3094 2024-04-11 10:11:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1000     1000    17311 2024-04-19 18:01:00.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1000     1000     4667 2024-04-28 01:11:39.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1000     1000    36507 2024-04-30 09:43:44.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1000     1000     7663 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/layers.rs
--rw-r--r--   0     1000     1000     7868 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/lib.rs
--rw-r--r--   0     1000     1000     8310 2024-04-25 00:00:52.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1000     1000    10703 2024-04-27 09:46:04.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1000     1000    16512 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1000     1000    15309 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1000     1000    17943 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1000     1000    22512 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1000     1000     2620 2024-04-26 13:56:27.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1000     1000    15629 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1000     1000    17509 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1000     1000    19605 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1000     1000    10138 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1000     1000    16101 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1000     1000     5912 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1000     1000    13809 2024-04-30 09:43:17.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1000     1000    15835 2024-04-30 09:43:17.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1000     1000    20832 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1000     1000    10912 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1000     1000    33649 2024-04-30 09:43:17.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1000     1000    12269 2024-04-30 09:43:17.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1000     1000     6358 2024-04-23 22:49:11.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1000     1000     1250 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/request.rs
--rw-r--r--   0     1000     1000     3848 2024-04-23 22:49:11.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/response.rs
--rw-r--r--   0     1000     1000    11276 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1000     1000     7286 2024-04-23 22:49:11.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1000     1000    15979 2024-04-30 09:43:17.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1000     1000     7395 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1000     1000     1716 2024-04-27 14:58:30.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1000     1000     4799 2024-04-23 22:49:11.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1000     1000    11049 2024-04-06 02:02:23.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1000     1000     1544 2024-04-23 22:49:11.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1000     1000    26714 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1000     1000    25200 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1000     1000    27603 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1000     1000    32915 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1000     1000     4305 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1000     1000    24492 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1000     1000    25455 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1000     1000    34219 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1000     1000      686 2024-03-08 12:45:25.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1000     1000     3516 2024-04-27 09:46:04.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/API.md
--rw-r--r--   0     1000     1000      855 2024-04-30 09:44:59.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1000     1000     3755 2024-04-27 10:12:38.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/README.md
--rw-r--r--   0     1000     1000     8231 2024-04-27 02:02:03.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1000     1000      530 2024-04-30 09:44:59.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1000     1000    28680 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1000     1000      397 2024-04-25 14:28:35.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/message.rs
--rw-r--r--   0     1000     1000     1672 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1000     1000     3114 2024-04-30 09:38:13.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1000     1000     2044 2024-04-27 10:25:16.000000 mistralrs_accelerate-0.1.2/mistralrs-pyo3/upload.py
--rw-r--r--   0     1000     1000    99209 2024-04-30 09:53:54.000000 mistralrs_accelerate-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.2/Cargo.toml
--rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4456 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.2/PKG-INFO
+-rw-r--r--   0     1001      127     1974 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/README.md
+-rw-r--r--   0     1001      127      133 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1001      127     6567 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1001      127      320 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1001      127    15114 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1001      127     9819 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1001      127      179 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1001      127     2447 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1001      127     1696 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1001      127     3094 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1001      127    17311 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1001      127     4667 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1001      127    36507 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1001      127     7663 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1001      127     7868 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1001      127     8310 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1001      127    10703 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1001      127    16512 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1001      127    15309 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1001      127    17943 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1001      127    22512 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1001      127     2620 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1001      127    15629 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1001      127    17509 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1001      127    19605 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1001      127    10138 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1001      127    16101 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1001      127     5912 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1001      127    13809 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1001      127    15835 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1001      127    20832 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1001      127    10912 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1001      127    33649 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1001      127    12269 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1001      127     6358 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1001      127     1250 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/request.rs
+-rw-r--r--   0     1001      127     3848 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/response.rs
+-rw-r--r--   0     1001      127    11276 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1001      127     7286 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1001      127    15979 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1001      127     7395 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1716 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1001      127     4799 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1001      127    11049 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1001      127     1544 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1001      127    26714 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1001      127    25200 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1001      127    27603 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1001      127    32915 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1001      127     4305 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1001      127    24492 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1001      127    25455 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1001      127    34219 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0     1001      127      794 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-lora/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-lora/README.md
+-rw-r--r--   0     1001      127     2395 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-lora/src/layer.rs
+-rw-r--r--   0     1001      127     5818 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-lora/src/lib.rs
+-rw-r--r--   0     1001      127     9472 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-lora/src/loralinear.rs
+-rw-r--r--   0     1001      127     9961 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-lora/src/qloralinear.rs
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1001      127     3508 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/API.md
+-rw-r--r--   0     1001      127      855 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1001      127     3755 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/README.md
+-rw-r--r--   0     1001      127     7962 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1001      127      530 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1001      127    28898 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1672 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1001      127     3114 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1001      127     2203 2024-05-02 01:30:24.000000 mistralrs_accelerate-0.1.3/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1001      127    99209 2024-05-02 01:30:41.000000 mistralrs_accelerate-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1320 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0      589 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4456 1970-01-01 00:00:00.000000 mistralrs_accelerate-0.1.3/PKG-INFO
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-lora/Cargo.toml` & `mistralrs_accelerate-0.1.3/mistralrs-lora/Cargo.toml`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-lora/src/layer.rs` & `mistralrs_accelerate-0.1.3/mistralrs-lora/src/layer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-lora/src/lib.rs` & `mistralrs_accelerate-0.1.3/mistralrs-lora/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-lora/src/loralinear.rs` & `mistralrs_accelerate-0.1.3/mistralrs-lora/src/loralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-lora/src/qloralinear.rs` & `mistralrs_accelerate-0.1.3/mistralrs-lora/src/qloralinear.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/Cargo.toml` & `mistralrs_accelerate-0.1.3/mistralrs-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.2", path = "../mistralrs-lora" }
+mistralrs-lora = { version = "0.1.3", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/bintokens.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/bintokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/cfg.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/cfg.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/lex.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/recognizer.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/rx.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/svob.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/svob.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/aici/toktree.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/device_map.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/device_map.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/engine/mod.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/engine/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/layers.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/layers.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/lib.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/model_loader.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/model_loader.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/model_selected.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/model_selected.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/gemma.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/gemma.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/llama.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/mistral.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/mistral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/mixtral.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/mod.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/phi2.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/phi3.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/quantized_llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/models/qwen2.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/models/qwen2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/ggml.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/gguf.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/loaders.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/macros.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/macros.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/mod.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/pipeline/normal.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/pipeline/normal.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/prefix_cacher.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/prefix_cacher.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/request.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/request.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/response.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/response.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/sampler.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/sampler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/scheduler.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/sequence.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/sequence.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/utils/mod.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/utils/tokens.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/utils/tokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/config.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/mod.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/phi2.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/phi3.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs_accelerate-0.1.3/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/Cargo.toml` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.2", path = "../mistralrs-core", features=["accelerate"] }
+mistralrs-core = { version = "0.1.3", path = "../mistralrs-core", features=["accelerate"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["accelerate"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/.gitignore` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/API.md` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/API.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,30 +92,30 @@
         tokenizer_json: str | None = None
         repeat_last_n: int = 64
 ```
 
 
 ## Example
 ```python
-from mistralrs import Runner, Which, ChatCompletionRequest, Message, Role
+from mistralrs import Runner, Which, ChatCompletionRequest
 
 runner = Runner(
     which=Which.GGUF(
         tok_model_id="mistralai/Mistral-7B-Instruct-v0.1",
         quantized_model_id="TheBloke/Mistral-7B-Instruct-v0.1-GGUF",
         quantized_filename="mistral-7b-instruct-v0.1.Q4_K_M.gguf",
         tokenizer_json=None,
         repeat_last_n=64,
     )
 )
 
 res = runner.send_chat_completion_request(
     ChatCompletionRequest(
         model="mistral",
-        messages=[Message(Role.User, "Tell me a story about the Rust type system.")],
+        messages=[{"role":"user", "content":"Tell me a story about the Rust type system."}],
         max_tokens=256,
         presence_penalty=1.0,
         top_p=0.1,
         temperature=0.1,
     )
 )
 print(res.choices[0].message.content)
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/Cargo_template.toml` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/Cargo_template.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.2", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.3", path = "../mistralrs-core", features=["$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/README.md` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/mistralrs.pyi` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/mistralrs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @dataclass
 class ChatCompletionRequest:
     """
     A ChatCompletionRequest represents a request sent to the mistral.rs engine. It encodes information
     about input data, sampling, and how to return the response.
     """
 
-    messages: list[Message] | str
+    messages: list[dict[str, str]] | str
     model: str
     logit_bias: dict[int, float] | None = None
     logprobs: bool = False
     top_logprobs: int | None = None
     max_tokens: int | None = None
     n_choices: int = 1
     presence_penalty: float | None = None
@@ -189,33 +189,14 @@
 
     def send_re_isq(self, dtype: str) -> CompletionResponse:
         """
         Send a request to re-ISQ the model. If the model was loaded as GGUF or GGML then nothing will happen.
         """
 
 @dataclass
-class Role(Enum):
-    """
-    The role for each `Message` of a chat completion request.
-    """
-
-    User = 1
-    Assistant = 2
-    System = 3
-
-@dataclass
-class Message:
-    """
-    A message for a chat completion request.
-    """
-
-    role: Role
-    content: str
-
-@dataclass
 class Usage:
     completion_tokens: int
     prompt_tokens: int
     total_tokens: int
     avg_tok_per_sec: float
     avg_prompt_tok_per_sec: float
     avg_compl_tok_per_sec: float
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/pyproject_template.toml` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/pyproject_template.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "$name"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/lib.rs` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #![allow(clippy::too_many_arguments)]
 
 use candle_core::{quantized::GgmlDType, Result};
 use either::Either;
 use indexmap::IndexMap;
-use message::{Message, Role};
 use std::{
     cell::RefCell,
     collections::HashMap,
     fmt::Debug,
     str::FromStr,
     sync::{Arc, Mutex},
 };
@@ -27,15 +26,14 @@
     prelude::*,
     types::{PyList, PyString},
 };
 use std::fs::File;
 mod stream;
 mod which;
 use which::{Architecture, Which};
-mod message;
 
 #[cfg(not(feature = "metal"))]
 static CUDA_DEVICE: std::sync::Mutex<Option<Device>> = std::sync::Mutex::new(None);
 #[cfg(feature = "metal")]
 static METAL_DEVICE: std::sync::Mutex<Option<Device>> = std::sync::Mutex::new(None);
 
 #[cfg(not(feature = "metal"))]
@@ -452,22 +450,24 @@
                     *last += 1;
                     last_v
                 },
                 messages: match request.messages {
                     Either::Left(ref messages) => {
                         let mut messages_vec = Vec::new();
                         for message in messages {
+                            let role = message.get("role").expect("Expected role");
+                            let content = message.get("content").expect("Expected role");
                             let mut message_map = IndexMap::new();
-                            let role = match message.role {
-                                Role::Assistant => "assistant",
-                                Role::User => "user",
-                                Role::System => "system",
-                            };
+                            if !["user", "assistant", "system"].contains(&role.as_str()) {
+                                return Err(PyValueError::new_err(
+                                    "Only `user`, `assistant`, `system` roles supported.",
+                                ));
+                            }
                             message_map.insert("role".to_string(), role.to_string());
-                            message_map.insert("content".to_string(), message.content.clone());
+                            message_map.insert("content".to_string(), content.clone());
                             messages_vec.push(message_map);
                         }
                         RequestMessage::Chat(messages_vec)
                     }
                     Either::Right(ref prompt) => {
                         let mut messages = Vec::new();
                         let mut message_map = IndexMap::new();
@@ -695,15 +695,15 @@
     }
 }
 
 #[pyclass]
 #[derive(Debug)]
 /// An OpenAI API compatible chat completion request.
 struct ChatCompletionRequest {
-    messages: Either<Vec<Message>, String>,
+    messages: Either<Vec<IndexMap<String, String>>, String>,
     _model: String,
     logit_bias: Option<HashMap<u32, f32>>,
     logprobs: bool,
     top_logprobs: Option<usize>,
     max_tokens: Option<usize>,
     n_choices: usize,
     presence_penalty: Option<f32>,
@@ -756,20 +756,22 @@
         grammar: Option<String>,
         grammar_type: Option<String>,
     ) -> PyResult<Self> {
         let messages = Python::with_gil(|py| {
             if let Ok(messages) = messages.bind(py).downcast_exact::<PyList>() {
                 let mut messages_vec = Vec::new();
                 for message in messages {
-                    messages_vec.push(message.extract::<Message>()?);
+                    messages_vec.push(message.extract::<IndexMap<String, String>>()?);
                 }
-                Ok::<Either<Vec<Message>, String>, PyErr>(Either::Left(messages_vec))
+                Ok::<Either<Vec<IndexMap<String, String>>, String>, PyErr>(Either::Left(
+                    messages_vec,
+                ))
             } else if let Ok(messages) = messages.bind(py).downcast_exact::<PyString>() {
                 let prompt = messages.extract::<String>()?;
-                Ok::<Either<Vec<Message>, String>, PyErr>(Either::Right(prompt))
+                Ok::<Either<Vec<IndexMap<String, String>>, String>, PyErr>(Either::Right(prompt))
             } else {
                 return Err(PyTypeError::new_err("Expected a string or list of dicts."));
             }
         })?;
         Ok(Self {
             messages,
             _model: model,
@@ -798,16 +800,14 @@
         .from_env_lossy();
     tracing_subscriber::fmt().with_env_filter(filter).init();
 
     m.add_class::<Runner>()?;
     m.add_class::<Which>()?;
     m.add_class::<ChatCompletionRequest>()?;
     m.add_class::<CompletionRequest>()?;
-    m.add_class::<Message>()?;
-    m.add_class::<Role>()?;
     m.add_class::<Architecture>()?;
 
     m.add_class::<mistralrs_core::ResponseMessage>()?;
     m.add_class::<mistralrs_core::Delta>()?;
     m.add_class::<mistralrs_core::ResponseLogprob>()?;
     m.add_class::<mistralrs_core::Logprobs>()?;
     m.add_class::<mistralrs_core::Choice>()?;
```

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/stream.rs` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/src/which.rs` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/src/which.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_accelerate-0.1.2/mistralrs-pyo3/upload.py` & `mistralrs_accelerate-0.1.3/mistralrs-pyo3/upload.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,16 +51,21 @@
 print(
     f"⭐ Generated sdists for features {[k for k,_ in features.items()]} with corresponding names {[v for _,v in features.items()]}"
 )
 
 # Generate CPU lib
 os.system("maturin sdist --out dist")
 
-password = input("Enter API token: ")
-target = input("Enter target (testpypi or pypi): ")
+if "PYPI_TOKEN" in os.environ:
+    password = os.environ["PYPI_TOKEN"]
+    print("Using PyPi token as environment variable")
+    target = "pypi"
+else:
+    password = input("Enter API token: ")
+    target = input("Enter target (testpypi or pypi): ")
 print(f"🚀 Uploading to {target} in 5 seconds. Press <CTRL>-C to abort.")
 time.sleep(5)
 
 # Upload
 os.system(
     f"twine upload --repository {target} --password {password} --username __token__ dist/*"
 )
```

### Comparing `mistralrs_accelerate-0.1.2/Cargo.lock` & `mistralrs_accelerate-0.1.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -234,17 +234,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bindgen_cuda"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f8489af5b7d17a81bffe37e0f4d6e1e4de87c87329d05447f22c35d95a1227d"
 dependencies = [
@@ -353,15 +353,15 @@
  "num_cpus",
  "rand",
  "rand_distr",
  "rayon",
  "safetensors",
  "thiserror",
  "yoke",
- "zip 1.1.2",
+ "zip 1.1.3",
 ]
 
 [[package]]
 name = "candle-flash-attn"
 version = "0.5.0"
 source = "git+https://github.com/EricLBuehler/candle.git#997a57c4d871c9ae1e6b955599dea81963b6c961"
 dependencies = [
@@ -440,17 +440,17 @@
  "serde_json",
  "serde_plain",
  "tracing",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
+checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -1831,25 +1831,25 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
  "tokio",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
@@ -1858,15 +1858,15 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
@@ -1903,28 +1903,28 @@
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
 name = "mistralrs-lora"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-nn",
  "either",
  "intel-mkl-src",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "mistralrs-pyo3"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
@@ -1933,15 +1933,15 @@
  "serde",
  "serde_json",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
  "dyn-fmt",
@@ -2128,15 +2128,15 @@
 [[package]]
 name = "ocipkg"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9bb3293021f06540803301af45e7ab81693d50e89a7398a3420bdab139e7ba5e"
 dependencies = [
  "base16ct",
- "base64 0.22.0",
+ "base64 0.22.1",
  "chrono",
  "directories",
  "flate2",
  "lazy_static",
  "log",
  "oci-spec",
  "regex",
@@ -2893,26 +2893,26 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
@@ -3547,15 +3547,15 @@
 
 [[package]]
 name = "ureq"
 version = "2.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d11a831e3c0b56e438a28308e7c810799e3c118417f342d30ecec080105395cd"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "flate2",
  "log",
  "native-tls",
  "once_cell",
  "rustls",
  "rustls-pki-types",
  "rustls-webpki",
@@ -4020,16 +4020,16 @@
  "crc32fast",
  "crossbeam-utils",
  "flate2",
 ]
 
 [[package]]
 name = "zip"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a23468b4a7a4e9e1e62812f8d1dd614f67f148e2b3faa72f4843bf00b573fd7"
+checksum = "2e6cb8909b2e8e6733c9ef67d35be1a27105644d362aafb5f8b2ba395727adf6"
 dependencies = [
  "arbitrary",
  "byteorder",
  "crc32fast",
  "crossbeam-utils",
 ]
```

### Comparing `mistralrs_accelerate-0.1.2/Cargo.toml` & `mistralrs_accelerate-0.1.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
```

### Comparing `mistralrs_accelerate-0.1.2/pyproject.toml` & `mistralrs_accelerate-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "mistralrs-accelerate"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_accelerate-0.1.2/PKG-INFO` & `mistralrs_accelerate-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs-accelerate
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

