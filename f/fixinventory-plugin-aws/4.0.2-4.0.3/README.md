# Comparing `tmp/fixinventory-plugin-aws-4.0.2.tar.gz` & `tmp/fixinventory_plugin_aws-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-aws-4.0.2.tar", last modified: Fri Apr 12 12:18:52 2024, max compression
+gzip compressed data, was "fixinventory_plugin_aws-4.0.3.tar", last modified: Wed Apr 24 10:33:35 2024, max compression
```

## Comparing `fixinventory-plugin-aws-4.0.2.tar` & `fixinventory_plugin_aws-4.0.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.286198 fixinventory-plugin-aws-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-12 12:18:52.286198 fixinventory-plugin-aws-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.270198 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (127)    31608 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.270198 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.278198 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/acm.py
--rw-r--r--   0 runner    (1001) docker     (127)    33155 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (127)    25343 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20225 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (127)    88117 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (127)    17752 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (127)    25355 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26450 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)   225895 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)   102274 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (127)    32936 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (127)    21508 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (127)    24841 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (127)    40921 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (127)    38170 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (127)    21081 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (127)    29715 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (127)    69161 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (127)    18123 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)   304012 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/secretsmanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30420 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ssm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73573 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/waf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/fix_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.286198 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-12 12:18:52.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-12 12:18:52.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:18:52.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 12:18:52.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:15:02.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 12:18:52.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 12:18:52.000000 fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 12:18:52.286198 fixinventory-plugin-aws-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.278198 fixinventory-plugin-aws-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:18:52.286198 fixinventory-plugin-aws-4.0.2/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/acm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/ecr_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/opensearch_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/secretsmanager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/ssm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/resources/waf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 12:14:39.000000 fixinventory-plugin-aws-4.0.2/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.203912 fixinventory_plugin_aws-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-24 10:33:35.203912 fixinventory_plugin_aws-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.183912 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (127)    31608 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14773 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.183912 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16203 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.191913 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/acm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33155 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12941 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20225 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88117 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17752 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25355 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14858 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26450 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)   225895 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102274 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22497 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32936 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21508 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24841 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40921 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14113 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38170 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21081 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29715 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69161 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14778 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18123 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)   304012 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/secretsmanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9958 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15648 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8131 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30420 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73573 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/waf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/fix_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.203912 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-24 10:33:35.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-24 10:33:35.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:35.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 10:33:35.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:29:40.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-24 10:33:35.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-24 10:33:35.000000 fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-24 10:33:35.203912 fixinventory_plugin_aws-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.195912 fixinventory_plugin_aws-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:35.203912 fixinventory_plugin_aws-4.0.3/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/acm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9820 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/ecr_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/opensearch_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/secretsmanager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/ssm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/resources/waf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-24 10:29:15.000000 fixinventory_plugin_aws-4.0.3/test/test_utils.py
```

### Comparing `fixinventory-plugin-aws-4.0.2/PKG-INFO` & `fixinventory_plugin_aws-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-aws
-Version: 4.0.2
+Version: 4.0.3
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/aws
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: fixinventorydata
 Requires-Dist: retrying
 Requires-Dist: boto3
 Requires-Dist: botocore
 
 # fix-plugin-aws
 An AWS collector plugin for Fix.
```

### Comparing `fixinventory-plugin-aws-4.0.2/README.md` & `fixinventory_plugin_aws-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/__init__.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/aws_client.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/aws_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 from functools import cached_property
-from itertools import islice
-from typing import Any, Callable, Dict, List, Optional, Set, TypeVar
+from typing import Any, Callable, List, Optional, TypeVar
 
-from attr import define, field
 from botocore.config import Config
 from botocore.exceptions import ClientError, EndpointConnectionError
 from botocore.model import ServiceModel
-from fix_plugin_aws.configuration import AwsConfig
 from retrying import retry
 
-from fixlib.core.actions import CoreFeedback
+from fix_plugin_aws.configuration import AwsConfig
+from fixlib.core.actions import ErrorAccumulator
 from fixlib.json import value_in_path
 from fixlib.types import Json, JsonElement
 from fixlib.utils import log_runtime, utc_str
-
 from .utils import global_region_by_partition
 
 log = logging.getLogger("fix.plugins.aws")
 
 ThrottlingErrors = {
     "EC2ThrottledException",
     "RequestThrottled",
@@ -45,75 +42,14 @@
 def is_retryable_exception(e: Exception) -> bool:
     if isinstance(e, ClientError) and e.response["Error"]["Code"] in RetryableErrors:
         log.debug("AWS API request limit exceeded or throttling, retrying with exponential backoff")
         return True
     return False
 
 
-@define
-class ErrorSummary:
-    error: str
-    message: str
-    info: bool
-    region: Optional[str] = None
-    service_actions: Dict[str, Set[str]] = field(factory=dict)
-
-
-class ErrorAccumulator:
-    def __init__(self) -> None:
-        self.regional_errors: Dict[Optional[str], Dict[str, ErrorSummary]] = {}
-
-    def add_error(
-        self,
-        as_info: bool,
-        error_kind: str,
-        service: str,
-        action: str,
-        message: str,
-        region: Optional[str],
-    ) -> None:
-        if region not in self.regional_errors:
-            self.regional_errors[region] = {}
-        regional_errors = self.regional_errors[region]
-
-        key = f"{error_kind}:{message}:{as_info}"
-        if key not in regional_errors:
-            regional_errors[key] = ErrorSummary(error_kind, message, as_info, region, {service: {action}})
-        else:
-            summary = regional_errors[key]
-            if service not in summary.service_actions:
-                summary.service_actions[service] = {action}
-            else:
-                summary.service_actions[service].add(action)
-
-    def report_region(self, core_feedback: CoreFeedback, region: Optional[str]) -> None:
-        if regional_errors := self.regional_errors.get(region):
-            # reset errors for this region
-            self.regional_errors[region] = {}
-            # add region as context
-            feedback = core_feedback.child_context(region) if region else core_feedback
-            # send to core
-            for err in regional_errors.values():
-                srv_acts = []
-                for aws_service, actions in islice(err.service_actions.items(), 10):
-                    suffix = " and more" if len(actions) > 3 else ""
-                    srv_acts.append(aws_service + ": " + ", ".join(islice(actions, 3)) + suffix)
-                message = f"[{err.error}] {err.message} Services and actions affected: {', '.join(srv_acts)}"
-                if len(err.service_actions) > 10:
-                    message += " and more..."
-                if err.info:
-                    feedback.info(message)
-                else:
-                    feedback.error(message)
-
-    def report_all(self, core_feedback: CoreFeedback) -> None:
-        for region in self.regional_errors.keys():
-            self.report_region(core_feedback, region)
-
-
 class AwsClient:
     def __init__(
         self,
         config: AwsConfig,
         account_id: str,
         *,
         role: Optional[str] = None,
```

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/collector.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from attrs import define
 from concurrent.futures import Future, ThreadPoolExecutor
 from typing import List, Type, Optional, ClassVar, Union
 from datetime import datetime, timezone
 
-from fix_plugin_aws.aws_client import AwsClient, ErrorAccumulator
+from fix_plugin_aws.aws_client import AwsClient
 from fix_plugin_aws.configuration import AwsConfig
 from fix_plugin_aws.resource import (
     apigateway,
     athena,
     autoscaling,
     cloudformation,
     cloudfront,
@@ -44,15 +44,15 @@
     opensearch,
     acm,
     waf,
 )
 from fix_plugin_aws.resource.base import AwsAccount, AwsApiSpec, AwsRegion, AwsResource, GraphBuilder
 
 from fixlib.baseresources import Cloud, EdgeType, BaseOrganizationalRoot, BaseOrganizationalUnit
-from fixlib.core.actions import CoreFeedback
+from fixlib.core.actions import CoreFeedback, ErrorAccumulator
 from fixlib.core.progress import ProgressDone, ProgressTree
 from fixlib.graph import Graph, BySearchCriteria, ByNodeId
 from fixlib.proc import set_thread_name
 from fixlib.threading import ExecutorQueue, GatherFutures
 from fixlib.types import Json
 from fixlib.json import value_in_path
```

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/configuration.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/configuration.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/acm.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/acm.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/apigateway.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/apigateway.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/athena.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/autoscaling.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/base.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from fixlib.graph import ByNodeId, BySearchCriteria, EdgeKey, Graph, NodeSelector
 from fixlib.json import from_json, value_in_path
 from fixlib.json_bender import Bender, bend
 from fixlib.lock import RWLock
 from fixlib.proc import set_thread_name
 from fixlib.threading import ExecutorQueue
 from fixlib.types import Json
-from fixinventorydata.cloud import instances as cloud_instance_data
+from fixinventorydata.cloud import instances as cloud_instance_data, regions as cloud_region_data
 
 log = logging.getLogger("fix.plugins.aws")
 
 
 def get_client(config: Config, resource: BaseResource) -> AwsClient:
     account = resource.account()
     assert isinstance(account, AwsAccount)
@@ -357,14 +357,20 @@
                 "aws_alb_target_group",
                 "aws_alb",
             ]
         }
     }
     ctime: Optional[datetime] = default_ctime
 
+    def __attrs_post_init__(self) -> None:
+        super().__attrs_post_init__()
+        self.long_name = cloud_region_data.get("aws", {}).get(self.id, {}).get("long_name")
+        self.latitude = cloud_region_data.get("aws", {}).get(self.id, {}).get("latitude")
+        self.longitude = cloud_region_data.get("aws", {}).get(self.id, {}).get("longitude")
+
 
 @define(eq=False, slots=False)
 class AwsEc2VolumeType(AwsResource, BaseVolumeType):
     kind: ClassVar[str] = "aws_ec2_volume_type"
     kind_display: ClassVar[str] = "AWS EC2 Volume Type"
     aws_metadata: ClassVar[Dict[str, Any]] = {"provider_link_tpl": None, "arn_tpl": "arn:{partition}:ec2:{region}:{account}:volume/{id}"}  # fmt: skip
     kind_description: ClassVar[str] = (
```

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudformation.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudformation.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudfront.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudtrail.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cloudwatch.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/cognito.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/cognito.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/config.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/dynamodb.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ec2.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ec2.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ecr.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ecr.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ecs.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ecs.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/efs.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/eks.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/eks.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elasticache.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elasticbeanstalk.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elb.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/elbv2.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/glacier.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/glacier.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/iam.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/iam.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/kinesis.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/kms.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/lambda_.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/opensearch.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/opensearch.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/pricing.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/pricing.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/rds.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/redshift.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/route53.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/route53.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/s3.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/sagemaker.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/sagemaker.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/secretsmanager.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/service_quotas.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/service_quotas.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/sns.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/sns.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/sqs.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/ssm.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/ssm.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/resource/waf.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/resource/waf.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fix_plugin_aws/utils.py` & `fixinventory_plugin_aws-4.0.3/fix_plugin_aws/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/PKG-INFO` & `fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-aws
-Version: 4.0.2
+Version: 4.0.3
 Summary: Runs collector plugins and sends the result to fixcore.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/aws
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: fixinventorydata
 Requires-Dist: retrying
 Requires-Dist: boto3
 Requires-Dist: botocore
 
 # fix-plugin-aws
 An AWS collector plugin for Fix.
```

### Comparing `fixinventory-plugin-aws-4.0.2/fixinventory_plugin_aws.egg-info/SOURCES.txt` & `fixinventory_plugin_aws-4.0.3/fixinventory_plugin_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/pyproject.toml` & `fixinventory_plugin_aws-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventory-plugin-aws"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Runs collector plugins and sends the result to fixcore."
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
     "fixinventorydata",
     "retrying",
     "boto3",
     "botocore",
 ]
 
 [project.entry-points."fix.plugins"]
```

### Comparing `fixinventory-plugin-aws-4.0.2/test/__init__.py` & `fixinventory_plugin_aws-4.0.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/aws_client_test.py` & `fixinventory_plugin_aws-4.0.3/test/aws_client_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Tuple
 
 from botocore.exceptions import ClientError
 
-from fix_plugin_aws.aws_client import AwsClient, ErrorAccumulator, is_retryable_exception
+from fix_plugin_aws.aws_client import AwsClient, is_retryable_exception
 from fix_plugin_aws.configuration import AwsConfig
+from fixlib.core.actions import ErrorAccumulator
 from test.resources import BotoFileBasedSession, BotoErrorSession
 
 
 def test_region() -> None:
     client = AwsClient(AwsConfig(), "test", role="test")
     east1 = client.for_region("us-east-1")
     assert client.account_id == east1.account_id
```

### Comparing `fixinventory-plugin-aws-4.0.2/test/collector_test.py` & `fixinventory_plugin_aws-4.0.3/test/collector_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/configuration_test.py` & `fixinventory_plugin_aws-4.0.3/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/graphbuilder_test.py` & `fixinventory_plugin_aws-4.0.3/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/__init__.py` & `fixinventory_plugin_aws-4.0.3/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/apigateway_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/athena_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/autoscaling_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/base_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/cloudformation_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/cloudfront_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/cloudtrail_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/cloudwatch_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/cognito_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/dynamodb_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/ec2_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/ecs_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/eks_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/elasticache_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/elasticbeanstalk_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/elb_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/elbv2_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/glacier_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/iam_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/kinesis_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/kms_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/lambda_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/pricing_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/rds_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/redshift_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/route53_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/s3_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/sagemaker_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/sagemaker_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/service_quotas_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/sns_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/sqs_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/sqs_test.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-aws-4.0.2/test/resources/ssm_test.py` & `fixinventory_plugin_aws-4.0.3/test/resources/ssm_test.py`

 * *Files identical despite different names*

