# Comparing `tmp/truss-0.9.9rc3.tar.gz` & `tmp/truss-0.9.9rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.9.9rc3.tar", max compression
+gzip compressed data, was "truss-0.9.9rc4.tar", max compression
```

## Comparing `truss-0.9.9rc3.tar` & `truss-0.9.9rc4.tar`

### file list

```diff
@@ -1,232 +1,232 @@
--rw-r--r--   0        0        0     5483 2024-04-03 21:50:07.351823 truss-0.9.9rc3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1842 2024-04-03 21:50:07.351823 truss-0.9.9rc3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2024-04-03 21:50:07.351823 truss-0.9.9rc3/LICENSE
--rw-r--r--   0        0        0     5107 2024-04-03 21:50:07.351823 truss-0.9.9rc3/README.md
--rw-r--r--   0        0        0      933 2024-04-03 21:50:07.351823 truss-0.9.9rc3/context_builder.Dockerfile
--rw-r--r--   0        0        0     2654 2024-04-04 23:25:04.174719 truss-0.9.9rc3/pyproject.toml
--rw-r--r--   0        0        0      255 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/__init__.py
--rw-r--r--   0        0        0      252 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0     4518 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/build.py
--rw-r--r--   0        0        0       51 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/cli/__init__.py
--rw-r--r--   0        0        0    19791 2024-04-04 23:24:58.070718 truss-0.9.9rc3/truss/cli/cli.py
--rw-r--r--   0        0        0      115 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/cli/console.py
--rw-r--r--   0        0        0      134 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/cli/create.py
--rw-r--r--   0        0        0     3096 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/config/trt_llm.py
--rw-r--r--   0        0        0     3259 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/constants.py
--rw-r--r--   0        0        0     7425 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/image_builder/cache_warmer.py
--rw-r--r--   0        0        0     1456 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0    18184 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     1561 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2120 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     5711 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/decorators.py
--rw-r--r--   0        0        0     3641 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/docker.py
--rw-r--r--   0        0        0      643 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/errors.py
--rw-r--r--   0        0        0      824 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     3934 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/model_inference.py
--rw-r--r--   0        0        0      510 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/notebook.py
--rw-r--r--   0        0        0    15195 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      139 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/constants.py
--rw-r--r--   0        0        0      908 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2110 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/hash.py
--rw-r--r--   0        0        0     2930 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/local_truss_patch_applier.py
--rw-r--r--   0        0        0      570 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/signature.py
--rw-r--r--   0        0        0     3410 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      960 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/patch/types.py
--rw-r--r--   0        0        0      237 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/pytest.ini
--rw-r--r--   0        0        0      705 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/readme_generator.py
--rw-r--r--   0        0        0      176 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/remote/baseten/__init__.py
--rw-r--r--   0        0        0     7767 2024-04-04 23:08:23.538679 truss-0.9.9rc3/truss/remote/baseten/api.py
--rw-r--r--   0        0        0      752 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/remote/baseten/auth.py
--rw-r--r--   0        0        0     7055 2024-04-04 22:16:40.358558 truss-0.9.9rc3/truss/remote/baseten/core.py
--rw-r--r--   0        0        0      541 2024-04-03 21:50:07.371823 truss-0.9.9rc3/truss/remote/baseten/error.py
--rw-r--r--   0        0        0    12334 2024-04-04 23:12:20.578689 truss-0.9.9rc3/truss/remote/baseten/remote.py
--rw-r--r--   0        0        0     3462 2024-04-04 23:11:06.938686 truss-0.9.9rc3/truss/remote/baseten/service.py
--rw-r--r--   0        0        0     1951 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/remote/baseten/utils/tar.py
--rw-r--r--   0        0        0      985 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/remote/baseten/utils/transfer.py
--rw-r--r--   0        0        0     1854 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/remote/remote_cli.py
--rw-r--r--   0        0        0     4219 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/remote/remote_factory.py
--rw-r--r--   0        0        0     7608 2024-04-04 23:10:42.998685 truss-0.9.9rc3/truss/remote/truss_remote.py
--rw-r--r--   0        0        0     2482 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/__init__.py
--rw-r--r--   0        0        0     2275 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     1026 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/cache.Dockerfile.jinja
--rw-r--r--   0        0        0       87 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/cache_requirements.txt
--rw-r--r--   0        0        0     3819 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     5397 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     6317 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     4245 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2652 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0      998 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1842 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     7419 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     5930 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     2354 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      158 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       98 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/copy_cache_files.Dockerfile.jinja
--rw-r--r--   0        0        0       48 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2561 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     2382 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     5758 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/schema.py
--rw-r--r--   0        0        0     2340 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/termination_handler_middleware.py
--rw-r--r--   0        0        0    14186 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      727 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0    16228 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      263 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     3196 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2024-04-03 21:50:07.375823 truss-0.9.9rc3/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1352 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/shared/logging.py
--rw-r--r--   0        0        0     2163 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0     3318 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/shared/serialization.py
--rw-r--r--   0        0        0     2396 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/shared/util.py
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/README.md
--rw-r--r--   0        0        0     4779 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/model/model.py
--rw-r--r--   0        0        0      860 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/build_engine_utils.py
--rw-r--r--   0        0        0      387 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/constants.py
--rw-r--r--   0        0        0     5775 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/schema.py
--rw-r--r--   0        0        0     5498 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt
--rw-r--r--   0        0        0     9023 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py
--rw-r--r--   0        0        0     2034 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt
--rw-r--r--   0        0        0    10875 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py
--rw-r--r--   0        0        0     2737 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt
--rw-r--r--   0        0        0     4457 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt
--rw-r--r--   0        0        0     4797 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/triton_client.py
--rw-r--r--   0        0        0     1729 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/templates/trtllm/packages/utils.py
--rw-r--r--   0        0        0      147 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/annotated_types_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/annotated_types_truss/model/__init__.py
--rw-r--r--   0        0        0      274 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/annotated_types_truss/model/model.py
--rw-r--r--   0        0        0    30286 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0      234 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/gcs_fix/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/gcs_fix/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/gcs_fix/model/model.py
--rw-r--r--   0        0        0     1394 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0       51 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1566 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0       57 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2024-04-03 21:50:07.379823 truss-0.9.9rc3/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0       44 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_async_truss/config.yaml
--rw-r--r--   0        0        0      646 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_async_truss/model/model.py
--rw-r--r--   0        0        0      238 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_basic_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_basic_truss/model/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_basic_truss/model/model.py
--rw-r--r--   0        0        0       34 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_concurrency_truss/config.yaml
--rw-r--r--   0        0        0      547 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_concurrency_truss/model/model.py
--rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v1/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v1/model/__init__.py
--rw-r--r--   0        0        0      850 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v1/model/model.py
--rw-r--r--   0        0        0       13 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v1/requirements.txt
--rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v2/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v2/model/__init__.py
--rw-r--r--   0        0        0      903 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v2/model/model.py
--rw-r--r--   0        0        0       14 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_pyantic_v2/requirements.txt
--rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_requirements_file_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_requirements_file_truss/model/__init__.py
--rw-r--r--   0        0        0     1106 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_requirements_file_truss/model/model.py
--rw-r--r--   0        0        0       13 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_requirements_file_truss/requirements.txt
--rw-r--r--   0        0        0       64 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_async_generator_truss/config.yaml
--rw-r--r--   0        0        0      521 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_async_generator_truss/model/model.py
--rw-r--r--   0        0        0      206 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_read_timeout/config.yaml
--rw-r--r--   0        0        0      636 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_read_timeout/model/model.py
--rw-r--r--   0        0        0       49 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_truss/config.yaml
--rw-r--r--   0        0        0      606 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_truss/model/model.py
--rw-r--r--   0        0        0       59 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_truss_with_error/config.yaml
--rw-r--r--   0        0        0      673 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_streaming_truss_with_error/model/model.py
--rw-r--r--   0        0        0       38 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        6 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss/packages/test_package/test.py
--rw-r--r--   0        0        0      352 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss_server_caching_truss/config.yaml
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss_server_caching_truss/model/__init__.py
--rw-r--r--   0        0        0      448 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/test_truss_server_caching_truss/model/model.py
--rw-r--r--   0        0        0       67 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/workflow_text_to_num/requirements.txt
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/workflow_text_to_num/user_package/__init__.py
--rw-r--r--   0        0        0      469 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/workflow_text_to_num/user_package/shared_processor.py
--rw-r--r--   0        0        0     2340 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/test_data/workflow_text_to_num/workflow.py
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/tests/__init__.py
--rw-r--r--   0        0        0    17477 2024-04-03 21:50:07.383823 truss-0.9.9rc3/truss/tests/conftest.py
--rw-r--r--   0        0        0    10496 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      555 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/helpers.py
--rw-r--r--   0        0        0        0 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0    19223 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0     1090 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      715 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     2604 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0     7658 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/remote/baseten/test_api.py
--rw-r--r--   0        0        0      580 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/remote/baseten/test_auth.py
--rw-r--r--   0        0        0     2589 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/remote/baseten/test_core.py
--rw-r--r--   0        0        0     8243 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/remote/baseten/test_remote.py
--rw-r--r--   0        0        0     4626 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/remote/test_remote_factory.py
--rw-r--r--   0        0        0     2475 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/remote/test_truss_remote.py
--rw-r--r--   0        0        0      283 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     6060 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     7513 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0     8326 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/control/control/test_server_integration.py
--rw-r--r--   0        0        0     1560 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/core/server/common/test_truss_server.py
--rw-r--r--   0        0        0      821 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2605 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/server/common/test_termination_handler_middleware.py
--rw-r--r--   0        0        0     3131 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     7941 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/templates/server/test_schema.py
--rw-r--r--   0        0        0     1952 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_build.py
--rw-r--r--   0        0        0     9997 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0    15051 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_control_truss_patching.py
--rw-r--r--   0        0        0      517 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_docker.py
--rw-r--r--   0        0        0    30398 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0    13995 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_model_schema.py
--rw-r--r--   0        0        0     1483 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2024-04-03 21:50:07.387823 truss-0.9.9rc3/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    28421 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0     1358 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/tests/test_util.py
--rw-r--r--   0        0        0     1865 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/tests/test_validation.py
--rw-r--r--   0        0        0     1888 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/tests/test_workflows.py
--rw-r--r--   0        0        0     7480 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/tests/util/test_path.py
--rw-r--r--   0        0        0    23145 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/truss_config.py
--rw-r--r--   0        0        0     2843 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/truss_gatherer.py
--rw-r--r--   0        0        0    37089 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/truss_handle.py
--rw-r--r--   0        0        0     5568 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/truss_spec.py
--rw-r--r--   0        0        0     2729 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/types.py
--rw-r--r--   0        0        0     3110 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/util/.truss_ignore
--rw-r--r--   0        0        0      379 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/util/data_structures.py
--rw-r--r--   0        0        0     2566 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/util/download.py
--rw-r--r--   0        0        0       46 2024-04-04 23:08:16.722679 truss-0.9.9rc3/truss/util/errors.py
--rw-r--r--   0        0        0      553 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/util/jinja.py
--rw-r--r--   0        0        0     6183 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/util/path.py
--rw-r--r--   0        0        0     2868 2024-04-03 21:50:07.391823 truss-0.9.9rc3/truss/validation.py
--rw-r--r--   0        0        0     6990 1970-01-01 00:00:00.000000 truss-0.9.9rc3/PKG-INFO
+-rw-r--r--   0        0        0     5483 2024-04-03 21:50:07.351823 truss-0.9.9rc4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1842 2024-04-03 21:50:07.351823 truss-0.9.9rc4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2024-04-03 21:50:07.351823 truss-0.9.9rc4/LICENSE
+-rw-r--r--   0        0        0     5107 2024-04-03 21:50:07.351823 truss-0.9.9rc4/README.md
+-rw-r--r--   0        0        0      933 2024-04-03 21:50:07.351823 truss-0.9.9rc4/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2654 2024-04-05 14:45:45.102542 truss-0.9.9rc4/pyproject.toml
+-rw-r--r--   0        0        0      255 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/__init__.py
+-rw-r--r--   0        0        0      252 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0     4518 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/build.py
+-rw-r--r--   0        0        0       51 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/cli/__init__.py
+-rw-r--r--   0        0        0    19837 2024-04-04 23:27:12.010724 truss-0.9.9rc4/truss/cli/cli.py
+-rw-r--r--   0        0        0      115 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/cli/console.py
+-rw-r--r--   0        0        0      134 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/cli/create.py
+-rw-r--r--   0        0        0     3096 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/config/trt_llm.py
+-rw-r--r--   0        0        0     3259 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/constants.py
+-rw-r--r--   0        0        0     7425 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/image_builder/cache_warmer.py
+-rw-r--r--   0        0        0     1456 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0    18184 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     1561 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2120 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     5711 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/docker.py
+-rw-r--r--   0        0        0      643 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/errors.py
+-rw-r--r--   0        0        0      824 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     3934 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/notebook.py
+-rw-r--r--   0        0        0    15195 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      139 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/constants.py
+-rw-r--r--   0        0        0      908 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2110 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/hash.py
+-rw-r--r--   0        0        0     2930 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      570 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/signature.py
+-rw-r--r--   0        0        0     3410 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      960 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/readme_generator.py
+-rw-r--r--   0        0        0      176 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/remote/baseten/__init__.py
+-rw-r--r--   0        0        0     7767 2024-04-04 23:08:23.538679 truss-0.9.9rc4/truss/remote/baseten/api.py
+-rw-r--r--   0        0        0      752 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/remote/baseten/auth.py
+-rw-r--r--   0        0        0     7055 2024-04-04 22:16:40.358558 truss-0.9.9rc4/truss/remote/baseten/core.py
+-rw-r--r--   0        0        0      541 2024-04-03 21:50:07.371823 truss-0.9.9rc4/truss/remote/baseten/error.py
+-rw-r--r--   0        0        0    12511 2024-04-05 14:15:11.458553 truss-0.9.9rc4/truss/remote/baseten/remote.py
+-rw-r--r--   0        0        0     3462 2024-04-04 23:11:06.938686 truss-0.9.9rc4/truss/remote/baseten/service.py
+-rw-r--r--   0        0        0     1951 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/remote/baseten/utils/tar.py
+-rw-r--r--   0        0        0      985 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/remote/baseten/utils/transfer.py
+-rw-r--r--   0        0        0     1854 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/remote/remote_cli.py
+-rw-r--r--   0        0        0     4219 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/remote/remote_factory.py
+-rw-r--r--   0        0        0     7608 2024-04-05 14:28:11.538549 truss-0.9.9rc4/truss/remote/truss_remote.py
+-rw-r--r--   0        0        0     2482 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     1026 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/cache.Dockerfile.jinja
+-rw-r--r--   0        0        0       87 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/cache_requirements.txt
+-rw-r--r--   0        0        0     3819 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     5397 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     6317 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     4245 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2652 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0      998 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1842 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     7419 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     5930 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     2354 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      158 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       98 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/copy_cache_files.Dockerfile.jinja
+-rw-r--r--   0        0        0       48 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2561 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     5758 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/schema.py
+-rw-r--r--   0        0        0     2340 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/termination_handler_middleware.py
+-rw-r--r--   0        0        0    14186 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0    16228 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      263 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     3196 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2024-04-03 21:50:07.375823 truss-0.9.9rc4/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     2163 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     2396 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/shared/util.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/README.md
+-rw-r--r--   0        0        0     4779 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/model/model.py
+-rw-r--r--   0        0        0      860 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/build_engine_utils.py
+-rw-r--r--   0        0        0      387 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/constants.py
+-rw-r--r--   0        0        0     5775 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/schema.py
+-rw-r--r--   0        0        0     5498 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt
+-rw-r--r--   0        0        0     9023 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py
+-rw-r--r--   0        0        0     2034 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt
+-rw-r--r--   0        0        0    10875 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py
+-rw-r--r--   0        0        0     2737 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt
+-rw-r--r--   0        0        0     4457 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt
+-rw-r--r--   0        0        0     4797 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/triton_client.py
+-rw-r--r--   0        0        0     1729 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/templates/trtllm/packages/utils.py
+-rw-r--r--   0        0        0      147 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/annotated_types_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/annotated_types_truss/model/__init__.py
+-rw-r--r--   0        0        0      274 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/annotated_types_truss/model/model.py
+-rw-r--r--   0        0        0    30286 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0      234 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/gcs_fix/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/gcs_fix/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/gcs_fix/model/model.py
+-rw-r--r--   0        0        0     1394 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0       51 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1566 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0       57 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-03 21:50:07.379823 truss-0.9.9rc4/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0       44 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_async_truss/config.yaml
+-rw-r--r--   0        0        0      646 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_async_truss/model/model.py
+-rw-r--r--   0        0        0      238 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_basic_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_basic_truss/model/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_basic_truss/model/model.py
+-rw-r--r--   0        0        0       34 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_concurrency_truss/config.yaml
+-rw-r--r--   0        0        0      547 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_concurrency_truss/model/model.py
+-rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v1/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v1/model/__init__.py
+-rw-r--r--   0        0        0      850 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v1/model/model.py
+-rw-r--r--   0        0        0       13 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v1/requirements.txt
+-rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v2/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v2/model/__init__.py
+-rw-r--r--   0        0        0      903 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v2/model/model.py
+-rw-r--r--   0        0        0       14 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_pyantic_v2/requirements.txt
+-rw-r--r--   0        0        0      270 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_requirements_file_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_requirements_file_truss/model/__init__.py
+-rw-r--r--   0        0        0     1106 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_requirements_file_truss/model/model.py
+-rw-r--r--   0        0        0       13 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_requirements_file_truss/requirements.txt
+-rw-r--r--   0        0        0       64 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_async_generator_truss/config.yaml
+-rw-r--r--   0        0        0      521 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_async_generator_truss/model/model.py
+-rw-r--r--   0        0        0      206 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_read_timeout/config.yaml
+-rw-r--r--   0        0        0      636 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_read_timeout/model/model.py
+-rw-r--r--   0        0        0       49 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_truss/config.yaml
+-rw-r--r--   0        0        0      606 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_truss/model/model.py
+-rw-r--r--   0        0        0       59 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_truss_with_error/config.yaml
+-rw-r--r--   0        0        0      673 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_streaming_truss_with_error/model/model.py
+-rw-r--r--   0        0        0       38 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        6 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss/packages/test_package/test.py
+-rw-r--r--   0        0        0      352 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss_server_caching_truss/config.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss_server_caching_truss/model/__init__.py
+-rw-r--r--   0        0        0      448 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/test_truss_server_caching_truss/model/model.py
+-rw-r--r--   0        0        0       67 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/workflow_text_to_num/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/workflow_text_to_num/user_package/__init__.py
+-rw-r--r--   0        0        0      469 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/workflow_text_to_num/user_package/shared_processor.py
+-rw-r--r--   0        0        0     2340 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/test_data/workflow_text_to_num/workflow.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/tests/__init__.py
+-rw-r--r--   0        0        0    17477 2024-04-03 21:50:07.383823 truss-0.9.9rc4/truss/tests/conftest.py
+-rw-r--r--   0        0        0    10496 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      555 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/helpers.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0    19223 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0     1090 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      715 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     2604 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0     6718 2024-04-05 14:39:15.542544 truss-0.9.9rc4/truss/tests/remote/baseten/test_api.py
+-rw-r--r--   0        0        0      580 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/remote/baseten/test_auth.py
+-rw-r--r--   0        0        0     2589 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/remote/baseten/test_core.py
+-rw-r--r--   0        0        0     8355 2024-04-05 14:45:17.750542 truss-0.9.9rc4/truss/tests/remote/baseten/test_remote.py
+-rw-r--r--   0        0        0     4626 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/remote/test_remote_factory.py
+-rw-r--r--   0        0        0     2582 2024-04-05 14:29:31.858548 truss-0.9.9rc4/truss/tests/remote/test_truss_remote.py
+-rw-r--r--   0        0        0      283 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     6060 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7513 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0     8326 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/control/control/test_server_integration.py
+-rw-r--r--   0        0        0     1560 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/core/server/common/test_truss_server.py
+-rw-r--r--   0        0        0      821 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2605 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/server/common/test_termination_handler_middleware.py
+-rw-r--r--   0        0        0     3131 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     7941 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/templates/server/test_schema.py
+-rw-r--r--   0        0        0     1952 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_build.py
+-rw-r--r--   0        0        0     9997 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    15051 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_docker.py
+-rw-r--r--   0        0        0    30398 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0    13995 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_model_schema.py
+-rw-r--r--   0        0        0     1483 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2024-04-03 21:50:07.387823 truss-0.9.9rc4/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    28421 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0     1358 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/tests/test_util.py
+-rw-r--r--   0        0        0     1865 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/tests/test_validation.py
+-rw-r--r--   0        0        0     1888 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/tests/test_workflows.py
+-rw-r--r--   0        0        0     7480 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/tests/util/test_path.py
+-rw-r--r--   0        0        0    23145 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/truss_config.py
+-rw-r--r--   0        0        0     2843 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    37089 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/truss_handle.py
+-rw-r--r--   0        0        0     5568 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/truss_spec.py
+-rw-r--r--   0        0        0     2729 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/types.py
+-rw-r--r--   0        0        0     3110 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/util/.truss_ignore
+-rw-r--r--   0        0        0      379 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/util/data_structures.py
+-rw-r--r--   0        0        0     2566 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/util/download.py
+-rw-r--r--   0        0        0       46 2024-04-04 23:08:16.722679 truss-0.9.9rc4/truss/util/errors.py
+-rw-r--r--   0        0        0      553 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/util/jinja.py
+-rw-r--r--   0        0        0     6183 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/util/path.py
+-rw-r--r--   0        0        0     2868 2024-04-03 21:50:07.391823 truss-0.9.9rc4/truss/validation.py
+-rw-r--r--   0        0        0     6990 1970-01-01 00:00:00.000000 truss-0.9.9rc4/PKG-INFO
```

### Comparing `truss-0.9.9rc3/CODE_OF_CONDUCT.md` & `truss-0.9.9rc4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/CONTRIBUTING.md` & `truss-0.9.9rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/LICENSE` & `truss-0.9.9rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/README.md` & `truss-0.9.9rc4/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/context_builder.Dockerfile` & `truss-0.9.9rc4/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/pyproject.toml` & `truss-0.9.9rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.9.9rc3"
+version = "0.9.9rc4"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = [
```

### Comparing `truss-0.9.9rc3/truss/blob/blob_backend_registry.py` & `truss-0.9.9rc4/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/blob/http_public_blob_backend.py` & `truss-0.9.9rc4/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/build.py` & `truss-0.9.9rc4/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/cli/cli.py` & `truss-0.9.9rc4/truss/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,15 +549,17 @@
                     if (
                         timeout_seconds is not None
                         and time.time() - start_time > timeout_seconds
                     ):
                         status.update("[bold red]Deployment timed out.")
                         sys.exit(1)
 
-                    status.update(f"[bold green]Deploying...Current Status: {deployment_status}")
+                    status.update(
+                        f"[bold green]Deploying...Current Status: {deployment_status}"
+                    )
 
                     if deployment_status == ACTIVE_STATUS:
                         console.print("Deployment succeeded.", style="bold green")
                         return
 
                     if deployment_status not in DEPLOYING_STATUSES:
                         console.print(
```

### Comparing `truss-0.9.9rc3/truss/config/trt_llm.py` & `truss-0.9.9rc4/truss/config/trt_llm.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/constants.py` & `truss-0.9.9rc4/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/image_builder/cache_warmer.py` & `truss-0.9.9rc4/truss/contexts/image_builder/cache_warmer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/image_builder/image_builder.py` & `truss-0.9.9rc4/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.9.9rc4/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/image_builder/util.py` & `truss-0.9.9rc4/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.9.9rc4/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/local_loader/load_model_local.py` & `truss-0.9.9rc4/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.9.9rc4/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/contexts/local_loader/utils.py` & `truss-0.9.9rc4/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/docker.py` & `truss-0.9.9rc4/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/errors.py` & `truss-0.9.9rc4/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/local/local_config.py` & `truss-0.9.9rc4/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/local/local_config_handler.py` & `truss-0.9.9rc4/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/model_inference.py` & `truss-0.9.9rc4/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/calc_patch.py` & `truss-0.9.9rc4/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/dir_signature.py` & `truss-0.9.9rc4/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/hash.py` & `truss-0.9.9rc4/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/local_truss_patch_applier.py` & `truss-0.9.9rc4/truss/patch/local_truss_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/signature.py` & `truss-0.9.9rc4/truss/patch/signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/truss_dir_patch_applier.py` & `truss-0.9.9rc4/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/patch/types.py` & `truss-0.9.9rc4/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/readme_generator.py` & `truss-0.9.9rc4/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/api.py` & `truss-0.9.9rc4/truss/remote/baseten/api.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/auth.py` & `truss-0.9.9rc4/truss/remote/baseten/auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/core.py` & `truss-0.9.9rc4/truss/remote/baseten/core.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/error.py` & `truss-0.9.9rc4/truss/remote/baseten/error.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/remote.py` & `truss-0.9.9rc4/truss/remote/baseten/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,24 +37,28 @@
     "https://app.baseten.co": "https://api.baseten.co",
     "https://app.staging.baseten.co": "https://api.staging.baseten.co",
     "https://app.dev.baseten.co": "https://api.staging.baseten.co",
     # For local development, this is how we map URLs
     "http://localhost:8000": "http://api.localhost:8000",
 }
 
+# If a non-standard domain is used with the baseten remote, default to 
+# using the production api routes
+DEFAULT_API_DOMAIN = "https://api.baseten.co"
+
 
 class BasetenRemote(TrussRemote):
     def __init__(self, remote_url: str, api_key: str, **kwargs):
         super().__init__(remote_url, **kwargs)
         self._auth_service = AuthService(api_key=api_key)
         self._api = BasetenApi(
             f"{self._remote_url}/graphql/",
             # Ensure we strip off trailing '/' to denormalize
             # URLs.
-            API_URL_MAPPING[self._remote_url.strip("/")],
+            API_URL_MAPPING.get(self._remote_url.strip("/"), DEFAULT_API_DOMAIN),
             self._auth_service,
         )
 
     def authenticate(self):
         return self._auth_service.validate()
 
     def push(  # type: ignore
```

### Comparing `truss-0.9.9rc3/truss/remote/baseten/service.py` & `truss-0.9.9rc4/truss/remote/baseten/service.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/utils/tar.py` & `truss-0.9.9rc4/truss/remote/baseten/utils/tar.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/baseten/utils/transfer.py` & `truss-0.9.9rc4/truss/remote/baseten/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/remote_cli.py` & `truss-0.9.9rc4/truss/remote/remote_cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/remote_factory.py` & `truss-0.9.9rc4/truss/remote/remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/remote/truss_remote.py` & `truss-0.9.9rc4/truss/remote/truss_remote.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/README.md.jinja` & `truss-0.9.9rc4/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/base.Dockerfile.jinja` & `truss-0.9.9rc4/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/cache.Dockerfile.jinja` & `truss-0.9.9rc4/truss/templates/cache.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/application.py` & `truss-0.9.9rc4/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/endpoints.py` & `truss-0.9.9rc4/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/errors.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/helpers/types.py` & `truss-0.9.9rc4/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/control/control/server.py` & `truss-0.9.9rc4/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/custom/model/model.py` & `truss-0.9.9rc4/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/errors.py` & `truss-0.9.9rc4/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.9.9rc4/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/patches.py` & `truss-0.9.9rc4/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/retry.py` & `truss-0.9.9rc4/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/schema.py` & `truss-0.9.9rc4/truss/templates/server/common/schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/termination_handler_middleware.py` & `truss-0.9.9rc4/truss/templates/server/common/termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/common/truss_server.py` & `truss-0.9.9rc4/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/inference_server.py` & `truss-0.9.9rc4/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server/model_wrapper.py` & `truss-0.9.9rc4/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/server.Dockerfile.jinja` & `truss-0.9.9rc4/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/shared/logging.py` & `truss-0.9.9rc4/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/shared/secrets_resolver.py` & `truss-0.9.9rc4/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/shared/serialization.py` & `truss-0.9.9rc4/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/shared/util.py` & `truss-0.9.9rc4/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/model/model.py` & `truss-0.9.9rc4/truss/templates/trtllm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/build_engine_utils.py` & `truss-0.9.9rc4/truss/templates/trtllm/packages/build_engine_utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/schema.py` & `truss-0.9.9rc4/truss/templates/trtllm/packages/schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt` & `truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/ensemble/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py` & `truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/1/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt` & `truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/postprocessing/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py` & `truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/1/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt` & `truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/preprocessing/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt` & `truss-0.9.9rc4/truss/templates/trtllm/packages/tensorrt_llm_model_repository/tensorrt_llm/config.pbtxt`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/triton_client.py` & `truss-0.9.9rc4/truss/templates/trtllm/packages/triton_client.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/templates/trtllm/packages/utils.py` & `truss-0.9.9rc4/truss/templates/trtllm/packages/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/auto-mpg.data` & `truss-0.9.9rc4/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/gcs_fix/model/model.py` & `truss-0.9.9rc4/truss/test_data/gcs_fix/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/happy.ipynb` & `truss-0.9.9rc4/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.9.9rc4/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/patch_ping_test_server/app.py` & `truss-0.9.9rc4/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/pima-indians-diabetes.csv` & `truss-0.9.9rc4/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/readme_int_example.md` & `truss-0.9.9rc4/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/readme_no_example.md` & `truss-0.9.9rc4/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/readme_str_example.md` & `truss-0.9.9rc4/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/server.Dockerfile` & `truss-0.9.9rc4/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_async_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_async_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_basic_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_basic_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_concurrency_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_concurrency_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_pyantic_v1/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_pyantic_v1/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_pyantic_v2/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_pyantic_v2/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_requirements_file_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_requirements_file_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_streaming_async_generator_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_streaming_async_generator_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_streaming_read_timeout/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_streaming_read_timeout/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_streaming_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_streaming_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_streaming_truss_with_error/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_streaming_truss_with_error/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/test_truss/model/model.py` & `truss-0.9.9rc4/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/test_data/workflow_text_to_num/workflow.py` & `truss-0.9.9rc4/truss/test_data/workflow_text_to_num/workflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/conftest.py` & `truss-0.9.9rc4/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.9.9rc4/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.9.9rc4/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.9.9rc4/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/helpers.py` & `truss-0.9.9rc4/truss/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/local/test_local_config_handler.py` & `truss-0.9.9rc4/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/patch/test_calc_patch.py` & `truss-0.9.9rc4/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/patch/test_dir_signature.py` & `truss-0.9.9rc4/truss/tests/patch/test_dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/patch/test_hash.py` & `truss-0.9.9rc4/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/patch/test_signature.py` & `truss-0.9.9rc4/truss/tests/patch/test_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.9.9rc4/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/remote/baseten/test_auth.py` & `truss-0.9.9rc4/truss/tests/remote/baseten/test_auth.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/remote/baseten/test_core.py` & `truss-0.9.9rc4/truss/tests/remote/baseten/test_core.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/remote/baseten/test_remote.py` & `truss-0.9.9rc4/truss/tests/remote/baseten/test_remote.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pytest
 import requests_mock
 from truss.remote.baseten.core import ModelId, ModelName, ModelVersionId
 from truss.remote.baseten.remote import BasetenRemote
 from truss.truss_handle import TrussHandle
 
 _TEST_REMOTE_URL = "http://test_remote.com"
+_TEST_REMOTE_GRAPHQL_PATH = "http://test_remote.com/graphql/"
 
 
 def test_get_service_by_version_id():
     remote = BasetenRemote(_TEST_REMOTE_URL, "api_key")
 
     version = {
         "id": "version_id",
@@ -17,29 +18,29 @@
             "id": "model_id",
         },
     }
     model_version_response = {"data": {"model_version": version}}
 
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_version_response,
         )
         service = remote.get_service(model_identifier=ModelVersionId("version_id"))
 
     assert service.model_id == "model_id"
     assert service.model_version_id == "version_id"
 
 
 def test_get_service_by_version_id_no_version():
     remote = BasetenRemote(_TEST_REMOTE_URL, "api_key")
     model_version_response = {"errors": [{"message": "error"}]}
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_version_response,
         )
         with pytest.raises(click.UsageError):
             remote.get_service(model_identifier=ModelVersionId("version_id"))
 
 
 def test_get_service_by_model_name():
@@ -58,15 +59,15 @@
                 "versions": versions,
             }
         }
     }
 
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
 
         # Check that the production version is returned when published is True.
         service = remote.get_service(
             model_identifier=ModelName("model_name"), published=True
         )
@@ -95,15 +96,15 @@
                 "versions": versions,
             }
         }
     }
 
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
 
         # Check that the production version is returned when published is True.
         service = remote.get_service(
             model_identifier=ModelName("model_name"), published=True
         )
@@ -132,15 +133,15 @@
                 "versions": versions,
             }
         }
     }
 
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
 
         # Since no production version exists, calling get_service with
         # published=True should raise an error.
         with pytest.raises(click.UsageError):
             remote.get_service(model_identifier=ModelName("model_name"), published=True)
@@ -164,29 +165,29 @@
                 "primary_version": {"id": "version_id"},
             }
         }
     }
 
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
 
         service = remote.get_service(model_identifier=ModelId("model_id"))
         assert service.model_id == "model_id"
         assert service.model_version_id == "version_id"
 
 
 def test_get_service_by_model_id_no_model():
     remote = BasetenRemote(_TEST_REMOTE_URL, "api_key")
     model_response = {"errors": [{"message": "error"}]}
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
         with pytest.raises(click.UsageError):
             remote.get_service(model_identifier=ModelId("model_id"))
 
 
 def test_push_raised_value_error_when_deployment_name_and_not_publish(
@@ -200,15 +201,15 @@
                 "id": "model_id",
                 "primary_version": {"id": "version_id"},
             }
         }
     }
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
         th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
 
         with pytest.raises(
             ValueError,
             match="Deployment name cannot be used for development deployment",
@@ -227,15 +228,15 @@
                 "id": "model_id",
                 "primary_version": {"id": "version_id"},
             }
         }
     }
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
         th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
 
         with pytest.raises(
             ValueError,
             match="Deployment name must only contain alphanumeric, -, _ and . characters",
@@ -254,15 +255,15 @@
                 "id": "model_id",
                 "primary_version": {"id": "version_id"},
             }
         }
     }
     with requests_mock.Mocker() as m:
         m.post(
-            remote._api._api_url,
+            _TEST_REMOTE_GRAPHQL_PATH,
             json=model_response,
         )
         th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
 
         with pytest.raises(
             ValueError,
             match="preserve-previous-production-deployment can only be used with the '--promote' option",
```

### Comparing `truss-0.9.9rc3/truss/tests/remote/test_remote_factory.py` & `truss-0.9.9rc4/truss/tests/remote/test_remote_factory.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/remote/test_truss_remote.py` & `truss-0.9.9rc4/truss/tests/remote/test_truss_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         if response.status_code == 200:
             return True
         return False
 
     def logs_url(self, base_url: str) -> str:
         return f"{base_url}/logs"
 
+    def poll_deployment_status():
+        for status in ["DEPLOYING", "ACTIVE"]:
+            yield status
+
 
 def mock_successful_response():
     response = Response()
     response.status_code = 200
     response.json = mock.Mock(return_value={"data": {"status": "success"}})
     return response
```

### Comparing `truss-0.9.9rc3/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.9.9rc4/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.9.9rc4/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/control/control/test_server.py` & `truss-0.9.9rc4/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/control/control/test_server_integration.py` & `truss-0.9.9rc4/truss/tests/templates/control/control/test_server_integration.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/core/server/common/test_truss_server.py` & `truss-0.9.9rc4/truss/tests/templates/core/server/common/test_truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/core/server/common/test_util.py` & `truss-0.9.9rc4/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.9.9rc4/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/server/common/test_retry.py` & `truss-0.9.9rc4/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/server/common/test_termination_handler_middleware.py` & `truss-0.9.9rc4/truss/tests/templates/server/common/test_termination_handler_middleware.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.9.9rc4/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/templates/server/test_schema.py` & `truss-0.9.9rc4/truss/tests/templates/server/test_schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_build.py` & `truss-0.9.9rc4/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_config.py` & `truss-0.9.9rc4/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_context_builder_image.py` & `truss-0.9.9rc4/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_control_truss_patching.py` & `truss-0.9.9rc4/truss/tests/test_control_truss_patching.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_docker.py` & `truss-0.9.9rc4/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_model_inference.py` & `truss-0.9.9rc4/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_model_schema.py` & `truss-0.9.9rc4/truss/tests/test_model_schema.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.9.9rc4/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_truss_gatherer.py` & `truss-0.9.9rc4/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_truss_handle.py` & `truss-0.9.9rc4/truss/tests/test_truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_util.py` & `truss-0.9.9rc4/truss/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_validation.py` & `truss-0.9.9rc4/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/test_workflows.py` & `truss-0.9.9rc4/truss/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/tests/util/test_path.py` & `truss-0.9.9rc4/truss/tests/util/test_path.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/truss_config.py` & `truss-0.9.9rc4/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/truss_gatherer.py` & `truss-0.9.9rc4/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/truss_handle.py` & `truss-0.9.9rc4/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/truss_spec.py` & `truss-0.9.9rc4/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/types.py` & `truss-0.9.9rc4/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/util/.truss_ignore` & `truss-0.9.9rc4/truss/util/.truss_ignore`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/util/download.py` & `truss-0.9.9rc4/truss/util/download.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/util/gpu.py` & `truss-0.9.9rc4/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/util/path.py` & `truss-0.9.9rc4/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/truss/validation.py` & `truss-0.9.9rc4/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.9.9rc3/PKG-INFO` & `truss-0.9.9rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.9.9rc3
+Version: 0.9.9rc4
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

