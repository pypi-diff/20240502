# Comparing `tmp/acai_aws-2.0.1.tar.gz` & `tmp/acai_aws-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acai_aws-2.0.1.tar", last modified: Thu Oct 26 03:09:53 2023, max compression
+gzip compressed data, was "acai_aws-2.1.0.tar", last modified: Thu May  2 01:01:28 2024, max compression
```

## Comparing `acai_aws-2.0.1.tar` & `acai_aws-2.1.0.tar`

### file list

```diff
@@ -1,192 +1,192 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.199945 acai_aws-2.0.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-10-26 03:09:36.000000 acai_aws-2.0.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2023-10-26 03:09:53.199945 acai_aws-2.0.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2092 2023-10-26 03:09:36.000000 acai_aws-2.0.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.179945 acai_aws-2.0.1/acai_aws/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.179945 acai_aws-2.0.1/acai_aws/apigateway/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1826 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/config_validator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/exception.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5236 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.179945 acai_aws-2.0.1/acai_aws/apigateway/resolver/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5046 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1117 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3765 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/importer.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.179945 acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3026 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3099 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/mapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2701 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4058 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5449 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/apigateway/router.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.179945 acai_aws-2.0.1/acai_aws/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/base/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2729 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/base/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/base/no_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/base/placeholder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/base/record.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      530 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/json_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/common/logger/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/logger/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1974 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/logger/common_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/logger/decorator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/common/records/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/records/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/records/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/records/exception.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/records/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/records/requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3290 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/schema.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5751 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/common/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/documentdb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/documentdb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/documentdb/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2387 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/documentdb/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/documentdb/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/dynamodb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/dynamodb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/dynamodb/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/dynamodb/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/dynamodb/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/firehose/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/firehose/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/firehose/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/firehose/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/firehose/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.183945 acai_aws-2.0.1/acai_aws/generic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/generic/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/generic/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/generic/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/acai_aws/kinesis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/kinesis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/kinesis/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2141 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/kinesis/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/kinesis/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/acai_aws/mq/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/mq/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/mq/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2415 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/mq/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/mq/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/acai_aws/msk/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/msk/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/msk/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/msk/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/msk/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/acai_aws/s3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/s3/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1398 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/s3/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/s3/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/s3/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/acai_aws/sns/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sns/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sns/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2629 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sns/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sns/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/acai_aws/sqs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sqs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sqs/event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sqs/record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-10-26 03:09:36.000000 acai_aws-2.0.1/acai_aws/sqs/requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.179945 acai_aws-2.0.1/acai_aws.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2023-10-26 03:09:53.000000 acai_aws-2.0.1/acai_aws.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5245 2023-10-26 03:09:53.000000 acai_aws-2.0.1/acai_aws.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-10-26 03:09:53.000000 acai_aws-2.0.1/acai_aws.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-10-26 03:09:53.000000 acai_aws-2.0.1/acai_aws.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-10-26 03:09:53.000000 acai_aws-2.0.1/acai_aws.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-10-26 03:09:53.199945 acai_aws-2.0.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1413 2023-10-26 03:09:36.000000 acai_aws-2.0.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.187945 acai_aws-2.0.1/tests/acai_aws/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/apigateway/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/test_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/test_mapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6020 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/test_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6695 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/test_cacher.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4685 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/test_importer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/test_init.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/apigateway/router/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/router/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25749 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_directory_router.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23227 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_mapping_router.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23394 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_pattern_router.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2570 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_timeout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5015 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/test_config_validator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4917 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/test_endpoint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9556 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/test_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3040 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/test_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3853 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/apigateway/test_response.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/common/records/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/records/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/records/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/records/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3637 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/records/test_requirements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/test_json_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4655 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5365 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/test_schema.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5065 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/common/test_validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.191945 acai_aws-2.0.1/tests/acai_aws/documentdb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/documentdb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5554 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/documentdb/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/documentdb/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/documentdb/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/dynamodb/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/dynamodb/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7744 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/dynamodb/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/dynamodb/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1549 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/dynamodb/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/firehose/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/firehose/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5174 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/firehose/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1579 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/firehose/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/firehose/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/generic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/generic/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/generic/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/generic/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/kinesis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/kinesis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5163 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/kinesis/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/kinesis/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/kinesis/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/mq/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/mq/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/mq/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1891 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/mq/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/mq/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/msk/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/msk/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5231 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/msk/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/msk/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/msk/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.195945 acai_aws-2.0.1/tests/acai_aws/s3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/s3/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6695 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/s3/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2565 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/s3/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1499 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/s3/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.199945 acai_aws-2.0.1/tests/acai_aws/sns/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sns/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sns/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2027 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sns/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sns/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.199945 acai_aws-2.0.1/tests/acai_aws/sqs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sqs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sqs/test_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1602 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sqs/test_record.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/acai_aws/sqs/test_requirements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:53.199945 acai_aws-2.0.1/tests/mocks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-26 03:09:36.000000 acai_aws-2.0.1/tests/mocks/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.726246 acai_aws-2.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-02 01:01:09.000000 acai_aws-2.1.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-05-02 01:01:28.726246 acai_aws-2.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-02 01:01:09.000000 acai_aws-2.1.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.694246 acai_aws-2.1.0/acai_aws/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.694246 acai_aws-2.1.0/acai_aws/apigateway/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1826 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/config_validator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      875 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      557 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/exception.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5236 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.694246 acai_aws-2.1.0/acai_aws/apigateway/resolver/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5046 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1117 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3765 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/importer.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1782 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3026 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3099 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/mapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2701 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4058 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5305 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/apigateway/router.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2729 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/no_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/placeholder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/base/record.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      530 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/json_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/common/logger/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      241 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/logger/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1974 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/logger/common_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      749 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/logger/decorator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.698246 acai_aws-2.1.0/acai_aws/common/records/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      567 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/exception.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      273 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/records/requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6486 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/common/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/documentdb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2387 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      130 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/documentdb/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/dynamodb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      269 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2434 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/dynamodb/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/firehose/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      357 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1726 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/firehose/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/generic/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/generic/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/generic/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1383 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/generic/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/kinesis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2141 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/kinesis/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.702246 acai_aws-2.1.0/acai_aws/mq/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      428 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2415 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/mq/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/msk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      818 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1472 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/msk/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/s3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1398 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2326 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/s3/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/sns/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2629 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sns/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/acai_aws/sqs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2024-05-02 01:01:09.000000 acai_aws-2.1.0/acai_aws/sqs/requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.726246 acai_aws-2.1.0/acai_aws.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5245 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2024-05-02 01:01:28.000000 acai_aws-2.1.0/acai_aws.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2024-05-02 01:01:28.726246 acai_aws-2.1.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1413 2024-05-02 01:01:09.000000 acai_aws-2.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/tests/acai_aws/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.706246 acai_aws-2.1.0/tests/acai_aws/apigateway/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.710246 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.710246 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5896 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_mapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6020 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6695 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_cacher.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4685 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_importer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3277 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_init.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.710246 acai_aws-2.1.0/tests/acai_aws/apigateway/router/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27945 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_directory_router.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23227 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_mapping_router.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23394 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_pattern_router.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2570 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5015 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_config_validator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4917 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9556 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3052 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3903 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/apigateway/test_response.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/common/records/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      955 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      619 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3637 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/records/test_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_json_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4655 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5662 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_schema.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5966 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/common/test_validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/documentdb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5554 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1417 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      974 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/documentdb/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.714246 acai_aws-2.1.0/tests/acai_aws/dynamodb/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7744 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2860 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1549 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/dynamodb/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/firehose/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5174 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1579 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      954 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/firehose/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/generic/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/generic/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/generic/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1423 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/generic/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/kinesis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5163 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/kinesis/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.718246 acai_aws-2.1.0/tests/acai_aws/mq/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1891 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      894 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/mq/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/msk/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5231 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1404 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      908 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/msk/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/s3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6700 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2565 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1499 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/s3/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/sns/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2027 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sns/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.722246 acai_aws-2.1.0/tests/acai_aws/sqs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/test_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1602 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/test_record.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      904 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/acai_aws/sqs/test_requirements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:28.726246 acai_aws-2.1.0/tests/mocks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 01:01:09.000000 acai_aws-2.1.0/tests/mocks/__init__.py
```

### Comparing `acai_aws-2.0.1/LICENSE` & `acai_aws-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/PKG-INFO` & `acai_aws-2.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acai_aws
-Version: 2.0.1
+Version: 2.1.0
 Summary: DRY, configurable, opinionated, minimalist framework for use with AWS Serverless Lambdas
 Home-page: https://github.com/syngenta/acai-python.git
 Author: Paul Cruse III
 Author-email: paulcruse3@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -26,14 +26,17 @@
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
 Requires-Dist: icecream
 Requires-Dist: pyyaml
 Requires-Dist: simplejson
 Requires-Dist: xmltodict
 
+[![CircleCI](https://circleci.com/gh/syngenta/acai-python.svg?style=shield)](https://circleci.com/gh/syngenta/acai-python)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=syngenta_acai-python&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=syngenta_acai-python)
+
 # Acai AWS
 DRY, configurable, declarative node library for working with Amazon Web Service Lambdas.
 
 ## Features
 * Highly configurable apigateway internal router
 * Openapi schema adherence for all event types
 * Extensible and customizable middleware for validation and other tasks
```

### Comparing `acai_aws-2.0.1/README.md` & `acai_aws-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![CircleCI](https://circleci.com/gh/syngenta/acai-python.svg?style=shield)](https://circleci.com/gh/syngenta/acai-python)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=syngenta_acai-python&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=syngenta_acai-python)
+
 # Acai AWS
 DRY, configurable, declarative node library for working with Amazon Web Service Lambdas.
 
 ## Features
 * Highly configurable apigateway internal router
 * Openapi schema adherence for all event types
 * Extensible and customizable middleware for validation and other tasks
```

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/config_validator.py` & `acai_aws-2.1.0/acai_aws/apigateway/config_validator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/endpoint.py` & `acai_aws-2.1.0/acai_aws/apigateway/endpoint.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/exception.py` & `acai_aws-2.1.0/acai_aws/apigateway/exception.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/request.py` & `acai_aws-2.1.0/acai_aws/apigateway/request.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/requirements.py` & `acai_aws-2.1.0/acai_aws/apigateway/requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/__init__.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/cache.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/cache.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/importer.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/importer.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/base.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/base.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/directory.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/directory.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/mapping.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/mapping.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/resolver/modes/pattern.py` & `acai_aws-2.1.0/acai_aws/apigateway/resolver/modes/pattern.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/response.py` & `acai_aws-2.1.0/acai_aws/apigateway/response.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/apigateway/router.py` & `acai_aws-2.1.0/acai_aws/apigateway/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,17 @@
         return response
 
     def __run_before_all(self, request, response, endpoint):
         if not response.has_errors and self.__before_all and callable(self.__before_all):
             self.__before_all(request, response, endpoint.requirements)
 
     def __run_with_auth(self, request, response, endpoint):
-        if not response.has_errors and self.__auto_validate and self.__validator.request_has_security(request) and self.__with_auth and callable(self.__with_auth):
-            self.__with_auth(request, response, endpoint.requirements)
-        elif not response.has_errors and endpoint.requires_auth and self.__with_auth and callable(self.__with_auth):
-            self.__with_auth(request, response, endpoint.requirements)
+        if not response.has_errors and self.__with_auth and callable(self.__with_auth):
+            if (self.__auto_validate and self.__validator.request_has_security(request)) or endpoint.requires_auth:
+                self.__with_auth(request, response, endpoint.requirements)
 
     def __run_request_validation(self, request, response, endpoint):
         if not response.has_errors and self.__auto_validate:
             self.__validator.validate_request_with_openapi(request, response)
         elif not response.has_errors and endpoint.has_requirements:
             self.__validator.validate_request(request, response, endpoint.requirements)
```

### Comparing `acai_aws-2.0.1/acai_aws/base/event.py` & `acai_aws-2.1.0/acai_aws/base/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/json_helper.py` & `acai_aws-2.1.0/acai_aws/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/logger/common_logger.py` & `acai_aws-2.1.0/acai_aws/common/logger/common_logger.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/logger/decorator.py` & `acai_aws-2.1.0/acai_aws/common/logger/decorator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/records/event.py` & `acai_aws-2.1.0/acai_aws/common/records/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/records/exception.py` & `acai_aws-2.1.0/acai_aws/common/records/exception.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/records/requirements.py` & `acai_aws-2.1.0/acai_aws/common/records/requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/common/schema.py` & `acai_aws-2.1.0/acai_aws/common/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
-import os
 import json
+import inspect
 
 import jsonref
+from pydantic import BaseModel
 import yaml
 
 
 class Schema:
 
     def __init__(self, **kwargs):
         self.__schema = kwargs.get('schema')
@@ -20,25 +21,27 @@
     def load_schema_file(self):
         self.__get_full_spec()
 
     def get_openapi_spec(self):
         return self.__get_full_spec()
 
     def get_body_spec(self, required_body=None):
-        if self.__schema and isinstance(self.__schema, dict):
+        if required_body and inspect.isclass(required_body) and issubclass(required_body, BaseModel):
+            return required_body
+        elif self.__schema and isinstance(self.__schema, dict):
             body_spec = self.__schema
         elif required_body and isinstance(required_body, dict):
             body_spec = required_body
-        else:
+        elif required_body and isinstance(required_body, str):
             body_spec = self.__get_component_spec(required_body)
         body_spec['additionalProperties'] = self.__config.get('allow_additional_properties', False)
         return body_spec
-
+    
     def get_route_spec(self, route, method):
-        return self.__get_route_spec(route, method)
+        return self.__get_route_spec(route, method)        
 
     def __get_full_spec(self):
         if not self.spec and self.__schema:
             unresolved_spec = self.__get_spec_from_file()
             resolved_spec = jsonref.loads(json.dumps(unresolved_spec), jsonschema=True, merge_props=True)
             self.__spec = self.__combine_all_of_spec(resolved_spec)
         return self.spec
```

### Comparing `acai_aws-2.0.1/acai_aws/common/validator.py` & `acai_aws-2.1.0/acai_aws/common/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import defaultdict
 
 from jsonschema import Draft7Validator
+from pydantic import BaseModel, ValidationError
 
 from acai_aws.common.schema import Schema
 
 
 class Validator:
 
     def __init__(self, **kwargs):
@@ -90,19 +91,26 @@
             avail_list += requirements['required_query']
         elif required == 'available_headers' and requirements.get('required_headers'):
             avail_list += requirements['required_headers']
         return avail_list
 
     @staticmethod
     def check_required_body(response, schema, request_body):
-        if schema:
+        if not Validator.is_json(response, request_body):
+            return False
+        if schema and isinstance(schema, dict):
             schema_validator = Draft7Validator(schema)
             for schema_error in sorted(schema_validator.iter_errors(request_body), key=str):
                 error_key = Validator.format_schema_error_key(schema_error)
                 response.set_error(key_path=error_key, message=schema_error.message)
+        elif issubclass(schema, BaseModel):
+            try:
+                schema(**request_body)
+            except ValidationError as error:
+                [response.set_error(key_path='.'.join(error['loc']), message=error['msg']) for error in error.errors()]
 
     @staticmethod
     def combine_parameters(parameters):
         requirements = defaultdict(lambda: [])
         for param in parameters:
             if param.get('in') == 'query' and param.get('required'):
                 requirements['required_query'].append(param['name'])
@@ -114,7 +122,14 @@
                 requirements['available_headers'].append(param['name'])
         return dict(requirements)
 
     @staticmethod
     def format_schema_error_key(schema_error):
         error_path = '.'.join(str(path) for path in schema_error.path)
         return error_path if error_path else 'root'
+
+    @staticmethod
+    def is_json(response, request_body):
+        if not isinstance(request_body, dict):
+            response.set_error('body', 'Expecting JSON request body; please make sure using proper content-type headers and body string is properly encoded')
+            return False
+        return True
```

### Comparing `acai_aws-2.0.1/acai_aws/documentdb/record.py` & `acai_aws-2.1.0/acai_aws/documentdb/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/dynamodb/record.py` & `acai_aws-2.1.0/acai_aws/dynamodb/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/firehose/record.py` & `acai_aws-2.1.0/acai_aws/firehose/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/generic/requirements.py` & `acai_aws-2.1.0/acai_aws/generic/requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/kinesis/record.py` & `acai_aws-2.1.0/acai_aws/kinesis/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/mq/record.py` & `acai_aws-2.1.0/acai_aws/mq/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/msk/event.py` & `acai_aws-2.1.0/acai_aws/msk/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/msk/record.py` & `acai_aws-2.1.0/acai_aws/msk/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/s3/event.py` & `acai_aws-2.1.0/acai_aws/s3/event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/s3/record.py` & `acai_aws-2.1.0/acai_aws/s3/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/sns/record.py` & `acai_aws-2.1.0/acai_aws/sns/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws/sqs/record.py` & `acai_aws-2.1.0/acai_aws/sqs/record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/acai_aws.egg-info/PKG-INFO` & `acai_aws-2.1.0/acai_aws.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: acai-aws
-Version: 2.0.1
+Name: acai_aws
+Version: 2.1.0
 Summary: DRY, configurable, opinionated, minimalist framework for use with AWS Serverless Lambdas
 Home-page: https://github.com/syngenta/acai-python.git
 Author: Paul Cruse III
 Author-email: paulcruse3@gmail.com
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
@@ -26,14 +26,17 @@
 Requires-Dist: jsonref
 Requires-Dist: jsonschema
 Requires-Dist: icecream
 Requires-Dist: pyyaml
 Requires-Dist: simplejson
 Requires-Dist: xmltodict
 
+[![CircleCI](https://circleci.com/gh/syngenta/acai-python.svg?style=shield)](https://circleci.com/gh/syngenta/acai-python)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=syngenta_acai-python&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=syngenta_acai-python)
+
 # Acai AWS
 DRY, configurable, declarative node library for working with Amazon Web Service Lambdas.
 
 ## Features
 * Highly configurable apigateway internal router
 * Openapi schema adherence for all event types
 * Extensible and customizable middleware for validation and other tasks
```

### Comparing `acai_aws-2.0.1/acai_aws.egg-info/SOURCES.txt` & `acai_aws-2.1.0/acai_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/setup.py` & `acai_aws-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/test_directory.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_directory.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/test_mapping.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_mapping.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/modes/test_pattern.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/modes/test_pattern.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/test_cacher.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_cacher.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/test_importer.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_importer.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/resolver/test_init.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/resolver/test_init.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_directory_router.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_directory_router.py`

 * *Files 5% similar despite different names*

```diff
@@ -595,42 +595,99 @@
                         'message': 'There was a problem with the APIs response; does not match defined schema'
                     }
                 ]
             },
             json_dict_response
         )
 
-    def test_basic_directory_routing_fails_with_response_body(self):
+    def test_basic_directory_routing_passes_with_pydantic_response_body(self):
         dynamic_event = self.mock_request.get_dynamic_event(
-            headers={'x-api-key': 'some-key'},
-            path='unit-test/v1/auto',
+            headers={'x-api-key': 'some-key', 'content-type': 'application/json'},
+            path='unit-test/v1/pydantic',
             proxy='auto',
-            method='delete'
+            method='post',
+            body={'id': 1, 'email': 'test@test.com', 'active': True, 'favorites': ['pizza'], 'notification_config': {'email': True}}
         )
         router = Router(
             base_path=self.base_path,
             handlers=self.handler_path,
             schema=self.schema_path,
             validate_response=True
         )
         result = router.route(dynamic_event, None)
         json_dict_response = json.loads(result['body'])
-        self.assertEqual(500, result['statusCode'])
+        self.assertEqual(200, result['statusCode'])
+        self.assertDictEqual({'pydantic_pass': True}, json_dict_response)
+
+    def test_basic_directory_routing_fails_with_pydantic_response_body(self):
+        dynamic_event = self.mock_request.get_dynamic_event(
+            headers={'x-api-key': 'some-key', 'content-type': 'application/json'},
+            path='unit-test/v1/pydantic',
+            proxy='auto',
+            method='post',
+            body={'fails': True}
+        )
+        router = Router(
+            base_path=self.base_path,
+            handlers=self.handler_path,
+            schema=self.schema_path,
+            validate_response=True
+        )
+        result = router.route(dynamic_event, None)
+        json_dict_response = json.loads(result['body'])
+        self.assertEqual(400, result['statusCode'])
         self.assertDictEqual(
             {
                 'errors': [
                     {
-                        'key_path': 'root',
-                        'message': "'data' is a required property"
-                    },
-                    {
-                        'key_path': 'root',
-                        'message': "Additional properties are not allowed ('bad-delete' was unexpected)"
-                    },
+                        'key_path': 'id', 
+                        'message': 'Field required'
+                    }, 
                     {
-                        'key_path': 'response',
-                        'message': 'There was a problem with the APIs response; does not match defined schema'
+                        'key_path': 'email', 
+                        'message': 'Field required'
+                    }, 
+                    {
+                        'key_path': 'active', 
+                        'message': 'Field required'
+                    }, 
+                    {
+                        'key_path': 'favorites', 
+                        'message': 'Field required'
+                    }, 
+                    {
+                        'key_path': 'notification_config', 
+                        'message': 'Field required'
                     }
                 ]
-            },
+            }, 
+            json_dict_response
+        )
+    
+    def test_basic_directory_routing_fails_with_non_json_body(self):
+        dynamic_event = self.mock_request.get_dynamic_event(
+            headers={'x-api-key': 'some-key'},
+            path='unit-test/v1/pydantic',
+            proxy='auto',
+            method='post',
+            body={'fails': True}
+        )
+        router = Router(
+            base_path=self.base_path,
+            handlers=self.handler_path,
+            schema=self.schema_path,
+            validate_response=True
+        )
+        result = router.route(dynamic_event, None)
+        json_dict_response = json.loads(result['body'])
+        self.assertEqual(400, result['statusCode'])
+        self.assertDictEqual(
+            {
+                'errors': [
+                    {
+                        'key_path': 'body', 
+                        'message': 'Expecting JSON request body; please make sure using proper content-type headers and body string is properly encoded'
+                    }
+                ]
+            }, 
             json_dict_response
         )
```

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_mapping_router.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_mapping_router.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_pattern_router.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_pattern_router.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/router/test_timeout.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/router/test_timeout.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/test_config_validator.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/test_config_validator.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/test_endpoint.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/test_request.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/test_request.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/test_requirements.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 from acai_aws.apigateway.exception import ApiTimeOutException
 from acai_aws.apigateway.request import Request
 from acai_aws.apigateway.response import Response
 
 from tests.mocks.apigateway import mock_request
-from tests.mocks.apigateway.requirements.basic import post, get, patch, before_call, after_call, call_order
+from tests.mocks.apigateway.requirements import basic
 
 
 class ApigatewayRequirementsTest(unittest.TestCase):
     basic_request = mock_request.get_basic()
     expected_data_class_result = {
         'hasErrors': False,
         'response': {
@@ -22,64 +22,62 @@
             'body': {
                 'requirements_basic': True
             }
         }
     }
 
     def test_requirements_decorator_has_attribute(self):
-        self.assertTrue(hasattr(post, 'requirements'))
+        self.assertTrue(hasattr(basic.post, 'requirements'))
 
     def test_requirements_runs_before(self):
         request = Request(self.basic_request)
         response = Response()
-        post(request, response)
-        self.assertTrue(before_call.has_been_called)
+        basic.post(request, response)
+        self.assertTrue(basic.before_call.has_been_called)
 
     def test_requirements_runs_after(self):
         request = Request(self.basic_request)
         response = Response()
-        post(request, response)
-        self.assertTrue(after_call.has_been_called)
+        basic.post(request, response)
+        self.assertTrue(basic.after_call.has_been_called)
 
     def test_requirements_runs_in_correct_order(self):
         request = Request(self.basic_request)
         response = Response()
-        post(request, response)
-        self.assertEqual('before', call_order[0])
-        self.assertEqual('after', call_order[1])
+        basic.post(request, response)
+        self.assertEqual('before', basic.call_order[0])
+        self.assertEqual('after', basic.call_order[1])
 
     def test_requirements_passes_after_data_class(self):
         request = Request(self.basic_request)
         response = Response()
-        result = post(request, response)
+        result = basic.post(request, response)
         self.assertEqual(str(self.expected_data_class_result), str(result))
     
     def test_requirements_global_timeout_raises_exception(self):
         request = Request(self.basic_request, None, 1)
         response = Response()
         try:
-            get(request, response)
+            basic.get(request, response)
             self.assertTrue(False)
         except ApiTimeOutException as error:
             self.assertTrue(isinstance(error, ApiTimeOutException))
         
     def test_requirements_local_timeout_raises_exception(self):
         event = mock_request.get_dynamic_event(method='patch')
         request = Request(event)
         response = Response()
         try:
-            patch(request, response)
+            basic.patch(request, response)
             self.assertTrue(False)
         except ApiTimeOutException as error:
             self.assertTrue(isinstance(error, ApiTimeOutException))
         
     def test_requirements_local_overwrites_global_timeout_setting(self):
         event = mock_request.get_dynamic_event(method='patch')
         request = Request(event, None, 10)
         response = Response()
         try:
-            patch(request, response)
+            basic.patch(request, response)
             self.assertTrue(False)
         except ApiTimeOutException as error:
-            self.assertTrue(isinstance(error, ApiTimeOutException))
-
-        
+            self.assertTrue(isinstance(error, ApiTimeOutException))
```

### Comparing `acai_aws-2.0.1/tests/acai_aws/apigateway/test_response.py` & `acai_aws-2.1.0/tests/acai_aws/apigateway/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     def test_closed_cors_headers(self):
         self.response.cors = False
         self.assertDictEqual(self.response.headers, {})
     
     def test_closed_open_cors_headers(self):
         self.response.open_cors = False
         self.assertDictEqual(self.response.headers, {})
+        self.assertFalse(self.response.open_cors)
 
     def test_header_assignment(self):
         self.response.headers = ('some-key', 'some-value')
         self.assertDictEqual(
             self.response.headers, {
                 'Access-Control-Allow-Origin': '*',
                 'Access-Control-Allow-Headers': '*',
```

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/records/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/common/records/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/records/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/common/records/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/records/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/common/records/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/test_json_helper.py` & `acai_aws-2.1.0/tests/acai_aws/common/test_json_helper.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/test_logger.py` & `acai_aws-2.1.0/tests/acai_aws/common/test_logger.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/test_schema.py` & `acai_aws-2.1.0/tests/acai_aws/common/test_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import unittest
 
+from pydantic import BaseModel
+
 from acai_aws.common.schema import Schema
+from tests.mocks.common.mock_pydantic_class import Request
 
 
 class SchemaTest(unittest.TestCase):
     maxDiff = None
     schema_path = 'tests/mocks/common/openapi.yml'
     schema_dict = {
         'type': 'object',
@@ -168,12 +171,17 @@
         spec = schema.get_body_spec('v1-test-request')
         self.assertDictEqual(self.expected_combined_dict, spec)
 
     def test_get_body_spec_from_dict(self):
         schema = Schema(schema=self.schema_dict)
         spec = schema.get_body_spec()
         self.assertDictEqual(self.expected_dict_from_dict, spec)
+    
+    def test_get_body_spec_from_pydantic_model(self):
+        schema = Schema(schema=self.schema_path)
+        spec = schema.get_body_spec(Request)
+        self.assertTrue(issubclass(spec, BaseModel))
 
     def test_get_spec_from_route(self):
         schema = Schema(schema=self.schema_path)
         spec = schema.get_route_spec('/unit-test/v1/schema', 'get')
         self.assertDictEqual(self.expected_route_spec, spec)
```

### Comparing `acai_aws-2.0.1/tests/acai_aws/common/test_validator.py` & `acai_aws-2.1.0/tests/acai_aws/common/test_validator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import unittest
 
 from acai_aws.apigateway.request import Request
 from acai_aws.apigateway.response import Response
 from acai_aws.common.validator import Validator
 
 from tests.mocks.apigateway import mock_request
+from tests.mocks.common.mock_pydantic_class import UserRequest
 
 
 class ValidatorTest(unittest.TestCase):
     schema_path = 'tests/mocks/common/openapi.yml'
 
     def setUp(self):
         self.validator = Validator(schema=self.schema_path)
@@ -115,7 +116,26 @@
         self.assertTrue(response.has_errors)
         self.assertEqual('{"errors": [{"key_path": "root", "message": "\'id\' is a required property"}]}', response.body)
 
     def test_validate_request_with_openapi_passes(self):
         request = Request(mock_request.get_auto_validated_data())
         response = Response()
         self.validator.validate_request_with_openapi(request, response)
+    
+    def test_required_pydantic_body_pass(self):
+        request = Request(mock_request.get_basic_passing_for_required_body_validation())
+        response = Response()
+        requirements = {
+            'required_body': UserRequest
+        }
+        self.validator.validate_request(request, response, requirements)
+        self.assertFalse(response.has_errors)
+    
+    def test_required_pydantic_body_fail(self):
+        request = Request(mock_request.get_basic_failing_for_required_body_validation())
+        response = Response()
+        requirements = {
+            'required_body': UserRequest
+        }
+        self.validator.validate_request(request, response, requirements)
+        self.assertTrue(response.has_errors)
+        self.assertEqual('{"errors": [{"key_path": "id", "message": "Field required"}]}', response.body)
```

### Comparing `acai_aws-2.0.1/tests/acai_aws/documentdb/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/documentdb/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/documentdb/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/documentdb/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/documentdb/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/documentdb/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/dynamodb/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/dynamodb/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/dynamodb/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/dynamodb/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/dynamodb/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/dynamodb/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/firehose/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/firehose/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/firehose/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/firehose/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/firehose/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/firehose/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/generic/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/generic/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/kinesis/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/kinesis/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/kinesis/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/kinesis/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/kinesis/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/kinesis/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/mq/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/mq/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/mq/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/mq/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/mq/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/mq/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/msk/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/msk/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/msk/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/msk/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/msk/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/msk/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/s3/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/s3/test_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import unittest
-from moto import mock_s3
+from moto import mock_aws
 import boto3
 import jsonpickle
 
 from acai_aws.s3.event import Event
 from acai_aws.s3.record import Record
 from acai_aws.common.records.exception import RecordException
 
 from tests.mocks.s3 import mock_event
 from tests.mocks.s3.mock_data_class import MockS3DataClass
 
 
 class S3EventTest(unittest.TestCase):
     basic_event = mock_event.get_basic()
     csv_event = mock_event.get_basic_csv()
-    mock_s3 = mock_s3()
+    mock_aws = mock_aws()
     schema_path = 'tests/mocks/s3/openapi.yml'
     starting_csv_string = ['Name,Job,Age,Income', 'Alice,Programmer,23,110000', 'Bob,Executive,34,90000', 'Carl,Sales,45,50000']
     expected_json_data = {
         'lang': 'en-us',
         'sms': False,
         'email': True,
         'push': True
@@ -26,15 +26,15 @@
     expected_csv_data = [
         {'Name': 'Alice', 'Job': 'Programmer', 'Age': '23', 'Income': '110000'},
         {'Name': 'Bob', 'Job': 'Executive', 'Age': '34', 'Income': '90000'},
         {'Name': 'Carl', 'Job': 'Sales', 'Age': '45', 'Income': '50000'}
     ]
 
     def setUp(self):
-        self.mock_s3.start()
+        self.mock_aws.start()
         self.bucket_name = self.basic_event['Records'][0]['s3']['bucket']['name']
         self.s3_json_key = self.basic_event['Records'][0]['s3']['object']['key']
         self.s3_csv_key = self.csv_event['Records'][0]['s3']['object']['key']
         s3 = boto3.resource('s3')
         bucket = s3.Bucket(self.bucket_name)
         bucket.create(CreateBucketConfiguration={'LocationConstraint': 'us-east-2'})
         json_data = jsonpickle.dumps(self.expected_json_data, unpicklable=False, use_decimal=True)
@@ -42,15 +42,15 @@
         s3_json_object = s3.Object(self.bucket_name, self.s3_json_key)
         s3_json_object.put(Body=json_data)
         csv_data = bytes('\n'.join(self.starting_csv_string).encode('UTF-8'))
         s3_csv_object = s3.Object(self.bucket_name, self.s3_csv_key)
         s3_csv_object.put(Body=csv_data)
 
     def tearDown(self):
-        self.mock_s3.stop()
+        self.mock_aws.stop()
 
     def test_event_accepts_event(self):
         event = Event(self.basic_event)
         self.assertEqual(event.context, None)
         self.assertEqual(event.data_class, None)
         self.assertDictEqual(event.event, self.basic_event)
         self.assertEqual(len(event.records), len(self.basic_event['Records']))
```

### Comparing `acai_aws-2.0.1/tests/acai_aws/s3/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/s3/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/s3/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/s3/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/sns/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/sns/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/sns/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/sns/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/sns/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/sns/test_requirements.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/sqs/test_event.py` & `acai_aws-2.1.0/tests/acai_aws/sqs/test_event.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/sqs/test_record.py` & `acai_aws-2.1.0/tests/acai_aws/sqs/test_record.py`

 * *Files identical despite different names*

### Comparing `acai_aws-2.0.1/tests/acai_aws/sqs/test_requirements.py` & `acai_aws-2.1.0/tests/acai_aws/sqs/test_requirements.py`

 * *Files identical despite different names*

