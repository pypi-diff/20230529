# Comparing `tmp/localstack-core-2.1.1.dev20230529183933.tar.gz` & `tmp/localstack-core-2.1.1.dev20230529184621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230529183933.tar", last modified: Mon May 29 18:39:41 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230529184621.tar", last modified: Mon May 29 18:46:28 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230529183933.tar` & `localstack-core-2.1.1.dev20230529184621.tar`

### file list

```diff
@@ -1,850 +1,849 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-05-29 18:39:33.000000 localstack-core-2.1.1.dev20230529183933/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.932254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.936254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.936254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125427 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.936254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.936254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.936254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755668 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48662 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71916 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.952254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.956254 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28125 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18437 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49652 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7805 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15553 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/contrib/thundra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.960254 localstack-core-2.1.1.dev20230529183933/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.964254 localstack-core-2.1.1.dev20230529183933/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.964254 localstack-core-2.1.1.dev20230529183933/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.964254 localstack-core-2.1.1.dev20230529183933/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.964254 localstack-core-2.1.1.dev20230529183933/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.964254 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.968254 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24219 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.968254 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.968254 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17789 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21256 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28278 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12461 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91859 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.968254 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155097 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.968254 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.972254 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17238 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64725 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.972254 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    30467 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28326 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5326 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11295 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36723 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.972254 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.972254 localstack-core-2.1.1.dev20230529183933/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.972254 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.976254 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.976254 localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.976254 localstack-core-2.1.1.dev20230529183933/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.992254 localstack-core-2.1.1.dev20230529183933/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22448 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19454 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:40.996254 localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3172 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    64987 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9218 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    47737 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54790 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.000254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.004254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.004254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.004254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.004254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.004254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.004254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.012254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.016254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.016254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.016254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.020254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.024254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.024254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.024254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.024254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.028254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.028254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.028254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.028254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.028254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.036254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.036254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.036254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.036254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.036254 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.044253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.048253 localstack-core-2.1.1.dev20230529183933/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.052253 localstack-core-2.1.1.dev20230529183933/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.052253 localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12950 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.052253 localstack-core-2.1.1.dev20230529183933/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.052253 localstack-core-2.1.1.dev20230529183933/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.052253 localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.052253 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67734 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.056253 localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.056253 localstack-core-2.1.1.dev20230529183933/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13471 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13278 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23998 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4512 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    44447 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33085 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:39:41.060253 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-29 18:39:40.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37732 2023-05-29 18:39:40.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 18:39:40.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-29 18:39:40.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 18:39:37.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-05-29 18:39:37.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2023-05-29 18:39:40.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-05-29 18:39:40.000000 localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3145 2023-05-29 18:39:41.064253 localstack-core-2.1.1.dev20230529183933/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-05-29 18:07:07.000000 localstack-core-2.1.1.dev20230529183933/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-05-29 18:46:21.000000 localstack-core-2.1.1.dev20230529184621/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.872997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125427 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755668 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48662 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71916 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.876997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.880997 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28125 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18437 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      997 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49526 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7805 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      193 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.884997 localstack-core-2.1.1.dev20230529184621/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.888997 localstack-core-2.1.1.dev20230529184621/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.888997 localstack-core-2.1.1.dev20230529184621/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.888997 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    41169 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12745 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12099 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67662 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.888997 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24219 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.888997 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.892997 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17789 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21256 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28278 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12461 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72195 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.892997 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155097 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.892997 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.892997 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17238 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    64725 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8781 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2316 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.896997 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    30467 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28326 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5326 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11295 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36723 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.896997 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.896997 localstack-core-2.1.1.dev20230529184621/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5747 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22448 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19454 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.900997 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.904997 localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3172 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    64987 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9218 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5648 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    47737 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1666 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54790 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.908997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.912997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.916997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.916997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.920997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.920997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.920997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.920997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.920997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.920997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.924997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.924997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.928997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.928997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.928997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.928997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.928997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.928997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.932997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.932997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.932997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.932997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.936997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.936997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.936997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.936997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.940997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.940997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.940997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.940997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.940997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.944997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.948997 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.948997 localstack-core-2.1.1.dev20230529184621/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.948997 localstack-core-2.1.1.dev20230529184621/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.948997 localstack-core-2.1.1.dev20230529184621/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.948997 localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      206 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12950 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.952997 localstack-core-2.1.1.dev20230529184621/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.952997 localstack-core-2.1.1.dev20230529184621/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.952997 localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.952997 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67734 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.952997 localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.956997 localstack-core-2.1.1.dev20230529184621/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.956997 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.956997 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13471 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13278 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23998 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4512 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    44447 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33085 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10057 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-05-29 18:46:28.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37702 2023-05-29 18:46:28.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 18:46:28.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4968 2023-05-29 18:46:28.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 18:46:25.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5055 2023-05-29 18:46:25.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2023-05-29 18:46:28.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-05-29 18:46:28.000000 localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3145 2023-05-29 18:46:28.960997 localstack-core-2.1.1.dev20230529184621/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-05-29 18:16:02.000000 localstack-core-2.1.1.dev20230529184621/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230529183933/LICENSE.txt` & `localstack-core-2.1.1.dev20230529184621/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/Makefile` & `localstack-core-2.1.1.dev20230529184621/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/PKG-INFO` & `localstack-core-2.1.1.dev20230529184621/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230529183933
+Version: 2.1.1.dev20230529184621
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230529183933/README.md` & `localstack-core-2.1.1.dev20230529184621/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/bin/localstack` & `localstack-core-2.1.1.dev20230529184621/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230529184621/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230529184621/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230529184621/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230529184621/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230529184621/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230529184621/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230529184621/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/config.py` & `localstack-core-2.1.1.dev20230529184621/localstack/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1130,18 +1130,14 @@
     "STEPFUNCTIONS_LAMBDA_ENDPOINT",
     "SYNCHRONOUS_KINESIS_EVENTS",
     "SYNCHRONOUS_SNS_EVENTS",
     "TEST_AWS_ACCOUNT_ID",
     "TEST_IAM_USER_ID",
     "TEST_IAM_USER_NAME",
     "TF_COMPAT_MODE",
-    "THUNDRA_APIKEY",
-    "THUNDRA_AGENT_JAVA_VERSION",
-    "THUNDRA_AGENT_NODE_VERSION",
-    "THUNDRA_AGENT_PYTHON_VERSION",
     "USE_SINGLE_REGION",
     "USE_SSL",
     "WAIT_FOR_DEBUGGER",
     "WINDOWS_DOCKER_MOUNT_PREFIX",
 ]
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/constants.py` & `localstack-core-2.1.1.dev20230529184621/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/contrib/thundra.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,449 +1,455 @@
+import base64
 import json
 import logging
 import os
-from typing import Optional, Union
+import re
+import tempfile
+import time
+from functools import lru_cache
+from io import BytesIO
+from typing import Any, Dict, List, Optional, Union
+
+from flask import Response
 
 from localstack import config
-from localstack.services.awslambda.lambda_executors import (
-    AdditionalInvocationOptions,
-    InvocationContext,
-    InvocationResult,
-    LambdaExecutorPlugin,
-    is_java_lambda,
-    is_nodejs_runtime,
-)
-from localstack.services.awslambda.lambda_utils import (
-    LAMBDA_RUNTIME_JAVA8,
-    LAMBDA_RUNTIME_JAVA8_AL2,
-    LAMBDA_RUNTIME_JAVA11,
-    LAMBDA_RUNTIME_NODEJS12X,
-    LAMBDA_RUNTIME_NODEJS14X,
-    LAMBDA_RUNTIME_NODEJS16X,
-    LAMBDA_RUNTIME_PYTHON37,
-    LAMBDA_RUNTIME_PYTHON38,
-    get_executor_mode,
-    is_python_runtime,
+from localstack.aws.accounts import get_aws_account_id
+from localstack.aws.api.lambda_ import FilterCriteria, Runtime
+from localstack.aws.connect import connect_to
+from localstack.services.awslambda.lambda_models import AwsLambdaStore, awslambda_stores
+from localstack.utils.aws import aws_stack
+from localstack.utils.aws.arns import extract_account_id_from_arn, extract_region_from_arn
+from localstack.utils.aws.aws_models import LambdaFunction
+from localstack.utils.aws.aws_responses import flask_error_response_json
+from localstack.utils.container_networking import (
+    get_endpoint_for_network,
+    get_main_container_network,
 )
-from localstack.utils import common
-from localstack.utils.http import download
+from localstack.utils.docker_utils import DOCKER_CLIENT
+from localstack.utils.strings import first_char_to_lower, short_uid
 
-# logger
 LOG = logging.getLogger(__name__)
+# Custom logger for proactive deprecation hints related to the migration from the old to the new lambda provider
+HINT_LOG = logging.getLogger("localstack.services.awslambda.hints")
 
-# Global constants
-THUNDRA_APIKEY_ENV_VAR_NAME = "THUNDRA_APIKEY"
-THUNDRA_AGENT_LAMBDA_HANDLER_ENV_VAR_NAME = "THUNDRA_AGENT_LAMBDA_HANDLER"
-THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME = "THUNDRA_AGENT_LAMBDA_LOG_DISABLE"
-THUNDRA_APIKEY = os.getenv(THUNDRA_APIKEY_ENV_VAR_NAME)
-
-# Java related constants
-THUNDRA_JAVA_AGENT_INITIALIZED = False
-THUNDRA_JAVA_AGENT_REMOTE_URL: Optional[str] = None
-THUNDRA_JAVA_AGENT_LOCAL_PATH: Optional[str] = None
-
-# Node related constants
-THUNDRA_NODE_AGENT_INITIALIZED = False
-THUNDRA_NODE_AGENT_VERSION: Optional[str] = None
-THUNDRA_NODE_AGENT_LOCAL_PATH: Optional[str] = None
-THUNDRA_NODE_AGENT_LOCAL_PATH_ON_HOST: Optional[str] = None
-
-# Python related constants
-THUNDRA_PYTHON_AGENT_INITIALIZED = False
-THUNDRA_PYTHON_AGENT_VERSION: Optional[str] = None
-THUNDRA_PYTHON_AGENT_LOCAL_PATH: Optional[str] = None
-THUNDRA_PYTHON_AGENT_LOCAL_PATH_ON_HOST: Optional[str] = None
-
-
-################
-# COMMON
-################
-
-
-def _log_install_msg(component):
-    LOG.info("Downloading and installing %s. This may take some time.", component)
-
-
-def _get_apikey(env_vars):
-    thundra_apikey = env_vars.get(THUNDRA_APIKEY_ENV_VAR_NAME)
+# root path of Lambda API endpoints
+API_PATH_ROOT = "/2015-03-31"
+API_PATH_ROOT_2 = "/2021-10-31"
+
+
+# Lambda runtime constants (LEGACY, use values in Runtime class instead)
+LAMBDA_RUNTIME_PYTHON37 = Runtime.python3_7
+LAMBDA_RUNTIME_PYTHON38 = Runtime.python3_8
+LAMBDA_RUNTIME_PYTHON39 = Runtime.python3_9
+LAMBDA_RUNTIME_NODEJS = Runtime.nodejs
+LAMBDA_RUNTIME_NODEJS12X = Runtime.nodejs12_x
+LAMBDA_RUNTIME_NODEJS14X = Runtime.nodejs14_x
+LAMBDA_RUNTIME_NODEJS16X = Runtime.nodejs16_x
+LAMBDA_RUNTIME_JAVA8 = Runtime.java8
+LAMBDA_RUNTIME_JAVA8_AL2 = Runtime.java8_al2
+LAMBDA_RUNTIME_JAVA11 = Runtime.java11
+LAMBDA_RUNTIME_DOTNETCORE31 = Runtime.dotnetcore3_1
+LAMBDA_RUNTIME_DOTNET6 = Runtime.dotnet6
+LAMBDA_RUNTIME_GOLANG = Runtime.go1_x
+LAMBDA_RUNTIME_RUBY27 = Runtime.ruby2_7
+LAMBDA_RUNTIME_PROVIDED = Runtime.provided
+LAMBDA_RUNTIME_PROVIDED_AL2 = Runtime.provided_al2
+
+
+# default handler and runtime
+LAMBDA_DEFAULT_HANDLER = "handler.handler"
+LAMBDA_DEFAULT_RUNTIME = LAMBDA_RUNTIME_PYTHON39  # FIXME (?)
+LAMBDA_DEFAULT_STARTING_POSITION = "LATEST"
+
+# List of Dotnet Lambda runtime names
+DOTNET_LAMBDA_RUNTIMES = [
+    LAMBDA_RUNTIME_DOTNETCORE31,
+    LAMBDA_RUNTIME_DOTNET6,
+]
+
+# IP address of main Docker container (lazily initialized)
+DOCKER_MAIN_CONTAINER_IP = None
+LAMBDA_CONTAINER_NETWORK = None
+
+FUNCTION_NAME_REGEX = re.compile(
+    r"(arn:(aws[a-zA-Z-]*)?:lambda:)?((?P<region>[a-z]{2}(-gov)?-[a-z]+-\d{1}):)?(?P<account>\d{12}:)?(function:)?(?P<name>[a-zA-Z0-9-_\.]+)(:(?P<qualifier>\$LATEST|[a-zA-Z0-9-_]+))?"
+)  # also length 1-170 incl.
+
+
+class ClientError(Exception):
+    def __init__(self, msg, code=400):
+        super(ClientError, self).__init__(msg)
+        self.code = code
+        self.msg = msg
+
+    def get_response(self):
+        if isinstance(self.msg, Response):
+            return self.msg
+        return error_response(self.msg, self.code)
+
+
+@lru_cache()
+def get_default_executor_mode() -> str:
+    """
+    Returns the default docker executor mode, which is "docker" if the docker socket is available via the docker
+    client, or "local"  otherwise.
 
-    # If Thundra API key is specified for the function through env vars, use it
-    if not thundra_apikey:
-        # Otherwise, try to get it from Localstack env vars
-        thundra_apikey = THUNDRA_APIKEY
-
-    return thundra_apikey
+    :return: 'docker' if docker socket available, otherwise 'local'
+    """
+    try:
+        return "docker" if DOCKER_CLIENT.has_docker() else "local"
+    except Exception:
+        return "local"
 
 
-################
-# JAVA AGENT
-################
+def get_executor_mode() -> str:
+    """
+    Returns the currently active lambda executor mode. If config.LAMBDA_EXECUTOR is set, then it returns that,
+    otherwise it falls back to get_default_executor_mode().
 
+    :return: the lambda executor mode (e.g., 'local', 'docker', or 'docker-reuse')
+    """
+    return config.LAMBDA_EXECUTOR or get_default_executor_mode()
 
-def _ensure_java_agent_initialized():
-    global THUNDRA_JAVA_AGENT_INITIALIZED
-    if not THUNDRA_JAVA_AGENT_INITIALIZED:
-        _init_java_agent_configs()
-        _install_java_agent()
-        THUNDRA_JAVA_AGENT_INITIALIZED = True
 
+def get_lambda_runtime(runtime_details: Union[LambdaFunction, str]) -> str:
+    """Return the runtime string from the given LambdaFunction (or runtime string)."""
+    if isinstance(runtime_details, LambdaFunction):
+        runtime_details = runtime_details.runtime
+    if not isinstance(runtime_details, str):
+        LOG.info("Unable to determine Lambda runtime from parameter: %s", runtime_details)
+    return runtime_details or ""
 
-def _get_latest_java_agent_version(metadata_url):
-    try:
-        import xml.etree.ElementTree as et
 
-        import requests
+def is_provided_runtime(runtime_details: Union[LambdaFunction, str]) -> bool:
+    """Whether the given LambdaFunction uses a 'provided' runtime."""
+    runtime = get_lambda_runtime(runtime_details) or ""
+    return runtime.startswith("provided")
 
-        response = requests.get(metadata_url)
-        xml = et.fromstring(response.content)
-        latest_version = xml.find("./versioning/latest").text
 
-        return latest_version
-    except Exception as e:
-        print("Unable to get latest version of Thundra Java agent: %s" % e)
-        return "LATEST"
+def format_name_to_path(handler_name: str, delimiter: str, extension: str):
+    file_path = handler_name.rpartition(delimiter)[0]
+    if delimiter == ":":
+        file_path = file_path.split(delimiter)[0]
 
+    if os.path.sep not in file_path:
+        file_path = file_path.replace(".", os.path.sep)
 
-def _init_java_agent_configs():
-    global THUNDRA_JAVA_AGENT_REMOTE_URL
-    global THUNDRA_JAVA_AGENT_LOCAL_PATH
-
-    metadata_url = (
-        "https://repo.thundra.io/service/local/repositories/thundra-releases/content/"
-        + "io/thundra/agent/thundra-agent-lambda-bootstrap/maven-metadata.xml"
-    )
-    latest_version = _get_latest_java_agent_version(metadata_url)
-    version = os.getenv("THUNDRA_AGENT_JAVA_VERSION", latest_version)
-    jar_name = "thundra-agent-%s.jar" % version
+    if file_path.startswith(f".{os.path.sep}"):
+        file_path = file_path[2:]
 
-    THUNDRA_JAVA_AGENT_REMOTE_URL = (
-        "https://repo.thundra.io/service/local/artifact/maven/redirect?"
-        + "r=thundra-releases&g=io.thundra.agent&a=thundra-agent-lambda-bootstrap&v={v}"
-    ).format(v=version)
-    THUNDRA_JAVA_AGENT_LOCAL_PATH = "%s/%s" % (config.dirs.tmp, jar_name)
+    return f"{file_path}{extension}"
 
 
-# TODO migrate these install commands to package installers
-def _install_java_agent():
-    # Install Thundra Java agent JAR file
-    if not os.path.exists(THUNDRA_JAVA_AGENT_LOCAL_PATH):
-        _log_install_msg("Thundra Java agent")
-        download(THUNDRA_JAVA_AGENT_REMOTE_URL, THUNDRA_JAVA_AGENT_LOCAL_PATH)
+def get_handler_file_from_name(handler_name: str, runtime: str = None):
+    runtime = runtime or LAMBDA_DEFAULT_RUNTIME
 
+    if runtime.startswith(LAMBDA_RUNTIME_PROVIDED):
+        return "bootstrap"
+    if runtime.startswith("nodejs"):
+        return format_name_to_path(handler_name, ".", ".js")
+    if runtime.startswith(LAMBDA_RUNTIME_GOLANG):
+        return handler_name
+    if runtime.startswith(tuple(DOTNET_LAMBDA_RUNTIMES)):
+        return format_name_to_path(handler_name, ":", ".dll")
+    if runtime.startswith("ruby"):
+        return format_name_to_path(handler_name, ".", ".rb")
 
-def _is_java8_lambda(func_details):
-    runtime = getattr(func_details, "runtime", func_details)
-    return runtime == LAMBDA_RUNTIME_JAVA8 or runtime == LAMBDA_RUNTIME_JAVA8_AL2
+    return format_name_to_path(handler_name, ".", ".py")
 
 
-def _is_java_lambda_with_support_version(lambda_details):
+def is_java_lambda(lambda_details):
     runtime = getattr(lambda_details, "runtime", lambda_details)
     return runtime in [LAMBDA_RUNTIME_JAVA8, LAMBDA_RUNTIME_JAVA8_AL2, LAMBDA_RUNTIME_JAVA11]
 
 
-def _prepare_invocation_for_java_lambda(context: InvocationContext) -> AdditionalInvocationOptions:
-    # Download and initialize Java agent
-    _ensure_java_agent_initialized()
-
-    # If agent could not be initialized, skip here
-    if not THUNDRA_JAVA_AGENT_INITIALIZED:
-        return None
-
-    result = AdditionalInvocationOptions()
-    environment = context.environment
-    agent_flag = "-javaagent:{agent_path}"
-
-    # Inject Thundra agent path into "JAVA_TOOL_OPTIONS" env var,
-    # so it will be automatically loaded on JVM startup
-    java_tool_opts = environment.get("JAVA_TOOL_OPTIONS", "")
-    if agent_flag not in java_tool_opts:
-        java_tool_opts += f" {agent_flag}"
-    result.env_updates["JAVA_TOOL_OPTIONS"] = java_tool_opts.strip()
-
-    # Disable CDS (Class Data Sharing),
-    # because "-javaagent" cannot be enabled when CDS is enabled on JDK 8.
-    # CDS can only be disabled by "_JAVA_OPTIONS" env var,
-    # because by default it is enabled ("-Xshare:on")
-    # on Lambci by command line parameters and
-    # "_JAVA_OPTIONS" has precedence over command line parameters
-    # but "JAVA_TOOL_OPTIONS" is not.
-    if _is_java8_lambda(context.lambda_function):
-        java_opts = environment.get("_JAVA_OPTIONS", "")
-        java_opts += " -Xshare:off"
-        result.env_updates["_JAVA_OPTIONS"] = java_opts.strip()
-
-    # If log disable is not configured explicitly, set it to false to enable log capturing by default
-    log_disabled = environment.get(THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME)
-    if not log_disabled:
-        result.env_updates[THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME] = "false"
-
-    # Make sure API key is contained in environment
-    result.env_updates[THUNDRA_APIKEY_ENV_VAR_NAME] = _get_apikey(environment)
-
-    # Note: The code below doesn't seem to be required, as LAMBDA_EXECUTOR=local also picks up $JAVA_TOOL_OPTIONS
-    # if context.lambda_command:
-    #     result.updated_command = context.lambda_command.replace(
-    #         "java ", f"java {agent_flag} ", 1
-    #     )
-    # construct agent file path mapping
-    result.files_to_add["agent_path"] = THUNDRA_JAVA_AGENT_LOCAL_PATH
-
-    return result
-
-
-################
-# NODE AGENT
-################
-
-
-def _ensure_node_agent_initialized():
-    global THUNDRA_NODE_AGENT_INITIALIZED
-    if not THUNDRA_NODE_AGENT_INITIALIZED:
-        if _init_node_agent_configs() and _install_node_agent():
-            THUNDRA_NODE_AGENT_INITIALIZED = True
+def is_nodejs_runtime(lambda_details):
+    runtime = getattr(lambda_details, "runtime", lambda_details) or ""
+    return runtime.startswith("nodejs")
+
+
+def is_python_runtime(lambda_details):
+    runtime = getattr(lambda_details, "runtime", lambda_details) or ""
+    return runtime.startswith("python")
+
+
+def store_lambda_logs(
+    lambda_function: LambdaFunction, log_output: str, invocation_time=None, container_id=None
+):
+    # leave here to avoid import issues from CLI
+    from localstack.utils.cloudwatch.cloudwatch_util import store_cloudwatch_logs
+
+    log_group_name = "/aws/lambda/%s" % lambda_function.name()
+    container_id = container_id or short_uid()
+    invocation_time = invocation_time or int(time.time() * 1000)
+    invocation_time_secs = int(invocation_time / 1000)
+    time_str = time.strftime("%Y/%m/%d", time.gmtime(invocation_time_secs))
+    log_stream_name = "%s/[LATEST]%s" % (time_str, container_id)
+    return store_cloudwatch_logs(log_group_name, log_stream_name, log_output, invocation_time)
+
+
+def get_main_endpoint_from_container() -> str:
+    if config.HOSTNAME_FROM_LAMBDA:
+        return config.HOSTNAME_FROM_LAMBDA
+    return get_endpoint_for_network(network=get_container_network_for_lambda())
+
+
+def get_container_network_for_lambda() -> str:
+    global LAMBDA_CONTAINER_NETWORK
+    if config.LAMBDA_DOCKER_NETWORK:
+        return config.LAMBDA_DOCKER_NETWORK
+    return get_main_container_network()
+
+
+def rm_docker_container(container_name_or_id, check_existence=False, safe=False):
+    # TODO: remove method / move to docker module
+    if not container_name_or_id:
+        return
+    if check_existence and container_name_or_id not in DOCKER_CLIENT.get_running_container_names():
+        # TODO: check names as well as container IDs!
+        return
+    try:
+        DOCKER_CLIENT.remove_container(container_name_or_id)
+    except Exception:
+        if not safe:
+            raise
 
 
-def _get_latest_node_agent_version():
+def get_record_from_event(event: Dict, key: str) -> Any:
+    """Retrieve a field with the given key from the list of Records within 'event'."""
     try:
-        return common.run("npm view @thundra/core version".split())
-    except Exception as e:
-        print("Unable to get latest version of Thundra Node agent: %s" % e)
+        return event["Records"][0][key]
+    except KeyError:
         return None
 
 
-def _init_node_agent_configs() -> bool:
-    global THUNDRA_NODE_AGENT_VERSION
-    global THUNDRA_NODE_AGENT_LOCAL_PATH
-    global THUNDRA_NODE_AGENT_LOCAL_PATH_ON_HOST
-
-    latest_version = _get_latest_node_agent_version()
-    version = os.getenv("THUNDRA_AGENT_NODE_VERSION", latest_version)
-    if not version:
-        return False
-
-    THUNDRA_NODE_AGENT_VERSION = version.strip()
-    THUNDRA_NODE_AGENT_LOCAL_PATH = "%s/thundra/node/%s/" % (
-        config.dirs.tmp,
-        THUNDRA_NODE_AGENT_VERSION,
-    )
-    THUNDRA_NODE_AGENT_LOCAL_PATH_ON_HOST = "%s/thundra/node/%s/" % (
-        config.dirs.functions,
-        THUNDRA_NODE_AGENT_VERSION,
-    )
-
-    return True
-
-
-def _install_node_agent() -> bool:
-    # Install Thundra Node agent NPM package
-    if not os.path.exists(THUNDRA_NODE_AGENT_LOCAL_PATH):
-        _log_install_msg("Thundra Node agent")
+def get_lambda_extraction_dir() -> str:
+    """
+    Get the directory a lambda is supposed to use as working directory (= the directory to extract the contents to).
+    This method is needed due to performance problems for IO on bind volumes when running inside Docker Desktop, due to
+    the file sharing with the host being slow when using gRPC-FUSE.
+    By extracting to a not-mounted directory, we can improve performance significantly.
+    The lambda zip file itself, however, should still be located on the mount.
+
+    :return: directory path
+    """
+    if config.LAMBDA_REMOTE_DOCKER:
+        return tempfile.gettempdir()
+    return config.dirs.tmp
+
+
+def get_zip_bytes(function_code):
+    """Returns the ZIP file contents from a FunctionCode dict.
+
+    :type function_code: dict
+    :param function_code: https://docs.aws.amazon.com/lambda/latest/dg/API_FunctionCode.html
+    :returns: bytes of the Zip file.
+    """
+    function_code = function_code or {}
+    if "S3Bucket" in function_code:
+        s3_client = connect_to().s3
+        bytes_io = BytesIO()
         try:
-            install_thundra_cmd = "npm install --prefix %s @thundra/core@%s --no-save" % (
-                THUNDRA_NODE_AGENT_LOCAL_PATH,
-                THUNDRA_NODE_AGENT_VERSION,
-            )
-            common.run(install_thundra_cmd.split())
+            s3_client.download_fileobj(function_code["S3Bucket"], function_code["S3Key"], bytes_io)
+            zip_file_content = bytes_io.getvalue()
         except Exception as e:
-            print("Unable to install Thundra Node agent: %s" % e)
-            return False
-    return True
-
-
-def _is_node_lambda_with_support_version(func_details):
-    runtime = getattr(func_details, "runtime", func_details)
-    return runtime in [
-        LAMBDA_RUNTIME_NODEJS12X,
-        LAMBDA_RUNTIME_NODEJS14X,
-        LAMBDA_RUNTIME_NODEJS16X,
-    ]
-
-
-def _prepare_invocation_for_node_lambda(context: InvocationContext) -> AdditionalInvocationOptions:
-    # Download and initialize Node agent
-    _ensure_node_agent_initialized()
-
-    # If agent could not be initialized, skip here
-    if not THUNDRA_NODE_AGENT_INITIALIZED:
-        return None
-
-    result = AdditionalInvocationOptions()
-
-    # Make sure API key is contained in environment
-    result.env_updates[THUNDRA_APIKEY_ENV_VAR_NAME] = _get_apikey(context.environment)
-
-    # Switch handler to Thundra and pass original handler to Thundra through environment variable
-    result.env_updates[THUNDRA_AGENT_LAMBDA_HANDLER_ENV_VAR_NAME] = context.handler
-    result.updated_handler = "/opt/nodejs/node_modules/@thundra/core/dist/handler.wrapper"
-
-    # If log disable is not configured explicitly, set it to false to enable log capturing by default
-    log_disabled = context.environment.get(THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME)
-    if not log_disabled:
-        result.env_updates[THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME] = "false"
-
-    # Map Thundra agent path into container so it will be accessible by Lambda function Node environment
-    agent_path_mapping = (
-        "-v %s/node_modules/:/opt/nodejs/node_modules/" % THUNDRA_NODE_AGENT_LOCAL_PATH_ON_HOST
-    )
-
-    if context.docker_flags:
-        context.docker_flags = f"{context.docker_flags} {agent_path_mapping}"
+            s3_key = str(function_code.get("S3Key") or "")
+            s3_url = f's3://{function_code["S3Bucket"]}{s3_key if s3_key.startswith("/") else f"/{s3_key}"}'
+            raise ClientError(f"Unable to fetch Lambda archive from {s3_url}: {e}", 404)
+    elif "ZipFile" in function_code:
+        zip_file_content = function_code["ZipFile"]
+        zip_file_content = base64.b64decode(zip_file_content)
+    elif "ImageUri" in function_code:
+        zip_file_content = None
     else:
-        context.docker_flags = agent_path_mapping
+        raise ClientError("No valid Lambda archive specified: %s" % list(function_code.keys()))
+    return zip_file_content
 
-    return result
 
+def event_source_arn_matches(mapped: str, searched: str) -> bool:
+    if not mapped:
+        return False
+    if not searched or mapped == searched:
+        return True
+    # Some types of ARNs can end with a path separated by slashes, for
+    # example the ARN of a DynamoDB stream is tableARN/stream/ID. It's
+    # a little counterintuitive that a more specific mapped ARN can
+    # match a less specific ARN on the event, but some integration tests
+    # rely on it for things like subscribing to a stream and matching an
+    # event labeled with the table ARN.
+    if re.match(r"^%s$" % searched, mapped):
+        return True
+    if mapped.startswith(searched):
+        suffix = mapped[len(searched) :]
+        return suffix[0] == "/"
+    return False
+
+
+def error_response(msg, code=500, error_type="InternalFailure"):
+    if code != 404:
+        LOG.debug(msg)
+    return flask_error_response_json(msg, code=code, error_type=error_type)
+
+
+def generate_lambda_arn(
+    account_id: int, region: str, fn_name: str, qualifier: Optional[str] = None
+):
+    if qualifier:
+        return f"arn:aws:lambda:{region}:{account_id}:function:{fn_name}:{qualifier}"
+    else:
+        return f"arn:aws:lambda:{region}:{account_id}:function:{fn_name}"
 
-################
-# PYTHON AGENT
-################
-
-
-def _ensure_python_agent_initialized():
-    global THUNDRA_PYTHON_AGENT_INITIALIZED
-    if not THUNDRA_PYTHON_AGENT_INITIALIZED:
-        if _init_python_agent_configs() and _install_python_agent():
-            THUNDRA_PYTHON_AGENT_INITIALIZED = True
-
-
-def _get_latest_python_agent_version():
-    try:
-        from distutils.version import StrictVersion
-
-        import requests
 
-        response = requests.get("https://pypi.org/pypi/thundra/json")
-        data = json.loads(response.content.decode())
-        versions = sorted(list(data["releases"].keys()), key=StrictVersion, reverse=True)
-        return versions[0]
-    except Exception as e:
-        print("Unable to get latest version of Thundra Python agent: %s" % e)
-        return None
+def parse_and_apply_numeric_filter(
+    record_value: Dict, numeric_filter: List[Union[str, int]]
+) -> bool:
+    if len(numeric_filter) % 2 > 0:
+        LOG.warn("Invalid numeric lambda filter given")
+        return True
 
-
-def _init_python_agent_configs() -> bool:
-    global THUNDRA_PYTHON_AGENT_VERSION
-    global THUNDRA_PYTHON_AGENT_LOCAL_PATH
-    global THUNDRA_PYTHON_AGENT_LOCAL_PATH_ON_HOST
-
-    latest_version = _get_latest_python_agent_version()
-    version = os.getenv("THUNDRA_AGENT_PYTHON_VERSION", latest_version)
-    if not version:
+    if not isinstance(record_value, (int, float)):
+        LOG.warn(f"Record {record_value} seem not to be a valid number")
         return False
 
-    THUNDRA_PYTHON_AGENT_VERSION = version.strip()
-    THUNDRA_PYTHON_AGENT_LOCAL_PATH = "%s/thundra/python/%s/" % (
-        config.dirs.tmp,
-        THUNDRA_PYTHON_AGENT_VERSION,
-    )
-    THUNDRA_PYTHON_AGENT_LOCAL_PATH_ON_HOST = "%s/thundra/python/%s/" % (
-        config.dirs.functions,
-        THUNDRA_PYTHON_AGENT_VERSION,
-    )
-
-    return True
+    for idx in range(0, len(numeric_filter), 2):
 
-
-def _install_python_agent() -> bool:
-    # Install Thundra Python agent PIP package
-    if not os.path.exists(THUNDRA_PYTHON_AGENT_LOCAL_PATH):
-        _log_install_msg("Thundra Python agent")
         try:
-            install_thundra_cmd = "pip install --target=%s thundra==%s --no-warn-conflicts" % (
-                THUNDRA_PYTHON_AGENT_LOCAL_PATH,
-                THUNDRA_PYTHON_AGENT_VERSION,
+            if numeric_filter[idx] == ">" and not (record_value > float(numeric_filter[idx + 1])):
+                return False
+            if numeric_filter[idx] == ">=" and not (record_value >= float(numeric_filter[idx + 1])):
+                return False
+            if numeric_filter[idx] == "=" and not (record_value == float(numeric_filter[idx + 1])):
+                return False
+            if numeric_filter[idx] == "<" and not (record_value < float(numeric_filter[idx + 1])):
+                return False
+            if numeric_filter[idx] == "<=" and not (record_value <= float(numeric_filter[idx + 1])):
+                return False
+        except ValueError:
+            LOG.warn(
+                f"Could not convert filter value {numeric_filter[idx + 1]} to a valid number value for filtering"
             )
-            common.run(install_thundra_cmd.split())
-        except Exception as e:
-            print("Unable to install Thundra Python agent: %s" % e)
-            return False
     return True
 
 
-def _is_python_lambda_with_support_version(func_details):
-    runtime = getattr(func_details, "runtime", func_details)
-    return runtime in [
-        LAMBDA_RUNTIME_PYTHON37,
-        LAMBDA_RUNTIME_PYTHON38,
-    ]
-
-
-def _prepare_invocation_for_python_lambda(
-    context: InvocationContext,
-) -> AdditionalInvocationOptions:
-    # Download and initialize Python agent
-    _ensure_python_agent_initialized()
-
-    # If agent could not be initialized, skip here
-    if not THUNDRA_PYTHON_AGENT_INITIALIZED:
-        return None
-
-    result = AdditionalInvocationOptions()
-
-    # Make sure API key is contained in environment
-    result.env_updates[THUNDRA_APIKEY_ENV_VAR_NAME] = _get_apikey(context.environment)
-
-    # Switch handler to Thundra and pass original handler to Thundra through environment variable
-    result.env_updates[THUNDRA_AGENT_LAMBDA_HANDLER_ENV_VAR_NAME] = context.handler
-    result.updated_handler = "thundra.handler.wrapper"
-
-    # If log disable is not configured explicitly, set it to false to enable log capturing by default
-    log_disabled = context.environment.get(THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME)
-    if not log_disabled:
-        result.env_updates[THUNDRA_AGENT_LOG_DISABLE_ENV_VAR_NAME] = "false"
-
-    # Map Thundra agent path into container so it will be accessible by Lambda function Python environment
-    agent_path_mapping = "-v %s/:/opt/python/" % THUNDRA_PYTHON_AGENT_LOCAL_PATH_ON_HOST
-
-    if context.docker_flags:
-        context.docker_flags = f"{context.docker_flags} {agent_path_mapping}"
-    else:
-        context.docker_flags = agent_path_mapping
-
-    return result
-
-
-################
-# THUNDRA PLUGIN
-################
-
+def verify_dict_filter(record_value: any, dict_filter: Dict[str, any]) -> bool:
+    # https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html#filtering-syntax
+    fits_filter = False
+    for key, filter_value in dict_filter.items():
+        if key.lower() == "anything-but":
+            fits_filter = record_value not in filter_value
+        elif key.lower() == "numeric":
+            fits_filter = parse_and_apply_numeric_filter(record_value, filter_value)
+        elif key.lower() == "exists":
+            fits_filter = bool(filter_value)  # exists means that the key exists in the event record
+        elif key.lower() == "prefix":
+            if not isinstance(record_value, str):
+                LOG.warn(f"Record Value {record_value} does not seem to be a valid string.")
+            fits_filter = isinstance(record_value, str) and record_value.startswith(
+                str(filter_value)
+            )
 
-class LambdaExecutorPluginThundra(LambdaExecutorPlugin):
-    def should_apply(self, context: InvocationContext) -> bool:
-        # Local executor is not supported yet
-        if "local" in get_executor_mode():
-            return False
+        if fits_filter:
+            return True
+    return fits_filter
 
-        # Plugin can only be applied if LAMBDA_REMOTE_DOCKER=0
-        if "docker" in get_executor_mode() and config.LAMBDA_REMOTE_DOCKER:
-            return False
 
-        # Plugin can only applied if API key is configured
-        thundra_apikey = _get_apikey(context.environment)
-        if not thundra_apikey:
+def filter_stream_record(filter_rule: Dict[str, any], record: Dict[str, any]) -> bool:
+    if not filter_rule:
+        return True
+    # https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html#filtering-syntax
+    filter_results = []
+    for key, value in filter_rule.items():
+        # check if rule exists in event
+        record_value = (
+            record.get(key.lower(), record.get(key)) if isinstance(record, Dict) else None
+        )
+        append_record = False
+        if record_value is not None:
+            # check if filter rule value is a list (leaf of rule tree) or a dict (rescursively call function)
+            if isinstance(value, list):
+                if len(value) > 0:
+                    if isinstance(value[0], (str, int)):
+                        append_record = record_value in value
+                    if isinstance(value[0], dict):
+                        append_record = verify_dict_filter(record_value, value[0])
+                else:
+                    LOG.warn(f"Empty lambda filter: {key}")
+            elif isinstance(value, dict):
+                append_record = filter_stream_record(value, record_value)
+        else:
+            # special case 'exists'
+            if isinstance(value, list) and len(value) > 0:
+                append_record = not value[0].get("exists", True)
+
+        filter_results.append(append_record)
+    return all(filter_results)
+
+
+def filter_stream_records(records, filters: List[FilterCriteria]):
+    filtered_records = []
+    for record in records:
+        for filter in filters:
+            for rule in filter["Filters"]:
+                if filter_stream_record(json.loads(rule["Pattern"]), record):
+                    filtered_records.append(record)
+                    break
+    return filtered_records
+
+
+def contains_list(filter: Dict) -> bool:
+    if isinstance(filter, dict):
+        for key, value in filter.items():
+            if isinstance(value, list) and len(value) > 0:
+                return True
+            return contains_list(value)
+    return False
+
+
+def validate_filters(filter: FilterCriteria) -> bool:
+    # filter needs to be json serializeable
+    for rule in filter["Filters"]:
+        try:
+            if not (filter_pattern := json.loads(rule["Pattern"])):
+                return False
+            return contains_list(filter_pattern)
+        except json.JSONDecodeError:
             return False
+    # needs to contain on what to filter (some list with citerias)
+    # https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html#filtering-syntax
 
-        # Plugin can be applied for Java Lambdas with supported versions
-        if _is_java_lambda_with_support_version(context.lambda_function.runtime):
-            return True
+    return True
 
-        # Plugin can be applied for Node Lambdas with supported versions
-        if _is_node_lambda_with_support_version(context.lambda_function.runtime):
-            return True
 
-        # Plugin can be applied for Python Lambdas with supported versions
-        if _is_python_lambda_with_support_version(context.lambda_function.runtime):
-            return True
+def function_name_from_arn(arn: str):
+    """Extract a function name from a arn/function name"""
+    return FUNCTION_NAME_REGEX.match(arn).group("name")
+
+
+def get_awslambda_store(
+    account_id: Optional[str] = None, region: Optional[str] = None
+) -> AwsLambdaStore:
+    """Get the legacy Lambda store."""
+    account_id = account_id or get_aws_account_id()
+    region = region or aws_stack.get_region()
+
+    return awslambda_stores[account_id][region]
+
+
+def get_awslambda_store_for_arn(resource_arn: str) -> AwsLambdaStore:
+    """
+    Return the store for the region extracted from the given resource ARN.
+    """
+    return get_awslambda_store(
+        account_id=extract_account_id_from_arn(resource_arn or ""),
+        region=extract_region_from_arn(resource_arn or ""),
+    )
 
-        # Not applicable for Thundra plugin
-        return False
 
-    def prepare_invocation(
-        self, context: InvocationContext
-    ) -> Optional[Union[AdditionalInvocationOptions, InvocationResult]]:
-        if is_java_lambda(context.lambda_function):
-            return _prepare_invocation_for_java_lambda(context)
-        elif is_nodejs_runtime(context.lambda_function):
-            return _prepare_invocation_for_node_lambda(context)
-        elif is_python_runtime(context.lambda_function):
-            return _prepare_invocation_for_python_lambda(context)
-        return None
+def message_attributes_to_lower(message_attrs):
+    """Convert message attribute details (first characters) to lower case (e.g., stringValue, dataType)."""
+    message_attrs = message_attrs or {}
+    for _, attr in message_attrs.items():
+        if not isinstance(attr, dict):
+            continue
+        for key, value in dict(attr).items():
+            attr[first_char_to_lower(key)] = attr.pop(key)
+    return message_attrs
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230529184621/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230529184621/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/request.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/response.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/http/router.py` & `localstack-core-2.1.1.dev20230529184621/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230529184621/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230529184621/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230529184621/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230529184621/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230529184621/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230529184621/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230529184621/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/plugins.py` & `localstack-core-2.1.1.dev20230529184621/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230529184621/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230529184621/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230529184621/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230529184621/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230529184621/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/helpers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/invocations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -2420,17 +2420,14 @@
 def serve(port):
     try:
         # initialize the Lambda executor
         LAMBDA_EXECUTOR.startup()
         # print warnings for potentially incorrect config options
         validate_lambda_config()
 
-        # initialize/import plugins - TODO find better place to import plugins! (to be integrated into proper plugin model)
-        import localstack.contrib.thundra  # noqa
-
         _serve_flask_app(app=app, port=port)
     except Exception:
         LOG.exception("Error while starting up lambda service")
         raise
 
 
 def _serve_flask_app(app, port, host=None, cors=True, asynchronous=False):
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/collections.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,455 +1,505 @@
-import base64
-import json
+"""
+This package provides custom collection types, as well as tools to analyze
+and manipulate python collection (dicts, list, sets).
+"""
+
 import logging
-import os
 import re
-import tempfile
-import time
-from functools import lru_cache
-from io import BytesIO
-from typing import Any, Dict, List, Optional, Union
-
-from flask import Response
-
-from localstack import config
-from localstack.aws.accounts import get_aws_account_id
-from localstack.aws.api.lambda_ import FilterCriteria, Runtime
-from localstack.aws.connect import connect_to
-from localstack.services.awslambda.lambda_models import AwsLambdaStore, awslambda_stores
-from localstack.utils.aws import aws_stack
-from localstack.utils.aws.arns import extract_account_id_from_arn, extract_region_from_arn
-from localstack.utils.aws.aws_models import LambdaFunction
-from localstack.utils.aws.aws_responses import flask_error_response_json
-from localstack.utils.container_networking import (
-    get_endpoint_for_network,
-    get_main_container_network,
+import sys
+from collections.abc import Mapping
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Sized,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
 )
-from localstack.utils.docker_utils import DOCKER_CLIENT
-from localstack.utils.strings import first_char_to_lower, short_uid
 
-LOG = logging.getLogger(__name__)
-# Custom logger for proactive deprecation hints related to the migration from the old to the new lambda provider
-HINT_LOG = logging.getLogger("localstack.services.awslambda.hints")
+import cachetools
 
-# root path of Lambda API endpoints
-API_PATH_ROOT = "/2015-03-31"
-API_PATH_ROOT_2 = "/2021-10-31"
+if sys.version_info >= (3, 8):
+    from typing import TypedDict, get_args, get_origin
+else:
+    from typing_extensions import TypedDict, get_args, get_origin
 
 
-# Lambda runtime constants (LEGACY, use values in Runtime class instead)
-LAMBDA_RUNTIME_PYTHON37 = Runtime.python3_7
-LAMBDA_RUNTIME_PYTHON38 = Runtime.python3_8
-LAMBDA_RUNTIME_PYTHON39 = Runtime.python3_9
-LAMBDA_RUNTIME_NODEJS = Runtime.nodejs
-LAMBDA_RUNTIME_NODEJS12X = Runtime.nodejs12_x
-LAMBDA_RUNTIME_NODEJS14X = Runtime.nodejs14_x
-LAMBDA_RUNTIME_NODEJS16X = Runtime.nodejs16_x
-LAMBDA_RUNTIME_JAVA8 = Runtime.java8
-LAMBDA_RUNTIME_JAVA8_AL2 = Runtime.java8_al2
-LAMBDA_RUNTIME_JAVA11 = Runtime.java11
-LAMBDA_RUNTIME_DOTNETCORE31 = Runtime.dotnetcore3_1
-LAMBDA_RUNTIME_DOTNET6 = Runtime.dotnet6
-LAMBDA_RUNTIME_GOLANG = Runtime.go1_x
-LAMBDA_RUNTIME_RUBY27 = Runtime.ruby2_7
-LAMBDA_RUNTIME_PROVIDED = Runtime.provided
-LAMBDA_RUNTIME_PROVIDED_AL2 = Runtime.provided_al2
+LOG = logging.getLogger(__name__)
 
 
-# default handler and runtime
-LAMBDA_DEFAULT_HANDLER = "handler.handler"
-LAMBDA_DEFAULT_RUNTIME = LAMBDA_RUNTIME_PYTHON39  # FIXME (?)
-LAMBDA_DEFAULT_STARTING_POSITION = "LATEST"
+class AccessTrackingDict(dict):
+    """
+    Simple utility class that can be used to track (write) accesses to a dict's attributes.
+    Note: could also be written as a proxy, to preserve the identity of "wrapped" - for now, it
+          simply duplicates the entries of "wrapped" in the constructor, for simplicity.
+    """
 
-# List of Dotnet Lambda runtime names
-DOTNET_LAMBDA_RUNTIMES = [
-    LAMBDA_RUNTIME_DOTNETCORE31,
-    LAMBDA_RUNTIME_DOTNET6,
-]
+    def __init__(self, wrapped, callback: Callable[[Dict, str, List, Dict], Any] = None):
+        super().__init__(wrapped)
+        self.callback = callback
 
-# IP address of main Docker container (lazily initialized)
-DOCKER_MAIN_CONTAINER_IP = None
-LAMBDA_CONTAINER_NETWORK = None
+    def __setitem__(self, key, value):
+        self.callback and self.callback(self, "__setitem__", [key, value], {})
+        return super().__setitem__(key, value)
 
-FUNCTION_NAME_REGEX = re.compile(
-    r"(arn:(aws[a-zA-Z-]*)?:lambda:)?((?P<region>[a-z]{2}(-gov)?-[a-z]+-\d{1}):)?(?P<account>\d{12}:)?(function:)?(?P<name>[a-zA-Z0-9-_\.]+)(:(?P<qualifier>\$LATEST|[a-zA-Z0-9-_]+))?"
-)  # also length 1-170 incl.
 
+class DelSafeDict(dict):
+    """Useful when applying jsonpatch. Use it as follows:
 
-class ClientError(Exception):
-    def __init__(self, msg, code=400):
-        super(ClientError, self).__init__(msg)
-        self.code = code
-        self.msg = msg
+    obj.__dict__ = DelSafeDict(obj.__dict__)
+    apply_patch(obj.__dict__, patch)
+    """
 
-    def get_response(self):
-        if isinstance(self.msg, Response):
-            return self.msg
-        return error_response(self.msg, self.code)
+    def __delitem__(self, key, *args, **kwargs):
+        self[key] = None
 
 
-@lru_cache()
-def get_default_executor_mode() -> str:
+class ImmutableList(tuple):
     """
-    Returns the default docker executor mode, which is "docker" if the docker socket is available via the docker
-    client, or "local"  otherwise.
-
-    :return: 'docker' if docker socket available, otherwise 'local'
+    Wrapper class to create an immutable view of a given list or sequence.
+    Note: Currently, this is simply a wrapper around `tuple` - could be replaced with
+    custom implementations over time, if needed.
     """
-    try:
-        return "docker" if DOCKER_CLIENT.has_docker() else "local"
-    except Exception:
-        return "local"
 
 
-def get_executor_mode() -> str:
-    """
-    Returns the currently active lambda executor mode. If config.LAMBDA_EXECUTOR is set, then it returns that,
-    otherwise it falls back to get_default_executor_mode().
+class HashableList(ImmutableList):
+    """Hashable, immutable list wrapper that can be used with dicts or hash sets."""
+
+    def __hash__(self):
+        return sum(hash(i) for i in self)
 
-    :return: the lambda executor mode (e.g., 'local', 'docker', or 'docker-reuse')
-    """
-    return config.LAMBDA_EXECUTOR or get_default_executor_mode()
 
+class ImmutableDict(Mapping):
+    """Wrapper class to create an immutable view of a given list or sequence."""
 
-def get_lambda_runtime(runtime_details: Union[LambdaFunction, str]) -> str:
-    """Return the runtime string from the given LambdaFunction (or runtime string)."""
-    if isinstance(runtime_details, LambdaFunction):
-        runtime_details = runtime_details.runtime
-    if not isinstance(runtime_details, str):
-        LOG.info("Unable to determine Lambda runtime from parameter: %s", runtime_details)
-    return runtime_details or ""
+    def __init__(self, seq=None, **kwargs):
+        self._dict = dict(seq, **kwargs)
 
+    def __len__(self) -> int:
+        return self._dict.__len__()
 
-def is_provided_runtime(runtime_details: Union[LambdaFunction, str]) -> bool:
-    """Whether the given LambdaFunction uses a 'provided' runtime."""
-    runtime = get_lambda_runtime(runtime_details) or ""
-    return runtime.startswith("provided")
+    def __iter__(self) -> Iterator:
+        return self._dict.__iter__()
 
+    def __getitem__(self, key):
+        return self._dict.__getitem__(key)
 
-def format_name_to_path(handler_name: str, delimiter: str, extension: str):
-    file_path = handler_name.rpartition(delimiter)[0]
-    if delimiter == ":":
-        file_path = file_path.split(delimiter)[0]
+    def __eq__(self, other):
+        return self._dict.__eq__(other._dict if isinstance(other, ImmutableDict) else other)
 
-    if os.path.sep not in file_path:
-        file_path = file_path.replace(".", os.path.sep)
+    def __str__(self):
+        return self._dict.__str__()
 
-    if file_path.startswith(f".{os.path.sep}"):
-        file_path = file_path[2:]
 
-    return f"{file_path}{extension}"
+class HashableJsonDict(ImmutableDict):
+    """
+    Simple dict wrapper that can be used with dicts or hash sets. Note: the assumption is that the dict
+    can be JSON-encoded (i.e., must be acyclic and contain only lists/dicts and simple types)
+    """
+
+    def __hash__(self):
+        from localstack.utils.json import canonical_json
+
+        return hash(canonical_json(self._dict))
+
 
+_ListType = TypeVar("_ListType")
 
-def get_handler_file_from_name(handler_name: str, runtime: str = None):
-    runtime = runtime or LAMBDA_DEFAULT_RUNTIME
 
-    if runtime.startswith(LAMBDA_RUNTIME_PROVIDED):
-        return "bootstrap"
-    if runtime.startswith("nodejs"):
-        return format_name_to_path(handler_name, ".", ".js")
-    if runtime.startswith(LAMBDA_RUNTIME_GOLANG):
-        return handler_name
-    if runtime.startswith(tuple(DOTNET_LAMBDA_RUNTIMES)):
-        return format_name_to_path(handler_name, ":", ".dll")
-    if runtime.startswith("ruby"):
-        return format_name_to_path(handler_name, ".", ".rb")
+class PaginatedList(List[_ListType]):
+    """List which can be paginated and filtered. For usage in AWS APIs with paginated responses"""
 
-    return format_name_to_path(handler_name, ".", ".py")
+    DEFAULT_PAGE_SIZE = 50
 
+    def get_page(
+        self,
+        token_generator: Callable[[_ListType], str],
+        next_token: str = None,
+        page_size: int = None,
+        filter_function: Callable[[_ListType], bool] = None,
+    ) -> Tuple[List[_ListType], Optional[str]]:
+        if filter_function is not None:
+            result_list = list(filter(filter_function, self))
+        else:
+            result_list = self
 
-def is_java_lambda(lambda_details):
-    runtime = getattr(lambda_details, "runtime", lambda_details)
-    return runtime in [LAMBDA_RUNTIME_JAVA8, LAMBDA_RUNTIME_JAVA8_AL2, LAMBDA_RUNTIME_JAVA11]
+        if page_size is None:
+            page_size = self.DEFAULT_PAGE_SIZE
 
+        if len(result_list) <= page_size:
+            return result_list, None
 
-def is_nodejs_runtime(lambda_details):
-    runtime = getattr(lambda_details, "runtime", lambda_details) or ""
-    return runtime.startswith("nodejs")
+        start_idx = 0
 
+        try:
+            start_item = next(item for item in result_list if token_generator(item) == next_token)
+            start_idx = result_list.index(start_item)
+        except StopIteration:
+            pass
 
-def is_python_runtime(lambda_details):
-    runtime = getattr(lambda_details, "runtime", lambda_details) or ""
-    return runtime.startswith("python")
+        if start_idx + page_size < len(result_list):
+            next_token = token_generator(result_list[start_idx + page_size])
+        else:
+            next_token = None
 
+        return result_list[start_idx : start_idx + page_size], next_token
 
-def store_lambda_logs(
-    lambda_function: LambdaFunction, log_output: str, invocation_time=None, container_id=None
-):
-    # leave here to avoid import issues from CLI
-    from localstack.utils.cloudwatch.cloudwatch_util import store_cloudwatch_logs
 
-    log_group_name = "/aws/lambda/%s" % lambda_function.name()
-    container_id = container_id or short_uid()
-    invocation_time = invocation_time or int(time.time() * 1000)
-    invocation_time_secs = int(invocation_time / 1000)
-    time_str = time.strftime("%Y/%m/%d", time.gmtime(invocation_time_secs))
-    log_stream_name = "%s/[LATEST]%s" % (time_str, container_id)
-    return store_cloudwatch_logs(log_group_name, log_stream_name, log_output, invocation_time)
+class CustomExpiryTTLCache(cachetools.TTLCache):
+    """TTLCache that allows to set custom expiry times for individual keys."""
 
+    def set_expiry(self, key: Any, ttl: Union[float, int]) -> float:
+        """Set the expiry of the given key in a TTLCache to (<current_time> + <ttl>)"""
+        with self.timer as time:
+            # note: need to access the internal dunder API here
+            self._TTLCache__getlink(key).expires = expiry = time + ttl
+            return expiry
 
-def get_main_endpoint_from_container() -> str:
-    if config.HOSTNAME_FROM_LAMBDA:
-        return config.HOSTNAME_FROM_LAMBDA
-    return get_endpoint_for_network(network=get_container_network_for_lambda())
 
+def get_safe(dictionary, path, default_value=None):
+    """
+    Performs a safe navigation on a Dictionary object and
+    returns the result or default value (if specified).
+    The function follows a common AWS path resolution pattern "$.a.b.c".
+
+    :type dictionary: dict
+    :param dictionary: Dict to perform safe navigation.
+
+    :type path: list|str
+    :param path: List or dot-separated string containing the path of an attribute,
+                 starting from the root node "$".
+
+    :type default_value: any
+    :param default_value: Default value to return in case resolved value is None.
 
-def get_container_network_for_lambda() -> str:
-    global LAMBDA_CONTAINER_NETWORK
-    if config.LAMBDA_DOCKER_NETWORK:
-        return config.LAMBDA_DOCKER_NETWORK
-    return get_main_container_network()
+    :rtype: any
+    :return: Resolved value or default_value.
+    """
+    if not isinstance(dictionary, dict) or len(dictionary) == 0:
+        return default_value
 
+    attribute_path = path if isinstance(path, list) else path.split(".")
+    if len(attribute_path) == 0 or attribute_path[0] != "$":
+        raise AttributeError('Safe navigation must begin with a root node "$"')
+
+    current_value = dictionary
+    for path_node in attribute_path:
+        if path_node == "$":
+            continue
 
-def rm_docker_container(container_name_or_id, check_existence=False, safe=False):
-    # TODO: remove method / move to docker module
-    if not container_name_or_id:
-        return
-    if check_existence and container_name_or_id not in DOCKER_CLIENT.get_running_container_names():
-        # TODO: check names as well as container IDs!
-        return
-    try:
-        DOCKER_CLIENT.remove_container(container_name_or_id)
-    except Exception:
-        if not safe:
-            raise
+        if re.compile("^\\d+$").search(str(path_node)):
+            path_node = int(path_node)
 
+        if isinstance(current_value, dict) and path_node in current_value:
+            current_value = current_value[path_node]
+        elif isinstance(current_value, list) and path_node < len(current_value):
+            current_value = current_value[path_node]
+        else:
+            current_value = None
 
-def get_record_from_event(event: Dict, key: str) -> Any:
-    """Retrieve a field with the given key from the list of Records within 'event'."""
-    try:
-        return event["Records"][0][key]
-    except KeyError:
-        return None
+    return current_value or default_value
 
 
-def get_lambda_extraction_dir() -> str:
+def set_safe_mutable(dictionary, path, value):
     """
-    Get the directory a lambda is supposed to use as working directory (= the directory to extract the contents to).
-    This method is needed due to performance problems for IO on bind volumes when running inside Docker Desktop, due to
-    the file sharing with the host being slow when using gRPC-FUSE.
-    By extracting to a not-mounted directory, we can improve performance significantly.
-    The lambda zip file itself, however, should still be located on the mount.
+    Mutates original dict and sets the specified value under provided path.
+
+    :type dictionary: dict
+    :param dictionary: Dict to mutate.
+
+    :type path: list|str
+    :param path: List or dot-separated string containing the path of an attribute,
+                 starting from the root node "$".
 
-    :return: directory path
+    :type value: any
+    :param value: Value to set under specified path.
+
+    :rtype: dict
+    :return: Returns mutated dictionary.
     """
-    if config.LAMBDA_REMOTE_DOCKER:
-        return tempfile.gettempdir()
-    return config.dirs.tmp
+    if not isinstance(dictionary, dict):
+        raise AttributeError('"dictionary" must be of type "dict"')
+
+    attribute_path = path if isinstance(path, list) else path.split(".")
+    attribute_path_len = len(attribute_path)
+
+    if attribute_path_len == 0 or attribute_path[0] != "$":
+        raise AttributeError('Dict navigation must begin with a root node "$"')
+
+    current_pointer = dictionary
+    for i in range(attribute_path_len):
+        path_node = attribute_path[i]
+
+        if path_node == "$":
+            continue
+
+        if i < attribute_path_len - 1:
+            if path_node not in current_pointer:
+                current_pointer[path_node] = {}
+            if not isinstance(current_pointer, dict):
+                raise RuntimeError(
+                    'Error while deeply setting a dict value. Supplied path is not of type "dict"'
+                )
+        else:
+            current_pointer[path_node] = value
 
+        current_pointer = current_pointer[path_node]
 
-def get_zip_bytes(function_code):
-    """Returns the ZIP file contents from a FunctionCode dict.
+    return dictionary
 
-    :type function_code: dict
-    :param function_code: https://docs.aws.amazon.com/lambda/latest/dg/API_FunctionCode.html
-    :returns: bytes of the Zip file.
+
+def pick_attributes(dictionary, paths):
     """
-    function_code = function_code or {}
-    if "S3Bucket" in function_code:
-        s3_client = connect_to().s3
-        bytes_io = BytesIO()
-        try:
-            s3_client.download_fileobj(function_code["S3Bucket"], function_code["S3Key"], bytes_io)
-            zip_file_content = bytes_io.getvalue()
-        except Exception as e:
-            s3_key = str(function_code.get("S3Key") or "")
-            s3_url = f's3://{function_code["S3Bucket"]}{s3_key if s3_key.startswith("/") else f"/{s3_key}"}'
-            raise ClientError(f"Unable to fetch Lambda archive from {s3_url}: {e}", 404)
-    elif "ZipFile" in function_code:
-        zip_file_content = function_code["ZipFile"]
-        zip_file_content = base64.b64decode(zip_file_content)
-    elif "ImageUri" in function_code:
-        zip_file_content = None
-    else:
-        raise ClientError("No valid Lambda archive specified: %s" % list(function_code.keys()))
-    return zip_file_content
+    Picks selected attributes a returns them as a new dictionary.
+    This function works as a whitelist of attributes to keep in a new dictionary.
 
+    :type dictionary: dict
+    :param dictionary: Dict to pick attributes from.
 
-def event_source_arn_matches(mapped: str, searched: str) -> bool:
-    if not mapped:
-        return False
-    if not searched or mapped == searched:
-        return True
-    # Some types of ARNs can end with a path separated by slashes, for
-    # example the ARN of a DynamoDB stream is tableARN/stream/ID. It's
-    # a little counterintuitive that a more specific mapped ARN can
-    # match a less specific ARN on the event, but some integration tests
-    # rely on it for things like subscribing to a stream and matching an
-    # event labeled with the table ARN.
-    if re.match(r"^%s$" % searched, mapped):
-        return True
-    if mapped.startswith(searched):
-        suffix = mapped[len(searched) :]
-        return suffix[0] == "/"
-    return False
-
-
-def error_response(msg, code=500, error_type="InternalFailure"):
-    if code != 404:
-        LOG.debug(msg)
-    return flask_error_response_json(msg, code=code, error_type=error_type)
-
-
-def generate_lambda_arn(
-    account_id: int, region: str, fn_name: str, qualifier: Optional[str] = None
-):
-    if qualifier:
-        return f"arn:aws:lambda:{region}:{account_id}:function:{fn_name}:{qualifier}"
-    else:
-        return f"arn:aws:lambda:{region}:{account_id}:function:{fn_name}"
-
-
-def parse_and_apply_numeric_filter(
-    record_value: Dict, numeric_filter: List[Union[str, int]]
-) -> bool:
-    if len(numeric_filter) % 2 > 0:
-        LOG.warn("Invalid numeric lambda filter given")
-        return True
+    :type paths: list of (list or str)
+    :param paths: List of lists or strings with dot-separated paths, starting from the root node "$".
 
-    if not isinstance(record_value, (int, float)):
-        LOG.warn(f"Record {record_value} seem not to be a valid number")
-        return False
+    :rtype: dict
+    :return: Returns whitelisted dictionary.
+    """
+    new_dictionary = {}
 
-    for idx in range(0, len(numeric_filter), 2):
+    for path in paths:
+        value = get_safe(dictionary, path)
 
-        try:
-            if numeric_filter[idx] == ">" and not (record_value > float(numeric_filter[idx + 1])):
-                return False
-            if numeric_filter[idx] == ">=" and not (record_value >= float(numeric_filter[idx + 1])):
-                return False
-            if numeric_filter[idx] == "=" and not (record_value == float(numeric_filter[idx + 1])):
-                return False
-            if numeric_filter[idx] == "<" and not (record_value < float(numeric_filter[idx + 1])):
-                return False
-            if numeric_filter[idx] == "<=" and not (record_value <= float(numeric_filter[idx + 1])):
-                return False
-        except ValueError:
-            LOG.warn(
-                f"Could not convert filter value {numeric_filter[idx + 1]} to a valid number value for filtering"
-            )
-    return True
+        if value is not None:
+            set_safe_mutable(new_dictionary, path, value)
 
+    return new_dictionary
 
-def verify_dict_filter(record_value: any, dict_filter: Dict[str, any]) -> bool:
-    # https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html#filtering-syntax
-    fits_filter = False
-    for key, filter_value in dict_filter.items():
-        if key.lower() == "anything-but":
-            fits_filter = record_value not in filter_value
-        elif key.lower() == "numeric":
-            fits_filter = parse_and_apply_numeric_filter(record_value, filter_value)
-        elif key.lower() == "exists":
-            fits_filter = bool(filter_value)  # exists means that the key exists in the event record
-        elif key.lower() == "prefix":
-            if not isinstance(record_value, str):
-                LOG.warn(f"Record Value {record_value} does not seem to be a valid string.")
-            fits_filter = isinstance(record_value, str) and record_value.startswith(
-                str(filter_value)
-            )
-
-        if fits_filter:
-            return True
-    return fits_filter
-
-
-def filter_stream_record(filter_rule: Dict[str, any], record: Dict[str, any]) -> bool:
-    if not filter_rule:
-        return True
-    # https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html#filtering-syntax
-    filter_results = []
-    for key, value in filter_rule.items():
-        # check if rule exists in event
-        record_value = (
-            record.get(key.lower(), record.get(key)) if isinstance(record, Dict) else None
-        )
-        append_record = False
-        if record_value is not None:
-            # check if filter rule value is a list (leaf of rule tree) or a dict (rescursively call function)
-            if isinstance(value, list):
-                if len(value) > 0:
-                    if isinstance(value[0], (str, int)):
-                        append_record = record_value in value
-                    if isinstance(value[0], dict):
-                        append_record = verify_dict_filter(record_value, value[0])
-                else:
-                    LOG.warn(f"Empty lambda filter: {key}")
-            elif isinstance(value, dict):
-                append_record = filter_stream_record(value, record_value)
-        else:
-            # special case 'exists'
-            if isinstance(value, list) and len(value) > 0:
-                append_record = not value[0].get("exists", True)
-
-        filter_results.append(append_record)
-    return all(filter_results)
-
-
-def filter_stream_records(records, filters: List[FilterCriteria]):
-    filtered_records = []
-    for record in records:
-        for filter in filters:
-            for rule in filter["Filters"]:
-                if filter_stream_record(json.loads(rule["Pattern"]), record):
-                    filtered_records.append(record)
-                    break
-    return filtered_records
-
-
-def contains_list(filter: Dict) -> bool:
-    if isinstance(filter, dict):
-        for key, value in filter.items():
-            if isinstance(value, list) and len(value) > 0:
+
+def select_attributes(obj: Dict, attributes: List[str]) -> Dict:
+    """Select a subset of attributes from the given dict (returns a copy)"""
+    attributes = attributes if is_list_or_tuple(attributes) else [attributes]
+    return {k: v for k, v in obj.items() if k in attributes}
+
+
+def remove_attributes(obj: Dict, attributes: List[str], recursive: bool = False) -> Dict:
+    """Remove a set of attributes from the given dict (in-place)"""
+    from localstack.utils.objects import recurse_object
+
+    if recursive:
+
+        def _remove(o, **kwargs):
+            if isinstance(o, dict):
+                remove_attributes(o, attributes)
+            return o
+
+        return recurse_object(obj, _remove)
+
+    attributes = ensure_list(attributes)
+    for attr in attributes:
+        obj.pop(attr, None)
+    return obj
+
+
+def rename_attributes(
+    obj: Dict, old_to_new_attributes: Dict[str, str], in_place: bool = False
+) -> Dict:
+    """Rename a set of attributes in the given dict object. Second parameter is a dict that maps old to
+    new attribute names. Default is to return a copy, but can also pass in_place=True."""
+    if not in_place:
+        obj = dict(obj)
+    for old_name, new_name in old_to_new_attributes.items():
+        if old_name in obj:
+            obj[new_name] = obj.pop(old_name)
+    return obj
+
+
+def is_list_or_tuple(obj) -> bool:
+    return isinstance(obj, (list, tuple))
+
+
+def ensure_list(obj: Any, wrap_none=False) -> Optional[List]:
+    """Wrap the given object in a list, or return the object itself if it already is a list."""
+    if obj is None and not wrap_none:
+        return obj
+    return obj if isinstance(obj, list) else [obj]
+
+
+def to_unique_items_list(inputs, comparator=None):
+    """Return a list of unique items from the given input iterable.
+    The comparator(item1, item2) returns True/False or an int for comparison."""
+
+    def contained(item):
+        for r in result:
+            if comparator:
+                cmp_res = comparator(item, r)
+                if cmp_res is True or str(cmp_res) == "0":
+                    return True
+            elif item == r:
                 return True
-            return contains_list(value)
-    return False
 
+    result = []
+    for it in inputs:
+        if not contained(it):
+            result.append(it)
+    return result
 
-def validate_filters(filter: FilterCriteria) -> bool:
-    # filter needs to be json serializeable
-    for rule in filter["Filters"]:
-        try:
-            if not (filter_pattern := json.loads(rule["Pattern"])):
-                return False
-            return contains_list(filter_pattern)
-        except json.JSONDecodeError:
-            return False
-    # needs to contain on what to filter (some list with citerias)
-    # https://docs.aws.amazon.com/lambda/latest/dg/invocation-eventfiltering.html#filtering-syntax
 
+def merge_recursive(source, destination, none_values=None, overwrite=False):
+    if none_values is None:
+        none_values = [None]
+    for key, value in source.items():
+        if isinstance(value, dict):
+            # get node or create one
+            node = destination.setdefault(key, {})
+            merge_recursive(value, node, none_values=none_values, overwrite=overwrite)
+        else:
+            from requests.models import CaseInsensitiveDict
+
+            if not isinstance(destination, (dict, CaseInsensitiveDict)):
+                LOG.warning(
+                    "Destination for merging %s=%s is not dict: %s (%s)",
+                    key,
+                    value,
+                    destination,
+                    type(destination),
+                )
+            if overwrite or destination.get(key) in none_values:
+                destination[key] = value
+    return destination
+
+
+def merge_dicts(*dicts, **kwargs):
+    """Merge all dicts in `*dicts` into a single dict, and return the result. If any of the entries
+    in `*dicts` is None, and `default` is specified as keyword argument, then return `default`."""
+    result = {}
+    for d in dicts:
+        if d is None and "default" in kwargs:
+            return kwargs["default"]
+        if d:
+            result.update(d)
+    return result
+
+
+def remove_none_values_from_dict(dict: Dict) -> Dict:
+    return {k: v for (k, v) in dict.items() if v is not None}
+
+
+def last_index_of(array, value):
+    """Return the last index of `value` in the given list, or -1 if it does not exist."""
+    result = -1
+    for i in reversed(range(len(array))):
+        entry = array[i]
+        if entry == value or (callable(value) and value(entry)):
+            return i
+    return result
+
+
+def is_sub_dict(child_dict: Dict, parent_dict: Dict) -> bool:
+    """Returns whether the first dict is a sub-dict (subset) of the second dict."""
+    return all(parent_dict.get(key) == val for key, val in child_dict.items())
+
+
+def items_equivalent(list1, list2, comparator):
+    """Returns whether two lists are equivalent (i.e., same items contained in both lists,
+    irrespective of the items' order) with respect to a comparator function."""
+
+    def contained(item):
+        for _item in list2:
+            if comparator(item, _item):
+                return True
+
+    if len(list1) != len(list2):
+        return False
+    for item in list1:
+        if not contained(item):
+            return False
     return True
 
 
-def function_name_from_arn(arn: str):
-    """Extract a function name from a arn/function name"""
-    return FUNCTION_NAME_REGEX.match(arn).group("name")
+def is_none_or_empty(obj: Union[Optional[str], Optional[list]]) -> bool:
+    return (
+        obj is None
+        or (isinstance(obj, str) and obj.strip() == "")
+        or (isinstance(obj, Sized) and len(obj) == 0)
+    )
 
 
-def get_awslambda_store(
-    account_id: Optional[str] = None, region: Optional[str] = None
-) -> AwsLambdaStore:
-    """Get the legacy Lambda store."""
-    account_id = account_id or get_aws_account_id()
-    region = region or aws_stack.get_region()
+def select_from_typed_dict(typed_dict: Type[TypedDict], obj: Dict, filter: bool = False) -> Dict:
+    """
+    Select a subset of attributes from a dictionary based on the keys of a given `TypedDict`.
+    :param typed_dict: the `TypedDict` blueprint
+    :param obj: the object to filter
+    :param filter: if True, remove all keys with an empty (e.g., empty string or dictionary) or `None` value
+    :return: the resulting dictionary (it returns a copy)
+    """
+    selection = select_attributes(
+        obj, [*typed_dict.__required_keys__, *typed_dict.__optional_keys__]
+    )
+    if filter:
+        selection = {k: v for k, v in selection.items() if v}
+    return selection
+
 
-    return awslambda_stores[account_id][region]
+T = TypeVar("T", bound=Dict)
 
 
-def get_awslambda_store_for_arn(resource_arn: str) -> AwsLambdaStore:
+def convert_to_typed_dict(typed_dict: Type[T], obj: Dict, strict: bool = False) -> T:
     """
-    Return the store for the region extracted from the given resource ARN.
+    Converts the given object to the given typed dict (by calling the type constructors).
+    Limitations:
+    - This does not work for ForwardRefs (type refs in quotes).
+    - If a type is a Union, the first type is used for the conversion.
+    - The conversion fails for types which cannot be instantiated with the constructor.
+
+    :param typed_dict: to convert the given object to
+    :param obj: object to convert matching keys to the types defined in the typed dict
+    :param strict: True if a TypeError should be raised in case the conversion fails
+    :return: obj converted to the typed dict T
     """
-    return get_awslambda_store(
-        account_id=extract_account_id_from_arn(resource_arn or ""),
-        region=extract_region_from_arn(resource_arn or ""),
-    )
+    result = cast(T, select_from_typed_dict(typed_dict, obj, filter=True))
+    for key, key_type in typed_dict.__annotations__.items():
+        if key in result:
+            # If it's a Union, or optional, we extract the first type argument
+            if get_origin(key_type) in [Union, Optional]:
+                key_type = get_args(key_type)[0]
+            # Use duck-typing to check if the dict is a typed dict
+            if hasattr(key_type, "__required_keys__") and hasattr(key_type, "__optional_keys__"):
+                result[key] = convert_to_typed_dict(key_type, result[key])
+            else:
+                # Otherwise, we call the type's constructor (on a best-effort basis)
+                try:
+                    result[key] = key_type(result[key])
+                except TypeError as e:
+                    if strict:
+                        raise e
+                    else:
+                        LOG.debug("Could not convert %s to %s.", key, key_type)
+    return result
 
 
-def message_attributes_to_lower(message_attrs):
-    """Convert message attribute details (first characters) to lower case (e.g., stringValue, dataType)."""
-    message_attrs = message_attrs or {}
-    for _, attr in message_attrs.items():
-        if not isinstance(attr, dict):
-            continue
-        for key, value in dict(attr).items():
-            attr[first_char_to_lower(key)] = attr.pop(key)
-    return message_attrs
+def dict_multi_values(elements: Union[List, Dict]) -> Dict[str, List[Any]]:
+    """
+    Return a dictionary with the original keys from the list of dictionary and the
+    values are the list of values of the original dictionary.
+    """
+    result_dict = {}
+    if isinstance(elements, dict):
+        for key, value in elements.items():
+            if isinstance(value, list):
+                result_dict[key] = value
+            else:
+                result_dict[key] = [value]
+    elif isinstance(elements, list):
+        if isinstance(elements[0], list):
+            for key, value in elements:
+                if key in result_dict:
+                    result_dict[key].append(value)
+                else:
+                    result_dict[key] = [value]
+        else:
+            result_dict[elements[0]] = elements[1:]
+    return result_dict
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/packages.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230529184621/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/state/core.py` & `localstack-core-2.1.1.dev20230529184621/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230529184621/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230529184621/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230529184621/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230529184621/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230529184621/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230529183933
+Version: 2.1.1.dev20230529184621
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 localstack/cli/localstack.py
 localstack/cli/lpm.py
 localstack/cli/main.py
 localstack/cli/plugin.py
 localstack/cli/plugins.py
 localstack/cli/profiles.py
 localstack/contrib/__init__.py
-localstack/contrib/thundra.py
 localstack/extensions/__init__.py
 localstack/extensions/api/__init__.py
 localstack/extensions/api/aws.py
 localstack/extensions/api/extension.py
 localstack/extensions/api/http.py
 localstack/extensions/api/runtime.py
 localstack/extensions/api/services.py
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9383223684210527%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(3, '*

 * *                                      "'validate_configuration=localstack.services.awslambda.plugins:validate_configuration')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.packages'": '{insert: [(0, '*

 * *                          "'cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package'), "*

 * *                          '(1, '*

 * *                          "'stepfunctions-local/community=localstack […]*

```diff
@@ -53,36 +53,36 @@
         "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers",
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown"
     ],
     "localstack.hooks.on_infra_start": [
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
         "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
         "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "terraform/community=localstack.packages.plugins:terraform_package",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
+        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
         "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
         "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
         "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
-        "ffmpeg/community=localstack.services.transcribe.plugins:ffmpeg_package",
-        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package"
+        "terraform/community=localstack.packages.plugins:terraform_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230529183933/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230529184621/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/pyproject.toml` & `localstack-core-2.1.1.dev20230529184621/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230529183933/setup.cfg` & `localstack-core-2.1.1.dev20230529184621/setup.cfg`

 * *Files identical despite different names*

