# Comparing `tmp/merlin-batch-predictor-0.41.3.tar.gz` & `tmp/merlin-batch-predictor-0.42.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-batch-predictor-0.41.3.tar", last modified: Thu Apr 18 09:05:42 2024, max compression
+gzip compressed data, was "merlin-batch-predictor-0.42.0rc1.tar", last modified: Thu May  2 15:21:50 2024, max compression
```

## Comparing `merlin-batch-predictor-0.41.3.tar` & `merlin-batch-predictor-0.42.0rc1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.404089 merlin-batch-predictor-0.41.3/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/docker/app.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/docker/base.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/docker/local-app.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/docker/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3910 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/docker/merlin_entrypoint.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1276 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/docker/process_conda_env.sh
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/go.mod
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/go.sum
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.400089 merlin-batch-predictor-0.41.3/integration_test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.404089 merlin-batch-predictor-0.41.3/integration_test/merlin/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/.helmignore
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/integration_test/merlin/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/templates/jobspec-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/templates/serviceaccount-secret.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/templates/spark-application.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/merlin/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/integration_test/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/scripts/init-credentials.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2497 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/scripts/run-test.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/integration_test/scripts/tear-down.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-18 09:05:42.000000 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-18 09:05:42.000000 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:05:42.000000 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 09:05:42.000000 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 09:05:42.000000 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-18 09:05:42.000000 merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/merlinpyspark/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5330 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/sink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/merlinpyspark/spec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/spec/prediction_job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/merlinpyspark/spec/prediction_job_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-18 09:05:41.000000 merlin-batch-predictor-0.41.3/merlinpyspark/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.404089 merlin-batch-predictor-0.41.3/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.400089 merlin-batch-predictor-0.41.3/pkg/github.com/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.400089 merlin-batch-predictor-0.41.3/pkg/github.com/caraml-dev/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.400089 merlin-batch-predictor-0.41.3/pkg/github.com/caraml-dev/merlin-pyspark-app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.400089 merlin-batch-predictor-0.41.3/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/spec/
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/spec/prediction_job.pb.json.go
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/pkg/spec/
--rw-r--r--   0 runner    (1001) docker     (127)    43262 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/pkg/spec/prediction_job.pb.go
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/pkg/spec/prediction_job.pb.json.go
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/requirements_test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.408089 merlin-batch-predictor-0.41.3/sample/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/sample/sample_1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/main_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/sink_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/source_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/test/util/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test/util/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/test-config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-config/.keep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/test-model/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-model/MLmodel
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:05:42.412089 merlin-batch-predictor-0.41.3/test-model/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-model/artifacts/model.joblib
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-model/conda.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-model/python_env.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-model/python_model.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 09:05:28.000000 merlin-batch-predictor-0.41.3/test-model/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.877251 merlin-batch-predictor-0.42.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-02 15:21:50.877251 merlin-batch-predictor-0.42.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.869251 merlin-batch-predictor-0.42.0rc1/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/docker/app.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/docker/base.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/docker/local-app.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/docker/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3910 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/docker/merlin_entrypoint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1276 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/docker/process_conda_env.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/go.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/go.sum
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.865251 merlin-batch-predictor-0.42.0rc1/integration_test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.869251 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/.helmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.869251 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/jobspec-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/serviceaccount-secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/spark-application.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/merlin/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.869251 merlin-batch-predictor-0.42.0rc1/integration_test/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      658 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/scripts/init-credentials.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2497 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/scripts/run-test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/integration_test/scripts/tear-down.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.869251 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/merlinpyspark/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5330 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5412 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/sink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/merlinpyspark/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/spec/prediction_job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/spec/prediction_job_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 15:21:50.000000 merlin-batch-predictor-0.42.0rc1/merlinpyspark/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.865251 merlin-batch-predictor-0.42.0rc1/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.865251 merlin-batch-predictor-0.42.0rc1/pkg/github.com/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.865251 merlin-batch-predictor-0.42.0rc1/pkg/github.com/caraml-dev/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.865251 merlin-batch-predictor-0.42.0rc1/pkg/github.com/caraml-dev/merlin-pyspark-app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.865251 merlin-batch-predictor-0.42.0rc1/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/spec/prediction_job.pb.json.go
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/pkg/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)    43262 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/pkg/spec/prediction_job.pb.go
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/pkg/spec/prediction_job.pb.json.go
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/sample/sample_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:21:50.877251 merlin-batch-predictor-0.42.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/sink_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/source_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/test/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test/util/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/test-config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-config/.keep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/test-model/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-model/MLmodel
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:21:50.873251 merlin-batch-predictor-0.42.0rc1/test-model/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-model/artifacts/model.joblib
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-model/conda.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-model/python_env.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-model/python_model.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 15:21:43.000000 merlin-batch-predictor-0.42.0rc1/test-model/requirements.txt
```

### Comparing `merlin-batch-predictor-0.41.3/.gitignore` & `merlin-batch-predictor-0.42.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/Makefile` & `merlin-batch-predictor-0.42.0rc1/Makefile`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/PKG-INFO` & `merlin-batch-predictor-0.42.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-batch-predictor
-Version: 0.41.3
+Version: 0.42.0rc1
 Summary: Base PySpark application for running Merlin prediction batch job
 Home-page: UNKNOWN
 Author-email: merlin-dev@gojek.com
 License: UNKNOWN
 Description: # Merlin Batch Predictor
         
         Merlin Batch Predictor is a PySpark application for running batch prediction job in Merlin system.
```

### Comparing `merlin-batch-predictor-0.41.3/README.md` & `merlin-batch-predictor-0.42.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/docker/app.Dockerfile` & `merlin-batch-predictor-0.42.0rc1/docker/app.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/docker/base.Dockerfile` & `merlin-batch-predictor-0.42.0rc1/docker/base.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/docker/local-app.Dockerfile` & `merlin-batch-predictor-0.42.0rc1/docker/local-app.Dockerfile`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/docker/merlin_entrypoint.sh` & `merlin-batch-predictor-0.42.0rc1/docker/merlin_entrypoint.sh`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/docker/process_conda_env.sh` & `merlin-batch-predictor-0.42.0rc1/docker/process_conda_env.sh`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/go.sum` & `merlin-batch-predictor-0.42.0rc1/go.sum`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/integration_test/merlin/templates/_helpers.tpl` & `merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/integration_test/merlin/templates/spark-application.yaml` & `merlin-batch-predictor-0.42.0rc1/integration_test/merlin/templates/spark-application.yaml`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/integration_test/merlin/values.yaml` & `merlin-batch-predictor-0.42.0rc1/integration_test/merlin/values.yaml`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/integration_test/scripts/init-credentials.sh` & `merlin-batch-predictor-0.42.0rc1/integration_test/scripts/init-credentials.sh`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/integration_test/scripts/run-test.sh` & `merlin-batch-predictor-0.42.0rc1/integration_test/scripts/run-test.sh`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/PKG-INFO` & `merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-batch-predictor
-Version: 0.41.3
+Version: 0.42.0rc1
 Summary: Base PySpark application for running Merlin prediction batch job
 Home-page: UNKNOWN
 Author-email: merlin-dev@gojek.com
 License: UNKNOWN
 Description: # Merlin Batch Predictor
         
         Merlin Batch Predictor is a PySpark application for running batch prediction job in Merlin system.
```

### Comparing `merlin-batch-predictor-0.41.3/merlin_batch_predictor.egg-info/SOURCES.txt` & `merlin-batch-predictor-0.42.0rc1/merlin_batch_predictor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/__init__.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/__main__.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/__main__.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/config.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/config.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/model.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/model.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/sink.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/sink.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/source.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/source.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/spec/prediction_job_pb2.py` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/spec/prediction_job_pb2.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/merlinpyspark/spec/prediction_job_pb2.pyi` & `merlin-batch-predictor-0.42.0rc1/merlinpyspark/spec/prediction_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/spec/prediction_job.pb.json.go` & `merlin-batch-predictor-0.42.0rc1/pkg/github.com/caraml-dev/merlin-pyspark-app/pkg/spec/prediction_job.pb.json.go`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/pkg/spec/prediction_job.pb.go` & `merlin-batch-predictor-0.42.0rc1/pkg/spec/prediction_job.pb.go`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/pkg/spec/prediction_job.pb.json.go` & `merlin-batch-predictor-0.42.0rc1/pkg/spec/prediction_job.pb.json.go`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/setup.py` & `merlin-batch-predictor-0.42.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/__init__.py` & `merlin-batch-predictor-0.42.0rc1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/config_test.py` & `merlin-batch-predictor-0.42.0rc1/test/config_test.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/conftest.py` & `merlin-batch-predictor-0.42.0rc1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/main_test.py` & `merlin-batch-predictor-0.42.0rc1/test/main_test.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/model_test.py` & `merlin-batch-predictor-0.42.0rc1/test/model_test.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/sink_test.py` & `merlin-batch-predictor-0.42.0rc1/test/sink_test.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/source_test.py` & `merlin-batch-predictor-0.42.0rc1/test/source_test.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test/util/test_utils.py` & `merlin-batch-predictor-0.42.0rc1/test/util/test_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test-model/artifacts/model.joblib` & `merlin-batch-predictor-0.42.0rc1/test-model/artifacts/model.joblib`

 * *Files identical despite different names*

### Comparing `merlin-batch-predictor-0.41.3/test-model/python_model.pkl` & `merlin-batch-predictor-0.42.0rc1/test-model/python_model.pkl`

 * *Files identical despite different names*

