# Comparing `tmp/localstack-core-2.0.3.dev20230418071728.tar.gz` & `tmp/localstack-core-2.0.3.dev20230418093340.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.0.3.dev20230418071728.tar", last modified: Tue Apr 18 07:17:36 2023, max compression
+gzip compressed data, was "localstack-core-2.0.3.dev20230418093340.tar", last modified: Tue Apr 18 09:33:47 2023, max compression
```

## Comparing `localstack-core-2.0.3.dev20230418071728.tar` & `localstack-core-2.0.3.dev20230418093340.tar`

### file list

```diff
@@ -1,836 +1,836 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.885269 localstack-core-2.0.3.dev20230418071728/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-18 07:17:36.885269 localstack-core-2.0.3.dev20230418071728/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10815 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.801265 localstack-core-2.0.3.dev20230418071728/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-04-18 07:17:28.000000 localstack-core-2.0.3.dev20230418071728/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1890 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42769 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   123939 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6035 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.805266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   754452 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47848 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71864 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64389 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132500 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.809266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14068 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59496 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22571 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8786 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2075 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6856 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11919 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.813266 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14226 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49876 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73217 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2211 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27186 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18064 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    51049 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8214 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/contrib/thundra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11624 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14172 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5033 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17128 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.817266 localstack-core-2.0.3.dev20230418071728/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.821266 localstack-core-2.0.3.dev20230418071728/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.821266 localstack-core-2.0.3.dev20230418071728/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.821266 localstack-core-2.0.3.dev20230418071728/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.821266 localstack-core-2.0.3.dev20230418071728/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3767 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.821266 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34409 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.825266 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23585 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.825266 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8672 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.825266 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17805 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4897 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21171 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27232 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12394 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32703 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.825266 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1489 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   152767 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7722 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/urlrouter.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.825266 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1699 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6328 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.829266 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17143 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60765 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2288 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.829266 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30425 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20593 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4204 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5112 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22228 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2769 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8661 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28098 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3019 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5197 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1382 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10505 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6593 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2650 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5194 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34242 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6479 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.829266 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.829266 localstack-core-2.0.3.dev20230418071728/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73346 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6107 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4406 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21786 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32264 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19028 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15974 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11820 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.833267 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34733 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      797 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48525 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24137 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9437 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2651 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12621 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2979 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23108 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60971 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68236 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8940 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5393 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15447 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.837267 localstack-core-2.0.3.dev20230418071728/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28951 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21143 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5644 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45859 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54173 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24311 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    53186 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6936 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6879 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.841267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1292 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2367 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.845267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.849267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.849267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.849267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.849267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.849267 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.853268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.853268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.853268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.853268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.853268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.857268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.857268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.857268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.857268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3243 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5976 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      816 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.861268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4967 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3281 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3618 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1006 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2421 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1348 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.865268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.869268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.869268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4647 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.869268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.869268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31024 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6407 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2551 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10302 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      609 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12180 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6391 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.873268 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65214 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4559 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.877268 localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25709 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.881269 localstack-core-2.0.3.dev20230418071728/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.881269 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2985 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.881269 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13418 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12903 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11597 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23334 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.881269 localstack-core-2.0.3.dev20230418071728/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4407 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.881269 localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43017 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28581 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    29580 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4619 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.885269 localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.885269 localstack-core-2.0.3.dev20230418071728/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5640 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 07:17:36.885269 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-18 07:17:36.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36772 2023-04-18 07:17:36.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 07:17:36.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-04-18 07:17:36.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 07:17:32.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-04-18 07:17:32.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2777 2023-04-18 07:17:36.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-04-18 07:17:36.000000 localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3137 2023-04-18 07:17:36.885269 localstack-core-2.0.3.dev20230418071728/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-04-18 06:46:56.000000 localstack-core-2.0.3.dev20230418071728/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.228742 localstack-core-2.0.3.dev20230418093340/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-18 09:33:47.228742 localstack-core-2.0.3.dev20230418093340/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10815 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.140743 localstack-core-2.0.3.dev20230418093340/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.140743 localstack-core-2.0.3.dev20230418093340/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-04-18 09:33:40.000000 localstack-core-2.0.3.dev20230418093340/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1890 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42769 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   123939 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6035 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   754452 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47848 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71864 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    64389 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.144743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132500 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14068 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59496 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22571 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8786 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.148743 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2075 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6856 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11919 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14226 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49876 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73217 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27186 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18064 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    51049 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8320 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/contrib/thundra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11624 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2881 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15814 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5033 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17128 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.152743 localstack-core-2.0.3.dev20230418093340/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.156743 localstack-core-2.0.3.dev20230418093340/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.156743 localstack-core-2.0.3.dev20230418093340/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.156743 localstack-core-2.0.3.dev20230418093340/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.156743 localstack-core-2.0.3.dev20230418093340/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3767 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.156743 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34409 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.160743 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23585 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.160743 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8672 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.160743 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17805 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4897 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21171 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27232 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12394 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32703 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.160743 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1489 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   152767 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7722 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/urlrouter.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.160743 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1699 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6328 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.164743 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17143 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60765 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2288 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.164743 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30425 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20593 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4204 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1916 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5112 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22228 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2769 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8661 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28098 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3019 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5197 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1382 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10505 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6593 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2650 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5194 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34242 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6479 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2940 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.164743 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.164743 localstack-core-2.0.3.dev20230418093340/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.164743 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3949 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73346 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6107 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7804 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4406 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21786 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32264 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19028 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15974 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11820 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34733 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      797 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48525 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.168743 localstack-core-2.0.3.dev20230418093340/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24137 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9437 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2651 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12621 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2979 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23108 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60971 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68236 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8940 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5393 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15447 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27006 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.172742 localstack-core-2.0.3.dev20230418093340/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21143 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5609 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47737 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54173 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24311 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    53754 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6936 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1292 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2367 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.176742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2270 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1909 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      658 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.180743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.184743 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.188742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.188742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.188742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.188742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.188742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.188742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.192742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.192742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.192742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3243 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5976 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.196742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      816 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.200742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.200742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4967 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3281 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3618 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1161 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1006 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2421 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1348 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.204742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.208742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.208742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4647 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.208742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      250 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31024 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6407 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2551 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10302 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      609 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.212742 localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12180 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.216742 localstack-core-2.0.3.dev20230418093340/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.216742 localstack-core-2.0.3.dev20230418093340/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.216742 localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6391 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.216742 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65214 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4559 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.216742 localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25709 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.220742 localstack-core-2.0.3.dev20230418093340/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2985 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13418 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12903 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11597 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23334 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4407 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43017 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28581 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    29580 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6852 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4619 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5640 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 09:33:47.224742 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-04-18 09:33:47.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36772 2023-04-18 09:33:47.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 09:33:47.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-04-18 09:33:47.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 09:33:43.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-04-18 09:33:43.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2777 2023-04-18 09:33:47.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-04-18 09:33:47.000000 localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3137 2023-04-18 09:33:47.228742 localstack-core-2.0.3.dev20230418093340/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-04-18 09:00:44.000000 localstack-core-2.0.3.dev20230418093340/setup.py
```

### Comparing `localstack-core-2.0.3.dev20230418071728/LICENSE.txt` & `localstack-core-2.0.3.dev20230418093340/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/Makefile` & `localstack-core-2.0.3.dev20230418093340/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/PKG-INFO` & `localstack-core-2.0.3.dev20230418093340/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.0.3.dev20230418071728
+Version: 2.0.3.dev20230418093340
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.0.3.dev20230418071728/README.md` & `localstack-core-2.0.3.dev20230418093340/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/bin/localstack` & `localstack-core-2.0.3.dev20230418093340/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/bin/localstack-supervisor` & `localstack-core-2.0.3.dev20230418093340/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/accounts.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/acm/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/config/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/core.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/es/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/events/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/iam/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/kms/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/logs/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/route53/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/s3/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ses/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sns/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/sts/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/support/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/swf/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/app.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/chain.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/connect.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/forwarder.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/gateway.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/analytics.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/auth.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/codec.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/cors.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/fallback.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/internal.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/legacy.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/logging.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/proxy.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/region.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/routes.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/service.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/mocking.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/op_router.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/parser.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/serializer.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/service_router.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/protocol/validate.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/proxy.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/scaffold.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/asgi.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/asgi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+import asyncio
 import concurrent.futures.thread
 from asyncio import AbstractEventLoop
 from typing import Optional
 
 from localstack.aws.gateway import Gateway
 from localstack.aws.serving.wsgi import WsgiGateway
-from localstack.http.asgi import ASGIAdapter
+from localstack.http.asgi import ASGIAdapter, ASGILifespanListener
 
 
 class _ThreadPool(concurrent.futures.thread.ThreadPoolExecutor):
     """
     This thread pool executor removes the threads it creates from the global ``_thread_queues`` of
     ``concurrent.futures.thread``, which joins all created threads at python exit and will block interpreter shutdown of
     any threads are still running, even if they are daemon threads.
@@ -30,37 +31,44 @@
     """
     Exposes a Gateway as an ASGI3 application. Under the hood, it uses a WsgiGateway with a threading async/sync bridge.
     """
 
     gateway: Gateway
 
     def __init__(
-        self, gateway: Gateway, event_loop: Optional[AbstractEventLoop] = None, threads: int = 1000
+        self,
+        gateway: Gateway,
+        event_loop: Optional[AbstractEventLoop] = None,
+        threads: int = 1000,
+        lifespan_listener: Optional[ASGILifespanListener] = None,
     ) -> None:
         self.gateway = gateway
 
+        self.event_loop = event_loop or asyncio.get_event_loop()
         self.executor = _ThreadPool(threads, thread_name_prefix="asgi_gw")
-        self.wsgi = ASGIAdapter(WsgiGateway(gateway), event_loop=event_loop, executor=self.executor)
+        self.wsgi = ASGIAdapter(
+            WsgiGateway(gateway),
+            event_loop=event_loop,
+            executor=self.executor,
+            lifespan_listener=lifespan_listener,
+        )
         self._closed = False
 
     async def __call__(self, scope, receive, send) -> None:
         """
         ASGI3 application interface.
 
         :param scope: the ASGI request scope
         :param receive: the receive callable
         :param send: the send callable
         """
         if self._closed:
             raise RuntimeError("Cannot except new request on closed ASGIGateway")
 
-        if scope["type"] == "http":
-            return await self.wsgi(scope, receive, send)
-
-        raise NotImplementedError(f"{scope['type']} protocol is not implemented")
+        return await self.wsgi(scope, receive, send)
 
     def close(self):
         """
         Close the ASGIGateway by shutting down the underlying executor.
         """
         self._closed = True
         self.executor.shutdown(wait=False, cancel_futures=True)
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/edge.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/hypercorn.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/werkzeug.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/serving/wsgi.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/skeleton.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/spec-patches.json` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/spec.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/aws/trace.py` & `localstack-core-2.0.3.dev20230418093340/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/cli/localstack.py` & `localstack-core-2.0.3.dev20230418093340/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/cli/lpm.py` & `localstack-core-2.0.3.dev20230418093340/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/cli/plugin.py` & `localstack-core-2.0.3.dev20230418093340/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/cli/plugins.py` & `localstack-core-2.0.3.dev20230418093340/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/cli/profiles.py` & `localstack-core-2.0.3.dev20230418093340/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/config.py` & `localstack-core-2.0.3.dev20230418093340/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/constants.py` & `localstack-core-2.0.3.dev20230418093340/localstack/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,18 +165,22 @@
 
 # environment variable to override max pool connections
 try:
     MAX_POOL_CONNECTIONS = int(os.environ["MAX_POOL_CONNECTIONS"])
 except Exception:
     MAX_POOL_CONNECTIONS = 150
 
-# test credentials used for generating signature for S3 presigned URLs (to be used by external clients)
+# credentials used in the test suite
 TEST_AWS_ACCESS_KEY_ID = "test"
 TEST_AWS_SECRET_ACCESS_KEY = "test"
 
+# additional credentials used in the test suite (mainly for cross-account access)
+SECONDARY_TEST_AWS_ACCESS_KEY_ID = "test2"
+SECONDARY_TEST_AWS_SECRET_ACCESS_KEY = "test2"
+
 # credentials being used for internal calls
 INTERNAL_AWS_ACCESS_KEY_ID = "__internal_call__"
 INTERNAL_AWS_SECRET_ACCESS_KEY = "__internal_call__"
 
 # This header must be set to the AWS Account ID
 # Presence of this header in an incoming request typically means that the request originated within localstack,
 # i.e. it is an internal cross-service call.
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/contrib/thundra.py` & `localstack-core-2.0.3.dev20230418093340/localstack/contrib/thundra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/deprecations.py` & `localstack-core-2.0.3.dev20230418093340/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/aws.py` & `localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/extensions/api/extension.py` & `localstack-core-2.0.3.dev20230418093340/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/adapters.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/asgi.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/asgi.py`

 * *Files 14% similar despite different names*

```diff
@@ -305,14 +305,27 @@
             raise ValueError("not started the response yet")
 
         if not self.finalized:
             self.finalized = True
             await self.send({"type": "http.response.body", "body": b"", "more_body": False})
 
 
+class ASGILifespanListener:
+    """
+    Simple event handler that is attached to the ASGIAdapter and called on ASGI lifespan events. See
+    https://asgi.readthedocs.io/en/latest/specs/lifespan.html.
+    """
+
+    def on_startup(self):
+        pass
+
+    def on_shutdown(self):
+        pass
+
+
 class ASGIAdapter:
     """
     Adapter to expose a WSGIApplication as an ASGI3Application. This allows you to serve synchronous WSGI applications
     through ASGI servers (e.g., Hypercorn).
 
     IMPORTANT: The ASGIAdapter needs to use the same event loop as the underlying server. If you pass a new event
     loop to the server, you need to also pass it to the ASGIAdapter.
@@ -321,32 +334,37 @@
     """
 
     def __init__(
         self,
         wsgi_app: "WSGIApplication",
         event_loop: AbstractEventLoop = None,
         executor: Executor = None,
+        lifespan_listener: ASGILifespanListener = None,
     ):
         self.wsgi_app = wsgi_app
         self.event_loop = event_loop or asyncio.get_event_loop()
         self.executor = executor
+        self.lifespan_listener = lifespan_listener or ASGILifespanListener()
 
     async def __call__(
         self, scope: "Scope", receive: "ASGIReceiveCallable", send: "ASGISendCallable"
     ):
         """
         The ASGI 3 interface. Can only handle HTTP calls.
 
         :param scope: the connection scope
         :param receive: the receive callable
         :param send: the send callable
         """
         if scope["type"] == "http":
             return await self.handle_http(scope, receive, send)
 
+        if scope["type"] == "lifespan":
+            return await self.handle_lifespan(scope, receive, send)
+
         raise NotImplementedError("Unhandled protocol %s" % scope["type"])
 
     def to_wsgi_environment(
         self,
         scope: "HTTPScope",
         receive: "ASGIReceiveCallable",
     ) -> "WSGIEnvironment":
@@ -397,14 +415,40 @@
                         await response.write(packet)
                 else:
                     for packet in iterable:
                         await response.write(packet)
         finally:
             await response.close()
 
+    async def handle_lifespan(
+        self, scope: "HTTPScope", receive: "ASGIReceiveCallable", send: "ASGISendCallable"
+    ):
+        while True:
+            message = await receive()
+            if message["type"] == "lifespan.startup":
+                try:
+                    await self.event_loop.run_in_executor(
+                        self.executor, self.lifespan_listener.on_startup
+                    )
+                    await send({"type": "lifespan.startup.complete"})
+                except Exception as e:
+                    await send({"type": "lifespan.startup.failed", "message": f"{e}"})
+
+            elif message["type"] == "lifespan.shutdown":
+                try:
+                    await self.event_loop.run_in_executor(
+                        self.executor, self.lifespan_listener.on_shutdown
+                    )
+                    await send({"type": "lifespan.shutdown.complete"})
+                except Exception as e:
+                    await send({"type": "lifespan.shutdown.failed", "message": f"{e}"})
+                return
+            else:
+                return
+
 
 def patch_werkzeug():
     from werkzeug.wsgi import LimitedStream
 
     from localstack.utils.patch import patch
 
     @patch(LimitedStream.read, pass_target=False)
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/dispatcher.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/hypercorn.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/proxy.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/request.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/resource.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/response.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/http/router.py` & `localstack-core-2.0.3.dev20230418093340/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/logging/format.py` & `localstack-core-2.0.3.dev20230418093340/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/logging/setup.py` & `localstack-core-2.0.3.dev20230418093340/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/packages/__init__.py` & `localstack-core-2.0.3.dev20230418093340/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/packages/api.py` & `localstack-core-2.0.3.dev20230418093340/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/packages/core.py` & `localstack-core-2.0.3.dev20230418093340/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/packages/debugpy.py` & `localstack-core-2.0.3.dev20230418093340/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/packages/terraform.py` & `localstack-core-2.0.3.dev20230418093340/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/plugins.py` & `localstack-core-2.0.3.dev20230418093340/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/runtime/analytics.py` & `localstack-core-2.0.3.dev20230418093340/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/runtime/hooks.py` & `localstack-core-2.0.3.dev20230418093340/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/runtime/init.py` & `localstack-core-2.0.3.dev20230418093340/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/runtime/main.py` & `localstack-core-2.0.3.dev20230418093340/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/runtime/shutdown.py` & `localstack-core-2.0.3.dev20230418093340/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/acm/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/context.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/helpers.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/integration.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/invocations.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/patches.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/router_asf.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/apigateway/templates.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/api_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/hooks.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/plugins.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/events.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/service_models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudformation/stores.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/cloudwatch/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/server.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodb/utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/exceptions.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/ec2/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/edge.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/es/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/events/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/events/scheduler.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/mappers.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/firehose/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/generic_proxy.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/iam/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/infra.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/internal.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kinesis/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kms/local_kms_server.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kms/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kms/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/kms/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/logs/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/logs/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/messages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/moto.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/motoserver.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/cluster.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/opensearch/versions.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/plugins.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/providers.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/redshift/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/route53/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/route53resolver/utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/constants.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/cors.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/multipart_content.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/notifications.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/presigned_url.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/s3_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/s3_starter.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/s3_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/virtual_host.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/s3/website_hosting.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/secretsmanager/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/secretsmanager/provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from moto.awslambda.models import LambdaFunction
 from moto.iam.policy_validation import IAMPolicyDocumentValidator
 from moto.secretsmanager import utils as secretsmanager_utils
 from moto.secretsmanager.exceptions import SecretNotFoundException as MotoSecretNotFoundException
 from moto.secretsmanager.models import FakeSecret, SecretsManagerBackend
 from moto.secretsmanager.responses import SecretsManagerResponse
 
-from localstack.aws.api import CommonServiceException, RequestContext, ServiceResponse, handler
+from localstack.aws.api import CommonServiceException, RequestContext, handler
 from localstack.aws.api.secretsmanager import (
     CancelRotateSecretRequest,
     CancelRotateSecretResponse,
     CreateSecretRequest,
     CreateSecretResponse,
     DeleteResourcePolicyRequest,
     DeleteResourcePolicyResponse,
@@ -58,15 +58,15 @@
     UpdateSecretRequest,
     UpdateSecretResponse,
     UpdateSecretVersionStageRequest,
     UpdateSecretVersionStageResponse,
     ValidateResourcePolicyRequest,
     ValidateResourcePolicyResponse,
 )
-from localstack.services.moto import call_moto, call_moto_with_request
+from localstack.services.moto import call_moto
 from localstack.utils.aws import arns, aws_stack
 from localstack.utils.patch import patch
 from localstack.utils.strings import short_uid
 from localstack.utils.time import today_no_time
 
 # Constants.
 AWSPREVIOUS: Final[str] = "AWSPREVIOUS"
@@ -101,32 +101,14 @@
 
 class SecretsmanagerProvider(SecretsmanagerApi):
     def __init__(self):
         super().__init__()
         apply_patches()
 
     @staticmethod
-    def _transform_context_secret_id(secret_id: SecretIdType) -> Optional[SecretIdType]:
-        # If secret ARN ends with "-<randomId>" this is removed from the request for upstream compatibility.
-        t_secret_id = secret_id
-        if secret_id and re.match(r"^arn:", secret_id):
-            arn = arns.parse_arn(secret_id)
-            aws_region = aws_stack.get_region()
-            if arn["region"] != aws_region:
-                LOG.info(f'Expected request region "{aws_region}" for secret "{secret_id}"')
-            resource_id = arn["resource"].split(":")[-1]
-            if resource_id[-7] == "-":
-                t_secret_id = resource_id[:-7]
-            elif resource_id[-1] != "-":
-                t_secret_id += "-"
-            elif resource_id[-1] == "-":
-                t_secret_id = resource_id
-        return None if secret_id == t_secret_id else t_secret_id
-
-    @staticmethod
     def _validate_secret_id(secret_id: SecretIdType) -> bool:
         # The secret name can contain ASCII letters, numbers, and the following characters: /_+=.@-
         return bool(re.match(r"^[A-Za-z0-9/_+=.@-]+\Z", secret_id))
 
     @staticmethod
     def _raise_if_invalid_secret_id(secret_id: Union[SecretIdType, NameType]):
         # Patches moto's implementation for which secret_ids are not validated, by raising a ValidationException.
@@ -136,165 +118,152 @@
         ):  # Check if it appears to be an arn: so to skip secret_id check: delegate parsing of arn to handlers.
             if not SecretsmanagerProvider._validate_secret_id(secret_id):
                 raise ValidationException(
                     "Invalid name. Must be a valid name containing alphanumeric "
                     "characters, or any of the following: -/_+=.@!"
                 )
 
-    @staticmethod
-    def _call_moto_with_request_secret_id(
-        context: RequestContext, request: dict
-    ) -> ServiceResponse:
-        t_secret_id = SecretsmanagerProvider._transform_context_secret_id(
-            request.get("SecretId", None)
-        )
-        if t_secret_id:
-            request.update({"SecretId": t_secret_id})
-            return call_moto_with_request(context, request)
-        return call_moto(context)
-
     @handler("CancelRotateSecret", expand=False)
     def cancel_rotate_secret(
         self, context: RequestContext, request: CancelRotateSecretRequest
     ) -> CancelRotateSecretResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("CreateSecret", expand=False)
     def create_secret(
         self, context: RequestContext, request: CreateSecretRequest
     ) -> CreateSecretResponse:
         self._raise_if_invalid_secret_id(request["Name"])
         return call_moto(context)
 
     @handler("DeleteResourcePolicy", expand=False)
     def delete_resource_policy(
         self, context: RequestContext, request: DeleteResourcePolicyRequest
     ) -> DeleteResourcePolicyResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("DeleteSecret", expand=False)
     def delete_secret(
         self, context: RequestContext, request: DeleteSecretRequest
     ) -> DeleteSecretResponse:
         secret_id: str = request["SecretId"]
         self._raise_if_invalid_secret_id(secret_id)
-        res = self._call_moto_with_request_secret_id(context, request)
+        res = call_moto(context, request)
         delete_arn_binding_for(context.region, secret_id)
         return res
 
     @handler("DescribeSecret", expand=False)
     def describe_secret(
         self, context: RequestContext, request: DescribeSecretRequest
     ) -> DescribeSecretResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        res = self._call_moto_with_request_secret_id(context, request)
-        return res
+        return call_moto(context, request)
 
     @handler("GetResourcePolicy", expand=False)
     def get_resource_policy(
         self, context: RequestContext, request: GetResourcePolicyRequest
     ) -> GetResourcePolicyResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("GetSecretValue", expand=False)
     def get_secret_value(
         self, context: RequestContext, request: GetSecretValueRequest
     ) -> GetSecretValueResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("ListSecretVersionIds", expand=False)
     def list_secret_version_ids(
         self, context: RequestContext, request: ListSecretVersionIdsRequest
     ) -> ListSecretVersionIdsResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("PutResourcePolicy", expand=False)
     def put_resource_policy(
         self, context: RequestContext, request: PutResourcePolicyRequest
     ) -> PutResourcePolicyResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("PutSecretValue", expand=False)
     def put_secret_value(
         self, context: RequestContext, request: PutSecretValueRequest
     ) -> PutSecretValueResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("RemoveRegionsFromReplication", expand=False)
     def remove_regions_from_replication(
         self, context: RequestContext, request: RemoveRegionsFromReplicationRequest
     ) -> RemoveRegionsFromReplicationResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("ReplicateSecretToRegions", expand=False)
     def replicate_secret_to_regions(
         self, context: RequestContext, request: ReplicateSecretToRegionsRequest
     ) -> ReplicateSecretToRegionsResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("RestoreSecret", expand=False)
     def restore_secret(
         self, context: RequestContext, request: RestoreSecretRequest
     ) -> RestoreSecretResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("RotateSecret", expand=False)
     def rotate_secret(
         self, context: RequestContext, request: RotateSecretRequest
     ) -> RotateSecretResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("StopReplicationToReplica", expand=False)
     def stop_replication_to_replica(
         self, context: RequestContext, request: StopReplicationToReplicaRequest
     ) -> StopReplicationToReplicaResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("TagResource", expand=False)
     def tag_resource(self, context: RequestContext, request: TagResourceRequest) -> None:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("UntagResource", expand=False)
     def untag_resource(self, context: RequestContext, request: UntagResourceRequest) -> None:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("UpdateSecret", expand=False)
     def update_secret(
         self, context: RequestContext, request: UpdateSecretRequest
     ) -> UpdateSecretResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("UpdateSecretVersionStage", expand=False)
     def update_secret_version_stage(
         self, context: RequestContext, request: UpdateSecretVersionStageRequest
     ) -> UpdateSecretVersionStageResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
     @handler("ValidateResourcePolicy", expand=False)
     def validate_resource_policy(
         self, context: RequestContext, request: ValidateResourcePolicyRequest
     ) -> ValidateResourcePolicyResponse:
         self._raise_if_invalid_secret_id(request["SecretId"])
-        return self._call_moto_with_request_secret_id(context, request)
+        return call_moto(context, request)
 
 
 @patch(FakeSecret.__init__)
 def fake_secret__init__(fn, self, *args, **kwargs):
     fn(self, *args, **kwargs)
 
     # Fix time not including millis.
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/ses/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sns/constants.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sns/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sns/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,16 +110,16 @@
 
 class SnsStore(BaseStore):
     # maps topic ARN to subscriptions ARN
     topic_subscriptions: Dict[str, List[str]] = LocalAttribute(default=dict)
     # maps subscription ARN to SnsSubscription
     subscriptions: Dict[str, SnsSubscription] = LocalAttribute(default=dict)
 
-    # maps topic Arn to subscription validation token to subscription ARN
-    subscription_tokens: Dict[str, Dict[str, str]] = LocalAttribute(default=dict)
+    # maps confirmation token to subscription ARN
+    subscription_tokens: Dict[str, str] = LocalAttribute(default=dict)
 
     # maps topic ARN to list of tags
     sns_tags: Dict[str, List[Dict]] = LocalAttribute(default=dict)
 
     # cache of topic ARN to platform endpoint messages (used primarily for testing)
     platform_endpoint_messages: Dict[str, List[Dict]] = LocalAttribute(default=dict)
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sns/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sns/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -400,22 +400,41 @@
         self,
         context: RequestContext,
         topic_arn: topicARN,
         token: String,
         authenticate_on_unsubscribe: authenticateOnUnsubscribe = None,
     ) -> ConfirmSubscriptionResponse:
         # TODO: validate format on the token (seems to be 288 hex chars)
-        store = self.get_store(account_id=context.account_id, region=context.region)
-        topic_tokens = store.subscription_tokens.get(topic_arn, {})
+        # this request can come from any http client, it might not be signed (we would need to implement
+        # `authenticate_on_unsubscribe` to force a signing client to do this request.
+        # so, the region and account_id might not be in the request. Use the ones from the topic_arn
+        try:
+            parsed_arn = parse_arn(topic_arn)
+        except InvalidArnException:
+            raise InvalidParameterException("Invalid parameter: Topic")
+
+        store = self.get_store(account_id=parsed_arn["account"], region=parsed_arn["region"])
+
+        # it seems SNS is able to know what the region of the topic should be, even though a wrong topic is accepted
+        if parsed_arn["region"] != get_region_from_subscription_token(token):
+            raise InvalidParameterException("Invalid parameter: Topic")
 
-        subscription_arn = topic_tokens.pop(token, None)
+        subscription_arn = store.subscription_tokens.get(token)
         if not subscription_arn:
             raise InvalidParameterException("Invalid parameter: Token")
 
         subscription = store.subscriptions.get(subscription_arn)
+        if not subscription:
+            # subscription could have been deleted in the meantime
+            raise InvalidParameterException("Invalid parameter: Token")
+
+        # ConfirmSubscription is idempotent
+        if subscription.get("PendingConfirmation") == "false":
+            return ConfirmSubscriptionResponse(SubscriptionArn=subscription_arn)
+
         subscription["PendingConfirmation"] = "false"
         subscription["ConfirmationWasAuthenticated"] = "true"
 
         return ConfirmSubscriptionResponse(SubscriptionArn=subscription_arn)
 
     def untag_resource(
         self, context: RequestContext, resource_arn: AmazonResourceName, tag_keys: TagKeyList
@@ -491,15 +510,15 @@
         if not subscription:
             # unsubscribe is idempotent, so unsubscribing from a non-existing topic does nothing
             return
 
         if subscription["Protocol"] in ["http", "https"]:
             # TODO: actually validate this (re)subscribe behaviour somehow (localhost.run?)
             #  we might need to save the sub token in the store
-            subscription_token = short_uid()
+            subscription_token = encode_subscription_token_with_region(region=context.region)
             message_ctx = SnsMessage(
                 type="UnsubscribeConfirmation",
                 token=subscription_token,
                 message=f"You have chosen to deactivate subscription {subscription_arn}.\nTo cancel this operation and restore the subscription, visit the SubscribeURL included in this message.",
             )
             publish_ctx = SnsPublishContext(
                 message=message_ctx, store=store, request_headers=context.request.headers
@@ -733,17 +752,17 @@
                     attributes["FilterPolicy"]
                 )
 
         store.subscriptions[subscription_arn] = subscription
         store.topic_subscriptions[topic_arn].append(subscription_arn)
 
         # store the token and subscription arn
-        subscription_token = short_uid()
-        topic_tokens = store.subscription_tokens.setdefault(topic_arn, {})
-        topic_tokens[subscription_token] = subscription_arn
+        # TODO: the token is a 288 hex char string
+        subscription_token = encode_subscription_token_with_region(region=context.region)
+        store.subscription_tokens[subscription_token] = subscription_arn
 
         # Send out confirmation message for HTTP(S), fix for https://github.com/localstack/localstack/issues/881
         if protocol in ["http", "https"]:
             message_ctx = SnsMessage(
                 type="SubscriptionConfirmation",
                 token=subscription_token,
                 message=f"You have chosen to subscribe to the topic {topic_arn}.\nTo confirm the subscription, visit the SubscribeURL included in this message.",
@@ -799,15 +818,14 @@
         call_moto(context)
         store = self.get_store(account_id=context.account_id, region=context.region)
         topic_subscriptions = store.topic_subscriptions.pop(topic_arn, [])
         for topic_sub in topic_subscriptions:
             store.subscriptions.pop(topic_sub, None)
 
         store.sns_tags.pop(topic_arn, None)
-        store.subscription_tokens.pop(topic_arn, None)
 
     def create_topic(
         self,
         context: RequestContext,
         name: topicName,
         attributes: TopicAttributesMap = None,
         tags: TagList = None,
@@ -964,14 +982,37 @@
             # this means topic already created with empty tags and when we try to create it
             # again with other tag value then it should fail according to aws documentation.
             if is_create_topic_request and existing_tags is not None and tag not in existing_tags:
                 return False
     return True
 
 
+def encode_subscription_token_with_region(region: str) -> str:
+    """
+    Create a 64 characters Subscription Token with the region encoded
+    :param region:
+    :return: a subscription token with the region encoded
+    """
+    return ((region.encode() + b"/").hex() + short_uid() * 8)[:64]
+
+
+def get_region_from_subscription_token(token: str) -> str:
+    """
+    Try to decode and return the region from a subscription token
+    :param token:
+    :return: the region if able to decode it
+    :raises: InvalidParameterException if the token is invalid
+    """
+    try:
+        region = token.split("2f", maxsplit=1)[0]
+        return bytes.fromhex(region).decode("utf-8")
+    except (IndexError, ValueError, TypeError, UnicodeDecodeError):
+        raise InvalidParameterException("Invalid parameter: Token")
+
+
 def register_sns_api_resource(router: Router):
     """Register the platform endpointmessages retrospection endpoint as an internal LocalStack endpoint."""
     router.add(SNSServicePlatformEndpointMessagesApiResource())
 
 
 def _format_platform_endpoint_messages(sent_messages: List[Dict[str, str]]):
     """
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sns/publisher.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/constants.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/exceptions.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import logging
 import re
 import threading
 import time
 from concurrent.futures.thread import ThreadPoolExecutor
 from queue import Empty
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Tuple
 
 from moto.sqs.models import BINARY_TYPE_FIELD_INDEX, STRING_TYPE_FIELD_INDEX
 from moto.sqs.models import Message as MotoMessage
 
 from localstack import config
 from localstack.aws.accounts import get_aws_account_id
 from localstack.aws.api import CommonServiceException, RequestContext, ServiceException
@@ -443,15 +443,15 @@
                 "InvalidRequest", "This endpoint only accepts ReceiveMessage calls"
             )
 
         if not request.values.get("QueueUrl"):
             raise QueueDoesNotExist()
 
         try:
-            region, account_id, queue_name = parse_queue_url(request.values["QueueUrl"])
+            account_id, region, queue_name = parse_queue_url(request.values["QueueUrl"])
         except ValueError:
             LOG.exception("Error while parsing Queue URL from request values: %s", request.values)
             raise InvalidAddress()
 
         if not region:
             region = extract_region_from_headers(request.headers)
 
@@ -535,14 +535,27 @@
     """
     LocalStack SQS Provider.
 
     LIMITATIONS:
         - Pagination of results (NextToken)
         - Delivery guarantees
         - The region is not encoded in the queue URL
+
+    CROSS-ACCOUNT ACCESS:
+    LocalStack permits cross-account access for all operations. However, AWS
+    disallows the same for following operations:
+        - AddPermission
+        - CreateQueue
+        - DeleteQueue
+        - ListQueues
+        - ListQueueTags
+        - RemovePermission
+        - SetQueueAttributes
+        - TagQueue
+        - UntagQueue
     """
 
     queues: Dict[str, SqsQueue]
 
     def __init__(self) -> None:
         super().__init__()
         self._mutex = threading.RLock()
@@ -564,33 +577,33 @@
         for rule in self._router_rules:
             ROUTER.remove_rule(rule)
 
         self._queue_update_worker.stop()
         self._cloudwatch_publish_worker.stop()
         self._cloudwatch_dispatcher.shutdown()
 
-    def _require_queue(self, context: RequestContext, name: str) -> SqsQueue:
+    def _require_queue(self, account_id: str, region_name: str, name: str) -> SqsQueue:
         """
         Returns the queue for the given name, or raises QueueDoesNotExist if it does not exist.
 
         :param: context: the request context
         :param name: the name to look for
         :returns: the queue
         :raises QueueDoesNotExist: if the queue does not exist
         """
-        store = self.get_store(context.account_id, context.region)
+        store = self.get_store(account_id, region_name)
         with self._mutex:
             if name not in store.queues.keys():
                 raise QueueDoesNotExist("The specified queue does not exist for this wsdl version.")
 
             return store.queues[name]
 
     def _require_queue_by_arn(self, context: RequestContext, queue_arn: str) -> SqsQueue:
         arn = parse_arn(queue_arn)
-        return self._require_queue(context, arn["resource"])
+        return self._require_queue(arn["account"], arn["region"], arn["resource"])
 
     def _resolve_queue(
         self,
         context: RequestContext,
         queue_name: Optional[str] = None,
         queue_url: Optional[str] = None,
     ) -> SqsQueue:
@@ -600,16 +613,16 @@
 
         :param context: the request context, used for getting region and account_id, and optionally the queue_url
         :param queue_name: the queue name (if this is set, then this will be used for the key)
         :param queue_url: the queue url (if name is not set, this will be used to determine the queue name)
         :returns: the queue
         :raises QueueDoesNotExist: if the queue does not exist
         """
-        name = resolve_queue_name(context, queue_name, queue_url)
-        return self._require_queue(context, name)
+        account_id, region_name, name = resolve_queue_location(context, queue_name, queue_url)
+        return self._require_queue(account_id, region_name or context.region, name)
 
     def create_queue(
         self,
         context: RequestContext,
         queue_name: String,
         attributes: QueueAttributeMap = None,
         tags: TagMap = None,
@@ -1272,36 +1285,36 @@
             decoded_binary_value = attr_value.get("BinaryValue")
             MotoMessage.update_binary_length_and_value(hash, decoded_binary_value)
         # string_list_value, binary_list_value type is not implemented, reserved for the future use.
         # See https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_MessageAttributeValue.html
     return hash.hexdigest()
 
 
-def get_queue_name_from_url(queue_url: str) -> str:
-    return queue_url.rstrip("/").split("/")[-1]
-
-
-def resolve_queue_name(
+def resolve_queue_location(
     context: RequestContext, queue_name: Optional[str] = None, queue_url: Optional[str] = None
-) -> str:
+) -> Tuple[str, Optional[str], str]:
     """
-    Resolves a queue name from the given information.
+    Resolves a queue location from the given information.
 
     :param context: the request context, used for getting region and account_id, and optionally the queue_url
     :param queue_name: the queue name (if this is set, then this will be used for the key)
     :param queue_url: the queue url (if name is not set, this will be used to determine the queue name)
-    :return: the queue name describing the queue being requested
+    :return: tuple of account id, region and queue_name
     """
     if not queue_name:
-        if queue_url:
-            queue_name = get_queue_name_from_url(queue_url)
-        else:
-            queue_name = get_queue_name_from_url(context.request.base_url)
+        try:
+            if queue_url:
+                return parse_queue_url(queue_url)
+            else:
+                return parse_queue_url(context.request.base_url)
+        except ValueError:
+            # should work if queue name is passed in QueueUrl
+            return context.account_id, context.region, queue_url
 
-    return queue_name
+    return context.account_id, context.region, queue_name
 
 
 def message_filter_attributes(message: Message, names: Optional[AttributeNameList]):
     """
     Utility function filter from the given message (in-place) the system attributes from the given list. It will
     apply all rules according to:
     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.receive_message.
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/query_api.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sqs/utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sqs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
 
 
 def is_sqs_queue_url(url):
     path = path_from_url(url).partition("?")[0]
     return re.match(r"^/(queue|%s)/[a-zA-Z0-9_-]+(.fifo)?$" % get_aws_account_id(), path)
 
 
-def parse_queue_url(queue_url: str) -> Tuple[Optional[str], str, str]:
+def parse_queue_url(queue_url: str) -> Tuple[str, Optional[str], str]:
     """
-    Parses an SQS Queue URL and returns a triple of region, account_id, and queue_name.
+    Parses an SQS Queue URL and returns a triple of account_id, region and queue_name.
 
     :param queue_url: the queue URL
-    :return: region (may be None), account_id, queue_name
+    :return: account_id, region (may be None), queue_name
     """
     url = urlparse(queue_url.rstrip("/"))
     path_parts = url.path.lstrip("/").split("/")
     domain_parts = url.netloc.split(".")
 
     if len(path_parts) != 2 and len(path_parts) != 4:
         raise ValueError(f"Not a valid queue URL: {queue_url}")
@@ -51,15 +51,15 @@
         region = domain_parts[0]
     elif url.netloc.startswith("queue"):
         # SQS_ENDPOINT_STRATEGY == "domain" (with default region)
         region = "us-east-1"
     else:
         region = None
 
-    return region, account_id, queue_name
+    return account_id, region, queue_name
 
 
 def parse_message_attributes(
     querystring, key="MessageAttribute", base="", value_namespace="Value."
 ):
     message_attributes = {}
     index = 1
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/ssm/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/stores.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/sts/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/packages.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/services/transcribe/provider.py` & `localstack-core-2.0.3.dev20230418093340/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/state/core.py` & `localstack-core-2.0.3.dev20230418093340/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/state/inspect.py` & `localstack-core-2.0.3.dev20230418093340/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/state/pickle.py` & `localstack-core-2.0.3.dev20230418093340/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/state/snapshot.py` & `localstack-core-2.0.3.dev20230418093340/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/asf_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/aws/util.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/filters.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/fixtures.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/snapshot.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/pytest/util.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/prototype.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/report.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/transformer.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.0.3.dev20230418093340/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/cli.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/events.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/logger.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/metadata.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/publisher.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/archives.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/asyncio.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/auth.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/arns.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/aws_models.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/aws_responses.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/aws_stack.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/client_types.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/queries.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/request_context.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/resources.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/aws/templating.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/bootstrap.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/collections.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/common.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/config_listener.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/container_networking.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/container_client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/coverage_docs.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/crypto.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/diagnose.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/docker_utils.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/files.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/functions.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/http.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/json.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/net.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/numbers.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/objects.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/patch.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/platform.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/run.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/scheduler.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/server/http2_server.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/server/proxy_server.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/serving.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/ssl.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/strings.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/sync.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/tagging.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/tail.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/testutil.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/threads.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/time.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/urls.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/venv.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack/utils/xml.py` & `localstack-core-2.0.3.dev20230418093340/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.0.3.dev20230418071728
+Version: 2.0.3.dev20230418093340
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/plux.json` & `localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9383223684210527%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(1, '*

 * *                                      "'validate_configuration=localstack.services.awslambda.plugins:validate_configuration')], "*

 * *                                      'delete: [3]}',*

 * * "'localstack.packages'": '{insert: [(1, '*

 * *                          "'cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package'), "*

 * *                          '(2, '*

 * *                          "'opensearch/community=localstack.services […]*

```diff
@@ -54,35 +54,35 @@
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
         "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
-        "terraform/community=localstack.packages.plugins:terraform_package",
-        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
         "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package"
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package"
     ]
 }
```

### Comparing `localstack-core-2.0.3.dev20230418071728/localstack_core.egg-info/requires.txt` & `localstack-core-2.0.3.dev20230418093340/localstack_core.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 flask-cors<3.1.0,>=3.0.3
 flask_swagger==0.2.12
 hypercorn==0.14.2
 json5==0.9.11
 jsonpatch<2.0,>=1.24
 jsonpath-ng>=1.5.3
 jsonpath-rw<2.0.0,>=1.4.0
-moto-ext[all]==4.1.5.post2
+moto-ext[all]==4.1.7.post2
 opensearch-py==2.1.1
 pproxy>=2.7.0
 pymongo>=4.2.0
 pyopenssl>=23.0.0
 Quart==0.17
 readerwriterlock>=1.0.7
 requests-aws4auth>=1.0
@@ -89,15 +89,15 @@
 flask-cors<3.1.0,>=3.0.3
 flask_swagger==0.2.12
 hypercorn==0.14.2
 json5==0.9.11
 jsonpatch<2.0,>=1.24
 jsonpath-ng>=1.5.3
 jsonpath-rw<2.0.0,>=1.4.0
-moto-ext[all]==4.1.5.post2
+moto-ext[all]==4.1.7.post2
 opensearch-py==2.1.1
 pproxy>=2.7.0
 pymongo>=4.2.0
 pyopenssl>=23.0.0
 Quart==0.17
 readerwriterlock>=1.0.7
 requests-aws4auth>=1.0
```

### Comparing `localstack-core-2.0.3.dev20230418071728/pyproject.toml` & `localstack-core-2.0.3.dev20230418093340/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.0.3.dev20230418071728/setup.cfg` & `localstack-core-2.0.3.dev20230418093340/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 	flask-cors>=3.0.3,<3.1.0
 	flask_swagger==0.2.12
 	hypercorn==0.14.2
 	json5==0.9.11
 	jsonpatch>=1.24,<2.0
 	jsonpath-ng>=1.5.3
 	jsonpath-rw>=1.4.0,<2.0.0
-	moto-ext[all]==4.1.5.post2
+	moto-ext[all]==4.1.7.post2
 	opensearch-py==2.1.1
 	pproxy>=2.7.0
 	pymongo>=4.2.0
 	pyopenssl>=23.0.0
 	Quart==0.17
 	readerwriterlock>=1.0.7
 	requests-aws4auth>=1.0
```

