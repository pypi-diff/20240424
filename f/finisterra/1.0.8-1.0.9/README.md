# Comparing `tmp/finisterra-1.0.8.tar.gz` & `tmp/finisterra-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finisterra-1.0.8.tar", last modified: Wed Mar  6 10:53:03 2024, max compression
+gzip compressed data, was "finisterra-1.0.9.tar", last modified: Wed Mar  6 11:13:29 2024, max compression
```

## Comparing `finisterra-1.0.8.tar` & `finisterra-1.0.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.932765 finisterra-1.0.8/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    11357 2024-02-12 15:45:31.000000 finisterra-1.0.8/LICENSE
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     3473 2024-03-06 10:53:03.932479 finisterra-1.0.8/PKG-INFO
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     2928 2024-02-12 15:47:26.000000 finisterra-1.0.8/README.md
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.912169 finisterra-1.0.8/finisterra/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:05:33.000000 finisterra-1.0.8/finisterra/__init__.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    12437 2024-03-05 13:57:33.000000 finisterra-1.0.8/finisterra/main.py
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.913565 finisterra-1.0.8/finisterra/providers/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:16:08.000000 finisterra-1.0.8/finisterra/providers/__init__.py
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.929089 finisterra-1.0.8/finisterra/providers/aws/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    23620 2024-02-29 11:42:10.000000 finisterra-1.0.8/finisterra/providers/aws/Aws.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:16:11.000000 finisterra-1.0.8/finisterra/providers/aws/__init__.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     5843 2024-02-29 11:50:06.000000 finisterra-1.0.8/finisterra/providers/aws/acm.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    35131 2024-02-29 20:36:08.000000 finisterra-1.0.8/finisterra/providers/aws/apigateway.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    44984 2024-02-29 12:20:46.000000 finisterra-1.0.8/finisterra/providers/aws/aurora.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    19749 2024-02-29 12:20:51.000000 finisterra-1.0.8/finisterra/providers/aws/autoscaling.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     3534 2024-02-12 15:43:48.000000 finisterra-1.0.8/finisterra/providers/aws/aws_clients.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    21130 2024-02-29 12:20:56.000000 finisterra-1.0.8/finisterra/providers/aws/aws_lambda.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    27915 2024-02-29 12:21:02.000000 finisterra-1.0.8/finisterra/providers/aws/cloudfront.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    10895 2024-02-29 12:21:07.000000 finisterra-1.0.8/finisterra/providers/aws/cloudmap.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     8902 2024-02-29 12:21:11.000000 finisterra-1.0.8/finisterra/providers/aws/codeartifact.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    17466 2024-02-29 12:21:15.000000 finisterra-1.0.8/finisterra/providers/aws/docdb.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     9294 2024-02-29 12:21:19.000000 finisterra-1.0.8/finisterra/providers/aws/dynamodb.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    31121 2024-02-29 12:21:24.000000 finisterra-1.0.8/finisterra/providers/aws/ec2.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    12647 2024-02-29 12:21:28.000000 finisterra-1.0.8/finisterra/providers/aws/ecr.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    34981 2024-03-05 11:22:18.000000 finisterra-1.0.8/finisterra/providers/aws/ecs.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    18487 2024-02-29 12:21:36.000000 finisterra-1.0.8/finisterra/providers/aws/eks.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    12017 2024-02-29 12:21:40.000000 finisterra-1.0.8/finisterra/providers/aws/elasticache_redis.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    13638 2024-02-29 12:21:43.000000 finisterra-1.0.8/finisterra/providers/aws/elasticbeanstalk.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    10992 2024-02-29 12:21:48.000000 finisterra-1.0.8/finisterra/providers/aws/elasticsearch.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    13636 2024-02-29 12:21:51.000000 finisterra-1.0.8/finisterra/providers/aws/elbv2.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    25066 2024-02-29 12:21:58.000000 finisterra-1.0.8/finisterra/providers/aws/iam_policy.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     8196 2024-02-29 22:09:33.000000 finisterra-1.0.8/finisterra/providers/aws/iam_role.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    17100 2024-02-29 12:22:05.000000 finisterra-1.0.8/finisterra/providers/aws/kms.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     7295 2024-02-29 12:22:09.000000 finisterra-1.0.8/finisterra/providers/aws/launchtemplate.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    13777 2024-02-29 12:22:13.000000 finisterra-1.0.8/finisterra/providers/aws/logs.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    14301 2024-02-29 12:22:18.000000 finisterra-1.0.8/finisterra/providers/aws/msk.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    19354 2024-02-29 12:22:23.000000 finisterra-1.0.8/finisterra/providers/aws/rds.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    28857 2024-02-29 22:00:35.000000 finisterra-1.0.8/finisterra/providers/aws/s3.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     8610 2024-02-29 12:22:29.000000 finisterra-1.0.8/finisterra/providers/aws/security_group.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     8330 2024-02-29 12:22:33.000000 finisterra-1.0.8/finisterra/providers/aws/sns.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     8720 2024-02-29 12:22:36.000000 finisterra-1.0.8/finisterra/providers/aws/sqs.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     6661 2024-02-29 12:22:41.000000 finisterra-1.0.8/finisterra/providers/aws/stepfunction.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    10546 2024-02-29 12:22:45.000000 finisterra-1.0.8/finisterra/providers/aws/target_group.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     1328 2024-02-21 03:58:45.000000 finisterra-1.0.8/finisterra/providers/aws/utils.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    64949 2024-02-29 12:22:54.000000 finisterra-1.0.8/finisterra/providers/aws/vpc.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    15164 2024-02-29 20:59:32.000000 finisterra-1.0.8/finisterra/providers/aws/vpc_endpoint.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    12295 2024-02-29 12:22:58.000000 finisterra-1.0.8/finisterra/providers/aws/wafv2.py
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.930355 finisterra-1.0.8/finisterra/providers/cloudflare/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     1408 2024-02-29 11:43:15.000000 finisterra-1.0.8/finisterra/providers/cloudflare/Cloudflare.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-27 22:19:41.000000 finisterra-1.0.8/finisterra/providers/cloudflare/__init__.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)      111 2024-02-28 10:48:31.000000 finisterra-1.0.8/finisterra/providers/cloudflare/cf_clients.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     4660 2024-02-29 14:16:53.000000 finisterra-1.0.8/finisterra/providers/cloudflare/dns.py
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.931760 finisterra-1.0.8/finisterra/utils/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:16:15.000000 finisterra-1.0.8/finisterra/utils/__init__.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     3745 2024-03-01 23:09:44.000000 finisterra-1.0.8/finisterra/utils/auth.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     1819 2024-03-05 14:02:46.000000 finisterra-1.0.8/finisterra/utils/filesystem.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)    14098 2024-03-01 23:13:15.000000 finisterra-1.0.8/finisterra/utils/hcl.py
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     7299 2024-02-20 22:00:50.000000 finisterra-1.0.8/finisterra/utils/tf_plan.py
-drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 10:53:03.932142 finisterra-1.0.8/finisterra.egg-info/
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     3473 2024-03-06 10:53:03.000000 finisterra-1.0.8/finisterra.egg-info/PKG-INFO
--rw-r--r--   0 danieljaramillo   (501) staff       (20)     2005 2024-03-06 10:53:03.000000 finisterra-1.0.8/finisterra.egg-info/SOURCES.txt
--rw-r--r--   0 danieljaramillo   (501) staff       (20)        1 2024-03-06 10:53:03.000000 finisterra-1.0.8/finisterra.egg-info/dependency_links.txt
--rw-r--r--   0 danieljaramillo   (501) staff       (20)       52 2024-03-06 10:53:03.000000 finisterra-1.0.8/finisterra.egg-info/entry_points.txt
--rw-r--r--   0 danieljaramillo   (501) staff       (20)      143 2024-03-06 10:53:03.000000 finisterra-1.0.8/finisterra.egg-info/requires.txt
--rw-r--r--   0 danieljaramillo   (501) staff       (20)       11 2024-03-06 10:53:03.000000 finisterra-1.0.8/finisterra.egg-info/top_level.txt
--rw-r--r--   0 danieljaramillo   (501) staff       (20)       38 2024-03-06 10:53:03.932822 finisterra-1.0.8/setup.cfg
--rw-r--r--   0 danieljaramillo   (501) staff       (20)      783 2024-03-06 10:51:06.000000 finisterra-1.0.8/setup.py
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.739354 finisterra-1.0.9/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    11357 2024-02-12 15:45:31.000000 finisterra-1.0.9/LICENSE
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     3473 2024-03-06 11:13:29.739084 finisterra-1.0.9/PKG-INFO
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     2928 2024-02-12 15:47:26.000000 finisterra-1.0.9/README.md
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.718954 finisterra-1.0.9/finisterra/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:05:33.000000 finisterra-1.0.9/finisterra/__init__.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    12505 2024-03-06 11:09:37.000000 finisterra-1.0.9/finisterra/main.py
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.719943 finisterra-1.0.9/finisterra/providers/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:16:08.000000 finisterra-1.0.9/finisterra/providers/__init__.py
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.735851 finisterra-1.0.9/finisterra/providers/aws/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    23620 2024-02-29 11:42:10.000000 finisterra-1.0.9/finisterra/providers/aws/Aws.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:16:11.000000 finisterra-1.0.9/finisterra/providers/aws/__init__.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     5843 2024-02-29 11:50:06.000000 finisterra-1.0.9/finisterra/providers/aws/acm.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    35131 2024-02-29 20:36:08.000000 finisterra-1.0.9/finisterra/providers/aws/apigateway.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    44984 2024-02-29 12:20:46.000000 finisterra-1.0.9/finisterra/providers/aws/aurora.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    19749 2024-02-29 12:20:51.000000 finisterra-1.0.9/finisterra/providers/aws/autoscaling.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     3534 2024-02-12 15:43:48.000000 finisterra-1.0.9/finisterra/providers/aws/aws_clients.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    21130 2024-02-29 12:20:56.000000 finisterra-1.0.9/finisterra/providers/aws/aws_lambda.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    27915 2024-02-29 12:21:02.000000 finisterra-1.0.9/finisterra/providers/aws/cloudfront.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    10895 2024-02-29 12:21:07.000000 finisterra-1.0.9/finisterra/providers/aws/cloudmap.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     8902 2024-02-29 12:21:11.000000 finisterra-1.0.9/finisterra/providers/aws/codeartifact.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    17466 2024-02-29 12:21:15.000000 finisterra-1.0.9/finisterra/providers/aws/docdb.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     9294 2024-02-29 12:21:19.000000 finisterra-1.0.9/finisterra/providers/aws/dynamodb.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    31121 2024-02-29 12:21:24.000000 finisterra-1.0.9/finisterra/providers/aws/ec2.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    12647 2024-02-29 12:21:28.000000 finisterra-1.0.9/finisterra/providers/aws/ecr.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    34981 2024-03-05 11:22:18.000000 finisterra-1.0.9/finisterra/providers/aws/ecs.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    18487 2024-02-29 12:21:36.000000 finisterra-1.0.9/finisterra/providers/aws/eks.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    12017 2024-02-29 12:21:40.000000 finisterra-1.0.9/finisterra/providers/aws/elasticache_redis.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    13638 2024-02-29 12:21:43.000000 finisterra-1.0.9/finisterra/providers/aws/elasticbeanstalk.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    10992 2024-02-29 12:21:48.000000 finisterra-1.0.9/finisterra/providers/aws/elasticsearch.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    13636 2024-02-29 12:21:51.000000 finisterra-1.0.9/finisterra/providers/aws/elbv2.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    25066 2024-02-29 12:21:58.000000 finisterra-1.0.9/finisterra/providers/aws/iam_policy.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     8196 2024-02-29 22:09:33.000000 finisterra-1.0.9/finisterra/providers/aws/iam_role.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    17100 2024-02-29 12:22:05.000000 finisterra-1.0.9/finisterra/providers/aws/kms.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     7295 2024-02-29 12:22:09.000000 finisterra-1.0.9/finisterra/providers/aws/launchtemplate.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    13777 2024-02-29 12:22:13.000000 finisterra-1.0.9/finisterra/providers/aws/logs.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    14301 2024-02-29 12:22:18.000000 finisterra-1.0.9/finisterra/providers/aws/msk.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    19354 2024-02-29 12:22:23.000000 finisterra-1.0.9/finisterra/providers/aws/rds.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    28857 2024-02-29 22:00:35.000000 finisterra-1.0.9/finisterra/providers/aws/s3.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     8610 2024-02-29 12:22:29.000000 finisterra-1.0.9/finisterra/providers/aws/security_group.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     8330 2024-02-29 12:22:33.000000 finisterra-1.0.9/finisterra/providers/aws/sns.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     8720 2024-02-29 12:22:36.000000 finisterra-1.0.9/finisterra/providers/aws/sqs.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     6661 2024-02-29 12:22:41.000000 finisterra-1.0.9/finisterra/providers/aws/stepfunction.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    10546 2024-02-29 12:22:45.000000 finisterra-1.0.9/finisterra/providers/aws/target_group.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     1328 2024-02-21 03:58:45.000000 finisterra-1.0.9/finisterra/providers/aws/utils.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    64949 2024-02-29 12:22:54.000000 finisterra-1.0.9/finisterra/providers/aws/vpc.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    15164 2024-02-29 20:59:32.000000 finisterra-1.0.9/finisterra/providers/aws/vpc_endpoint.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    12295 2024-02-29 12:22:58.000000 finisterra-1.0.9/finisterra/providers/aws/wafv2.py
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.737054 finisterra-1.0.9/finisterra/providers/cloudflare/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     1408 2024-02-29 11:43:15.000000 finisterra-1.0.9/finisterra/providers/cloudflare/Cloudflare.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-27 22:19:41.000000 finisterra-1.0.9/finisterra/providers/cloudflare/__init__.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)      111 2024-02-28 10:48:31.000000 finisterra-1.0.9/finisterra/providers/cloudflare/cf_clients.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     4660 2024-02-29 14:16:53.000000 finisterra-1.0.9/finisterra/providers/cloudflare/dns.py
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.738421 finisterra-1.0.9/finisterra/utils/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)        0 2024-02-13 04:16:15.000000 finisterra-1.0.9/finisterra/utils/__init__.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     3745 2024-03-01 23:09:44.000000 finisterra-1.0.9/finisterra/utils/auth.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     1819 2024-03-05 14:02:46.000000 finisterra-1.0.9/finisterra/utils/filesystem.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)    14098 2024-03-01 23:13:15.000000 finisterra-1.0.9/finisterra/utils/hcl.py
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     7299 2024-02-20 22:00:50.000000 finisterra-1.0.9/finisterra/utils/tf_plan.py
+drwxr-xr-x   0 danieljaramillo   (501) staff       (20)        0 2024-03-06 11:13:29.738751 finisterra-1.0.9/finisterra.egg-info/
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     3473 2024-03-06 11:13:29.000000 finisterra-1.0.9/finisterra.egg-info/PKG-INFO
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)     2005 2024-03-06 11:13:29.000000 finisterra-1.0.9/finisterra.egg-info/SOURCES.txt
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)        1 2024-03-06 11:13:29.000000 finisterra-1.0.9/finisterra.egg-info/dependency_links.txt
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)       52 2024-03-06 11:13:29.000000 finisterra-1.0.9/finisterra.egg-info/entry_points.txt
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)      143 2024-03-06 11:13:29.000000 finisterra-1.0.9/finisterra.egg-info/requires.txt
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)       11 2024-03-06 11:13:29.000000 finisterra-1.0.9/finisterra.egg-info/top_level.txt
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)       38 2024-03-06 11:13:29.739400 finisterra-1.0.9/setup.cfg
+-rw-r--r--   0 danieljaramillo   (501) staff       (20)      783 2024-03-06 11:13:12.000000 finisterra-1.0.9/setup.py
```

### Comparing `finisterra-1.0.8/LICENSE` & `finisterra-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/PKG-INFO` & `finisterra-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finisterra
-Version: 1.0.8
+Version: 1.0.9
 Summary: Terraform in minutes not weeks.
 Home-page: https://github.com/finisterra-io/finisterra
 Author: Finisterra
 Author-email: daniel@finisterra.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3==1.26.94
```

### Comparing `finisterra-1.0.8/README.md` & `finisterra-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/main.py` & `finisterra-1.0.9/finisterra/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 @click.option('--module', '-m', required=True, help='Module name(s), separated by commas or "all" for all modules')
 @click.option('--output_dir', '-o', default=os.getcwd(), help='Output directory')
 @click.option('--process_dependencies', '-d', default=True, help='Process dependencies')
 @click.option('--run-plan', '-r', default=True, help='Run plan')
 @click.option('--token', '-t', default=None, help='Token')
 @click.option('--cache-dir', '-c', default=None, help='Cache directory to save the terraform providers schema')
 def main(provider, module, output_dir, process_dependencies, run_plan, token, cache_dir):
+    if output_dir:
+        output_dir = os.path.abspath(output_dir)
     if not os.environ.get('FT_PROCESS_DEPENDENCIES'):
         os.environ['FT_PROCESS_DEPENDENCIES'] = str(process_dependencies)
 
     if not os.environ.get('FT_CACHE_DIR') and cache_dir:
         os.environ['FT_CACHE_DIR'] = cache_dir
 
     setup_logger()
```

### Comparing `finisterra-1.0.8/finisterra/providers/aws/Aws.py` & `finisterra-1.0.9/finisterra/providers/aws/Aws.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/acm.py` & `finisterra-1.0.9/finisterra/providers/aws/acm.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/apigateway.py` & `finisterra-1.0.9/finisterra/providers/aws/apigateway.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/aurora.py` & `finisterra-1.0.9/finisterra/providers/aws/aurora.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/autoscaling.py` & `finisterra-1.0.9/finisterra/providers/aws/autoscaling.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/aws_clients.py` & `finisterra-1.0.9/finisterra/providers/aws/aws_clients.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/aws_lambda.py` & `finisterra-1.0.9/finisterra/providers/aws/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/cloudfront.py` & `finisterra-1.0.9/finisterra/providers/aws/cloudfront.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/cloudmap.py` & `finisterra-1.0.9/finisterra/providers/aws/cloudmap.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/codeartifact.py` & `finisterra-1.0.9/finisterra/providers/aws/codeartifact.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/docdb.py` & `finisterra-1.0.9/finisterra/providers/aws/docdb.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/dynamodb.py` & `finisterra-1.0.9/finisterra/providers/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/ec2.py` & `finisterra-1.0.9/finisterra/providers/aws/ec2.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/ecr.py` & `finisterra-1.0.9/finisterra/providers/aws/ecr.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/ecs.py` & `finisterra-1.0.9/finisterra/providers/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/eks.py` & `finisterra-1.0.9/finisterra/providers/aws/eks.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/elasticache_redis.py` & `finisterra-1.0.9/finisterra/providers/aws/elasticache_redis.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/elasticbeanstalk.py` & `finisterra-1.0.9/finisterra/providers/aws/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/elasticsearch.py` & `finisterra-1.0.9/finisterra/providers/aws/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/elbv2.py` & `finisterra-1.0.9/finisterra/providers/aws/elbv2.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/iam_policy.py` & `finisterra-1.0.9/finisterra/providers/aws/iam_policy.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/iam_role.py` & `finisterra-1.0.9/finisterra/providers/aws/iam_role.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/kms.py` & `finisterra-1.0.9/finisterra/providers/aws/kms.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/launchtemplate.py` & `finisterra-1.0.9/finisterra/providers/aws/launchtemplate.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/logs.py` & `finisterra-1.0.9/finisterra/providers/aws/logs.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/msk.py` & `finisterra-1.0.9/finisterra/providers/aws/msk.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/rds.py` & `finisterra-1.0.9/finisterra/providers/aws/rds.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/s3.py` & `finisterra-1.0.9/finisterra/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/security_group.py` & `finisterra-1.0.9/finisterra/providers/aws/security_group.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/sns.py` & `finisterra-1.0.9/finisterra/providers/aws/sns.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/sqs.py` & `finisterra-1.0.9/finisterra/providers/aws/sqs.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/stepfunction.py` & `finisterra-1.0.9/finisterra/providers/aws/stepfunction.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/target_group.py` & `finisterra-1.0.9/finisterra/providers/aws/target_group.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/utils.py` & `finisterra-1.0.9/finisterra/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/vpc.py` & `finisterra-1.0.9/finisterra/providers/aws/vpc.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/vpc_endpoint.py` & `finisterra-1.0.9/finisterra/providers/aws/vpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/aws/wafv2.py` & `finisterra-1.0.9/finisterra/providers/aws/wafv2.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/cloudflare/Cloudflare.py` & `finisterra-1.0.9/finisterra/providers/cloudflare/Cloudflare.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/providers/cloudflare/dns.py` & `finisterra-1.0.9/finisterra/providers/cloudflare/dns.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/utils/auth.py` & `finisterra-1.0.9/finisterra/utils/auth.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/utils/filesystem.py` & `finisterra-1.0.9/finisterra/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/utils/hcl.py` & `finisterra-1.0.9/finisterra/utils/hcl.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra/utils/tf_plan.py` & `finisterra-1.0.9/finisterra/utils/tf_plan.py`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/finisterra.egg-info/PKG-INFO` & `finisterra-1.0.9/finisterra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finisterra
-Version: 1.0.8
+Version: 1.0.9
 Summary: Terraform in minutes not weeks.
 Home-page: https://github.com/finisterra-io/finisterra
 Author: Finisterra
 Author-email: daniel@finisterra.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3==1.26.94
```

### Comparing `finisterra-1.0.8/finisterra.egg-info/SOURCES.txt` & `finisterra-1.0.9/finisterra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finisterra-1.0.8/setup.py` & `finisterra-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='finisterra',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     install_requires=[
         'boto3==1.26.94',
         'PyJWT==2.7.0',
         'pycryptodome==3.18.0',
         'cryptography==41.0.1',
         'PyYAML==6.0',
```

