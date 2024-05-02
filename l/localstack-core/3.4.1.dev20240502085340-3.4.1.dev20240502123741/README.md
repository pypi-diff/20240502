# Comparing `tmp/localstack_core-3.4.1.dev20240502085340.tar.gz` & `tmp/localstack_core-3.4.1.dev20240502123741.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack_core-3.4.1.dev20240502085340.tar", last modified: Thu May  2 08:54:04 2024, max compression
+gzip compressed data, was "localstack_core-3.4.1.dev20240502123741.tar", last modified: Thu May  2 12:38:04 2024, max compression
```

## Comparing `localstack_core-3.4.1.dev20240502085340.tar` & `localstack_core-3.4.1.dev20240502123741.tar`

### file list

```diff
@@ -1,1383 +1,1383 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.403066 localstack_core-3.4.1.dev20240502085340/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19977 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5464 2024-05-02 08:54:04.403066 localstack_core-3.4.1.dev20240502085340/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13116 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/README.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       24 2024-05-02 08:53:40.000000 localstack_core-3.4.1.dev20240502085340/VERSION
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.735076 localstack_core-3.4.1.dev20240502085340/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     6157 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.739076 localstack_core-3.4.1.dev20240502085340/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.747075 localstack_core-3.4.1.dev20240502085340/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3043 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.747075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.747075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17659 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.747075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75049 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.751075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10739 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.751075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   106163 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.751075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43772 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.755075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   135405 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.755075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    87711 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.759075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6954 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.759075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   811395 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.763075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    63522 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.763075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    56604 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.767075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48880 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.767075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   106761 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.771075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27200 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.771075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52805 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.771075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74323 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.775075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59701 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.775075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    78880 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.775075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   148750 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.779075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14828 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.779075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8623 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.779075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69704 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.779075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    58025 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.783075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   142987 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.783075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89829 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.787075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15493 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/scheduler/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.787075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23419 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.787075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55788 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.787075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28332 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.787075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19153 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.791075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   220012 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.791075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    44031 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.791075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10092 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.795075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16813 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.795075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60518 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.795075 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47602 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4972 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8024 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26256 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/connect.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.719076 localstack_core-3.4.1.dev20240502085340/localstack/aws/data/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.719076 localstack_core-3.4.1.dev20240502085340/localstack/aws/data/sqs-json/
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.799075 localstack_core-3.4.1.dev20240502085340/localstack/aws/data/sqs-json/2012-11-05/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      793 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/data/sqs-json/2012-11-05/README.md
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36725 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/data/sqs-json/2012-11-05/service-2.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12084 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      687 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.807075 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1876 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2455 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10596 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1464 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1790 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1628 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6079 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6241 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12518 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      988 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11678 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3577 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13778 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.815075 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50501 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    80430 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18967 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5317 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19961 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.819074 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3918 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5852 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/twisted.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2093 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8216 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37980 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11599 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12838 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.823074 localstack_core-3.4.1.dev20240502085340/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30929 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4222 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      877 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    58425 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7725 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12965 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.823074 localstack_core-3.4.1.dev20240502085340/localstack/dev/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.823074 localstack_core-3.4.1.dev20240502085340/localstack/dev/kubernetes/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/kubernetes/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6325 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/kubernetes/__main__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.827074 localstack_core-3.4.1.dev20240502085340/localstack/dev/run/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/run/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12603 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/run/__main__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13833 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/run/configurators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dev/run/paths.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.827074 localstack_core-3.4.1.dev20240502085340/localstack/dns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5785 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1428 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dns/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33217 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/dns/server.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.827074 localstack_core-3.4.1.dev20240502085340/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       96 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.831074 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      139 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      739 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2867 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.831074 localstack_core-3.4.1.dev20240502085340/localstack/extensions/patterns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/patterns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13465 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/extensions/patterns/webapp.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.839074 localstack_core-3.4.1.dev20240502085340/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      471 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      755 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/duplex_socket.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5356 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      115 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      418 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      591 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      300 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/http/websocket.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.839074 localstack_core-3.4.1.dev20240502085340/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5078 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.847074 localstack_core-3.4.1.dev20240502085340/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16302 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14645 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1310 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      898 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.851074 localstack_core-3.4.1.dev20240502085340/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4126 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3112 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7332 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      818 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2276 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.859074 localstack_core-3.4.1.dev20240502085340/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.859074 localstack_core-3.4.1.dev20240502085340/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.871074 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6310 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13445 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/exporter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69249 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47983 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15097 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3248 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9586 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   115626 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.895073 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2896 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_account.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1081 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3726 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4214 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1855 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11600 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4719 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2565 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3494 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8627 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_method.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10052 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3757 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_model.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2020 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1917 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      632 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1788 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      592 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7513 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3921 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5067 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9587 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6642 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5762 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3091 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1776 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      612 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6078 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15000 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.895073 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.895073 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2129 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/cdk_metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/cdk_metadata.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      521 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.895073 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.899073 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4341 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1978 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      655 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.899073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.903073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4052 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2468 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10054 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.911073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13849 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8600 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3542 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/quirks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/schema.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60802 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1802 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16933 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/template_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10828 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.911073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       13 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48835 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5923 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/provider_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21982 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.915073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2812 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      680 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6447 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2306 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      546 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      351 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      671 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.915073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/scaffolding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30872 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/scaffolding/__main__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7821 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/scaffolding/propgen.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5186 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4479 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.919073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15637 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16749 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/cloudwatch_database_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19150 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35869 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/provider_v2.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.923073 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3829 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5149 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4118 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.923073 localstack_core-3.4.1.dev20240502085340/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.931073 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4008 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    89510 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.935073 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14456 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14592 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14688 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12160 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6437 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11609 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.935073 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8003 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6411 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.939073 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20681 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.959072 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4694 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2752 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10103 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_instance.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11562 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3456 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1650 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3674 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_keypair.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      520 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5790 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2703 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3124 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3364 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_prefixlist_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_route.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1178 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_route_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_routetable.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1959 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4018 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2951 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5578 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnet.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3233 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4381 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1376 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4268 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      580 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3816 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3101 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6920 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpc.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4974 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpc_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6049 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3227 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3189 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.959072 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.959072 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5022 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/aws_ecr_repository.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7832 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6704 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.959072 localstack_core-3.4.1.dev20240502085340/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17509 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.967072 localstack_core-3.4.1.dev20240502085340/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      783 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/event_bus.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2563 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/event_ruler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2691 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/models_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1046 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22100 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21501 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/provider_v2.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.971072 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3234 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_apidestination.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1874 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_apidestination.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      598 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_apidestination_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4444 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_connection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_connection.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      578 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_connection_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2782 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbus.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1121 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbus.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4388 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1079 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      598 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8269 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10787 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_rule.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      523 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_rule_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6766 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11116 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/target.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12612 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/events/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.975072 localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6844 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37255 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.975072 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20613 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.987072 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3905 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_accesskey.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      662 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4333 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_group.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_group.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_group_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4157 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1915 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3815 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_policy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_policy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7879 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_role.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5495 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_role.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_role_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3756 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servercertificate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3458 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4773 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_user.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_user.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_user_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11028 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12533 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.991072 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6751 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7630 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.995072 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5302 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5738 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3963 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      858 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.995072 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:03.999072 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16350 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29805 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.007072 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32637 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60841 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.011072 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2630 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_alias.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1795 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_alias.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_alias_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4258 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_key.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5752 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_key.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_key_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.015072 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24036 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1362 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/custom_endpoints.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.023072 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9817 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3771 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2451 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      204 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6591 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      584 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/lambda_legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12587 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20150 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9720 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      763 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.031072 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6619 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/assignment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11752 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/counting_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21693 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24779 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/event_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16704 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/execution_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7600 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7292 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/internal_sqs_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18579 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27268 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2580 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/metrics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      402 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4197 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11130 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1878 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.031072 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      938 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/networking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3570 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1275 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   171538 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.043071 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3397 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3318 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6434 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13019 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17919 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16077 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3301 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      639 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_permission.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1096 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4941 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4011 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_version.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1073 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4563 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/lambda_alias.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/lambda_alias.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7455 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/runtimes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8185 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      397 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.043071 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18481 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.047071 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4161 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_loggroup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4890 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      556 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_logstream.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      561 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3051 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7769 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/moto.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.051071 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25638 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15220 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27982 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.055071 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6974 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6977 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10221 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11638 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      617 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10344 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24425 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13385 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.055071 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2053 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.059071 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9140 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/aws_redshift_cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15749 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.059071 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.059071 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4752 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.059071 localstack_core-3.4.1.dev20240502085340/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.059071 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4606 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.063071 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3627 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_healthcheck.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6336 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_recordset.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2475 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.067071 localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8325 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34472 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.079071 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3641 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13339 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1554 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3515 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34546 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37147 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    85348 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.079071 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22741 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucket.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52629 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      509 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucket_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      527 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37612 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2274 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/utils_moto.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.083071 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26562 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   157358 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.087071 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/storage/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/storage/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7303 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/storage/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20244 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/storage/ephemeral.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16129 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/validation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16627 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.087071 localstack_core-3.4.1.dev20240502085340/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.087071 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.091071 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6213 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21941 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      586 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3526 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3196 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      611 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.091071 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37052 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.099071 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3084 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2045 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6637 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2360 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2738 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      573 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.099071 localstack_core-3.4.1.dev20240502085340/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22213 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.103071 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1882 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/certificate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5630 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52779 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65164 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.111070 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4170 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_subscription.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1059 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5281 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topic.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topic.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topic_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1677 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.115070 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2228 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48438 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71592 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8532 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/query_api.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.119070 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8116 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6980 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queue_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3294 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      547 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6483 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.119070 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17767 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.127070 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3432 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1384 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3304 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1264 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5919 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5344 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      615 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5552 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3788 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.131070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.131070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.131070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1306 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.143070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13817 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24010 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4096 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2546 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81947 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   299585 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32416 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19200 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.143070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.143070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.147070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.151070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       83 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4111 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      161 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/comment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.167070 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      669 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2674 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      574 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.175069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      295 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      586 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.179069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      736 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      786 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.179069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.183069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      151 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.183069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.187069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      633 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2180 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1006 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.187069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.191069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      590 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.199069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1598 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1590 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4300 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.199069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/timeouts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1576 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2062 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      492 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/version.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2771 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.203069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.207069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      682 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.207069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.211069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.215069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1050 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1714 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1781 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1596 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2299 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1895 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.215069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2032 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2014 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.215069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3624 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.219069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2858 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.219069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3162 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1323 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.219069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2507 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2323 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.219069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.223069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.223069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.223069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6628 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.227069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7716 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.231069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      987 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.235069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3314 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1226 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2227 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      962 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.235069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.239069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5580 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6009 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6399 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2456 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      357 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.239069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11236 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.239069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/execution_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.239069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2934 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.243069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_header_location.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_headers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.247069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      826 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2512 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.247069 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      164 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2110 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.251068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8679 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4297 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.255068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2334 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6034 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2183 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1648 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6630 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      820 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      789 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1004 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8427 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.259068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5120 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1522 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1703 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1519 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3247 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3255 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10009 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.259068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1967 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4404 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.263068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2571 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.271068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5272 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12414 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10571 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8450 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5417 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5014 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4713 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2499 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3797 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9188 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3946 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4144 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3407 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8877 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6854 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.271068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/error_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2302 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.275068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      408 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3328 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2097 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.275068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.275068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.279068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2506 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1593 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2950 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1392 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.279068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.279068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2342 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/program/test_state_program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.283068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1003 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/state/test_state_state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.287068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      286 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/aws_execution_details.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.287068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/callback/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/callback/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7829 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/callback/callback.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.287068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1412 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7859 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.291068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2726 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1582 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/program_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.291068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/test_state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/test_state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2192 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/test_state/environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/test_state/program_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.295068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.295068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6145 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40495 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/preprocessor.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.295068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/test_state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/test_state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1595 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/test_state/asl_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5443 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/test_state/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.295068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      419 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/static_analyser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.295068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/test_state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/test_state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1996 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/test_state/test_state_analyser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.299068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/boto_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      689 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.303068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/activity.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12060 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3842 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      387 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7821 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/store.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.303068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/test_state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/test_state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4997 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/test_state/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1294 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/test_state/execution_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.303068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/legacy/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/legacy/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2829 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/legacy/provider_legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4955 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/legacy/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7013 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39007 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/quotas.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.307068 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3263 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7105 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5388 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      801 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11685 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.307068 localstack_core-3.4.1.dev20240502085340/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      319 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sts/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2456 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.311068 localstack_core-3.4.1.dev20240502085340/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.311068 localstack_core-3.4.1.dev20240502085340/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.319068 localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13806 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.323068 localstack_core-3.4.1.dev20240502085340/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4383 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      749 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.323068 localstack_core-3.4.1.dev20240502085340/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.327067 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5917 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1733 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/eventbus_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12281 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8030 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.335067 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.335067 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      214 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/app.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.339067 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2198 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.339067 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2450 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.339067 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/tests/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/tests/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2353 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2846 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9181 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/container.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1336 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74205 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/in_memory_localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5549 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/marker_report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7547 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/marking.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3417 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/path_filter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5000 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/validation_tracking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.339067 localstack_core-3.4.1.dev20240502085340/localstack/testing/scenario/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/scenario/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7376 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/scenario/cdk_lambda_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18243 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/scenario/provisioning.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.339067 localstack_core-3.4.1.dev20240502085340/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32371 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.343067 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/git.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      893 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/github.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6919 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/matching.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2025 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/opt_in.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.347067 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1043 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/filter_by_test_selection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2400 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2631 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1187 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/testselection.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.371067 localstack_core-3.4.1.dev20240502085340/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.379067 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3425 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6500 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8629 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.387067 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13900 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10609 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14987 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12235 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8601 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7504 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4666 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48628 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.387067 localstack_core-3.4.1.dev20240502085340/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8474 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17435 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5473 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.391067 localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51151 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34506 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34554 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7297 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4187 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9635 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2967 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11352 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2084 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/iputils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6290 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.395067 localstack_core-3.4.1.dev20240502085340/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3827 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14773 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19689 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7264 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1750 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16839 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.395067 localstack_core-3.4.1.dev20240502085340/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12434 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3995 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/server/tcp_proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5935 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3664 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22646 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5056 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2017 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      717 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1465 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/localstack/utils/xml.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack/version.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 08:54:04.399066 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5464 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73949 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19316 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19515 2024-05-02 08:53:53.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2306 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2024-05-02 08:54:03.000000 localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8240 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2024-05-02 08:54:04.403066 localstack_core-3.4.1.dev20240502085340/setup.cfg
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      552 2024-05-02 08:04:07.000000 localstack_core-3.4.1.dev20240502085340/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.677853 localstack_core-3.4.1.dev20240502123741/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19977 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5464 2024-05-02 12:38:04.677853 localstack_core-3.4.1.dev20240502123741/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13116 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/README.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       24 2024-05-02 12:37:41.000000 localstack_core-3.4.1.dev20240502123741/VERSION
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:03.985855 localstack_core-3.4.1.dev20240502123741/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     6157 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:03.989855 localstack_core-3.4.1.dev20240502123741/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.001855 localstack_core-3.4.1.dev20240502123741/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3043 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.005855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.005855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17659 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.005855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75049 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.005855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10739 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.005855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   106163 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.009855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43772 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.009855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   135405 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.013855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    87711 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.013855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6954 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.013855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   812918 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.017855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    63522 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.021855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    56604 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.021855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48880 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.021855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   106761 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.025855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27200 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.025855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52805 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.025855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74323 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.029855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59701 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.033855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    78880 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.033855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   148750 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.033855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14828 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.033855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8623 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.037855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69704 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.037855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    58025 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.037855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   142987 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.041855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89829 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.041855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15493 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/scheduler/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.041855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23419 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.041855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55788 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.041855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28332 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.045855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20646 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.045855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   223600 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.045855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45370 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.049855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10092 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.049855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16813 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.049855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60518 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.049855 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47602 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4972 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8024 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26256 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/connect.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:03.969855 localstack_core-3.4.1.dev20240502123741/localstack/aws/data/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:03.969855 localstack_core-3.4.1.dev20240502123741/localstack/aws/data/sqs-query/
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.053855 localstack_core-3.4.1.dev20240502123741/localstack/aws/data/sqs-query/2012-11-05/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      792 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/data/sqs-query/2012-11-05/README.md
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34047 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/data/sqs-query/2012-11-05/service-2.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12084 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      687 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.061855 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1876 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2455 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10596 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1464 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1790 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1628 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6079 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6241 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12518 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      988 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11678 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3577 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13778 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.065855 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15560 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50501 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81658 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18970 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5317 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19961 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.069855 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3918 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5852 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/twisted.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2093 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       76 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8216 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37980 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11687 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12838 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.077855 localstack_core-3.4.1.dev20240502123741/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30929 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4222 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      877 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3499 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    58425 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7725 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12965 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.077855 localstack_core-3.4.1.dev20240502123741/localstack/dev/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.077855 localstack_core-3.4.1.dev20240502123741/localstack/dev/kubernetes/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/kubernetes/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6325 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/kubernetes/__main__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.077855 localstack_core-3.4.1.dev20240502123741/localstack/dev/run/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/run/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12603 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/run/__main__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13833 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/run/configurators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dev/run/paths.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.081855 localstack_core-3.4.1.dev20240502123741/localstack/dns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5785 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1428 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dns/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33217 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/dns/server.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.081855 localstack_core-3.4.1.dev20240502123741/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       96 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.085855 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      139 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      739 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2867 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.085855 localstack_core-3.4.1.dev20240502123741/localstack/extensions/patterns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/patterns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13465 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/extensions/patterns/webapp.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.093855 localstack_core-3.4.1.dev20240502123741/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      471 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      152 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      755 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/duplex_socket.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5356 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      115 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      418 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      591 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      300 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/http/websocket.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.093855 localstack_core-3.4.1.dev20240502123741/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5078 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.097855 localstack_core-3.4.1.dev20240502123741/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16302 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14645 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1310 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      898 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.101855 localstack_core-3.4.1.dev20240502123741/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4126 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3112 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7332 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      818 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2276 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.105855 localstack_core-3.4.1.dev20240502123741/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.105855 localstack_core-3.4.1.dev20240502123741/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.117855 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6310 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13445 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/exporter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69249 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47983 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15097 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3248 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9586 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   115626 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.133855 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2896 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_account.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1081 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3726 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4214 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1855 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11600 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4719 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2565 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3494 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1946 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      627 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8627 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_method.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10052 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3757 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_model.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2020 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1917 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      632 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3856 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1788 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      592 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7513 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3921 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      587 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5067 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9587 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6642 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5762 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3091 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1776 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      612 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6078 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15000 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.133855 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.133855 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2129 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/cdk_metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/cdk_metadata.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      521 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.133855 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.137855 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4341 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1978 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      655 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.137855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.145855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4052 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2468 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10054 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.149855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13849 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8600 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      438 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3542 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/quirks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      494 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/schema.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60802 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1802 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16933 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/template_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10828 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1518 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2164 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.153855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       13 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48835 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5923 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/provider_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21982 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.157855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2812 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      680 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6447 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1192 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2306 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      546 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2495 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      351 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      671 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.157855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/scaffolding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30872 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/scaffolding/__main__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7821 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/scaffolding/propgen.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5186 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4479 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.161855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15637 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16749 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/cloudwatch_database_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19150 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35869 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/provider_v2.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.161855 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3829 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      577 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5149 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4118 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.165855 localstack_core-3.4.1.dev20240502123741/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.169854 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4008 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    89510 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.169854 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14456 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14592 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14688 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12160 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6437 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11609 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.173854 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8003 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6411 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.173854 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20681 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.197854 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4694 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2752 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10103 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_instance.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11562 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3456 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1650 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3674 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_keypair.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      520 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5790 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2703 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3124 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5104 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3364 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_prefixlist_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_route.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1178 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_route_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3340 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_routetable.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1959 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4018 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2951 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5578 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnet.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3233 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4381 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1376 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4268 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      580 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3816 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3101 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6920 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpc.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4974 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpc_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6049 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3227 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3189 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.197854 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.197854 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5022 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/aws_ecr_repository.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7832 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      560 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6704 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.197854 localstack_core-3.4.1.dev20240502123741/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17509 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.205855 localstack_core-3.4.1.dev20240502123741/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      783 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/event_bus.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2563 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/event_ruler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2691 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/models_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1046 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22100 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21501 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/provider_v2.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.209854 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3234 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_apidestination.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1874 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_apidestination.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      598 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_apidestination_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4444 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_connection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_connection.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      578 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_connection_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2782 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbus.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1121 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbus.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4388 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1079 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      598 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8269 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10787 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_rule.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      523 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_rule_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6766 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11116 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/target.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12612 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/events/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.209854 localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6844 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37255 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.213854 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20613 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.221854 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3905 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_accesskey.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      662 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4333 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_group.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_group.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_group_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4157 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1915 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      585 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3815 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4979 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_policy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_policy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      515 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7879 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_role.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5495 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_role.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_role_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3756 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servercertificate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3458 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2549 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      622 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4773 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_user.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2102 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_user.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      505 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_user_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11028 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12533 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.225854 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6751 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7630 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.229854 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5302 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5738 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3963 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      858 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.229854 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.229854 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16350 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29805 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.233854 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32637 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60841 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.237854 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2630 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_alias.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1795 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_alias.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_alias_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4258 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_key.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5752 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_key.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      500 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_key_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1256 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.249854 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24036 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1362 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/custom_endpoints.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.257854 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9817 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3771 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2451 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      204 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6591 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      584 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/lambda_legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12587 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20150 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9720 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      763 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.269854 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6619 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/assignment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11752 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/counting_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21693 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24779 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/event_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16704 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/execution_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7600 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7332 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/internal_sqs_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18579 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27268 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2580 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1134 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/metrics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      402 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4197 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11130 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1878 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.269854 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      601 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      938 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/networking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3570 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1275 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   171538 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.285854 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3397 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3318 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      614 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6434 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13019 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17919 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16077 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3301 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1463 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      639 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4367 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_permission.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1096 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4941 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4011 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_version.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1073 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4563 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/lambda_alias.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/lambda_alias.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      525 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7455 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/runtimes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8185 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      397 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.285854 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      569 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18481 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.289854 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4161 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_loggroup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4890 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      556 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_logstream.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      561 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3451 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3051 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7769 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/moto.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.293854 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25638 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15220 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27982 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.293854 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6974 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6977 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10221 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11638 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      617 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10344 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24425 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13385 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.293854 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2053 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.297854 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9140 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/aws_redshift_cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15749 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.297854 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.297854 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4752 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      602 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.301854 localstack_core-3.4.1.dev20240502123741/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.301854 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4606 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.309854 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3627 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_healthcheck.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      589 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6336 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_recordset.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2475 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      579 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.313854 localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8325 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34472 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.325854 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4781 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3641 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13339 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1554 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3515 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34546 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37147 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    85348 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.329854 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22741 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucket.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52629 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      509 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucket_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      527 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      564 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37612 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2274 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/utils_moto.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.329854 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26562 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   157358 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.333854 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/storage/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/storage/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7303 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/storage/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20244 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/storage/ephemeral.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16129 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/validation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16627 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.333854 localstack_core-3.4.1.dev20240502123741/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.333854 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      238 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.345854 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6213 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21941 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      586 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3526 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3196 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      611 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.345854 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37052 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.349854 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3084 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      619 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3386 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2045 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      656 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6637 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2360 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2738 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      573 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.349854 localstack_core-3.4.1.dev20240502123741/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22213 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.353854 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1882 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/certificate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1210 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5630 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52779 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65164 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.357854 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4170 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_subscription.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1059 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5281 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topic.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6001 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topic.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topic_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3325 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1677 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.361854 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2228 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48438 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71785 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8544 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/query_api.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.365854 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8116 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6980 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      510 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queue_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3294 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      547 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      565 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6483 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.365854 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17767 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.373854 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3432 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1384 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      595 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3304 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1264 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5919 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5344 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      615 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5552 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_parameter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      832 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      555 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4209 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3788 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      575 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.373854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.373854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.377854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1306 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.393854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13817 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24010 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4096 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2546 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81947 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   299585 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32416 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19200 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.393854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.393854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.397854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.397854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       83 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4111 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      161 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/comment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.401854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      669 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2674 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      574 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.405854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      295 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      586 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.405854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      871 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      736 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      786 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.405854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.405854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      151 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.409854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.413854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      633 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2180 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1006 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.413854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.417854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      590 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.421854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1598 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1590 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      930 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4300 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.421854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/timeouts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/timeouts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1576 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2062 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      492 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/version.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      171 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2771 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.425854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.429854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      682 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      747 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.429854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.433854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.437854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1050 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1714 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1781 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1596 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2299 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2042 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1895 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.437854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2032 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2014 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.437854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3624 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.441854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2858 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.441854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3162 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1323 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.441854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2507 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2323 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      597 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.441854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.441854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.445854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1072 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      394 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.445854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6628 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.449854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7716 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.453854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      987 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.453854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3314 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1226 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2227 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      962 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.457854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.457854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3512 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5580 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6009 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6399 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2456 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      357 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.457854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11236 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.461854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      167 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/execution_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.461854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2934 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.465854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      502 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_header_location.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/csv_headers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      712 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.469853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      826 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2512 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.469853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      164 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1202 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2110 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.473853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8679 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4297 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.477854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2334 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6034 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2183 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1708 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1648 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6630 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      820 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      789 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1004 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8427 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.481854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2213 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5120 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1522 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1703 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1519 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3247 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3255 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10009 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.481854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1967 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4404 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3727 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.485854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2571 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.497853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5272 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12414 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10571 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5661 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8450 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5417 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5014 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4713 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2499 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3797 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9188 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3946 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4144 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3407 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8877 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6854 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.501854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      404 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/error_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1774 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2302 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.501854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      408 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3328 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2097 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.501854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.501854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.505854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2506 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1593 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2950 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1392 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.505854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.505854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2342 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/program/test_state_program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.505854 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1003 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/state/test_state_state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.509853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      286 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/aws_execution_details.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.509853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/callback/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/callback/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7829 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/callback/callback.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.509853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1412 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7859 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.513853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2726 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1582 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/program_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.513853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/test_state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/test_state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2192 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/test_state/environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/test_state/program_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.517853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2380 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.521853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6145 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40495 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/preprocessor.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.525853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/test_state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/test_state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1595 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/test_state/asl_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5443 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/test_state/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.525853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      419 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/static_analyser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.525853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/test_state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/test_state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1996 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/test_state/test_state_analyser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.529853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/boto_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      689 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.533853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1371 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/activity.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12060 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3842 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      387 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7821 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      947 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/store.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.533853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/test_state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/test_state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4997 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/test_state/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1294 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/test_state/execution_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.549853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/legacy/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/legacy/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2829 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/legacy/provider_legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4955 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/legacy/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7013 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39007 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/quotas.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.561853 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3263 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1864 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      610 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7105 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5388 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      630 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      801 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11685 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.561853 localstack_core-3.4.1.dev20240502123741/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      319 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sts/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2456 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.561853 localstack_core-3.4.1.dev20240502123741/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.565853 localstack_core-3.4.1.dev20240502123741/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.565853 localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      704 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      198 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13806 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.569853 localstack_core-3.4.1.dev20240502123741/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4003 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4383 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10540 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      749 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.569853 localstack_core-3.4.1.dev20240502123741/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.573853 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5917 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1733 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/eventbus_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12281 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8030 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.585853 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       73 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.585853 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      214 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/app.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.585853 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2198 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.585853 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2450 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.585853 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/tests/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/tests/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2353 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2846 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9181 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/container.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1336 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1497 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74621 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/in_memory_localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5549 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/marker_report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7547 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/marking.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3417 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/path_filter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5000 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/validation_tracking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.589853 localstack_core-3.4.1.dev20240502123741/localstack/testing/scenario/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/scenario/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7376 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/scenario/cdk_lambda_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18243 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/scenario/provisioning.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.589853 localstack_core-3.4.1.dev20240502123741/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32371 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.593853 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/git.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      893 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/github.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6919 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/matching.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2025 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/opt_in.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.593853 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1043 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/filter_by_test_selection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2400 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2631 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1187 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/testselection.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.629853 localstack_core-3.4.1.dev20240502123741/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.633853 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3425 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6500 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8629 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.653853 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13900 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10609 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3524 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14988 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5517 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12235 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2785 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8601 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7504 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4666 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48628 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.657853 localstack_core-3.4.1.dev20240502123741/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8474 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17435 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6402 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1218 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5473 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.665853 localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51151 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34506 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34554 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7297 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4187 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9635 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2967 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11352 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2084 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/iputils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6290 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.669853 localstack_core-3.4.1.dev20240502123741/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3827 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14773 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19689 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7264 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1750 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16839 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.669853 localstack_core-3.4.1.dev20240502123741/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12434 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3995 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/server/tcp_proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5935 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3664 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22646 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5056 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2017 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      717 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3194 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1465 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/localstack/utils/xml.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack/version.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-02 12:38:04.673853 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5464 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73951 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19316 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19515 2024-05-02 12:37:56.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2306 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2024-05-02 12:38:03.000000 localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8240 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       38 2024-05-02 12:38:04.677853 localstack_core-3.4.1.dev20240502123741/setup.cfg
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      552 2024-05-02 11:52:11.000000 localstack_core-3.4.1.dev20240502123741/setup.py
```

### Comparing `localstack_core-3.4.1.dev20240502085340/LICENSE.txt` & `localstack_core-3.4.1.dev20240502123741/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/Makefile` & `localstack_core-3.4.1.dev20240502123741/Makefile`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/PKG-INFO` & `localstack_core-3.4.1.dev20240502123741/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 3.4.1.dev20240502085340
+Version: 3.4.1.dev20240502123741
 Summary: The core library and runtime of LocalStack
 Author-email: LocalStack Contributors <info@localstack.cloud>
 Project-URL: Homepage, https://localstack.cloud
 Project-URL: Documentation, https://docs.localstack.cloud
 Project-URL: Repository, https://github.com/localstack/localstack.git
 Project-URL: Issues, https://github.com/localstack/localstack/issues
 Classifier: Programming Language :: Python :: 3
@@ -28,16 +28,16 @@
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: rich>=12.3.0
 Requires-Dist: requests>=2.20.0
 Requires-Dist: semver>=2.10
 Requires-Dist: stevedore>=3.4.0
 Requires-Dist: tailer>=0.4.1
 Provides-Extra: base-runtime
-Requires-Dist: boto3==1.34.84; extra == "base-runtime"
-Requires-Dist: botocore==1.34.84; extra == "base-runtime"
+Requires-Dist: boto3==1.34.93; extra == "base-runtime"
+Requires-Dist: botocore==1.34.93; extra == "base-runtime"
 Requires-Dist: awscrt>=0.13.14; extra == "base-runtime"
 Requires-Dist: cbor2>=5.2.0; extra == "base-runtime"
 Requires-Dist: dnspython>=1.16.0; extra == "base-runtime"
 Requires-Dist: docker<7.0.0,>=6.1.1; extra == "base-runtime"
 Requires-Dist: jsonpatch>=1.24; extra == "base-runtime"
 Requires-Dist: hypercorn>=0.14.4; extra == "base-runtime"
 Requires-Dist: localstack-twisted>=23.0; extra == "base-runtime"
@@ -48,15 +48,15 @@
 Requires-Dist: Werkzeug>=3.0.0; extra == "base-runtime"
 Requires-Dist: xmltodict>=0.13.0; extra == "base-runtime"
 Requires-Dist: rolo>=0.4; extra == "base-runtime"
 Requires-Dist: flask>=3.0.0; extra == "base-runtime"
 Requires-Dist: Quart>=0.19.2; extra == "base-runtime"
 Provides-Extra: runtime
 Requires-Dist: localstack-core[base-runtime]; extra == "runtime"
-Requires-Dist: awscli==1.32.84; extra == "runtime"
+Requires-Dist: awscli==1.32.93; extra == "runtime"
 Requires-Dist: airspeed-ext>=0.6.3; extra == "runtime"
 Requires-Dist: amazon_kclpy!=2.1.0,!=2.1.4,>=2.0.6; extra == "runtime"
 Requires-Dist: antlr4-python3-runtime==4.13.1; extra == "runtime"
 Requires-Dist: apispec>=5.1.1; extra == "runtime"
 Requires-Dist: aws-sam-translator>=1.15.1; extra == "runtime"
 Requires-Dist: crontab>=0.22.6; extra == "runtime"
 Requires-Dist: cryptography>=41.0.5; extra == "runtime"
@@ -90,8 +90,8 @@
 Requires-Dist: pandoc; extra == "dev"
 Requires-Dist: pre-commit>=3.5.0; extra == "dev"
 Requires-Dist: pypandoc; extra == "dev"
 Requires-Dist: ruff>=0.3.3; extra == "dev"
 Requires-Dist: rstr>=3.2.0; extra == "dev"
 Provides-Extra: typehint
 Requires-Dist: localstack-core[dev]; extra == "typehint"
-Requires-Dist: boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.84; extra == "typehint"
+Requires-Dist: boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.93; extra == "typehint"
```

### Comparing `localstack_core-3.4.1.dev20240502085340/README.md` & `localstack_core-3.4.1.dev20240502123741/README.md`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/bin/localstack` & `localstack_core-3.4.1.dev20240502123741/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/bin/localstack-supervisor` & `localstack_core-3.4.1.dev20240502123741/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/accounts.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/acm/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/apigateway/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudcontrol/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudformation/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/cloudwatch/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/config/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/core.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/dynamodb/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ec2/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ec2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1098,14 +1098,15 @@
     blockDeviceMapping = "blockDeviceMapping"
     sriovNetSupport = "sriovNetSupport"
     bootMode = "bootMode"
     tpmSupport = "tpmSupport"
     uefiData = "uefiData"
     lastLaunchedTime = "lastLaunchedTime"
     imdsSupport = "imdsSupport"
+    deregistrationProtection = "deregistrationProtection"
 
 
 class ImageBlockPublicAccessDisabledState(str):
     unblocked = "unblocked"
 
 
 class ImageBlockPublicAccessEnabledState(str):
@@ -2428,14 +2429,15 @@
 
 
 class NetworkInterfaceAttribute(str):
     description = "description"
     groupSet = "groupSet"
     sourceDestCheck = "sourceDestCheck"
     attachment = "attachment"
+    associatePublicIpAddress = "associatePublicIpAddress"
 
 
 class NetworkInterfaceCreationType(str):
     efa = "efa"
     branch = "branch"
     trunk = "trunk"
 
@@ -10961,14 +10963,16 @@
     Tags: Optional[TagList]
     VirtualizationType: Optional[VirtualizationType]
     BootMode: Optional[BootModeValues]
     TpmSupport: Optional[TpmSupportValues]
     DeprecationTime: Optional[String]
     ImdsSupport: Optional[ImdsSupportValues]
     SourceInstanceId: Optional[String]
+    DeregistrationProtection: Optional[String]
+    LastLaunchedTime: Optional[String]
 
 
 ImageList = List[Image]
 
 
 class DescribeImagesResult(TypedDict, total=False):
     Images: Optional[ImageList]
@@ -12383,14 +12387,15 @@
 
 class DescribeNetworkInterfaceAttributeResult(TypedDict, total=False):
     Attachment: Optional[NetworkInterfaceAttachment]
     Description: Optional[AttributeValue]
     Groups: Optional[GroupIdentifierList]
     NetworkInterfaceId: Optional[String]
     SourceDestCheck: Optional[AttributeBooleanValue]
+    AssociatePublicIpAddress: Optional[Boolean]
 
 
 NetworkInterfacePermissionIdList = List[NetworkInterfacePermissionId]
 
 
 class DescribeNetworkInterfacePermissionsRequest(ServiceRequest):
     NetworkInterfacePermissionIds: Optional[NetworkInterfacePermissionIdList]
@@ -14417,14 +14422,23 @@
     DryRun: Optional[Boolean]
 
 
 class DisableImageDeprecationResult(TypedDict, total=False):
     Return: Optional[Boolean]
 
 
+class DisableImageDeregistrationProtectionRequest(ServiceRequest):
+    ImageId: ImageId
+    DryRun: Optional[Boolean]
+
+
+class DisableImageDeregistrationProtectionResult(TypedDict, total=False):
+    Return: Optional[String]
+
+
 class DisableImageRequest(ServiceRequest):
     ImageId: ImageId
     DryRun: Optional[Boolean]
 
 
 class DisableImageResult(TypedDict, total=False):
     Return: Optional[Boolean]
@@ -14814,14 +14828,24 @@
     DryRun: Optional[Boolean]
 
 
 class EnableImageDeprecationResult(TypedDict, total=False):
     Return: Optional[Boolean]
 
 
+class EnableImageDeregistrationProtectionRequest(ServiceRequest):
+    ImageId: ImageId
+    WithCooldown: Optional[Boolean]
+    DryRun: Optional[Boolean]
+
+
+class EnableImageDeregistrationProtectionResult(TypedDict, total=False):
+    Return: Optional[String]
+
+
 class EnableImageRequest(ServiceRequest):
     ImageId: ImageId
     DryRun: Optional[Boolean]
 
 
 class EnableImageResult(TypedDict, total=False):
     Return: Optional[Boolean]
@@ -15917,14 +15941,15 @@
     RamdiskId: Optional[AttributeValue]
     SriovNetSupport: Optional[AttributeValue]
     BootMode: Optional[AttributeValue]
     TpmSupport: Optional[AttributeValue]
     UefiData: Optional[AttributeValue]
     LastLaunchedTime: Optional[AttributeValue]
     ImdsSupport: Optional[AttributeValue]
+    DeregistrationProtection: Optional[AttributeValue]
 
 
 class UserBucket(TypedDict, total=False):
     S3Bucket: Optional[String]
     S3Key: Optional[String]
 
 
@@ -16707,14 +16732,15 @@
     DryRun: Optional[Boolean]
     Groups: Optional[SecurityGroupIdStringList]
     NetworkInterfaceId: NetworkInterfaceId
     SourceDestCheck: Optional[AttributeBooleanValue]
     EnaSrdSpecification: Optional[EnaSrdSpecification]
     EnablePrimaryIpv6: Optional[Boolean]
     ConnectionTrackingSpecification: Optional[ConnectionTrackingSpecificationRequest]
+    AssociatePublicIpAddress: Optional[Boolean]
 
 
 class ModifyPrivateDnsNameOptionsRequest(ServiceRequest):
     DryRun: Optional[Boolean]
     InstanceId: InstanceId
     PrivateDnsHostnameType: Optional[HostnameType]
     EnableResourceNameDnsARecord: Optional[Boolean]
@@ -22960,14 +22986,20 @@
 
     @handler("DisableImageDeprecation")
     def disable_image_deprecation(
         self, context: RequestContext, image_id: ImageId, dry_run: Boolean = None, **kwargs
     ) -> DisableImageDeprecationResult:
         raise NotImplementedError
 
+    @handler("DisableImageDeregistrationProtection")
+    def disable_image_deregistration_protection(
+        self, context: RequestContext, image_id: ImageId, dry_run: Boolean = None, **kwargs
+    ) -> DisableImageDeregistrationProtectionResult:
+        raise NotImplementedError
+
     @handler("DisableIpamOrganizationAdminAccount")
     def disable_ipam_organization_admin_account(
         self,
         context: RequestContext,
         delegated_admin_account_id: String,
         dry_run: Boolean = None,
         **kwargs,
@@ -23244,14 +23276,25 @@
         image_id: ImageId,
         deprecate_at: MillisecondDateTime,
         dry_run: Boolean = None,
         **kwargs,
     ) -> EnableImageDeprecationResult:
         raise NotImplementedError
 
+    @handler("EnableImageDeregistrationProtection")
+    def enable_image_deregistration_protection(
+        self,
+        context: RequestContext,
+        image_id: ImageId,
+        with_cooldown: Boolean = None,
+        dry_run: Boolean = None,
+        **kwargs,
+    ) -> EnableImageDeregistrationProtectionResult:
+        raise NotImplementedError
+
     @handler("EnableIpamOrganizationAdminAccount")
     def enable_ipam_organization_admin_account(
         self,
         context: RequestContext,
         delegated_admin_account_id: String,
         dry_run: Boolean = None,
         **kwargs,
@@ -24455,14 +24498,15 @@
         description: AttributeValue = None,
         dry_run: Boolean = None,
         groups: SecurityGroupIdStringList = None,
         source_dest_check: AttributeBooleanValue = None,
         ena_srd_specification: EnaSrdSpecification = None,
         enable_primary_ipv6: Boolean = None,
         connection_tracking_specification: ConnectionTrackingSpecificationRequest = None,
+        associate_public_ip_address: Boolean = None,
         **kwargs,
     ) -> None:
         raise NotImplementedError
 
     @handler("ModifyPrivateDnsNameOptions")
     def modify_private_dns_name_options(
         self,
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/es/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/events/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/firehose/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/iam/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/kinesis/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/kms/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/lambda_/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/logs/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/opensearch/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/redshift/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/resource_groups/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/route53/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/route53resolver/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/s3/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/s3control/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/scheduler/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/secretsmanager/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ses/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sns/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sqs/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sqs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Dict, List, Optional, TypedDict
 
 from localstack.aws.api import RequestContext, ServiceException, ServiceRequest, handler
 
 Boolean = bool
 BoxedInteger = int
-Integer = int
+ExceptionMessage = str
 MessageAttributeName = str
+NullableInteger = int
 String = str
 TagKey = str
 TagValue = str
 Token = str
 
 
 class MessageSystemAttributeName(str):
@@ -50,40 +51,52 @@
     DeduplicationScope = "DeduplicationScope"
     FifoThroughputLimit = "FifoThroughputLimit"
     RedriveAllowPolicy = "RedriveAllowPolicy"
     SqsManagedSseEnabled = "SqsManagedSseEnabled"
 
 
 class BatchEntryIdsNotDistinct(ServiceException):
-    code: str = "AWS.SimpleQueueService.BatchEntryIdsNotDistinct"
-    sender_fault: bool = True
+    code: str = "BatchEntryIdsNotDistinct"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class BatchRequestTooLong(ServiceException):
-    code: str = "AWS.SimpleQueueService.BatchRequestTooLong"
-    sender_fault: bool = True
+    code: str = "BatchRequestTooLong"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class EmptyBatchRequest(ServiceException):
-    code: str = "AWS.SimpleQueueService.EmptyBatchRequest"
-    sender_fault: bool = True
+    code: str = "EmptyBatchRequest"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class InvalidAddress(ServiceException):
+    code: str = "InvalidAddress"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class InvalidAttributeName(ServiceException):
     code: str = "InvalidAttributeName"
     sender_fault: bool = False
     status_code: int = 400
 
 
+class InvalidAttributeValue(ServiceException):
+    code: str = "InvalidAttributeValue"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
 class InvalidBatchEntryId(ServiceException):
-    code: str = "AWS.SimpleQueueService.InvalidBatchEntryId"
-    sender_fault: bool = True
+    code: str = "InvalidBatchEntryId"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class InvalidIdFormat(ServiceException):
     code: str = "InvalidIdFormat"
     sender_fault: bool = False
     status_code: int = 400
@@ -91,71 +104,125 @@
 
 class InvalidMessageContents(ServiceException):
     code: str = "InvalidMessageContents"
     sender_fault: bool = False
     status_code: int = 400
 
 
+class InvalidSecurity(ServiceException):
+    code: str = "InvalidSecurity"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsAccessDenied(ServiceException):
+    code: str = "KmsAccessDenied"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsDisabled(ServiceException):
+    code: str = "KmsDisabled"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsInvalidKeyUsage(ServiceException):
+    code: str = "KmsInvalidKeyUsage"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsInvalidState(ServiceException):
+    code: str = "KmsInvalidState"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsNotFound(ServiceException):
+    code: str = "KmsNotFound"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsOptInRequired(ServiceException):
+    code: str = "KmsOptInRequired"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
+class KmsThrottled(ServiceException):
+    code: str = "KmsThrottled"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
 class MessageNotInflight(ServiceException):
-    code: str = "AWS.SimpleQueueService.MessageNotInflight"
-    sender_fault: bool = True
+    code: str = "MessageNotInflight"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class OverLimit(ServiceException):
     code: str = "OverLimit"
-    sender_fault: bool = True
-    status_code: int = 403
+    sender_fault: bool = False
+    status_code: int = 400
 
 
 class PurgeQueueInProgress(ServiceException):
-    code: str = "AWS.SimpleQueueService.PurgeQueueInProgress"
-    sender_fault: bool = True
-    status_code: int = 403
+    code: str = "PurgeQueueInProgress"
+    sender_fault: bool = False
+    status_code: int = 400
 
 
 class QueueDeletedRecently(ServiceException):
-    code: str = "AWS.SimpleQueueService.QueueDeletedRecently"
-    sender_fault: bool = True
+    code: str = "QueueDeletedRecently"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class QueueDoesNotExist(ServiceException):
-    code: str = "AWS.SimpleQueueService.NonExistentQueue"
-    sender_fault: bool = True
+    code: str = "QueueDoesNotExist"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class QueueNameExists(ServiceException):
-    code: str = "QueueAlreadyExists"
-    sender_fault: bool = True
+    code: str = "QueueNameExists"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class ReceiptHandleIsInvalid(ServiceException):
     code: str = "ReceiptHandleIsInvalid"
     sender_fault: bool = False
     status_code: int = 400
 
 
+class RequestThrottled(ServiceException):
+    code: str = "RequestThrottled"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
 class ResourceNotFoundException(ServiceException):
     code: str = "ResourceNotFoundException"
-    sender_fault: bool = True
-    status_code: int = 404
+    sender_fault: bool = False
+    status_code: int = 400
 
 
 class TooManyEntriesInBatchRequest(ServiceException):
-    code: str = "AWS.SimpleQueueService.TooManyEntriesInBatchRequest"
-    sender_fault: bool = True
+    code: str = "TooManyEntriesInBatchRequest"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 class UnsupportedOperation(ServiceException):
-    code: str = "AWS.SimpleQueueService.UnsupportedOperation"
-    sender_fault: bool = True
+    code: str = "UnsupportedOperation"
+    sender_fault: bool = False
     status_code: int = 400
 
 
 AWSAccountIdList = List[String]
 ActionNameList = List[String]
 
 
@@ -191,15 +258,15 @@
 class CancelMessageMoveTaskResult(TypedDict, total=False):
     ApproximateNumberOfMessagesMoved: Optional[Long]
 
 
 class ChangeMessageVisibilityBatchRequestEntry(TypedDict, total=False):
     Id: String
     ReceiptHandle: String
-    VisibilityTimeout: Optional[Integer]
+    VisibilityTimeout: Optional[NullableInteger]
 
 
 ChangeMessageVisibilityBatchRequestEntryList = List[ChangeMessageVisibilityBatchRequestEntry]
 
 
 class ChangeMessageVisibilityBatchRequest(ServiceRequest):
     QueueUrl: String
@@ -217,15 +284,15 @@
     Successful: ChangeMessageVisibilityBatchResultEntryList
     Failed: BatchResultErrorEntryList
 
 
 class ChangeMessageVisibilityRequest(ServiceRequest):
     QueueUrl: String
     ReceiptHandle: String
-    VisibilityTimeout: Integer
+    VisibilityTimeout: NullableInteger
 
 
 TagMap = Dict[TagKey, TagValue]
 QueueAttributeMap = Dict[QueueAttributeName, String]
 
 
 class CreateQueueRequest(ServiceRequest):
@@ -302,25 +369,28 @@
 class ListDeadLetterSourceQueuesResult(TypedDict, total=False):
     queueUrls: QueueUrlList
     NextToken: Optional[Token]
 
 
 class ListMessageMoveTasksRequest(ServiceRequest):
     SourceArn: String
-    MaxResults: Optional[Integer]
+    MaxResults: Optional[NullableInteger]
+
+
+NullableLong = int
 
 
 class ListMessageMoveTasksResultEntry(TypedDict, total=False):
     TaskHandle: Optional[String]
     Status: Optional[String]
     SourceArn: Optional[String]
     DestinationArn: Optional[String]
-    MaxNumberOfMessagesPerSecond: Optional[Integer]
+    MaxNumberOfMessagesPerSecond: Optional[NullableInteger]
     ApproximateNumberOfMessagesMoved: Optional[Long]
-    ApproximateNumberOfMessagesToMove: Optional[Long]
+    ApproximateNumberOfMessagesToMove: Optional[NullableLong]
     FailureReason: Optional[String]
     StartedTimestamp: Optional[Long]
 
 
 ListMessageMoveTasksResultEntryList = List[ListMessageMoveTasksResultEntry]
 
 
@@ -393,17 +463,17 @@
     QueueUrl: String
 
 
 class ReceiveMessageRequest(ServiceRequest):
     QueueUrl: String
     AttributeNames: Optional[AttributeNameList]
     MessageAttributeNames: Optional[MessageAttributeNameList]
-    MaxNumberOfMessages: Optional[Integer]
-    VisibilityTimeout: Optional[Integer]
-    WaitTimeSeconds: Optional[Integer]
+    MaxNumberOfMessages: Optional[NullableInteger]
+    VisibilityTimeout: Optional[NullableInteger]
+    WaitTimeSeconds: Optional[NullableInteger]
     ReceiveRequestAttemptId: Optional[String]
 
 
 class ReceiveMessageResult(TypedDict, total=False):
     Messages: Optional[MessageList]
 
 
@@ -411,15 +481,15 @@
     QueueUrl: String
     Label: String
 
 
 class SendMessageBatchRequestEntry(TypedDict, total=False):
     Id: String
     MessageBody: String
-    DelaySeconds: Optional[Integer]
+    DelaySeconds: Optional[NullableInteger]
     MessageAttributes: Optional[MessageBodyAttributeMap]
     MessageSystemAttributes: Optional[MessageBodySystemAttributeMap]
     MessageDeduplicationId: Optional[String]
     MessageGroupId: Optional[String]
 
 
 SendMessageBatchRequestEntryList = List[SendMessageBatchRequestEntry]
@@ -446,15 +516,15 @@
     Successful: SendMessageBatchResultEntryList
     Failed: BatchResultErrorEntryList
 
 
 class SendMessageRequest(ServiceRequest):
     QueueUrl: String
     MessageBody: String
-    DelaySeconds: Optional[Integer]
+    DelaySeconds: Optional[NullableInteger]
     MessageAttributes: Optional[MessageBodyAttributeMap]
     MessageSystemAttributes: Optional[MessageBodySystemAttributeMap]
     MessageDeduplicationId: Optional[String]
     MessageGroupId: Optional[String]
 
 
 class SendMessageResult(TypedDict, total=False):
@@ -469,15 +539,15 @@
     QueueUrl: String
     Attributes: QueueAttributeMap
 
 
 class StartMessageMoveTaskRequest(ServiceRequest):
     SourceArn: String
     DestinationArn: Optional[String]
-    MaxNumberOfMessagesPerSecond: Optional[Integer]
+    MaxNumberOfMessagesPerSecond: Optional[NullableInteger]
 
 
 class StartMessageMoveTaskResult(TypedDict, total=False):
     TaskHandle: Optional[String]
 
 
 TagKeyList = List[TagKey]
@@ -517,15 +587,15 @@
 
     @handler("ChangeMessageVisibility")
     def change_message_visibility(
         self,
         context: RequestContext,
         queue_url: String,
         receipt_handle: String,
-        visibility_timeout: Integer,
+        visibility_timeout: NullableInteger,
         **kwargs,
     ) -> None:
         raise NotImplementedError
 
     @handler("ChangeMessageVisibilityBatch")
     def change_message_visibility_batch(
         self,
@@ -596,15 +666,19 @@
         max_results: BoxedInteger = None,
         **kwargs,
     ) -> ListDeadLetterSourceQueuesResult:
         raise NotImplementedError
 
     @handler("ListMessageMoveTasks")
     def list_message_move_tasks(
-        self, context: RequestContext, source_arn: String, max_results: Integer = None, **kwargs
+        self,
+        context: RequestContext,
+        source_arn: String,
+        max_results: NullableInteger = None,
+        **kwargs,
     ) -> ListMessageMoveTasksResult:
         raise NotImplementedError
 
     @handler("ListQueueTags")
     def list_queue_tags(
         self, context: RequestContext, queue_url: String, **kwargs
     ) -> ListQueueTagsResult:
@@ -628,17 +702,17 @@
     @handler("ReceiveMessage")
     def receive_message(
         self,
         context: RequestContext,
         queue_url: String,
         attribute_names: AttributeNameList = None,
         message_attribute_names: MessageAttributeNameList = None,
-        max_number_of_messages: Integer = None,
-        visibility_timeout: Integer = None,
-        wait_time_seconds: Integer = None,
+        max_number_of_messages: NullableInteger = None,
+        visibility_timeout: NullableInteger = None,
+        wait_time_seconds: NullableInteger = None,
         receive_request_attempt_id: String = None,
         **kwargs,
     ) -> ReceiveMessageResult:
         raise NotImplementedError
 
     @handler("RemovePermission")
     def remove_permission(
@@ -648,15 +722,15 @@
 
     @handler("SendMessage")
     def send_message(
         self,
         context: RequestContext,
         queue_url: String,
         message_body: String,
-        delay_seconds: Integer = None,
+        delay_seconds: NullableInteger = None,
         message_attributes: MessageBodyAttributeMap = None,
         message_system_attributes: MessageBodySystemAttributeMap = None,
         message_deduplication_id: String = None,
         message_group_id: String = None,
         **kwargs,
     ) -> SendMessageResult:
         raise NotImplementedError
@@ -679,15 +753,15 @@
 
     @handler("StartMessageMoveTask")
     def start_message_move_task(
         self,
         context: RequestContext,
         source_arn: String,
         destination_arn: String = None,
-        max_number_of_messages_per_second: Integer = None,
+        max_number_of_messages_per_second: NullableInteger = None,
         **kwargs,
     ) -> StartMessageMoveTaskResult:
         raise NotImplementedError
 
     @handler("TagQueue")
     def tag_queue(self, context: RequestContext, queue_url: String, tags: TagMap, **kwargs) -> None:
         raise NotImplementedError
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/ssm/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/ssm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ActivationId = str
 AgentErrorCode = str
 AggregatorSchemaOnly = bool
 AlarmName = str
 AllowedPattern = str
 ApplyOnlyAtCronInterval = bool
 ApproveAfterDays = int
+Architecture = str
 AssociationExecutionFilterValue = str
 AssociationExecutionId = str
 AssociationExecutionTargetsFilterValue = str
 AssociationFilterValue = str
 AssociationId = str
 AssociationName = str
 AssociationResourceId = str
@@ -66,14 +67,15 @@
 ComplianceStringFilterKey = str
 ComplianceSummaryCount = int
 ComplianceTypeName = str
 ComputerName = str
 DefaultBaseline = bool
 DefaultInstanceName = str
 DeliveryTimedOutCount = int
+DescribeInstancePropertiesMaxResults = int
 DescriptionInDocument = str
 DocumentARN = str
 DocumentAuthor = str
 DocumentContent = str
 DocumentDisplayName = str
 DocumentFilterValue = str
 DocumentHash = str
@@ -106,17 +108,23 @@
 IdempotencyToken = str
 InstallOverrideList = str
 InstanceAssociationExecutionSummary = str
 InstanceCount = int
 InstanceId = str
 InstanceInformationFilterValue = str
 InstanceInformationStringFilterKey = str
+InstanceName = str
 InstancePatchStateFilterKey = str
 InstancePatchStateFilterValue = str
+InstancePropertyFilterValue = str
+InstancePropertyStringFilterKey = str
+InstanceRole = str
+InstanceState = str
 InstanceTagName = str
+InstanceType = str
 InstancesCount = int
 Integer = int
 InventoryAggregatorExpression = str
 InventoryDeletionLastStatusMessage = str
 InventoryFilterKey = str
 InventoryFilterValue = str
 InventoryGroupName = str
@@ -127,14 +135,15 @@
 InventoryItemTypeName = str
 InventoryItemTypeNameFilter = str
 InventoryResultEntityId = str
 InventoryResultItemKey = str
 InventoryTypeDisplayName = str
 InvocationTraceOutput = str
 IsSubTypeSchema = bool
+KeyName = str
 LastResourceDataSyncMessage = str
 ListOpsMetadataMaxResults = int
 MaintenanceWindowAllowUnassociatedTargets = bool
 MaintenanceWindowCutoff = int
 MaintenanceWindowDescription = str
 MaintenanceWindowDurationHours = int
 MaintenanceWindowEnabled = bool
@@ -268,14 +277,16 @@
 PatchSourceName = str
 PatchSourceProduct = str
 PatchStringDateTime = str
 PatchTitle = str
 PatchUnreportedNotApplicableCount = int
 PatchVendor = str
 PatchVersion = str
+PlatformName = str
+PlatformVersion = str
 Policy = str
 PolicyHash = str
 PolicyId = str
 Product = str
 PutInventoryMessage = str
 Region = str
 RegistrationLimit = int
@@ -638,14 +649,34 @@
 class InstancePatchStateOperatorType(str):
     Equal = "Equal"
     NotEqual = "NotEqual"
     LessThan = "LessThan"
     GreaterThan = "GreaterThan"
 
 
+class InstancePropertyFilterKey(str):
+    InstanceIds = "InstanceIds"
+    AgentVersion = "AgentVersion"
+    PingStatus = "PingStatus"
+    PlatformTypes = "PlatformTypes"
+    DocumentName = "DocumentName"
+    ActivationIds = "ActivationIds"
+    IamRole = "IamRole"
+    ResourceType = "ResourceType"
+    AssociationStatus = "AssociationStatus"
+
+
+class InstancePropertyFilterOperator(str):
+    Equal = "Equal"
+    NotEqual = "NotEqual"
+    BeginWith = "BeginWith"
+    LessThan = "LessThan"
+    GreaterThan = "GreaterThan"
+
+
 class InventoryAttributeDataType(str):
     string = "string"
     number = "number"
 
 
 class InventoryDeletionStatus(str):
     InProgress = "InProgress"
@@ -1327,14 +1358,20 @@
 
 class InvalidInstanceInformationFilterValue(ServiceException):
     code: str = "InvalidInstanceInformationFilterValue"
     sender_fault: bool = False
     status_code: int = 400
 
 
+class InvalidInstancePropertyFilterValue(ServiceException):
+    code: str = "InvalidInstancePropertyFilterValue"
+    sender_fault: bool = False
+    status_code: int = 400
+
+
 class InvalidInventoryGroupException(ServiceException):
     code: str = "InvalidInventoryGroupException"
     sender_fault: bool = False
     status_code: int = 400
 
 
 class InvalidInventoryItemContextException(ServiceException):
@@ -3440,14 +3477,78 @@
 
 
 class DescribeInstancePatchesResult(TypedDict, total=False):
     Patches: Optional[PatchComplianceDataList]
     NextToken: Optional[NextToken]
 
 
+InstancePropertyFilterValueSet = List[InstancePropertyFilterValue]
+
+
+class InstancePropertyStringFilter(TypedDict, total=False):
+    Key: InstancePropertyStringFilterKey
+    Values: InstancePropertyFilterValueSet
+    Operator: Optional[InstancePropertyFilterOperator]
+
+
+InstancePropertyStringFilterList = List[InstancePropertyStringFilter]
+
+
+class InstancePropertyFilter(TypedDict, total=False):
+    key: InstancePropertyFilterKey
+    valueSet: InstancePropertyFilterValueSet
+
+
+InstancePropertyFilterList = List[InstancePropertyFilter]
+
+
+class DescribeInstancePropertiesRequest(ServiceRequest):
+    InstancePropertyFilterList: Optional[InstancePropertyFilterList]
+    FiltersWithOperator: Optional[InstancePropertyStringFilterList]
+    MaxResults: Optional[DescribeInstancePropertiesMaxResults]
+    NextToken: Optional[NextToken]
+
+
+class InstanceProperty(TypedDict, total=False):
+    Name: Optional[InstanceName]
+    InstanceId: Optional[InstanceId]
+    InstanceType: Optional[InstanceType]
+    InstanceRole: Optional[InstanceRole]
+    KeyName: Optional[KeyName]
+    InstanceState: Optional[InstanceState]
+    Architecture: Optional[Architecture]
+    IPAddress: Optional[IPAddress]
+    LaunchTime: Optional[DateTime]
+    PingStatus: Optional[PingStatus]
+    LastPingDateTime: Optional[DateTime]
+    AgentVersion: Optional[Version]
+    PlatformType: Optional[PlatformType]
+    PlatformName: Optional[PlatformName]
+    PlatformVersion: Optional[PlatformVersion]
+    ActivationId: Optional[ActivationId]
+    IamRole: Optional[IamRole]
+    RegistrationDate: Optional[DateTime]
+    ResourceType: Optional[String]
+    ComputerName: Optional[ComputerName]
+    AssociationStatus: Optional[StatusName]
+    LastAssociationExecutionDate: Optional[DateTime]
+    LastSuccessfulAssociationExecutionDate: Optional[DateTime]
+    AssociationOverview: Optional[InstanceAggregatedAssociationOverview]
+    SourceId: Optional[SourceId]
+    SourceType: Optional[SourceType]
+
+
+InstanceProperties = List[InstanceProperty]
+
+
+class DescribeInstancePropertiesResult(TypedDict, total=False):
+    InstanceProperties: Optional[InstanceProperties]
+    NextToken: Optional[NextToken]
+
+
 class DescribeInventoryDeletionsRequest(ServiceRequest):
     DeletionId: Optional[UUID]
     NextToken: Optional[NextToken]
     MaxResults: Optional[MaxResults]
 
 
 InventoryDeletionLastStatusUpdateTime = datetime
@@ -6043,14 +6144,26 @@
         filters: PatchOrchestratorFilterList = None,
         next_token: NextToken = None,
         max_results: PatchComplianceMaxResults = None,
         **kwargs,
     ) -> DescribeInstancePatchesResult:
         raise NotImplementedError
 
+    @handler("DescribeInstanceProperties")
+    def describe_instance_properties(
+        self,
+        context: RequestContext,
+        instance_property_filter_list: InstancePropertyFilterList = None,
+        filters_with_operator: InstancePropertyStringFilterList = None,
+        max_results: DescribeInstancePropertiesMaxResults = None,
+        next_token: NextToken = None,
+        **kwargs,
+    ) -> DescribeInstancePropertiesResult:
+        raise NotImplementedError
+
     @handler("DescribeInventoryDeletions")
     def describe_inventory_deletions(
         self,
         context: RequestContext,
         deletion_id: UUID = None,
         next_token: NextToken = None,
         max_results: MaxResults = None,
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/stepfunctions/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/stepfunctions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 TagKey = str
 TagValue = str
 TaskToken = str
 ToleratedFailurePercentage = float
 TraceHeader = str
 URL = str
 UnsignedInteger = int
+ValidateStateMachineDefinitionCode = str
+ValidateStateMachineDefinitionLocation = str
+ValidateStateMachineDefinitionMessage = str
 VersionDescription = str
 VersionWeight = int
 includedDetails = bool
 truncated = bool
 
 
 class ExecutionRedriveFilter(str):
@@ -173,14 +176,23 @@
 class TestExecutionStatus(str):
     SUCCEEDED = "SUCCEEDED"
     FAILED = "FAILED"
     RETRIABLE = "RETRIABLE"
     CAUGHT_ERROR = "CAUGHT_ERROR"
 
 
+class ValidateStateMachineDefinitionResultCode(str):
+    OK = "OK"
+    FAIL = "FAIL"
+
+
+class ValidateStateMachineDefinitionSeverity(str):
+    ERROR = "ERROR"
+
+
 class ValidationExceptionReason(str):
     API_DOES_NOT_SUPPORT_LABELED_ARNS = "API_DOES_NOT_SUPPORT_LABELED_ARNS"
     MISSING_REQUIRED_PARAMETER = "MISSING_REQUIRED_PARAMETER"
     CANNOT_UPDATE_COMPLETED_MAP_RUN = "CANNOT_UPDATE_COMPLETED_MAP_RUN"
     INVALID_ROUTING_CONFIGURATION = "INVALID_ROUTING_CONFIGURATION"
 
 
@@ -1235,14 +1247,37 @@
 
 class UpdateStateMachineOutput(TypedDict, total=False):
     updateDate: Timestamp
     revisionId: Optional[RevisionId]
     stateMachineVersionArn: Optional[Arn]
 
 
+class ValidateStateMachineDefinitionDiagnostic(TypedDict, total=False):
+    severity: ValidateStateMachineDefinitionSeverity
+    code: ValidateStateMachineDefinitionCode
+    message: ValidateStateMachineDefinitionMessage
+    location: Optional[ValidateStateMachineDefinitionLocation]
+
+
+ValidateStateMachineDefinitionDiagnosticList = List[ValidateStateMachineDefinitionDiagnostic]
+ValidateStateMachineDefinitionInput = TypedDict(
+    "ValidateStateMachineDefinitionInput",
+    {
+        "definition": Definition,
+        "type": Optional[StateMachineType],
+    },
+    total=False,
+)
+
+
+class ValidateStateMachineDefinitionOutput(TypedDict, total=False):
+    result: ValidateStateMachineDefinitionResultCode
+    diagnostics: ValidateStateMachineDefinitionDiagnosticList
+
+
 class StepfunctionsApi:
     service = "stepfunctions"
     version = "2016-11-23"
 
     @handler("CreateActivity")
     def create_activity(
         self, context: RequestContext, name: Name, tags: TagList = None, **kwargs
@@ -1555,7 +1590,13 @@
         context: RequestContext,
         state_machine_alias_arn: Arn,
         description: AliasDescription = None,
         routing_configuration: RoutingConfigurationList = None,
         **kwargs,
     ) -> UpdateStateMachineAliasOutput:
         raise NotImplementedError
+
+    @handler("ValidateStateMachineDefinition", expand=False)
+    def validate_state_machine_definition(
+        self, context: RequestContext, request: ValidateStateMachineDefinitionInput, **kwargs
+    ) -> ValidateStateMachineDefinitionOutput:
+        raise NotImplementedError
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/sts/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/support/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/swf/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/api/transcribe/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/app.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/chain.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/connect.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/data/sqs-json/2012-11-05/README.md` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/data/sqs-query/2012-11-05/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 This spec preserves the SQS query protocol spec, which was part of botocore until the protocol was switched to json with `botocore==1.31.81`.
 This switch removed a lot of spec data which is necessary for the proper parsing and serialization, which is why we have to preserve them on our own.
 
-- The spec content was preserved from this state: https://github.com/boto/botocore/blob/143e3925dac58976b5e83864a3ed9a2dea1db91b/botocore/data/sqs/2012-11-05/service-2.json
-- This was the last commit before the protocol switched back (again) to query (with https://github.com/boto/botocore/commit/143e3925dac58976b5e83864a3ed9a2dea1db91b).
+- The spec content was preserved from this state: https://github.com/boto/botocore/blob/79c92132e266b15f62bc743ae0816c27d598c36e/botocore/data/sqs/2012-11-05/service-2.json
+- This was the last commit before the protocol switched back (again) to json (with https://github.com/boto/botocore/commit/47a515f6727a7585487d58c069c7c0063c28899e).
 - The file is licensed with Apache License 2.0.
 - Modifications:
   - Removal of documentation strings with the following regex: `(,)?\n\s+"documentation":".*"`
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/data/sqs-json/2012-11-05/service-2.json` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/data/sqs-query/2012-11-05/service-2.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9225933273947549%*

 * *Differences: {"'metadata'": "{'protocol': 'query', 'xmlNamespace': "*

 * *               "'http://queue.amazonaws.com/doc/2012-11-05/', delete: ['awsQueryCompatible', "*

 * *               "'jsonVersion', 'targetPrefix']}",*

 * * "'operations'": "{'AddPermission': {'errors': {delete: [5, 4, 3, 2, 1]}}, "*

 * *                 "'CancelMessageMoveTask': {'output': {'resultWrapper': "*

 * *                 "'CancelMessageMoveTaskResult'}, 'errors': {delete: [3, 2, 1]}}, "*

 * *                 "'ChangeMessageVisibility': {'errors': {delete: [6, 5, 4, 3 […]*

```diff
@@ -1,41 +1,24 @@
 {
     "metadata": {
         "apiVersion": "2012-11-05",
-        "awsQueryCompatible": {},
         "endpointPrefix": "sqs",
-        "jsonVersion": "1.0",
-        "protocol": "json",
+        "protocol": "query",
         "serviceAbbreviation": "Amazon SQS",
         "serviceFullName": "Amazon Simple Queue Service",
         "serviceId": "SQS",
         "signatureVersion": "v4",
-        "targetPrefix": "AmazonSQS",
-        "uid": "sqs-2012-11-05"
+        "uid": "sqs-2012-11-05",
+        "xmlNamespace": "http://queue.amazonaws.com/doc/2012-11-05/"
     },
     "operations": {
         "AddPermission": {
             "errors": [
                 {
                     "shape": "OverLimit"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -45,60 +28,37 @@
         },
         "CancelMessageMoveTask": {
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
                     "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CancelMessageMoveTaskRequest"
             },
             "name": "CancelMessageMoveTask",
             "output": {
+                "resultWrapper": "CancelMessageMoveTaskResult",
                 "shape": "CancelMessageMoveTaskResult"
             }
         },
         "ChangeMessageVisibility": {
             "errors": [
                 {
                     "shape": "MessageNotInflight"
                 },
                 {
                     "shape": "ReceiptHandleIsInvalid"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -115,104 +75,58 @@
                     "shape": "EmptyBatchRequest"
                 },
                 {
                     "shape": "BatchEntryIdsNotDistinct"
                 },
                 {
                     "shape": "InvalidBatchEntryId"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ChangeMessageVisibilityBatchRequest"
             },
             "name": "ChangeMessageVisibilityBatch",
             "output": {
+                "resultWrapper": "ChangeMessageVisibilityBatchResult",
                 "shape": "ChangeMessageVisibilityBatchResult"
             }
         },
         "CreateQueue": {
             "errors": [
                 {
                     "shape": "QueueDeletedRecently"
                 },
                 {
                     "shape": "QueueNameExists"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidAttributeName"
-                },
-                {
-                    "shape": "InvalidAttributeValue"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidSecurity"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "CreateQueueRequest"
             },
             "name": "CreateQueue",
             "output": {
+                "resultWrapper": "CreateQueueResult",
                 "shape": "CreateQueueResult"
             }
         },
         "DeleteMessage": {
             "errors": [
                 {
                     "shape": "InvalidIdFormat"
                 },
                 {
                     "shape": "ReceiptHandleIsInvalid"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "InvalidAddress"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -229,352 +143,184 @@
                     "shape": "EmptyBatchRequest"
                 },
                 {
                     "shape": "BatchEntryIdsNotDistinct"
                 },
                 {
                     "shape": "InvalidBatchEntryId"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteMessageBatchRequest"
             },
             "name": "DeleteMessageBatch",
             "output": {
+                "resultWrapper": "DeleteMessageBatchResult",
                 "shape": "DeleteMessageBatchResult"
             }
         },
         "DeleteQueue": {
-            "errors": [
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "DeleteQueueRequest"
             },
             "name": "DeleteQueue"
         },
         "GetQueueAttributes": {
             "errors": [
                 {
                     "shape": "InvalidAttributeName"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "InvalidAddress"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetQueueAttributesRequest"
             },
             "name": "GetQueueAttributes",
             "output": {
+                "resultWrapper": "GetQueueAttributesResult",
                 "shape": "GetQueueAttributesResult"
             }
         },
         "GetQueueUrl": {
             "errors": [
                 {
-                    "shape": "RequestThrottled"
-                },
-                {
                     "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "GetQueueUrlRequest"
             },
             "name": "GetQueueUrl",
             "output": {
+                "resultWrapper": "GetQueueUrlResult",
                 "shape": "GetQueueUrlResult"
             }
         },
         "ListDeadLetterSourceQueues": {
             "errors": [
                 {
                     "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListDeadLetterSourceQueuesRequest"
             },
             "name": "ListDeadLetterSourceQueues",
             "output": {
+                "resultWrapper": "ListDeadLetterSourceQueuesResult",
                 "shape": "ListDeadLetterSourceQueuesResult"
             }
         },
         "ListMessageMoveTasks": {
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
                     "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListMessageMoveTasksRequest"
             },
             "name": "ListMessageMoveTasks",
             "output": {
+                "resultWrapper": "ListMessageMoveTasksResult",
                 "shape": "ListMessageMoveTasksResult"
             }
         },
         "ListQueueTags": {
-            "errors": [
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListQueueTagsRequest"
             },
             "name": "ListQueueTags",
             "output": {
+                "resultWrapper": "ListQueueTagsResult",
                 "shape": "ListQueueTagsResult"
             }
         },
         "ListQueues": {
-            "errors": [
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ListQueuesRequest"
             },
             "name": "ListQueues",
             "output": {
+                "resultWrapper": "ListQueuesResult",
                 "shape": "ListQueuesResult"
             }
         },
         "PurgeQueue": {
             "errors": [
                 {
                     "shape": "QueueDoesNotExist"
                 },
                 {
                     "shape": "PurgeQueueInProgress"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "PurgeQueueRequest"
             },
             "name": "PurgeQueue"
         },
         "ReceiveMessage": {
             "errors": [
                 {
-                    "shape": "UnsupportedOperation"
-                },
-                {
                     "shape": "OverLimit"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "KmsDisabled"
-                },
-                {
-                    "shape": "KmsInvalidState"
-                },
-                {
-                    "shape": "KmsNotFound"
-                },
-                {
-                    "shape": "KmsOptInRequired"
-                },
-                {
-                    "shape": "KmsThrottled"
-                },
-                {
-                    "shape": "KmsAccessDenied"
-                },
-                {
-                    "shape": "KmsInvalidKeyUsage"
-                },
-                {
-                    "shape": "InvalidAddress"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "ReceiveMessageRequest"
             },
             "name": "ReceiveMessage",
             "output": {
+                "resultWrapper": "ReceiveMessageResult",
                 "shape": "ReceiveMessageResult"
             }
         },
         "RemovePermission": {
-            "errors": [
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "RemovePermissionRequest"
             },
@@ -583,58 +329,26 @@
         "SendMessage": {
             "errors": [
                 {
                     "shape": "InvalidMessageContents"
                 },
                 {
                     "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "KmsDisabled"
-                },
-                {
-                    "shape": "KmsInvalidState"
-                },
-                {
-                    "shape": "KmsNotFound"
-                },
-                {
-                    "shape": "KmsOptInRequired"
-                },
-                {
-                    "shape": "KmsThrottled"
-                },
-                {
-                    "shape": "KmsAccessDenied"
-                },
-                {
-                    "shape": "KmsInvalidKeyUsage"
-                },
-                {
-                    "shape": "InvalidAddress"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "SendMessageRequest"
             },
             "name": "SendMessage",
             "output": {
+                "resultWrapper": "SendMessageResult",
                 "shape": "SendMessageResult"
             }
         },
         "SendMessageBatch": {
             "errors": [
                 {
                     "shape": "TooManyEntriesInBatchRequest"
@@ -649,86 +363,33 @@
                     "shape": "BatchRequestTooLong"
                 },
                 {
                     "shape": "InvalidBatchEntryId"
                 },
                 {
                     "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "KmsDisabled"
-                },
-                {
-                    "shape": "KmsInvalidState"
-                },
-                {
-                    "shape": "KmsNotFound"
-                },
-                {
-                    "shape": "KmsOptInRequired"
-                },
-                {
-                    "shape": "KmsThrottled"
-                },
-                {
-                    "shape": "KmsAccessDenied"
-                },
-                {
-                    "shape": "KmsInvalidKeyUsage"
-                },
-                {
-                    "shape": "InvalidAddress"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "SendMessageBatchRequest"
             },
             "name": "SendMessageBatch",
             "output": {
+                "resultWrapper": "SendMessageBatchResult",
                 "shape": "SendMessageBatchResult"
             }
         },
         "SetQueueAttributes": {
             "errors": [
                 {
                     "shape": "InvalidAttributeName"
-                },
-                {
-                    "shape": "InvalidAttributeValue"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                },
-                {
-                    "shape": "OverLimit"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
@@ -738,104 +399,64 @@
         },
         "StartMessageMoveTask": {
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
                     "shape": "UnsupportedOperation"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "StartMessageMoveTaskRequest"
             },
             "name": "StartMessageMoveTask",
             "output": {
+                "resultWrapper": "StartMessageMoveTaskResult",
                 "shape": "StartMessageMoveTaskResult"
             }
         },
         "TagQueue": {
-            "errors": [
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "TagQueueRequest"
             },
             "name": "TagQueue"
         },
         "UntagQueue": {
-            "errors": [
-                {
-                    "shape": "InvalidAddress"
-                },
-                {
-                    "shape": "RequestThrottled"
-                },
-                {
-                    "shape": "QueueDoesNotExist"
-                },
-                {
-                    "shape": "InvalidSecurity"
-                },
-                {
-                    "shape": "UnsupportedOperation"
-                }
-            ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "UntagQueueRequest"
             },
             "name": "UntagQueue"
         }
     },
     "shapes": {
         "AWSAccountIdList": {
             "flattened": true,
             "member": {
+                "locationName": "AWSAccountId",
                 "shape": "String"
             },
             "type": "list"
         },
         "ActionNameList": {
             "flattened": true,
             "member": {
+                "locationName": "ActionName",
                 "shape": "String"
             },
             "type": "list"
         },
         "AddPermissionRequest": {
             "members": {
                 "AWSAccountIds": {
@@ -858,34 +479,37 @@
                 "Actions"
             ],
             "type": "structure"
         },
         "AttributeNameList": {
             "flattened": true,
             "member": {
+                "locationName": "AttributeName",
                 "shape": "QueueAttributeName"
             },
             "type": "list"
         },
         "BatchEntryIdsNotDistinct": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.BatchEntryIdsNotDistinct",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "BatchRequestTooLong": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.BatchRequestTooLong",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "BatchResultErrorEntry": {
             "members": {
                 "Code": {
                     "shape": "String"
                 },
@@ -905,23 +529,25 @@
                 "Code"
             ],
             "type": "structure"
         },
         "BatchResultErrorEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "BatchResultErrorEntry",
                 "shape": "BatchResultErrorEntry"
             },
             "type": "list"
         },
         "Binary": {
             "type": "blob"
         },
         "BinaryList": {
             "member": {
+                "locationName": "BinaryListValue",
                 "shape": "Binary"
             },
             "type": "list"
         },
         "Boolean": {
             "type": "boolean"
         },
@@ -968,26 +594,27 @@
                 "Id": {
                     "shape": "String"
                 },
                 "ReceiptHandle": {
                     "shape": "String"
                 },
                 "VisibilityTimeout": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 }
             },
             "required": [
                 "Id",
                 "ReceiptHandle"
             ],
             "type": "structure"
         },
         "ChangeMessageVisibilityBatchRequestEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "ChangeMessageVisibilityBatchRequestEntry",
                 "shape": "ChangeMessageVisibilityBatchRequestEntry"
             },
             "type": "list"
         },
         "ChangeMessageVisibilityBatchResult": {
             "members": {
                 "Failed": {
@@ -1013,46 +640,49 @@
                 "Id"
             ],
             "type": "structure"
         },
         "ChangeMessageVisibilityBatchResultEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "ChangeMessageVisibilityBatchResultEntry",
                 "shape": "ChangeMessageVisibilityBatchResultEntry"
             },
             "type": "list"
         },
         "ChangeMessageVisibilityRequest": {
             "members": {
                 "QueueUrl": {
                     "shape": "String"
                 },
                 "ReceiptHandle": {
                     "shape": "String"
                 },
                 "VisibilityTimeout": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 }
             },
             "required": [
                 "QueueUrl",
                 "ReceiptHandle",
                 "VisibilityTimeout"
             ],
             "type": "structure"
         },
         "CreateQueueRequest": {
             "members": {
                 "Attributes": {
+                    "locationName": "Attribute",
                     "shape": "QueueAttributeMap"
                 },
                 "QueueName": {
                     "shape": "String"
                 },
                 "tags": {
+                    "locationName": "Tag",
                     "shape": "TagMap"
                 }
             },
             "required": [
                 "QueueName"
             ],
             "type": "structure"
@@ -1094,14 +724,15 @@
                 "ReceiptHandle"
             ],
             "type": "structure"
         },
         "DeleteMessageBatchRequestEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "DeleteMessageBatchRequestEntry",
                 "shape": "DeleteMessageBatchRequestEntry"
             },
             "type": "list"
         },
         "DeleteMessageBatchResult": {
             "members": {
                 "Failed": {
@@ -1127,14 +758,15 @@
                 "Id"
             ],
             "type": "structure"
         },
         "DeleteMessageBatchResultEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "DeleteMessageBatchResultEntry",
                 "shape": "DeleteMessageBatchResultEntry"
             },
             "type": "list"
         },
         "DeleteMessageRequest": {
             "members": {
                 "QueueUrl": {
@@ -1158,25 +790,23 @@
             },
             "required": [
                 "QueueUrl"
             ],
             "type": "structure"
         },
         "EmptyBatchRequest": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.EmptyBatchRequest",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
-        "ExceptionMessage": {
-            "type": "string"
-        },
         "GetQueueAttributesRequest": {
             "members": {
                 "AttributeNames": {
                     "shape": "AttributeNameList"
                 },
                 "QueueUrl": {
                     "shape": "String"
@@ -1186,14 +816,15 @@
                 "QueueUrl"
             ],
             "type": "structure"
         },
         "GetQueueAttributesResult": {
             "members": {
                 "Attributes": {
+                    "locationName": "Attribute",
                     "shape": "QueueAttributeMap"
                 }
             },
             "type": "structure"
         },
         "GetQueueUrlRequest": {
             "members": {
@@ -1213,136 +844,40 @@
             "members": {
                 "QueueUrl": {
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
-        "InvalidAddress": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
+        "Integer": {
+            "type": "integer"
         },
         "InvalidAttributeName": {
             "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "InvalidAttributeValue": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
+            "members": {},
             "type": "structure"
         },
         "InvalidBatchEntryId": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.InvalidBatchEntryId",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "InvalidIdFormat": {
-            "deprecated": true,
-            "deprecatedMessage": "exception has been included in ReceiptHandleIsInvalid",
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "InvalidMessageContents": {
             "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "InvalidSecurity": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsAccessDenied": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsDisabled": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsInvalidKeyUsage": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsInvalidState": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsNotFound": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsOptInRequired": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
-        "KmsThrottled": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
+            "members": {},
             "type": "structure"
         },
         "ListDeadLetterSourceQueuesRequest": {
             "members": {
                 "MaxResults": {
                     "shape": "BoxedInteger"
                 },
@@ -1371,50 +906,49 @@
                 "queueUrls"
             ],
             "type": "structure"
         },
         "ListMessageMoveTasksRequest": {
             "members": {
                 "MaxResults": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "SourceArn": {
                     "shape": "String"
                 }
             },
             "required": [
                 "SourceArn"
             ],
             "type": "structure"
         },
         "ListMessageMoveTasksResult": {
             "members": {
                 "Results": {
-                    "flattened": true,
                     "shape": "ListMessageMoveTasksResultEntryList"
                 }
             },
             "type": "structure"
         },
         "ListMessageMoveTasksResultEntry": {
             "members": {
                 "ApproximateNumberOfMessagesMoved": {
                     "shape": "Long"
                 },
                 "ApproximateNumberOfMessagesToMove": {
-                    "shape": "NullableLong"
+                    "shape": "Long"
                 },
                 "DestinationArn": {
                     "shape": "String"
                 },
                 "FailureReason": {
                     "shape": "String"
                 },
                 "MaxNumberOfMessagesPerSecond": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "SourceArn": {
                     "shape": "String"
                 },
                 "StartedTimestamp": {
                     "shape": "Long"
                 },
@@ -1426,14 +960,15 @@
                 }
             },
             "type": "structure"
         },
         "ListMessageMoveTasksResultEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "ListMessageMoveTasksResultEntry",
                 "shape": "ListMessageMoveTasksResultEntry"
             },
             "type": "list"
         },
         "ListQueueTagsRequest": {
             "members": {
                 "QueueUrl": {
@@ -1444,14 +979,15 @@
                 "QueueUrl"
             ],
             "type": "structure"
         },
         "ListQueueTagsResult": {
             "members": {
                 "Tags": {
+                    "locationName": "Tag",
                     "shape": "TagMap"
                 }
             },
             "type": "structure"
         },
         "ListQueuesRequest": {
             "members": {
@@ -1480,26 +1016,28 @@
         },
         "Long": {
             "type": "long"
         },
         "Message": {
             "members": {
                 "Attributes": {
+                    "locationName": "Attribute",
                     "shape": "MessageSystemAttributeMap"
                 },
                 "Body": {
                     "shape": "String"
                 },
                 "MD5OfBody": {
                     "shape": "String"
                 },
                 "MD5OfMessageAttributes": {
                     "shape": "String"
                 },
                 "MessageAttributes": {
+                    "locationName": "MessageAttribute",
                     "shape": "MessageBodyAttributeMap"
                 },
                 "MessageId": {
                     "shape": "String"
                 },
                 "ReceiptHandle": {
                     "shape": "String"
@@ -1509,82 +1047,98 @@
         },
         "MessageAttributeName": {
             "type": "string"
         },
         "MessageAttributeNameList": {
             "flattened": true,
             "member": {
+                "locationName": "MessageAttributeName",
                 "shape": "MessageAttributeName"
             },
             "type": "list"
         },
         "MessageAttributeValue": {
             "members": {
                 "BinaryListValues": {
                     "flattened": true,
+                    "locationName": "BinaryListValue",
                     "shape": "BinaryList"
                 },
                 "BinaryValue": {
                     "shape": "Binary"
                 },
                 "DataType": {
                     "shape": "String"
                 },
                 "StringListValues": {
                     "flattened": true,
+                    "locationName": "StringListValue",
                     "shape": "StringList"
                 },
                 "StringValue": {
                     "shape": "String"
                 }
             },
             "required": [
                 "DataType"
             ],
             "type": "structure"
         },
         "MessageBodyAttributeMap": {
             "flattened": true,
             "key": {
+                "locationName": "Name",
                 "shape": "String"
             },
             "type": "map",
             "value": {
+                "locationName": "Value",
                 "shape": "MessageAttributeValue"
             }
         },
         "MessageBodySystemAttributeMap": {
             "flattened": true,
             "key": {
+                "locationName": "Name",
                 "shape": "MessageSystemAttributeNameForSends"
             },
             "type": "map",
             "value": {
+                "locationName": "Value",
                 "shape": "MessageSystemAttributeValue"
             }
         },
         "MessageList": {
             "flattened": true,
             "member": {
+                "locationName": "Message",
                 "shape": "Message"
             },
             "type": "list"
         },
         "MessageNotInflight": {
+            "error": {
+                "code": "AWS.SimpleQueueService.MessageNotInflight",
+                "httpStatusCode": 400,
+                "senderFault": true
+            },
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "MessageSystemAttributeMap": {
             "flattened": true,
             "key": {
+                "locationName": "Name",
                 "shape": "MessageSystemAttributeName"
             },
+            "locationName": "Attribute",
             "type": "map",
             "value": {
+                "locationName": "Value",
                 "shape": "String"
             }
         },
         "MessageSystemAttributeName": {
             "enum": [
                 "SenderId",
                 "SentTimestamp",
@@ -1604,57 +1158,55 @@
             ],
             "type": "string"
         },
         "MessageSystemAttributeValue": {
             "members": {
                 "BinaryListValues": {
                     "flattened": true,
+                    "locationName": "BinaryListValue",
                     "shape": "BinaryList"
                 },
                 "BinaryValue": {
                     "shape": "Binary"
                 },
                 "DataType": {
                     "shape": "String"
                 },
                 "StringListValues": {
                     "flattened": true,
+                    "locationName": "StringListValue",
                     "shape": "StringList"
                 },
                 "StringValue": {
                     "shape": "String"
                 }
             },
             "required": [
                 "DataType"
             ],
             "type": "structure"
         },
-        "NullableInteger": {
-            "type": "integer"
-        },
-        "NullableLong": {
-            "type": "long"
-        },
         "OverLimit": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "OverLimit",
+                "httpStatusCode": 403,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "PurgeQueueInProgress": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.PurgeQueueInProgress",
+                "httpStatusCode": 403,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "PurgeQueueRequest": {
             "members": {
                 "QueueUrl": {
                     "shape": "String"
                 }
@@ -1663,18 +1215,21 @@
                 "QueueUrl"
             ],
             "type": "structure"
         },
         "QueueAttributeMap": {
             "flattened": true,
             "key": {
+                "locationName": "Name",
                 "shape": "QueueAttributeName"
             },
+            "locationName": "Attribute",
             "type": "map",
             "value": {
+                "locationName": "Value",
                 "shape": "String"
             }
         },
         "QueueAttributeName": {
             "enum": [
                 "All",
                 "Policy",
@@ -1698,78 +1253,78 @@
                 "FifoThroughputLimit",
                 "RedriveAllowPolicy",
                 "SqsManagedSseEnabled"
             ],
             "type": "string"
         },
         "QueueDeletedRecently": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.QueueDeletedRecently",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "QueueDoesNotExist": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.NonExistentQueue",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "QueueNameExists": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "QueueAlreadyExists",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "QueueUrlList": {
             "flattened": true,
             "member": {
+                "locationName": "QueueUrl",
                 "shape": "String"
             },
             "type": "list"
         },
         "ReceiptHandleIsInvalid": {
             "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
+            "members": {},
             "type": "structure"
         },
         "ReceiveMessageRequest": {
             "members": {
                 "AttributeNames": {
                     "shape": "AttributeNameList"
                 },
                 "MaxNumberOfMessages": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "MessageAttributeNames": {
                     "shape": "MessageAttributeNameList"
                 },
                 "QueueUrl": {
                     "shape": "String"
                 },
                 "ReceiveRequestAttemptId": {
                     "shape": "String"
                 },
                 "VisibilityTimeout": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "WaitTimeSeconds": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 }
             },
             "required": [
                 "QueueUrl"
             ],
             "type": "structure"
         },
@@ -1792,30 +1347,22 @@
             },
             "required": [
                 "QueueUrl",
                 "Label"
             ],
             "type": "structure"
         },
-        "RequestThrottled": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
-            },
-            "type": "structure"
-        },
         "ResourceNotFoundException": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "ResourceNotFoundException",
+                "httpStatusCode": 404,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "SendMessageBatchRequest": {
             "members": {
                 "Entries": {
                     "shape": "SendMessageBatchRequestEntryList"
                 },
@@ -1828,44 +1375,47 @@
                 "Entries"
             ],
             "type": "structure"
         },
         "SendMessageBatchRequestEntry": {
             "members": {
                 "DelaySeconds": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "Id": {
                     "shape": "String"
                 },
                 "MessageAttributes": {
+                    "locationName": "MessageAttribute",
                     "shape": "MessageBodyAttributeMap"
                 },
                 "MessageBody": {
                     "shape": "String"
                 },
                 "MessageDeduplicationId": {
                     "shape": "String"
                 },
                 "MessageGroupId": {
                     "shape": "String"
                 },
                 "MessageSystemAttributes": {
+                    "locationName": "MessageSystemAttribute",
                     "shape": "MessageBodySystemAttributeMap"
                 }
             },
             "required": [
                 "Id",
                 "MessageBody"
             ],
             "type": "structure"
         },
         "SendMessageBatchRequestEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "SendMessageBatchRequestEntry",
                 "shape": "SendMessageBatchRequestEntry"
             },
             "type": "list"
         },
         "SendMessageBatchResult": {
             "members": {
                 "Failed": {
@@ -1908,36 +1458,39 @@
                 "MD5OfMessageBody"
             ],
             "type": "structure"
         },
         "SendMessageBatchResultEntryList": {
             "flattened": true,
             "member": {
+                "locationName": "SendMessageBatchResultEntry",
                 "shape": "SendMessageBatchResultEntry"
             },
             "type": "list"
         },
         "SendMessageRequest": {
             "members": {
                 "DelaySeconds": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "MessageAttributes": {
+                    "locationName": "MessageAttribute",
                     "shape": "MessageBodyAttributeMap"
                 },
                 "MessageBody": {
                     "shape": "String"
                 },
                 "MessageDeduplicationId": {
                     "shape": "String"
                 },
                 "MessageGroupId": {
                     "shape": "String"
                 },
                 "MessageSystemAttributes": {
+                    "locationName": "MessageSystemAttribute",
                     "shape": "MessageBodySystemAttributeMap"
                 },
                 "QueueUrl": {
                     "shape": "String"
                 }
             },
             "required": [
@@ -1965,14 +1518,15 @@
                 }
             },
             "type": "structure"
         },
         "SetQueueAttributesRequest": {
             "members": {
                 "Attributes": {
+                    "locationName": "Attribute",
                     "shape": "QueueAttributeMap"
                 },
                 "QueueUrl": {
                     "shape": "String"
                 }
             },
             "required": [
@@ -1983,15 +1537,15 @@
         },
         "StartMessageMoveTaskRequest": {
             "members": {
                 "DestinationArn": {
                     "shape": "String"
                 },
                 "MaxNumberOfMessagesPerSecond": {
-                    "shape": "NullableInteger"
+                    "shape": "Integer"
                 },
                 "SourceArn": {
                     "shape": "String"
                 }
             },
             "required": [
                 "SourceArn"
@@ -2007,35 +1561,40 @@
             "type": "structure"
         },
         "String": {
             "type": "string"
         },
         "StringList": {
             "member": {
+                "locationName": "StringListValue",
                 "shape": "String"
             },
             "type": "list"
         },
         "TagKey": {
             "type": "string"
         },
         "TagKeyList": {
             "flattened": true,
             "member": {
+                "locationName": "TagKey",
                 "shape": "TagKey"
             },
             "type": "list"
         },
         "TagMap": {
             "flattened": true,
             "key": {
+                "locationName": "Key",
                 "shape": "TagKey"
             },
+            "locationName": "Tag",
             "type": "map",
             "value": {
+                "locationName": "Value",
                 "shape": "TagValue"
             }
         },
         "TagQueueRequest": {
             "members": {
                 "QueueUrl": {
                     "shape": "String"
@@ -2053,29 +1612,31 @@
         "TagValue": {
             "type": "string"
         },
         "Token": {
             "type": "string"
         },
         "TooManyEntriesInBatchRequest": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.TooManyEntriesInBatchRequest",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "UnsupportedOperation": {
-            "exception": true,
-            "members": {
-                "message": {
-                    "shape": "ExceptionMessage"
-                }
+            "error": {
+                "code": "AWS.SimpleQueueService.UnsupportedOperation",
+                "httpStatusCode": 400,
+                "senderFault": true
             },
+            "exception": true,
+            "members": {},
             "type": "structure"
         },
         "UntagQueueRequest": {
             "members": {
                 "QueueUrl": {
                     "shape": "String"
                 },
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/forwarder.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/gateway.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/analytics.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/auth.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/codec.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/cors.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/fallback.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/internal.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/internal_requests.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/legacy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/logging.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/metric_handler.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/partition_rewriter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/presigned_url.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/proxy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/region.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/service.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/handlers/service_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/mocking.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/op_router.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/parser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/serializer.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1600,21 +1600,42 @@
     None of the prominent XML frameworks for python allow HTML entity escapes when serializing XML.
     This serializer implements the following workaround:
     - Escape quotes and \r with their HTML entities (&quot; and &#xD;).
     - Since & is (correctly) escaped in XML, the serialized string contains &amp;quot; and &amp;#xD;
     - These double-escapes are corrected by replacing such strings with their original.
     """
 
+    # those are deleted from the JSON specs, but need to be kept for legacy reason (sent in 'x-amzn-query-error')
+    QUERY_PREFIXED_ERRORS = {
+        "BatchEntryIdsNotDistinct",
+        "BatchRequestTooLong",
+        "EmptyBatchRequest",
+        "InvalidBatchEntryId",
+        "MessageNotInflight",
+        "PurgeQueueInProgress",
+        "QueueDeletedRecently",
+        "TooManyEntriesInBatchRequest",
+        "UnsupportedOperation",
+    }
+
     # Some error code changed between JSON and query, and we need to have a way to map it for legacy reason
     JSON_TO_QUERY_ERROR_CODES = {
         "InvalidParameterValueException": "InvalidParameterValue",
         "MissingRequiredParameterException": "MissingParameter",
         "AccessDeniedException": "AccessDenied",
+        "QueueDoesNotExist": "AWS.SimpleQueueService.NonExistentQueue",
+        "QueueNameExists": "QueueAlreadyExists",
     }
 
+    SENDER_FAULT_ERRORS = (
+        QUERY_PREFIXED_ERRORS
+        | JSON_TO_QUERY_ERROR_CODES.keys()
+        | {"OverLimit", "ResourceNotFoundException"}
+    )
+
     def _default_serialize(self, xmlnode: ETree.Element, params: str, _, name: str, __) -> None:
         """
         Ensures that we "mark" characters in the node's text which need to be specifically encoded.
         This is necessary to easily identify these specific characters later, after the standard XML serialization is
         done, while not replacing any other occurrences of these characters which might appear in the serialized string.
         """
         node = ETree.SubElement(xmlnode, name)
@@ -1643,36 +1664,48 @@
         self, error: ServiceException, error_tag: ETree.Element, mime_type: str
     ) -> None:
         """The SQS API stubs is now generated from JSON specs, and some fields have been modified"""
         code_tag = ETree.SubElement(error_tag, "Code")
 
         if error.code in self.JSON_TO_QUERY_ERROR_CODES:
             error_code = self.JSON_TO_QUERY_ERROR_CODES[error.code]
+        elif error.code in self.QUERY_PREFIXED_ERRORS:
+            error_code = f"AWS.SimpleQueueService.{error.code}"
         else:
             error_code = error.code
         code_tag.text = error_code
         message = self._get_error_message(error)
         if message:
             self._default_serialize(error_tag, message, None, "Message", mime_type)
-        if error.sender_fault:
+        if error.code in self.SENDER_FAULT_ERRORS or error.sender_fault:
             # The sender fault is either not set or "Sender"
             self._default_serialize(error_tag, "Sender", None, "Type", mime_type)
 
 
 class SqsJsonResponseSerializer(JSONResponseSerializer):
+    # those are deleted from the JSON specs, but need to be kept for legacy reason (sent in 'x-amzn-query-error')
+    QUERY_PREFIXED_ERRORS = {
+        "BatchEntryIdsNotDistinct",
+        "BatchRequestTooLong",
+        "EmptyBatchRequest",
+        "InvalidBatchEntryId",
+        "MessageNotInflight",
+        "PurgeQueueInProgress",
+        "QueueDeletedRecently",
+        "TooManyEntriesInBatchRequest",
+        "UnsupportedOperation",
+    }
+
     # Some error code changed between JSON and query, and we need to have a way to map it for legacy reason
     JSON_TO_QUERY_ERROR_CODES = {
         "InvalidParameterValueException": "InvalidParameterValue",
         "MissingRequiredParameterException": "MissingParameter",
         "AccessDeniedException": "AccessDenied",
-    }
-
-    QUERY_TO_JSON_ERROR_CODES = {
-        "NonExistentQueue": "QueueDoesNotExist",
-        "QueueAlreadyExists": "QueueNameExists",
+        "QueueDoesNotExist": "AWS.SimpleQueueService.NonExistentQueue",
+        "QueueNameExists": "QueueAlreadyExists",
     }
 
     def _serialize_error(
         self,
         error: ServiceException,
         response: HttpResponse,
         shape: StructureShape,
@@ -1685,26 +1718,24 @@
         which contained the exception code as well as a Sender field.
         Ex: 'x-amzn-query-error': 'InvalidParameterValue;Sender'
         """
         # TODO: for body["__type"] = error.code, it seems AWS differs from what we send for SQS
         # AWS: "com.amazon.coral.service#InvalidParameterValueException"
         # or AWS: "com.amazonaws.sqs#BatchRequestTooLong"
         # LocalStack: "InvalidParameterValue"
-
+        super()._serialize_error(error, response, shape, operation_model, mime_type, request_id)
         # We need to add a prefix to certain errors, as they have been deleted in the specs. These will not change
         if error.code in self.JSON_TO_QUERY_ERROR_CODES:
             code = self.JSON_TO_QUERY_ERROR_CODES[error.code]
+        elif error.code in self.QUERY_PREFIXED_ERRORS:
+            code = f"AWS.SimpleQueueService.{error.code}"
         else:
             code = error.code
-        response.headers["x-amzn-query-error"] = f"{code};Sender"
 
-        error.code = error.code.removeprefix("AWS.SimpleQueueService.")
-        if error.code in self.QUERY_TO_JSON_ERROR_CODES:
-            error.code = self.QUERY_TO_JSON_ERROR_CODES[error.code]
-        super()._serialize_error(error, response, shape, operation_model, mime_type, request_id)
+        response.headers["x-amzn-query-error"] = f"{code};Sender"
 
 
 def gen_amzn_requestid():
     """
     Generate generic AWS request ID.
 
     3 uses a different format and set of request Ids.
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/service_router.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/service_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 
 def custom_path_addressing_rules(path: str) -> Optional[ServiceModelIdentifier]:
     """
     Rules which are only based on the request path.
     """
 
     if is_sqs_queue_url(path):
-        return ServiceModelIdentifier("sqs")
+        return ServiceModelIdentifier("sqs", protocol="query")
 
     if path.startswith("/2015-03-31/functions/"):
         return ServiceModelIdentifier("lambda")
 
 
 def legacy_rules(request: Request) -> Optional[ServiceModelIdentifier]:
     """
@@ -296,24 +296,24 @@
     if service_name_candidates == {"timestream-query", "timestream-write"}:
         return ServiceModelIdentifier("timestream-query")
     if service_name_candidates == {"docdb", "neptune", "rds"}:
         return ServiceModelIdentifier("rds")
     if service_name_candidates == {"sqs"}:
         # SQS now have 2 different specs for `query` and `json` protocol. From our current implementation with the
         # parser and serializer, we need to have 2 different service names for them, but they share one provider
-        # implementation. `sqs-json` represents the `json` protocol spec, and `sqs` the `query` protocol
+        # implementation. `sqs` represents the `json` protocol spec, and `sqs-query` the `query` protocol
         # (default again in botocore starting with 1.32.6).
         # The `application/x-amz-json-1.0` header is mandatory for requests targeting SQS with the `json` protocol. We
-        # can safely route them to the `sqs-json` JSON parser/serializer. If not present, route the request to the
-        # default sqs protocol (`query`).
+        # can safely route them to the `sqs` JSON parser/serializer. If not present, route the request to the
+        # sqs-query protocol.
         content_type = request.headers.get("Content-Type")
         return (
-            ServiceModelIdentifier("sqs", "json")
+            ServiceModelIdentifier("sqs")
             if content_type == "application/x-amz-json-1.0"
-            else ServiceModelIdentifier("sqs")
+            else ServiceModelIdentifier("sqs", "query")
         )
 
 
 def determine_aws_service_model_for_data_plane(
     request: Request, services: ServiceCatalog = None
 ) -> Optional[ServiceModel]:
     """
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/protocol/validate.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/scaffold.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/edge.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/hypercorn.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/twisted.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/twisted.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/serving/werkzeug.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/skeleton.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/spec-patches.json` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/spec.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,43 +93,44 @@
 
 
 def load_service(
     service: ServiceName, version: Optional[str] = None, protocol: Optional[ProtocolName] = None
 ) -> ServiceModel:
     """
     Loads a service
-    :param service: to load, f.e. "sqs". For custom, internalized, service protocol specs (f.e. sqs-json) it's also
-                    possible to directly define the protocol in the service name (f.e. use sqs-json)
+    :param service: to load, f.e. "sqs". For custom, internalized, service protocol specs (f.e. sqs-query) it's also
+                    possible to directly define the protocol in the service name (f.e. use sqs-query)
     :param version: of the service to load, f.e. "2012-11-05", by default the latest version will be used
     :param protocol: specific protocol to load for the specific service, f.e. "json" for the "sqs" service
                      if the service cannot be found
     :return: Loaded service model of the service
     :raises: UnknownServiceError if the service cannot be found
     :raises: UnknownServiceProtocolError if the specific protocol of the service cannot be found
     """
     service_description = loader.load_service_model(service, "service-2", version)
 
     # check if the protocol is defined, and if so, if the loaded service defines this protocol
     if protocol is not None and protocol != service_description.get("metadata", {}).get("protocol"):
         # if the protocol is defined, but not the one of the currently loaded service,
         # check if we already loaded the custom spec based on the naming convention (<service>-<protocol>),
-        # f.e. "sqs-json"
+        # f.e. "sqs-query"
         if service.endswith(f"-{protocol}"):
             # if so, we raise an exception
             raise UnknownServiceProtocolError(service_name=service, protocol=protocol)
         # otherwise we try to load it (recursively)
         try:
             return load_service(f"{service}-{protocol}", version, protocol=protocol)
         except UnknownServiceError:
             # raise an unknown protocol error in case the service also can't be loaded with the naming convention
             raise UnknownServiceProtocolError(service_name=service, protocol=protocol)
 
     # remove potential protocol names from the service name
-    # FIXME add more protocols here if we have to internalize more than just sqs-json
-    service = service.removesuffix("-json")
+    # FIXME add more protocols here if we have to internalize more than just sqs-query
+    # TODO this should not contain specific internalized serivce names
+    service = {"sqs-query": "sqs"}.get(service, service)
     return ServiceModel(service_description, service)
 
 
 def iterate_service_operations() -> Generator[Tuple[ServiceModel, OperationModel], None, None]:
     """
     Returns one record per operation in the AWS service spec, where the first item is the service model the operation
     belongs to, and the second is the operation model.
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/aws/trace.py` & `localstack_core-3.4.1.dev20240502123741/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/cli/exceptions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/cli/localstack.py` & `localstack_core-3.4.1.dev20240502123741/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/cli/lpm.py` & `localstack_core-3.4.1.dev20240502123741/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/cli/plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/cli/plugins.py` & `localstack_core-3.4.1.dev20240502123741/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/cli/profiles.py` & `localstack_core-3.4.1.dev20240502123741/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/config.py` & `localstack_core-3.4.1.dev20240502123741/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/constants.py` & `localstack_core-3.4.1.dev20240502123741/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/deprecations.py` & `localstack_core-3.4.1.dev20240502123741/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dev/kubernetes/__main__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dev/kubernetes/__main__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dev/run/__main__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dev/run/__main__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dev/run/configurators.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dev/run/configurators.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dev/run/paths.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dev/run/paths.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dns/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dns/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dns/plugins.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dns/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/dns/server.py` & `localstack_core-3.4.1.dev20240502123741/localstack/dns/server.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/aws.py` & `localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/extensions/api/extension.py` & `localstack_core-3.4.1.dev20240502123741/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/extensions/patterns/webapp.py` & `localstack_core-3.4.1.dev20240502123741/localstack/extensions/patterns/webapp.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/http/dispatcher.py` & `localstack_core-3.4.1.dev20240502123741/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/http/duplex_socket.py` & `localstack_core-3.4.1.dev20240502123741/localstack/http/duplex_socket.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/http/hypercorn.py` & `localstack_core-3.4.1.dev20240502123741/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/http/response.py` & `localstack_core-3.4.1.dev20240502123741/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/http/router.py` & `localstack_core-3.4.1.dev20240502123741/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/logging/format.py` & `localstack_core-3.4.1.dev20240502123741/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/logging/setup.py` & `localstack_core-3.4.1.dev20240502123741/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/packages/__init__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/packages/api.py` & `localstack_core-3.4.1.dev20240502123741/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/packages/core.py` & `localstack_core-3.4.1.dev20240502123741/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/packages/debugpy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/packages/ffmpeg.py` & `localstack_core-3.4.1.dev20240502123741/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/packages/terraform.py` & `localstack_core-3.4.1.dev20240502123741/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/plugins.py` & `localstack_core-3.4.1.dev20240502123741/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/runtime/analytics.py` & `localstack_core-3.4.1.dev20240502123741/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/runtime/hooks.py` & `localstack_core-3.4.1.dev20240502123741/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/runtime/init.py` & `localstack_core-3.4.1.dev20240502123741/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/runtime/main.py` & `localstack_core-3.4.1.dev20240502123741/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/runtime/shutdown.py` & `localstack_core-3.4.1.dev20240502123741/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/acm/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/context.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/exporter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/exporter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/helpers.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/integration.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/invocations.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/patches.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_account.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_account.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_account.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_account_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_apikey.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_apikey_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_basepathmapping_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_deployment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_deployment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_domainname.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_domainname_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_gatewayresponse_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_method.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_method.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_method.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_method_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_model.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_model.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_model.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_model_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_requestvalidator_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_resource.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_resource.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_resource_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_restapi.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_restapi_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_stage.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_stage.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_stage_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplan_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/resource_providers/aws_apigateway_usageplankey_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/router_asf.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/apigateway/templates.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/cdk_metadata.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/cdk_metadata.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cdk/resource_providers/cdk_metadata_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/certificatemanager/resource_providers/aws_certificatemanager_certificate_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/api_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/cfn_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/deploy.html` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/deployment_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/entities.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/parameters.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/quirks.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/quirks.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/template_deployer.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/template_preparer.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/template_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/template_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/transformers.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/types.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/types.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/provider_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/provider_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_macro_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_stack_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitcondition_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/resource_providers/aws_cloudformation_waitconditionhandle_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/scaffolding/__main__.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/scaffolding/__main__.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/scaffolding/propgen.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/scaffolding/propgen.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/service_models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudformation/stores.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/cloudwatch_database_helper.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/cloudwatch_database_helper.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/provider_v2.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_alarm_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/cloudwatch/resource_providers/aws_cloudwatch_compositealarm_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_globaltable_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_table.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/resource_providers/aws_dynamodb_table_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/server.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodb/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/dynamodbstreams/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/exceptions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_dhcpoptions_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_instance.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_instance.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_instance.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_instance_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_internetgateway.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_internetgateway_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_keypair.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_keypair.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_keypair.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_keypair_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_natgateway.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_natgateway.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_natgateway_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_networkacl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_networkacl.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_networkacl_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_prefixlist.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_prefixlist_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_prefixlist_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_route.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_route.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_route.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_routetable.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_routetable.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_routetable.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_routetable_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_securitygroup.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_securitygroup_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnet.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnet.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnet.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnet_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_subnetroutetableassociation_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgateway.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgateway_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_transitgatewayattachment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpc.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpc.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpc.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcendpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ec2/resource_providers/aws_ec2_vpcgatewayattachment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/aws_ecr_repository.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/aws_ecr_repository.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/aws_ecr_repository.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ecr/resource_providers/aws_ecr_repository_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/edge.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/es/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/event_bus.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/event_bus.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/event_ruler.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/event_ruler.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/models_v2.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/models_v2.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/provider_v2.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_apidestination.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_apidestination.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_apidestination.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_apidestination.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_apidestination_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_apidestination_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_connection.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_connection.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_connection.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_connection.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_connection_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_connection_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbus.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbus.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbus.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbus.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbus_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbuspolicy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbuspolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_eventbuspolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_rule.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_rule.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_rule.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_rule.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/resource_providers/aws_events_rule_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/resource_providers/aws_events_rule_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/rule.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/rule.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/scheduler.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/target.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/target.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/events/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/events/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/mappers.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/firehose/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_accesskey.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_accesskey.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_accesskey.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_accesskey_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_group.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_group.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_group.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_group.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_instanceprofile.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_instanceprofile.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_instanceprofile_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_managedpolicy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_managedpolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_managedpolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_policy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_policy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_policy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_policy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_policy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_role.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_role.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_role.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_role.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servercertificate.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servercertificate.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servercertificate.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servercertificate_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_servicelinkedrole_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_user.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_user.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/iam/resource_providers/aws_iam_user.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/iam/resource_providers/aws_iam_user.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/infra.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/internal.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/kinesis_mock_server.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_stream.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_stream.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_stream_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesis/resource_providers/aws_kinesis_streamconsumer_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kinesisfirehose/resource_providers/aws_kinesisfirehose_deliverystream_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_alias.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_alias.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_alias.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_alias.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_key.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_key.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/resource_providers/aws_kms_key.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/resource_providers/aws_kms_key.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/kms/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/api_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/custom_endpoints.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/custom_endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/adapters.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/event_source_listener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/lambda_legacy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/lambda_legacy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/event_source_listeners/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/event_source_listeners/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/hooks.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/assignment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/assignment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/counting_service.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/counting_service.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/docker_runtime_executor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/event_manager.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/event_manager.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/execution_environment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/execution_environment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/executor_endpoint.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/internal_sqs_queue.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/internal_sqs_queue.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 from typing import Iterable
 
 from localstack import config
 from localstack.aws.api.sqs import (
     AttributeNameList,
     CreateQueueResult,
     GetQueueAttributesResult,
-    Integer,
     Message,
     MessageAttributeNameList,
     MessageBodyAttributeMap,
     MessageBodySystemAttributeMap,
     MessageSystemAttributeName,
+    NullableInteger,
     QueueAttributeMap,
     ReceiveMessageResult,
     SendMessageResult,
     String,
     TagMap,
 )
 from localstack.services.sqs.models import SqsQueue, StandardQueue
@@ -128,17 +128,17 @@
         queue.clear()
 
     def receive_message(
         self,
         QueueUrl: String,
         AttributeNames: AttributeNameList = None,
         MessageAttributeNames: MessageAttributeNameList = None,
-        MaxNumberOfMessages: Integer = None,
-        VisibilityTimeout: Integer = None,
-        WaitTimeSeconds: Integer = None,
+        MaxNumberOfMessages: NullableInteger = None,
+        VisibilityTimeout: NullableInteger = None,
+        WaitTimeSeconds: NullableInteger = None,
         ReceiveRequestAttemptId: String = None,
     ) -> ReceiveMessageResult:
         queue = self.queue_manager.get_queue(queue_name=QueueUrl)
         num = MaxNumberOfMessages or 1
         result = queue.receive(
             num_messages=num,
             visibility_timeout=VisibilityTimeout,
@@ -172,15 +172,15 @@
 
         return result
 
     def send_message(
         self,
         QueueUrl: String,
         MessageBody: String,
-        DelaySeconds: Integer = None,
+        DelaySeconds: NullableInteger = None,
         MessageAttributes: MessageBodyAttributeMap = None,
         MessageSystemAttributes: MessageBodySystemAttributeMap = None,
         MessageDeduplicationId: String = None,
         MessageGroupId: String = None,
     ) -> SendMessageResult:
         queue = self.queue_manager.get_queue(queue_name=QueueUrl)
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/lambda_models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/lambda_service.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/logs.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/logs.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/metrics.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/metrics.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/runtime_executor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/invocation/version_manager.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/lambda_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/layerfetcher/layer_fetcher.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/networking.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/networking.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/plugins.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_codesigningconfig_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventinvokeconfig_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_eventsourcemapping_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_function.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_function.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_function.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_function_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversion.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversion_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_layerversionpermission_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_permission.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_permission.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_permission.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_permission_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_url.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_url.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_url.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_url_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_version.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_version.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_version.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/aws_lambda_version_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/lambda_alias.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/lambda_alias.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/lambda_alias.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/lambda_alias.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/resource_providers/lambda_alias_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/runtimes.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/runtimes.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/lambda_/urlrouter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/lambda_/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_loggroup.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_loggroup.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_loggroup.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_loggroup_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_logstream.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_logstream.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_logstream.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_logstream_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/logs/resource_providers/aws_logs_subscriptionfilter_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/messages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/moto.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/cluster.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/cluster_manager.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_elasticsearch_domain_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/resource_providers/aws_opensearchservice_domain_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/opensearch/versions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/plugins.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/providers.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/aws_redshift_cluster.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/aws_redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/aws_redshift_cluster.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/redshift/resource_providers/aws_redshift_cluster_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/resource_groups/resource_providers/aws_resourcegroups_group_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_healthcheck.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_healthcheck.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_healthcheck.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_healthcheck_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_recordset.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_recordset.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_recordset.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53/resource_providers/aws_route53_recordset_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/route53resolver/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/codec.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/codec.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/constants.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/cors.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/exceptions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/notifications.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/presigned_url.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucket.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucket.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucketpolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/resource_providers/aws_s3_bucketpolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/utils_moto.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/utils_moto.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/storage/core.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/storage/core.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/v3/storage/ephemeral.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/v3/storage/ephemeral.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/validation.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/validation.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/virtual_host.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/s3/website_hosting.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedule.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedule_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/scheduler/resource_providers/aws_scheduler_schedulegroup_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_resourcepolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_rotationschedule_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secret_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/secretsmanager/resource_providers/aws_secretsmanager_secrettargetattachment_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ses/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/certificate.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/certificate.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/constants.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/publisher.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_subscription.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_subscription.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_subscription.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_subscription_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topic.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topic.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topic.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topic.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topicpolicy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topicpolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sns/resource_providers/aws_sns_topicpolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/constants.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/exceptions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/models.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     CreateQueueResult,
     DeleteMessageBatchRequestEntryList,
     DeleteMessageBatchResult,
     DeleteMessageBatchResultEntry,
     EmptyBatchRequest,
     GetQueueAttributesResult,
     GetQueueUrlResult,
-    Integer,
     InvalidAttributeName,
     InvalidBatchEntryId,
     InvalidMessageContents,
     ListDeadLetterSourceQueuesResult,
     ListMessageMoveTasksResult,
     ListMessageMoveTasksResultEntry,
     ListQueuesResult,
     ListQueueTagsResult,
     Message,
     MessageAttributeNameList,
     MessageBodyAttributeMap,
     MessageBodySystemAttributeMap,
     MessageSystemAttributeName,
+    NullableInteger,
     PurgeQueueInProgress,
     QueueAttributeMap,
     QueueAttributeName,
     QueueDeletedRecently,
     QueueDoesNotExist,
     QueueNameExists,
     ReceiveMessageResult,
@@ -616,19 +616,19 @@
     A set of SQS developer tool endpoints:
 
     - ``/_aws/sqs/messages``: list SQS messages without side effects, compatible with ``ReceiveMessage``.
     """
 
     def __init__(self, stores=None):
         self.stores = stores or sqs_stores
-        self.service = load_service("sqs")
+        self.service = load_service("sqs-query")
         self.serializer = create_serializer(self.service)
 
     @route("/_aws/sqs/messages")
-    @aws_response_serializer("sqs", "ReceiveMessage")
+    @aws_response_serializer("sqs-query", "ReceiveMessage")
     def list_messages(self, request: Request) -> ReceiveMessageResult:
         """
         This endpoint expects a ``QueueUrl`` request parameter (either as query arg or form parameter), similar to
         the ``ReceiveMessage`` operation. It will parse the Queue URL generated by one of the SQS endpoint strategies.
         """
         # TODO migrate this endpoint to JSON (the new default protocol for SQS), or implement content negotiation
         if "Action" in request.values and request.values["Action"] != "ReceiveMessage":
@@ -647,15 +647,15 @@
 
         if not region:
             region = extract_region_from_headers(request.headers)
 
         return self._get_and_serialize_messages(request, region, account_id, queue_name)
 
     @route("/_aws/sqs/messages/<region>/<account_id>/<queue_name>")
-    @aws_response_serializer("sqs", "ReceiveMessage")
+    @aws_response_serializer("sqs-query", "ReceiveMessage")
     def list_messages_for_queue_url(
         self, request: Request, region: str, account_id: str, queue_name: str
     ) -> ReceiveMessageResult:
         """
         This endpoint extracts the region, account_id, and queue_name directly from the URL rather than requiring the
         QueueUrl as parameter.
         """
@@ -952,15 +952,15 @@
         return ListQueuesResult(QueueUrls=urls)
 
     def change_message_visibility(
         self,
         context: RequestContext,
         queue_url: String,
         receipt_handle: String,
-        visibility_timeout: Integer,
+        visibility_timeout: NullableInteger,
         **kwargs,
     ) -> None:
         queue = self._resolve_queue(context, queue_url=queue_url)
         queue.update_visibility_timeout(receipt_handle, visibility_timeout)
 
     def change_message_visibility_batch(
         self,
@@ -1035,15 +1035,15 @@
         return GetQueueAttributesResult(Attributes=(result if result else None))
 
     def send_message(
         self,
         context: RequestContext,
         queue_url: String,
         message_body: String,
-        delay_seconds: Integer = None,
+        delay_seconds: NullableInteger = None,
         message_attributes: MessageBodyAttributeMap = None,
         message_system_attributes: MessageBodySystemAttributeMap = None,
         message_deduplication_id: String = None,
         message_group_id: String = None,
         **kwargs,
     ) -> SendMessageResult:
         queue = self._resolve_queue(context, queue_url=queue_url)
@@ -1141,15 +1141,15 @@
         )
 
     def _put_message(
         self,
         queue: SqsQueue,
         context: RequestContext,
         message_body: String,
-        delay_seconds: Integer = None,
+        delay_seconds: NullableInteger = None,
         message_attributes: MessageBodyAttributeMap = None,
         message_system_attributes: MessageBodySystemAttributeMap = None,
         message_deduplication_id: String = None,
         message_group_id: String = None,
     ) -> SqsMessage:
         check_message_size(message_body, message_attributes, queue.maximum_message_size)
         check_message_content(message_body)
@@ -1180,17 +1180,17 @@
 
     def receive_message(
         self,
         context: RequestContext,
         queue_url: String,
         attribute_names: AttributeNameList = None,
         message_attribute_names: MessageAttributeNameList = None,
-        max_number_of_messages: Integer = None,
-        visibility_timeout: Integer = None,
-        wait_time_seconds: Integer = None,
+        max_number_of_messages: NullableInteger = None,
+        visibility_timeout: NullableInteger = None,
+        wait_time_seconds: NullableInteger = None,
         receive_request_attempt_id: String = None,
         **kwargs,
     ) -> ReceiveMessageResult:
         queue = self._resolve_queue(context, queue_url=queue_url)
 
         if wait_time_seconds is None:
             wait_time_seconds = queue.wait_time_seconds
@@ -1360,15 +1360,19 @@
             if not valid_count:
                 raise InvalidParameterValueException(
                     f"Value {redrive_policy} for parameter RedrivePolicy is invalid. Reason: Invalid value for "
                     f"maxReceiveCount: {max_receive_count}, valid values are from 1 to 1000 both inclusive."
                 )
 
     def list_message_move_tasks(
-        self, context: RequestContext, source_arn: String, max_results: Integer = None, **kwargs
+        self,
+        context: RequestContext,
+        source_arn: String,
+        max_results: NullableInteger = None,
+        **kwargs,
     ) -> ListMessageMoveTasksResult:
         try:
             self._require_queue_by_arn(context, source_arn)
         except InvalidArnException:
             raise InvalidParameterValueException(
                 "You must use this format to specify the SourceArn: arn:<partition>:<service>:<region>:<account-id>:<resource-id>"
             )
@@ -1426,15 +1430,15 @@
         return entry
 
     def start_message_move_task(
         self,
         context: RequestContext,
         source_arn: String,
         destination_arn: String = None,
-        max_number_of_messages_per_second: Integer = None,
+        max_number_of_messages_per_second: NullableInteger = None,
         **kwargs,
     ) -> StartMessageMoveTaskResult:
         try:
             self._require_queue_by_arn(context, source_arn)
         except QueueDoesNotExist as e:
             raise ResourceNotFoundException(
                 "The resource that you specified for the SourceArn parameter doesn't exist.",
@@ -1824,9 +1828,11 @@
             matched.append(k)
             continue
 
         for prefix in prefixes:
             if k.startswith(prefix):
                 matched.append(k)
             break
-
-    message["MessageAttributes"] = {k: attributes[k] for k in matched}
+    if matched:
+        message["MessageAttributes"] = {k: attributes[k] for k in matched}
+    else:
+        message.pop("MessageAttributes")
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/query_api.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/query_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     extract_access_key_id_from_auth_header,
     extract_region_from_headers,
 )
 from localstack.utils.strings import long_uid
 
 LOG = logging.getLogger(__name__)
 
-service = load_service("sqs")
+service = load_service("sqs-query")
 parser = create_parser(service)
 serializer = create_serializer(service)
 
 
 @route(
     '/<regex("[0-9]{12}"):account_id>/<regex("[a-zA-Z0-9_-]+(.fifo)?"):queue_name>',
     host='sqs.<regex("([a-z0-9-]+\\.)?"):region><regex(".*"):domain><regex("(:[0-9]{2,5})?"):port>',
@@ -211,15 +211,15 @@
     #  problem yet since we generally don't enforce permissions.
     account_id: Optional[str] = extract_access_key_id_from_auth_header(headers)
 
     client = connect_to(
         region_name=region,
         aws_access_key_id=account_id or INTERNAL_AWS_ACCESS_KEY_ID,
         aws_secret_access_key=INTERNAL_AWS_SECRET_ACCESS_KEY,
-    ).sqs
+    ).sqs_query
 
     try:
         # using the layer below boto3.client("sqs").<operation>(...) to make the call
         boto_response = client._make_api_call(operation.name, service_request)
     except ClientError as e:
         raise BotoException(e.response) from e
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queue.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queue.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queue.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/resource_providers/aws_sqs_queuepolicy_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sqs/utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindow_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtarget_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_maintenancewindowtask_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_parameter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_parameter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_parameter.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_parameter_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/ssm/resource_providers/aws_ssm_patchbaseline_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/Makefile` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/Makefile`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicLexer.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserListener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLIntrinsicParserVisitor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLLexer.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLParser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserListener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlr/runtime/ASLParserVisitor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/jitter_strategy_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/max_delay_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/timeouts/heartbeat.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/common/timeouts/timeout.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_context_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_variable.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/variable.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/item_reader_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/input_type.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/max_items_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/reader_config/reader_config_props.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_eval_s3.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_csv.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_reader/resource_eval/resource_output_transformer/resource_output_transformer_json.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/item_selector.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/distributed_iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/inline_iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/distributed_item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/inline_item_processor_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/item_processor_factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/map_run_record.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/itemprocessor/processor_config.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_component.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_declaration.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iteration_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/distributed_iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/inline_iterator_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/iterator/iterator_factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/iteration/job.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branch_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/lambda_eval_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_api_gateway.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_callback.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_ecs.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_events.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sfn.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sns.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_activitiy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_factory.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/cause_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/error_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/program/test_state_program.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/program/test_state_program.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/component/test_state/state/test_state_state_props.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/component/test_state/state/test_state_state_props.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/callback/callback.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/callback/callback.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/program_state.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/program_state.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/eval/test_state/environment.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/eval/test_state/environment.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/test_state/asl_parser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/test_state/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/test_state/preprocessor.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/test_state/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/static_analyser/test_state/test_state_analyser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/static_analyser/test_state/test_state_analyser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/boto_client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/boto_client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/asl/utils/json_path.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/asl/utils/json_path.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/activity.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/activity.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/execution.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/state_machine.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/store.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/test_state/execution.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/test_state/execution.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/backend/test_state/execution_worker.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/backend/test_state/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/legacy/provider_legacy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/legacy/provider_legacy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/legacy/stepfunctions_starter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/legacy/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_activity_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine.schema.json`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/resource_providers/aws_stepfunctions_statemachine_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/stores.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/sts/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/packages.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/packages.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/services/transcribe/provider.py` & `localstack_core-3.4.1.dev20240502123741/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/state/core.py` & `localstack_core-3.4.1.dev20240502123741/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/state/inspect.py` & `localstack_core-3.4.1.dev20240502123741/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/state/pickle.py` & `localstack_core-3.4.1.dev20240502123741/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/state/snapshot.py` & `localstack_core-3.4.1.dev20240502123741/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/asf_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/cloudformation_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/eventbus_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/eventbus_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/lambda_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/aws/util.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/cloudtrail_tracking_stack.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/cloudtrail_tracking/handler/index.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking/tests/test_cloudtrail_tracking_handler.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/cloudtrail_tracking.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/cloudtrail_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/container.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/container.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/detect_thread_leakage.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/filters.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/fixture_conflicts.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/fixtures.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1918,14 +1918,20 @@
         is_aws_cloud(),
         reason="test only applicable if run against localstack",
     )
     for item in items:
         for mark in item.iter_markers():
             if mark.name.endswith("only_localstack"):
                 item.add_marker(only_localstack)
+        if hasattr(item, "fixturenames") and "snapshot" in item.fixturenames:
+            # add a marker that indicates that this test is snapshot validated
+            # if it uses the snapshot fixture -> allows selecting only snapshot
+            # validated tests in order to capture new snapshots for a whole
+            # test file with "-m snapshot_validated"
+            item.add_marker("snapshot_validated")
 
 
 @pytest.fixture
 def sample_stores() -> AccountRegionBundle:
     class SampleStore(BaseStore):
         CROSS_ACCOUNT_ATTR = CrossAccountAttribute(default=list)
         CROSS_REGION_ATTR = CrossRegionAttribute(default=list)
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/in_memory_localstack.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/in_memory_localstack.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/marker_report.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/marker_report.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/marking.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/marking.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/metric_collection.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/path_filter.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/path_filter.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/util.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/pytest/validation_tracking.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/pytest/validation_tracking.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/scenario/cdk_lambda_helper.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/scenario/cdk_lambda_helper.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/scenario/provisioning.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/scenario/provisioning.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/snapshots/transformer_utility.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/git.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/git.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/github.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/github.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/matching.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/matching.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/opt_in.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/opt_in.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/filter_by_test_selection.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/filter_by_test_selection.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/generate_test_selection_from_commits.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/scripts/generate_test_selection_from_pr.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/testing/testselection/testselection.py` & `localstack_core-3.4.1.dev20240502123741/localstack/testing/testselection/testselection.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/cli.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/events.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/logger.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/metadata.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/publisher.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/service_request_aggregator.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/analytics/usage.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/archives.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/asyncio.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/auth.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/arns.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/aws_responses.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/aws_stack.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/client_types.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/client_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     servicediscovery: Union[
         "ServiceDiscoveryClient", "MetadataRequestInjector[ServiceDiscoveryClient]"
     ]
     ses: Union["SESClient", "MetadataRequestInjector[SESClient]"]
     sesv2: Union["SESV2Client", "MetadataRequestInjector[SESV2Client]"]
     sns: Union["SNSClient", "MetadataRequestInjector[SNSClient]"]
     sqs: Union["SQSClient", "MetadataRequestInjector[SQSClient]"]
-    sqs_json: Union["SQSClient", "MetadataRequestInjector[SQSClient]"]
+    sqs_query: Union["SQSClient", "MetadataRequestInjector[SQSClient]"]
     ssm: Union["SSMClient", "MetadataRequestInjector[SSMClient]"]
     sso_admin: Union["SSOAdminClient", "MetadataRequestInjector[SSOAdminClient]"]
     stepfunctions: Union["SFNClient", "MetadataRequestInjector[SFNClient]"]
     sts: Union["STSClient", "MetadataRequestInjector[STSClient]"]
     timestream_query: Union[
         "TimestreamQueryClient", "MetadataRequestInjector[TimestreamQueryClient]"
     ]
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/dead_letter_queue.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/message_forwarding.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/queries.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/request_context.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/resources.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/aws/templating.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/bootstrap.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/collections.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/common.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/config_listener.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/container_networking.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/container_client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/docker_cmd_client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/container_utils/docker_sdk_client.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/coverage_docs.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/crypto.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/diagnose.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/docker_utils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/files.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/functions.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/http.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/iputils.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/iputils.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/json.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/kinesis/kclipy_helper.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/kinesis/kinesis_connector.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/net.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/no_exit_argument_parser.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/numbers.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/objects.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/patch.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/platform.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/run.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/scheduler.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/server/http2_server.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/server/tcp_proxy.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/server/tcp_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/serving.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/ssl.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/strings.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/sync.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/tagging.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/testutil.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/threads.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/time.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/urls.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/venv.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack/utils/xml.py` & `localstack_core-3.4.1.dev20240502123741/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/PKG-INFO` & `localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 3.4.1.dev20240502085340
+Version: 3.4.1.dev20240502123741
 Summary: The core library and runtime of LocalStack
 Author-email: LocalStack Contributors <info@localstack.cloud>
 Project-URL: Homepage, https://localstack.cloud
 Project-URL: Documentation, https://docs.localstack.cloud
 Project-URL: Repository, https://github.com/localstack/localstack.git
 Project-URL: Issues, https://github.com/localstack/localstack/issues
 Classifier: Programming Language :: Python :: 3
@@ -28,16 +28,16 @@
 Requires-Dist: pyyaml>=5.1
 Requires-Dist: rich>=12.3.0
 Requires-Dist: requests>=2.20.0
 Requires-Dist: semver>=2.10
 Requires-Dist: stevedore>=3.4.0
 Requires-Dist: tailer>=0.4.1
 Provides-Extra: base-runtime
-Requires-Dist: boto3==1.34.84; extra == "base-runtime"
-Requires-Dist: botocore==1.34.84; extra == "base-runtime"
+Requires-Dist: boto3==1.34.93; extra == "base-runtime"
+Requires-Dist: botocore==1.34.93; extra == "base-runtime"
 Requires-Dist: awscrt>=0.13.14; extra == "base-runtime"
 Requires-Dist: cbor2>=5.2.0; extra == "base-runtime"
 Requires-Dist: dnspython>=1.16.0; extra == "base-runtime"
 Requires-Dist: docker<7.0.0,>=6.1.1; extra == "base-runtime"
 Requires-Dist: jsonpatch>=1.24; extra == "base-runtime"
 Requires-Dist: hypercorn>=0.14.4; extra == "base-runtime"
 Requires-Dist: localstack-twisted>=23.0; extra == "base-runtime"
@@ -48,15 +48,15 @@
 Requires-Dist: Werkzeug>=3.0.0; extra == "base-runtime"
 Requires-Dist: xmltodict>=0.13.0; extra == "base-runtime"
 Requires-Dist: rolo>=0.4; extra == "base-runtime"
 Requires-Dist: flask>=3.0.0; extra == "base-runtime"
 Requires-Dist: Quart>=0.19.2; extra == "base-runtime"
 Provides-Extra: runtime
 Requires-Dist: localstack-core[base-runtime]; extra == "runtime"
-Requires-Dist: awscli==1.32.84; extra == "runtime"
+Requires-Dist: awscli==1.32.93; extra == "runtime"
 Requires-Dist: airspeed-ext>=0.6.3; extra == "runtime"
 Requires-Dist: amazon_kclpy!=2.1.0,!=2.1.4,>=2.0.6; extra == "runtime"
 Requires-Dist: antlr4-python3-runtime==4.13.1; extra == "runtime"
 Requires-Dist: apispec>=5.1.1; extra == "runtime"
 Requires-Dist: aws-sam-translator>=1.15.1; extra == "runtime"
 Requires-Dist: crontab>=0.22.6; extra == "runtime"
 Requires-Dist: cryptography>=41.0.5; extra == "runtime"
@@ -90,8 +90,8 @@
 Requires-Dist: pandoc; extra == "dev"
 Requires-Dist: pre-commit>=3.5.0; extra == "dev"
 Requires-Dist: pypandoc; extra == "dev"
 Requires-Dist: ruff>=0.3.3; extra == "dev"
 Requires-Dist: rstr>=3.2.0; extra == "dev"
 Provides-Extra: typehint
 Requires-Dist: localstack-core[dev]; extra == "typehint"
-Requires-Dist: boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.84; extra == "typehint"
+Requires-Dist: boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.93; extra == "typehint"
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/SOURCES.txt` & `localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 localstack/aws/api/sqs/__init__.py
 localstack/aws/api/ssm/__init__.py
 localstack/aws/api/stepfunctions/__init__.py
 localstack/aws/api/sts/__init__.py
 localstack/aws/api/support/__init__.py
 localstack/aws/api/swf/__init__.py
 localstack/aws/api/transcribe/__init__.py
-localstack/aws/data/sqs-json/2012-11-05/README.md
-localstack/aws/data/sqs-json/2012-11-05/service-2.json
+localstack/aws/data/sqs-query/2012-11-05/README.md
+localstack/aws/data/sqs-query/2012-11-05/service-2.json
 localstack/aws/handlers/__init__.py
 localstack/aws/handlers/analytics.py
 localstack/aws/handlers/auth.py
 localstack/aws/handlers/codec.py
 localstack/aws/handlers/cors.py
 localstack/aws/handlers/fallback.py
 localstack/aws/handlers/internal.py
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/entry_points.txt` & `localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/plux.json` & `localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/plux.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7978395061728395%*

 * *Differences: {"'localstack.cloudformation.resource_providers'": '{insert: [(0, '*

 * *                                                   "'AWS::ApiGateway::ApiKey=localstack.services.apigateway.resource_providers.aws_apigateway_apikey_plugin:ApiGatewayApiKeyProviderPlugin'), "*

 * *                                                   '(3, '*

 * *                                                   "'AWS::Redshift::Cluster=localstack.services.redshift.resource_providers.aws_redshift_cluster_plugin:RedshiftClusterProviderPlugin'), "*

 * *        […]*

```diff
@@ -47,154 +47,154 @@
         "stepfunctions:v2=localstack.services.providers:stepfunctions_v2",
         "sts:default=localstack.services.providers:sts",
         "support:default=localstack.services.providers:support",
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.cloudformation.resource_providers": [
-        "AWS::KinesisFirehose::DeliveryStream=localstack.services.kinesisfirehose.resource_providers.aws_kinesisfirehose_deliverystream_plugin:KinesisFirehoseDeliveryStreamProviderPlugin",
-        "AWS::ApiGateway::Deployment=localstack.services.apigateway.resource_providers.aws_apigateway_deployment_plugin:ApiGatewayDeploymentProviderPlugin",
-        "AWS::IAM::ManagedPolicy=localstack.services.iam.resource_providers.aws_iam_managedpolicy_plugin:IAMManagedPolicyProviderPlugin",
-        "AWS::ApiGateway::GatewayResponse=localstack.services.apigateway.resource_providers.aws_apigateway_gatewayresponse_plugin:ApiGatewayGatewayResponseProviderPlugin",
-        "AWS::ApiGateway::Resource=localstack.services.apigateway.resource_providers.aws_apigateway_resource_plugin:ApiGatewayResourceProviderPlugin",
-        "AWS::DynamoDB::Table=localstack.services.dynamodb.resource_providers.aws_dynamodb_table_plugin:DynamoDBTableProviderPlugin",
+        "AWS::ApiGateway::ApiKey=localstack.services.apigateway.resource_providers.aws_apigateway_apikey_plugin:ApiGatewayApiKeyProviderPlugin",
         "AWS::KMS::Key=localstack.services.kms.resource_providers.aws_kms_key_plugin:KMSKeyProviderPlugin",
-        "AWS::EC2::PrefixList=localstack.services.ec2.resource_providers.aws_ec2_prefixlist_plugin:EC2PrefixListProviderPlugin",
-        "AWS::IAM::ServerCertificate=localstack.services.iam.resource_providers.aws_iam_servercertificate_plugin:IAMServerCertificateProviderPlugin",
         "AWS::IAM::User=localstack.services.iam.resource_providers.aws_iam_user_plugin:IAMUserProviderPlugin",
-        "AWS::EC2::TransitGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_transitgatewayattachment_plugin:EC2TransitGatewayAttachmentProviderPlugin",
-        "AWS::EC2::NatGateway=localstack.services.ec2.resource_providers.aws_ec2_natgateway_plugin:EC2NatGatewayProviderPlugin",
-        "AWS::ApiGateway::DomainName=localstack.services.apigateway.resource_providers.aws_apigateway_domainname_plugin:ApiGatewayDomainNameProviderPlugin",
-        "AWS::Lambda::Alias=localstack.services.lambda_.resource_providers.lambda_alias_plugin:LambdaAliasProviderPlugin",
+        "AWS::Redshift::Cluster=localstack.services.redshift.resource_providers.aws_redshift_cluster_plugin:RedshiftClusterProviderPlugin",
+        "AWS::SNS::Subscription=localstack.services.sns.resource_providers.aws_sns_subscription_plugin:SNSSubscriptionProviderPlugin",
+        "AWS::ApiGateway::RequestValidator=localstack.services.apigateway.resource_providers.aws_apigateway_requestvalidator_plugin:ApiGatewayRequestValidatorProviderPlugin",
+        "AWS::ApiGateway::UsagePlanKey=localstack.services.apigateway.resource_providers.aws_apigateway_usageplankey_plugin:ApiGatewayUsagePlanKeyProviderPlugin",
+        "AWS::ApiGateway::UsagePlan=localstack.services.apigateway.resource_providers.aws_apigateway_usageplan_plugin:ApiGatewayUsagePlanProviderPlugin",
+        "AWS::S3::BucketPolicy=localstack.services.s3.resource_providers.aws_s3_bucketpolicy_plugin:S3BucketPolicyProviderPlugin",
         "AWS::EC2::NetworkAcl=localstack.services.ec2.resource_providers.aws_ec2_networkacl_plugin:EC2NetworkAclProviderPlugin",
-        "AWS::IAM::ServiceLinkedRole=localstack.services.iam.resource_providers.aws_iam_servicelinkedrole_plugin:IAMServiceLinkedRoleProviderPlugin",
-        "AWS::EC2::DHCPOptions=localstack.services.ec2.resource_providers.aws_ec2_dhcpoptions_plugin:EC2DHCPOptionsProviderPlugin",
+        "AWS::EC2::SecurityGroup=localstack.services.ec2.resource_providers.aws_ec2_securitygroup_plugin:EC2SecurityGroupProviderPlugin",
+        "AWS::Logs::LogGroup=localstack.services.logs.resource_providers.aws_logs_loggroup_plugin:LogsLogGroupProviderPlugin",
+        "AWS::EC2::PrefixList=localstack.services.ec2.resource_providers.aws_ec2_prefixlist_plugin:EC2PrefixListProviderPlugin",
+        "AWS::CDK::Metadata=localstack.services.cdk.resource_providers.cdk_metadata_plugin:LambdaAliasProviderPlugin",
+        "AWS::Lambda::EventInvokeConfig=localstack.services.lambda_.resource_providers.aws_lambda_eventinvokeconfig_plugin:LambdaEventInvokeConfigProviderPlugin",
+        "AWS::SecretsManager::ResourcePolicy=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_resourcepolicy_plugin:SecretsManagerResourcePolicyProviderPlugin",
+        "AWS::CloudFormation::Macro=localstack.services.cloudformation.resource_providers.aws_cloudformation_macro_plugin:CloudFormationMacroProviderPlugin",
+        "AWS::EC2::Instance=localstack.services.ec2.resource_providers.aws_ec2_instance_plugin:EC2InstanceProviderPlugin",
+        "AWS::Events::Connection=localstack.services.events.resource_providers.aws_events_connection_plugin:EventsConnectionProviderPlugin",
+        "AWS::IAM::Role=localstack.services.iam.resource_providers.aws_iam_role_plugin:IAMRoleProviderPlugin",
+        "AWS::Logs::LogStream=localstack.services.logs.resource_providers.aws_logs_logstream_plugin:LogsLogStreamProviderPlugin",
+        "AWS::SNS::Topic=localstack.services.sns.resource_providers.aws_sns_topic_plugin:SNSTopicProviderPlugin",
+        "AWS::SQS::QueuePolicy=localstack.services.sqs.resource_providers.aws_sqs_queuepolicy_plugin:SQSQueuePolicyProviderPlugin",
+        "AWS::Lambda::Permission=localstack.services.lambda_.resource_providers.aws_lambda_permission_plugin:LambdaPermissionProviderPlugin",
         "AWS::Elasticsearch::Domain=localstack.services.opensearch.resource_providers.aws_elasticsearch_domain_plugin:ElasticsearchDomainProviderPlugin",
-        "AWS::EC2::VPCGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_vpcgatewayattachment_plugin:EC2VPCGatewayAttachmentProviderPlugin",
-        "AWS::EC2::Subnet=localstack.services.ec2.resource_providers.aws_ec2_subnet_plugin:EC2SubnetProviderPlugin",
-        "AWS::Redshift::Cluster=localstack.services.redshift.resource_providers.aws_redshift_cluster_plugin:RedshiftClusterProviderPlugin",
         "AWS::SSM::PatchBaseline=localstack.services.ssm.resource_providers.aws_ssm_patchbaseline_plugin:SSMPatchBaselineProviderPlugin",
+        "AWS::IAM::ManagedPolicy=localstack.services.iam.resource_providers.aws_iam_managedpolicy_plugin:IAMManagedPolicyProviderPlugin",
+        "AWS::Events::EventBusPolicy=localstack.services.events.resource_providers.aws_events_eventbuspolicy_plugin:EventsEventBusPolicyProviderPlugin",
+        "AWS::SSM::MaintenanceWindowTask=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtask_plugin:SSMMaintenanceWindowTaskProviderPlugin",
         "AWS::SSM::MaintenanceWindow=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindow_plugin:SSMMaintenanceWindowProviderPlugin",
+        "AWS::EC2::DHCPOptions=localstack.services.ec2.resource_providers.aws_ec2_dhcpoptions_plugin:EC2DHCPOptionsProviderPlugin",
+        "AWS::CertificateManager::Certificate=localstack.services.certificatemanager.resource_providers.aws_certificatemanager_certificate_plugin:CertificateManagerCertificateProviderPlugin",
         "AWS::CloudWatch::CompositeAlarm=localstack.services.cloudwatch.resource_providers.aws_cloudwatch_compositealarm_plugin:CloudWatchCompositeAlarmProviderPlugin",
-        "AWS::SecretsManager::ResourcePolicy=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_resourcepolicy_plugin:SecretsManagerResourcePolicyProviderPlugin",
+        "AWS::IAM::ServerCertificate=localstack.services.iam.resource_providers.aws_iam_servercertificate_plugin:IAMServerCertificateProviderPlugin",
+        "AWS::ApiGateway::Stage=localstack.services.apigateway.resource_providers.aws_apigateway_stage_plugin:ApiGatewayStageProviderPlugin",
+        "AWS::ECR::Repository=localstack.services.ecr.resource_providers.aws_ecr_repository_plugin:ECRRepositoryProviderPlugin",
         "AWS::ResourceGroups::Group=localstack.services.resource_groups.resource_providers.aws_resourcegroups_group_plugin:ResourceGroupsGroupProviderPlugin",
-        "AWS::SNS::Subscription=localstack.services.sns.resource_providers.aws_sns_subscription_plugin:SNSSubscriptionProviderPlugin",
-        "AWS::SecretsManager::SecretTargetAttachment=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secrettargetattachment_plugin:SecretsManagerSecretTargetAttachmentProviderPlugin",
-        "AWS::SNS::TopicPolicy=localstack.services.sns.resource_providers.aws_sns_topicpolicy_plugin:SNSTopicPolicyProviderPlugin",
-        "AWS::Kinesis::StreamConsumer=localstack.services.kinesis.resource_providers.aws_kinesis_streamconsumer_plugin:KinesisStreamConsumerProviderPlugin",
-        "AWS::CloudFormation::Stack=localstack.services.cloudformation.resource_providers.aws_cloudformation_stack_plugin:CloudFormationStackProviderPlugin",
         "AWS::StepFunctions::Activity=localstack.services.stepfunctions.resource_providers.aws_stepfunctions_activity_plugin:StepFunctionsActivityProviderPlugin",
-        "AWS::Logs::LogGroup=localstack.services.logs.resource_providers.aws_logs_loggroup_plugin:LogsLogGroupProviderPlugin",
-        "AWS::CloudFormation::WaitConditionHandle=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitconditionhandle_plugin:CloudFormationWaitConditionHandleProviderPlugin",
-        "AWS::ApiGateway::Account=localstack.services.apigateway.resource_providers.aws_apigateway_account_plugin:ApiGatewayAccountProviderPlugin",
-        "AWS::ECR::Repository=localstack.services.ecr.resource_providers.aws_ecr_repository_plugin:ECRRepositoryProviderPlugin",
-        "AWS::SNS::Topic=localstack.services.sns.resource_providers.aws_sns_topic_plugin:SNSTopicProviderPlugin",
-        "AWS::Lambda::Url=localstack.services.lambda_.resource_providers.aws_lambda_url_plugin:LambdaUrlProviderPlugin",
-        "AWS::Route53::RecordSet=localstack.services.route53.resource_providers.aws_route53_recordset_plugin:Route53RecordSetProviderPlugin",
-        "AWS::EC2::VPCEndpoint=localstack.services.ec2.resource_providers.aws_ec2_vpcendpoint_plugin:EC2VPCEndpointProviderPlugin",
-        "AWS::ApiGateway::UsagePlan=localstack.services.apigateway.resource_providers.aws_apigateway_usageplan_plugin:ApiGatewayUsagePlanProviderPlugin",
-        "AWS::SecretsManager::RotationSchedule=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_rotationschedule_plugin:SecretsManagerRotationScheduleProviderPlugin",
-        "AWS::ApiGateway::BasePathMapping=localstack.services.apigateway.resource_providers.aws_apigateway_basepathmapping_plugin:ApiGatewayBasePathMappingProviderPlugin",
-        "AWS::ApiGateway::Stage=localstack.services.apigateway.resource_providers.aws_apigateway_stage_plugin:ApiGatewayStageProviderPlugin",
+        "AWS::Events::Rule=localstack.services.events.resource_providers.aws_events_rule_plugin:EventsRuleProviderPlugin",
+        "AWS::Scheduler::Schedule=localstack.services.scheduler.resource_providers.aws_scheduler_schedule_plugin:SchedulerScheduleProviderPlugin",
         "AWS::SecretsManager::Secret=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secret_plugin:SecretsManagerSecretProviderPlugin",
+        "AWS::EC2::KeyPair=localstack.services.ec2.resource_providers.aws_ec2_keypair_plugin:EC2KeyPairProviderPlugin",
+        "AWS::Lambda::CodeSigningConfig=localstack.services.lambda_.resource_providers.aws_lambda_codesigningconfig_plugin:LambdaCodeSigningConfigProviderPlugin",
+        "AWS::Logs::SubscriptionFilter=localstack.services.logs.resource_providers.aws_logs_subscriptionfilter_plugin:LogsSubscriptionFilterProviderPlugin",
+        "AWS::SNS::TopicPolicy=localstack.services.sns.resource_providers.aws_sns_topicpolicy_plugin:SNSTopicPolicyProviderPlugin",
+        "AWS::DynamoDB::GlobalTable=localstack.services.dynamodb.resource_providers.aws_dynamodb_globaltable_plugin:DynamoDBGlobalTableProviderPlugin",
+        "AWS::ApiGateway::Resource=localstack.services.apigateway.resource_providers.aws_apigateway_resource_plugin:ApiGatewayResourceProviderPlugin",
         "AWS::IAM::AccessKey=localstack.services.iam.resource_providers.aws_iam_accesskey_plugin:IAMAccessKeyProviderPlugin",
+        "AWS::Lambda::LayerVersion=localstack.services.lambda_.resource_providers.aws_lambda_layerversion_plugin:LambdaLayerVersionProviderPlugin",
+        "AWS::Lambda::LayerVersionPermission=localstack.services.lambda_.resource_providers.aws_lambda_layerversionpermission_plugin:LambdaLayerVersionPermissionProviderPlugin",
         "AWS::EC2::VPC=localstack.services.ec2.resource_providers.aws_ec2_vpc_plugin:EC2VPCProviderPlugin",
-        "AWS::ApiGateway::Model=localstack.services.apigateway.resource_providers.aws_apigateway_model_plugin:ApiGatewayModelProviderPlugin",
+        "AWS::ApiGateway::BasePathMapping=localstack.services.apigateway.resource_providers.aws_apigateway_basepathmapping_plugin:ApiGatewayBasePathMappingProviderPlugin",
+        "AWS::Lambda::Version=localstack.services.lambda_.resource_providers.aws_lambda_version_plugin:LambdaVersionProviderPlugin",
+        "AWS::EC2::NatGateway=localstack.services.ec2.resource_providers.aws_ec2_natgateway_plugin:EC2NatGatewayProviderPlugin",
+        "AWS::EC2::VPCGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_vpcgatewayattachment_plugin:EC2VPCGatewayAttachmentProviderPlugin",
+        "AWS::ApiGateway::Account=localstack.services.apigateway.resource_providers.aws_apigateway_account_plugin:ApiGatewayAccountProviderPlugin",
+        "AWS::Lambda::Function=localstack.services.lambda_.resource_providers.aws_lambda_function_plugin:LambdaFunctionProviderPlugin",
         "AWS::IAM::InstanceProfile=localstack.services.iam.resource_providers.aws_iam_instanceprofile_plugin:IAMInstanceProfileProviderPlugin",
-        "AWS::Lambda::CodeSigningConfig=localstack.services.lambda_.resource_providers.aws_lambda_codesigningconfig_plugin:LambdaCodeSigningConfigProviderPlugin",
-        "AWS::CloudWatch::Alarm=localstack.services.cloudwatch.resource_providers.aws_cloudwatch_alarm_plugin:CloudWatchAlarmProviderPlugin",
-        "AWS::Events::Connection=localstack.services.events.resource_providers.aws_events_connection_plugin:EventsConnectionProviderPlugin",
-        "AWS::CloudFormation::Macro=localstack.services.cloudformation.resource_providers.aws_cloudformation_macro_plugin:CloudFormationMacroProviderPlugin",
-        "AWS::EC2::SecurityGroup=localstack.services.ec2.resource_providers.aws_ec2_securitygroup_plugin:EC2SecurityGroupProviderPlugin",
+        "AWS::Events::ApiDestination=localstack.services.events.resource_providers.aws_events_apidestination_plugin:EventsApiDestinationProviderPlugin",
+        "AWS::IAM::Group=localstack.services.iam.resource_providers.aws_iam_group_plugin:IAMGroupProviderPlugin",
+        "AWS::EC2::Subnet=localstack.services.ec2.resource_providers.aws_ec2_subnet_plugin:EC2SubnetProviderPlugin",
+        "AWS::ApiGateway::Deployment=localstack.services.apigateway.resource_providers.aws_apigateway_deployment_plugin:ApiGatewayDeploymentProviderPlugin",
         "AWS::Kinesis::Stream=localstack.services.kinesis.resource_providers.aws_kinesis_stream_plugin:KinesisStreamProviderPlugin",
-        "AWS::Lambda::EventSourceMapping=localstack.services.lambda_.resource_providers.aws_lambda_eventsourcemapping_plugin:LambdaEventSourceMappingProviderPlugin",
-        "AWS::Lambda::Function=localstack.services.lambda_.resource_providers.aws_lambda_function_plugin:LambdaFunctionProviderPlugin",
-        "AWS::SSM::MaintenanceWindowTask=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtask_plugin:SSMMaintenanceWindowTaskProviderPlugin",
+        "AWS::Scheduler::ScheduleGroup=localstack.services.scheduler.resource_providers.aws_scheduler_schedulegroup_plugin:SchedulerScheduleGroupProviderPlugin",
         "AWS::CloudFormation::WaitCondition=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitcondition_plugin:CloudFormationWaitConditionProviderPlugin",
-        "AWS::Events::EventBusPolicy=localstack.services.events.resource_providers.aws_events_eventbuspolicy_plugin:EventsEventBusPolicyProviderPlugin",
-        "AWS::EC2::TransitGateway=localstack.services.ec2.resource_providers.aws_ec2_transitgateway_plugin:EC2TransitGatewayProviderPlugin",
-        "AWS::Events::ApiDestination=localstack.services.events.resource_providers.aws_events_apidestination_plugin:EventsApiDestinationProviderPlugin",
-        "AWS::CertificateManager::Certificate=localstack.services.certificatemanager.resource_providers.aws_certificatemanager_certificate_plugin:CertificateManagerCertificateProviderPlugin",
-        "AWS::ApiGateway::RequestValidator=localstack.services.apigateway.resource_providers.aws_apigateway_requestvalidator_plugin:ApiGatewayRequestValidatorProviderPlugin",
+        "AWS::Lambda::EventSourceMapping=localstack.services.lambda_.resource_providers.aws_lambda_eventsourcemapping_plugin:LambdaEventSourceMappingProviderPlugin",
+        "AWS::Route53::HealthCheck=localstack.services.route53.resource_providers.aws_route53_healthcheck_plugin:Route53HealthCheckProviderPlugin",
+        "AWS::ApiGateway::Model=localstack.services.apigateway.resource_providers.aws_apigateway_model_plugin:ApiGatewayModelProviderPlugin",
+        "AWS::Lambda::Url=localstack.services.lambda_.resource_providers.aws_lambda_url_plugin:LambdaUrlProviderPlugin",
+        "AWS::EC2::InternetGateway=localstack.services.ec2.resource_providers.aws_ec2_internetgateway_plugin:EC2InternetGatewayProviderPlugin",
+        "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter_plugin:SSMParameterProviderPlugin",
         "AWS::KMS::Alias=localstack.services.kms.resource_providers.aws_kms_alias_plugin:KMSAliasProviderPlugin",
-        "AWS::ApiGateway::UsagePlanKey=localstack.services.apigateway.resource_providers.aws_apigateway_usageplankey_plugin:ApiGatewayUsagePlanKeyProviderPlugin",
-        "AWS::ApiGateway::Method=localstack.services.apigateway.resource_providers.aws_apigateway_method_plugin:ApiGatewayMethodProviderPlugin",
-        "AWS::S3::BucketPolicy=localstack.services.s3.resource_providers.aws_s3_bucketpolicy_plugin:S3BucketPolicyProviderPlugin",
-        "AWS::Logs::LogStream=localstack.services.logs.resource_providers.aws_logs_logstream_plugin:LogsLogStreamProviderPlugin",
-        "AWS::EC2::Route=localstack.services.ec2.resource_providers.aws_ec2_route_plugin:EC2RouteProviderPlugin",
-        "AWS::EC2::SubnetRouteTableAssociation=localstack.services.ec2.resource_providers.aws_ec2_subnetroutetableassociation_plugin:EC2SubnetRouteTableAssociationProviderPlugin",
+        "AWS::ApiGateway::RestApi=localstack.services.apigateway.resource_providers.aws_apigateway_restapi_plugin:ApiGatewayRestApiProviderPlugin",
+        "AWS::SecretsManager::SecretTargetAttachment=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_secrettargetattachment_plugin:SecretsManagerSecretTargetAttachmentProviderPlugin",
+        "AWS::Route53::RecordSet=localstack.services.route53.resource_providers.aws_route53_recordset_plugin:Route53RecordSetProviderPlugin",
         "AWS::S3::Bucket=localstack.services.s3.resource_providers.aws_s3_bucket_plugin:S3BucketProviderPlugin",
-        "AWS::Events::EventBus=localstack.services.events.resource_providers.aws_events_eventbus_plugin:EventsEventBusProviderPlugin",
-        "AWS::ApiGateway::ApiKey=localstack.services.apigateway.resource_providers.aws_apigateway_apikey_plugin:ApiGatewayApiKeyProviderPlugin",
-        "AWS::Logs::SubscriptionFilter=localstack.services.logs.resource_providers.aws_logs_subscriptionfilter_plugin:LogsSubscriptionFilterProviderPlugin",
+        "AWS::SSM::MaintenanceWindowTarget=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtarget_plugin:SSMMaintenanceWindowTargetProviderPlugin",
+        "AWS::CloudFormation::Stack=localstack.services.cloudformation.resource_providers.aws_cloudformation_stack_plugin:CloudFormationStackProviderPlugin",
         "AWS::StepFunctions::StateMachine=localstack.services.stepfunctions.resource_providers.aws_stepfunctions_statemachine_plugin:StepFunctionsStateMachineProviderPlugin",
-        "AWS::OpenSearchService::Domain=localstack.services.opensearch.resource_providers.aws_opensearchservice_domain_plugin:OpenSearchServiceDomainProviderPlugin",
-        "AWS::EC2::Instance=localstack.services.ec2.resource_providers.aws_ec2_instance_plugin:EC2InstanceProviderPlugin",
-        "AWS::ApiGateway::RestApi=localstack.services.apigateway.resource_providers.aws_apigateway_restapi_plugin:ApiGatewayRestApiProviderPlugin",
-        "AWS::Events::Rule=localstack.services.events.resource_providers.aws_events_rule_plugin:EventsRuleProviderPlugin",
-        "AWS::Route53::HealthCheck=localstack.services.route53.resource_providers.aws_route53_healthcheck_plugin:Route53HealthCheckProviderPlugin",
-        "AWS::Lambda::Permission=localstack.services.lambda_.resource_providers.aws_lambda_permission_plugin:LambdaPermissionProviderPlugin",
-        "AWS::IAM::Policy=localstack.services.iam.resource_providers.aws_iam_policy_plugin:IAMPolicyProviderPlugin",
-        "AWS::EC2::KeyPair=localstack.services.ec2.resource_providers.aws_ec2_keypair_plugin:EC2KeyPairProviderPlugin",
-        "AWS::CDK::Metadata=localstack.services.cdk.resource_providers.cdk_metadata_plugin:LambdaAliasProviderPlugin",
-        "AWS::Lambda::EventInvokeConfig=localstack.services.lambda_.resource_providers.aws_lambda_eventinvokeconfig_plugin:LambdaEventInvokeConfigProviderPlugin",
-        "AWS::IAM::Group=localstack.services.iam.resource_providers.aws_iam_group_plugin:IAMGroupProviderPlugin",
-        "AWS::DynamoDB::GlobalTable=localstack.services.dynamodb.resource_providers.aws_dynamodb_globaltable_plugin:DynamoDBGlobalTableProviderPlugin",
-        "AWS::IAM::Role=localstack.services.iam.resource_providers.aws_iam_role_plugin:IAMRoleProviderPlugin",
-        "AWS::EC2::InternetGateway=localstack.services.ec2.resource_providers.aws_ec2_internetgateway_plugin:EC2InternetGatewayProviderPlugin",
         "AWS::SQS::Queue=localstack.services.sqs.resource_providers.aws_sqs_queue_plugin:SQSQueueProviderPlugin",
-        "AWS::Scheduler::ScheduleGroup=localstack.services.scheduler.resource_providers.aws_scheduler_schedulegroup_plugin:SchedulerScheduleGroupProviderPlugin",
-        "AWS::Lambda::LayerVersion=localstack.services.lambda_.resource_providers.aws_lambda_layerversion_plugin:LambdaLayerVersionProviderPlugin",
-        "AWS::SSM::Parameter=localstack.services.ssm.resource_providers.aws_ssm_parameter_plugin:SSMParameterProviderPlugin",
-        "AWS::Scheduler::Schedule=localstack.services.scheduler.resource_providers.aws_scheduler_schedule_plugin:SchedulerScheduleProviderPlugin",
+        "AWS::CloudFormation::WaitConditionHandle=localstack.services.cloudformation.resource_providers.aws_cloudformation_waitconditionhandle_plugin:CloudFormationWaitConditionHandleProviderPlugin",
+        "AWS::OpenSearchService::Domain=localstack.services.opensearch.resource_providers.aws_opensearchservice_domain_plugin:OpenSearchServiceDomainProviderPlugin",
+        "AWS::EC2::TransitGateway=localstack.services.ec2.resource_providers.aws_ec2_transitgateway_plugin:EC2TransitGatewayProviderPlugin",
+        "AWS::KinesisFirehose::DeliveryStream=localstack.services.kinesisfirehose.resource_providers.aws_kinesisfirehose_deliverystream_plugin:KinesisFirehoseDeliveryStreamProviderPlugin",
+        "AWS::ApiGateway::GatewayResponse=localstack.services.apigateway.resource_providers.aws_apigateway_gatewayresponse_plugin:ApiGatewayGatewayResponseProviderPlugin",
         "AWS::EC2::RouteTable=localstack.services.ec2.resource_providers.aws_ec2_routetable_plugin:EC2RouteTableProviderPlugin",
-        "AWS::SQS::QueuePolicy=localstack.services.sqs.resource_providers.aws_sqs_queuepolicy_plugin:SQSQueuePolicyProviderPlugin",
-        "AWS::SSM::MaintenanceWindowTarget=localstack.services.ssm.resource_providers.aws_ssm_maintenancewindowtarget_plugin:SSMMaintenanceWindowTargetProviderPlugin",
-        "AWS::Lambda::Version=localstack.services.lambda_.resource_providers.aws_lambda_version_plugin:LambdaVersionProviderPlugin",
-        "AWS::Lambda::LayerVersionPermission=localstack.services.lambda_.resource_providers.aws_lambda_layerversionpermission_plugin:LambdaLayerVersionPermissionProviderPlugin"
+        "AWS::Lambda::Alias=localstack.services.lambda_.resource_providers.lambda_alias_plugin:LambdaAliasProviderPlugin",
+        "AWS::EC2::TransitGatewayAttachment=localstack.services.ec2.resource_providers.aws_ec2_transitgatewayattachment_plugin:EC2TransitGatewayAttachmentProviderPlugin",
+        "AWS::EC2::VPCEndpoint=localstack.services.ec2.resource_providers.aws_ec2_vpcendpoint_plugin:EC2VPCEndpointProviderPlugin",
+        "AWS::IAM::Policy=localstack.services.iam.resource_providers.aws_iam_policy_plugin:IAMPolicyProviderPlugin",
+        "AWS::EC2::Route=localstack.services.ec2.resource_providers.aws_ec2_route_plugin:EC2RouteProviderPlugin",
+        "AWS::ApiGateway::DomainName=localstack.services.apigateway.resource_providers.aws_apigateway_domainname_plugin:ApiGatewayDomainNameProviderPlugin",
+        "AWS::EC2::SubnetRouteTableAssociation=localstack.services.ec2.resource_providers.aws_ec2_subnetroutetableassociation_plugin:EC2SubnetRouteTableAssociationProviderPlugin",
+        "AWS::Events::EventBus=localstack.services.events.resource_providers.aws_events_eventbus_plugin:EventsEventBusProviderPlugin",
+        "AWS::SecretsManager::RotationSchedule=localstack.services.secretsmanager.resource_providers.aws_secretsmanager_rotationschedule_plugin:SecretsManagerRotationScheduleProviderPlugin",
+        "AWS::CloudWatch::Alarm=localstack.services.cloudwatch.resource_providers.aws_cloudwatch_alarm_plugin:CloudWatchAlarmProviderPlugin",
+        "AWS::DynamoDB::Table=localstack.services.dynamodb.resource_providers.aws_dynamodb_table_plugin:DynamoDBTableProviderPlugin",
+        "AWS::IAM::ServiceLinkedRole=localstack.services.iam.resource_providers.aws_iam_servicelinkedrole_plugin:IAMServiceLinkedRoleProviderPlugin",
+        "AWS::Kinesis::StreamConsumer=localstack.services.kinesis.resource_providers.aws_kinesis_streamconsumer_plugin:KinesisStreamConsumerProviderPlugin",
+        "AWS::ApiGateway::Method=localstack.services.apigateway.resource_providers.aws_apigateway_method_plugin:ApiGatewayMethodProviderPlugin"
     ],
     "localstack.hooks.configure_localstack_container": [
         "_mount_machine_file=localstack.utils.analytics.metadata:_mount_machine_file"
     ],
     "localstack.hooks.on_infra_ready": [
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
-        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
-        "remove_custom_endpoints=localstack.services.lambda_.plugins:remove_custom_endpoints",
-        "stop_server=localstack.dns.plugins:stop_server",
         "run_on_after_service_shutdown_handlers=localstack.runtime.shutdown:run_on_after_service_shutdown_handlers",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
-        "shutdown_services=localstack.runtime.shutdown:shutdown_services"
+        "shutdown_services=localstack.runtime.shutdown:shutdown_services",
+        "stop_server=localstack.dns.plugins:stop_server",
+        "remove_custom_endpoints=localstack.services.lambda_.plugins:remove_custom_endpoints",
+        "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "register_custom_endpoints=localstack.services.lambda_.plugins:register_custom_endpoints",
-        "validate_configuration=localstack.services.lambda_.plugins:validate_configuration",
+        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "setup_dns_configuration_on_host=localstack.dns.plugins:setup_dns_configuration_on_host",
         "start_dns_server=localstack.dns.plugins:start_dns_server",
-        "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
+        "register_custom_endpoints=localstack.services.lambda_.plugins:register_custom_endpoints",
+        "validate_configuration=localstack.services.lambda_.plugins:validate_configuration",
+        "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.lambda_.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
         "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "vosk/community=localstack.services.transcribe.plugins:vosk_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
         "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "vosk/community=localstack.services.transcribe.plugins:vosk_package",
         "lambda-java-libs/community=localstack.services.lambda_.plugins:lambda_java_libs",
         "lambda-runtime/community=localstack.services.lambda_.plugins:lambda_runtime_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package"
+        "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
+        "terraform/community=localstack.packages.plugins:terraform_package"
     ]
 }
```

### Comparing `localstack_core-3.4.1.dev20240502085340/localstack_core.egg-info/requires.txt` & `localstack_core-3.4.1.dev20240502123741/localstack_core.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 rich>=12.3.0
 requests>=2.20.0
 semver>=2.10
 stevedore>=3.4.0
 tailer>=0.4.1
 
 [base-runtime]
-boto3==1.34.84
-botocore==1.34.84
+boto3==1.34.93
+botocore==1.34.93
 awscrt>=0.13.14
 cbor2>=5.2.0
 dnspython>=1.16.0
 docker<7.0.0,>=6.1.1
 jsonpatch>=1.24
 hypercorn>=0.14.4
 localstack-twisted>=23.0
@@ -44,15 +44,15 @@
 pre-commit>=3.5.0
 pypandoc
 ruff>=0.3.3
 rstr>=3.2.0
 
 [runtime]
 localstack-core[base-runtime]
-awscli==1.32.84
+awscli==1.32.93
 airspeed-ext>=0.6.3
 amazon_kclpy!=2.1.0,!=2.1.4,>=2.0.6
 antlr4-python3-runtime==4.13.1
 apispec>=5.1.1
 aws-sam-translator>=1.15.1
 crontab>=0.22.6
 cryptography>=41.0.5
@@ -78,8 +78,8 @@
 pytest-tinybird>=0.2.0
 aws-cdk-lib>=2.88.0
 websocket-client>=1.7.0
 localstack-snapshot>=0.1.1
 
 [typehint]
 localstack-core[dev]
-boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.84
+boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.93
```

### Comparing `localstack_core-3.4.1.dev20240502085340/pyproject.toml` & `localstack_core-3.4.1.dev20240502123741/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 Repository = "https://github.com/localstack/localstack.git"
 Issues = "https://github.com/localstack/localstack/issues"
 
 [project.optional-dependencies]
 # minimal required to actually run localstack on the host for services natively implemented in python
 base-runtime = [
     # pinned / updated by ASF update action
-    "boto3==1.34.84",
+    "boto3==1.34.93",
     # pinned / updated by ASF update action
-    "botocore==1.34.84",
+    "botocore==1.34.93",
     "awscrt>=0.13.14",
     "cbor2>=5.2.0",
     "dnspython>=1.16.0",
     # TODO tag incompatibility introduced in 7.0.0 with https://github.com/docker/docker-py/pull/3191
     "docker>=6.1.1,<7.0.0",
     "jsonpatch>=1.24",
     "hypercorn>=0.14.4",
@@ -72,15 +72,15 @@
     "Quart>=0.19.2",
 ]
 
 # required to actually run localstack on the host
 runtime = [
     "localstack-core[base-runtime]",
     # pinned / updated by ASF update action
-    "awscli==1.32.84",
+    "awscli==1.32.93",
     "airspeed-ext>=0.6.3",
     "amazon_kclpy>=2.0.6,!=2.1.0,!=2.1.4",
     # antlr4-python3-runtime: exact pin because antlr4 runtime is tightly coupled to the generated parser code
     "antlr4-python3-runtime==4.13.1",
     "apispec>=5.1.1",
     "aws-sam-translator>=1.15.1",
     "crontab>=0.22.6",
@@ -129,15 +129,15 @@
 ]
 
 # not strictly necessary for development, but provides type hint support for a better developer experience
 typehint = [
     # typehint is an optional extension of the dev dependencies
     "localstack-core[dev]",
     # pinned / updated by ASF update action
-    "boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.84",
+    "boto3-stubs[acm,acm-pca,amplify,apigateway,apigatewayv2,appconfig,appconfigdata,application-autoscaling,appsync,athena,autoscaling,backup,batch,ce,cloudcontrol,cloudformation,cloudfront,cloudtrail,cloudwatch,codecommit,cognito-identity,cognito-idp,dms,docdb,dynamodb,dynamodbstreams,ec2,ecr,ecs,efs,eks,elasticache,elasticbeanstalk,elbv2,emr,emr-serverless,es,events,firehose,fis,glacier,glue,iam,identitystore,iot,iot-data,iotanalytics,iotwireless,kafka,kinesis,kinesisanalytics,kinesisanalyticsv2,kms,lakeformation,lambda,logs,managedblockchain,mediaconvert,mediastore,mq,mwaa,neptune,opensearch,organizations,pi,pipes,qldb,qldb-session,rds,rds-data,redshift,redshift-data,resource-groups,resourcegroupstaggingapi,route53,route53resolver,s3,s3control,sagemaker,sagemaker-runtime,secretsmanager,serverlessrepo,servicediscovery,ses,sesv2,sns,sqs,ssm,sso-admin,stepfunctions,sts,timestream-query,timestream-write,transcribe,wafv2,xray]==1.34.93",
 ]
 
 [tool.setuptools]
 include-package-data = false
 # TODO using this is discouraged by setuptools, `project.scripts` should be used instead
 # However, `project.scripts` does not support non-python scripts.
 script-files = [
```

### Comparing `localstack_core-3.4.1.dev20240502085340/setup.py` & `localstack_core-3.4.1.dev20240502123741/setup.py`

 * *Files identical despite different names*

