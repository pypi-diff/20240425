# Comparing `tmp/aws_ec2_instance_reaper-0.1.0.tar.gz` & `tmp/aws_ec2_instance_reaper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_ec2_instance_reaper-0.1.0.tar", last modified: Thu Apr 25 13:30:35 2024, max compression
+gzip compressed data, was "aws_ec2_instance_reaper-0.1.4.tar", last modified: Thu Apr 25 16:30:03 2024, max compression
```

## Comparing `aws_ec2_instance_reaper-0.1.0.tar` & `aws_ec2_instance_reaper-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.512597 aws_ec2_instance_reaper-0.1.0/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      499 2024-04-25 09:57:42.000000 aws_ec2_instance_reaper-0.1.0/.buildspec.yaml
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1217 2024-04-25 12:48:08.000000 aws_ec2_instance_reaper-0.1.0/.dockerignore
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.500670 aws_ec2_instance_reaper-0.1.0/.github/
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.506140 aws_ec2_instance_reaper-0.1.0/.github/workflows/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      914 2023-11-04 17:42:59.000000 aws_ec2_instance_reaper-0.1.0/.github/workflows/dependabot.yaml
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1217 2024-04-25 12:48:08.000000 aws_ec2_instance_reaper-0.1.0/.gitignore
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      159 2020-03-28 19:35:34.000000 aws_ec2_instance_reaper-0.1.0/.gitlab-ci.yml
--rw-------   0 mvanholsteijn   (502) staff       (20)     2565 2020-03-05 16:32:57.000000 aws_ec2_instance_reaper-0.1.0/.make-release-support
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      272 2024-04-25 10:08:56.000000 aws_ec2_instance_reaper-0.1.0/.release
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      533 2024-04-25 13:13:37.000000 aws_ec2_instance_reaper-0.1.0/Dockerfile.lambda
--rw-------   0 mvanholsteijn   (502) staff       (20)    11342 2020-03-05 16:32:57.000000 aws_ec2_instance_reaper-0.1.0/LICENSE
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     4706 2024-04-25 13:30:18.000000 aws_ec2_instance_reaper-0.1.0/Makefile
--rw-------   0 mvanholsteijn   (502) staff       (20)     3704 2020-03-05 16:32:57.000000 aws_ec2_instance_reaper-0.1.0/Makefile.mk
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     3911 2024-04-25 13:30:35.512484 aws_ec2_instance_reaper-0.1.0/PKG-INFO
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      138 2024-04-24 13:48:41.000000 aws_ec2_instance_reaper-0.1.0/Pipfile
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     2956 2024-04-25 10:08:46.000000 aws_ec2_instance_reaper-0.1.0/README.md
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.507293 aws_ec2_instance_reaper-0.1.0/cloudformation/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     2682 2024-04-25 12:52:37.000000 aws_ec2_instance_reaper-0.1.0/cloudformation/aws-ec2-instance-reaper.yaml
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     3007 2024-04-24 15:23:49.000000 aws_ec2_instance_reaper-0.1.0/cloudformation/cicd-pipeline.yaml
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1033 2024-04-25 13:13:27.000000 aws_ec2_instance_reaper-0.1.0/cloudformation/demo-stack.yaml
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      112 2024-04-25 09:24:58.000000 aws_ec2_instance_reaper-0.1.0/pyproject.toml
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     1212 2024-04-25 13:30:35.513010 aws_ec2_instance_reaper-0.1.0/setup.cfg
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.501505 aws_ec2_instance_reaper-0.1.0/src/
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.510072 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       51 2023-11-30 11:01:27.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/__init__.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     2219 2024-04-25 13:12:05.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/__main__.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     5128 2023-12-01 11:06:31.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/aws.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      927 2024-04-25 09:54:43.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/click_argument_types.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      178 2023-11-30 19:38:38.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/logger.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     2820 2024-04-25 13:10:11.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/reaper.py
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     2551 2024-04-25 09:54:43.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/schema.py
-drwxr-xr-x   0 mvanholsteijn   (502) staff       (20)        0 2024-04-25 13:30:35.512139 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)     3911 2024-04-25 13:30:35.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/PKG-INFO
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      966 2024-04-25 13:30:35.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/SOURCES.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)        1 2024-04-25 13:30:35.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/dependency_links.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       82 2024-04-25 13:30:35.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/entry_points.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)        1 2023-11-30 16:16:15.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/not-zip-safe
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       47 2024-04-25 13:30:35.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/requires.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)       24 2024-04-25 13:30:35.000000 aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/top_level.txt
--rw-r--r--   0 mvanholsteijn   (502) staff       (20)      183 2024-04-24 13:23:35.000000 aws_ec2_instance_reaper-0.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.107883 aws_ec2_instance_reaper-0.1.4/
+-rw-r--r--   0 root         (0) root         (0)      495 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.buildspec.yaml
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.dockerignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.099883 aws_ec2_instance_reaper-0.1.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.103883 aws_ec2_instance_reaper-0.1.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      914 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.github/workflows/dependabot.yaml
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.make-release-support
+-rw-r--r--   0 root         (0) root         (0)      272 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/.release
+-rw-r--r--   0 root         (0) root         (0)      511 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/Dockerfile.lambda
+-rw-r--r--   0 root         (0) root         (0)    11342 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4629 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/Makefile
+-rw-r--r--   0 root         (0) root         (0)     3704 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/Makefile.mk
+-rw-r--r--   0 root         (0) root         (0)     3911 2024-04-25 16:30:03.107883 aws_ec2_instance_reaper-0.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/Pipfile
+-rw-r--r--   0 root         (0) root         (0)     2956 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.103883 aws_ec2_instance_reaper-0.1.4/cloudformation/
+-rw-r--r--   0 root         (0) root         (0)     2668 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/cloudformation/aws-ec2-instance-reaper.yaml
+-rw-r--r--   0 root         (0) root         (0)     2926 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/cloudformation/cicd-pipeline.yaml
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/cloudformation/demo-stack.yaml
+-rw-r--r--   0 root         (0) root         (0)      112 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-25 16:30:03.139883 aws_ec2_instance_reaper-0.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.099883 aws_ec2_instance_reaper-0.1.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.103883 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5128 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/aws.py
+-rw-r--r--   0 root         (0) root         (0)      927 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/click_argument_types.py
+-rw-r--r--   0 root         (0) root         (0)      178 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/logger.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/reaper.py
+-rw-r--r--   0 root         (0) root         (0)     2551 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.107883 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3911 2024-04-25 16:30:02.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      983 2024-04-25 16:30:03.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 16:30:02.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-25 16:30:02.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 16:30:02.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-25 16:30:02.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-04-25 16:30:02.000000 aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 16:30:03.107883 aws_ec2_instance_reaper-0.1.4/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/tests/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-25 16:29:23.000000 aws_ec2_instance_reaper-0.1.4/tox.ini
```

### Comparing `aws_ec2_instance_reaper-0.1.0/.dockerignore` & `aws_ec2_instance_reaper-0.1.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/.github/workflows/dependabot.yaml` & `aws_ec2_instance_reaper-0.1.4/.github/workflows/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/.gitignore` & `aws_ec2_instance_reaper-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/.make-release-support` & `aws_ec2_instance_reaper-0.1.4/.make-release-support`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/LICENSE` & `aws_ec2_instance_reaper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/Makefile` & `aws_ec2_instance_reaper-0.1.4/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -79,17 +79,15 @@
 	aws cloudformation delete-stack --stack-name $(NAME)
 	aws cloudformation wait stack-delete-complete  --stack-name $(NAME)
 
 deploy-pipeline:				## to your AWS account
 	aws cloudformation deploy \
 	--capabilities CAPABILITY_IAM \
 	--stack-name $(NAME)-pipeline \
-	--template-file ./cloudformation/cicd-pipeline.yaml \
-	--parameter-overrides \
-	S3BucketPrefix=$(S3_BUCKET_PREFIX)-$(AWS_REGION)
+	--template-file ./cloudformation/cicd-pipeline.yaml
 
 delete-pipeline:				## from your AWS account
 	aws cloudformation delete-stack --stack-name $(NAME)-pipeline
 	aws cloudformation wait stack-delete-complete  --stack-name $(NAME)-pipeline
 
 
 demo: 						## to your AWS account
```

### Comparing `aws_ec2_instance_reaper-0.1.0/Makefile.mk` & `aws_ec2_instance_reaper-0.1.4/Makefile.mk`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/PKG-INFO` & `aws_ec2_instance_reaper-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ec2-instance-reaper
-Version: 0.1.0
+Version: 0.1.4
 Summary: reap dangling EC2 machines on AWS
 Home-page: https://github.com/binxio/aws-ec2-instance-reaper
 Author: Mark van Holsteijn
 Author-email: mark@binx.io
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aws_ec2_instance_reaper-0.1.0/README.md` & `aws_ec2_instance_reaper-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/cloudformation/aws-ec2-instance-reaper.yaml` & `aws_ec2_instance_reaper-0.1.4/cloudformation/aws-ec2-instance-reaper.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
       Description: reap empheral EC2 instances
       FunctionName: aws-ec2-instance-reaper
       Code:
         S3Bucket: !If
           - UsePublicBucket
           - !Sub 'binxio-public-${AWS::Region}'
           - !Ref 'LambdaS3Bucket'
-        S3Key:  lambdas/aws-ec2-instance-reaper-0.1.0-6c961ac-dirty.zip
+        S3Key:  lambdas/aws-ec2-instance-reaper-0.1.4.zip
       Handler: aws_ec2_instance_reaper.handler
       Role: !GetAtt LambdaRole.Arn
       Runtime: python3.9
       Timeout: 60
       LoggingConfig:
         LogGroup: !Ref LogGroup
```

### Comparing `aws_ec2_instance_reaper-0.1.0/cloudformation/cicd-pipeline.yaml` & `aws_ec2_instance_reaper-0.1.4/cloudformation/cicd-pipeline.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -52,28 +52,27 @@
           - Effect: Allow
             Action: sts:AssumeRole
             Principal:
               Service: codebuild.amazonaws.com
             Condition: {}
       Path: /
       Policies:
-        - PolicyName: CFNSecretProviderBuilder
+        - PolicyName: LamdbaCodeBuilder
           PolicyDocument:
             Statement:
               - Effect: Allow
                 Action:
                   - s3:ListObjects
                   - s3:GetBucketLocation
                 Resource: 
                   - !Sub 'arn:aws:s3:::${S3BucketPrefix}-*'
               - Effect: Allow
                 Action:
-                  - s3:GetObject
-                  - s3:PutObject
-                  - s3:PutObjectAcl
+                  - s3:GetObject*
+                  - s3:PutObject*
                 Resource: 
                   - !Sub 'arn:aws:s3:::${S3BucketPrefix}-*/lambdas/aws-ec2-instance-reaper-*'
               - Effect: Allow
                 Action:
                   - ssm:GetParameter
                   - ssm:GetParameters
                 Resource: 
@@ -82,15 +81,14 @@
                 Action:
                   - ec2:DescribeRegions
                 Resource: 
                   - '*'
               - Sid: CloudWatchLogsPolicy
                 Effect: Allow
                 Action:
-                  - logs:CreateLogGroup
                   - logs:CreateLogStream
                   - logs:PutLogEvents
                 Resource:
                   - '*'
 
   LogGroup:
     Type: AWS::Logs::LogGroup
```

### Comparing `aws_ec2_instance_reaper-0.1.0/cloudformation/demo-stack.yaml` & `aws_ec2_instance_reaper-0.1.4/cloudformation/demo-stack.yaml`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/setup.cfg` & `aws_ec2_instance_reaper-0.1.4/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aws-ec2-instance-reaper
-version = 0.1.0
+version = 0.1.4
 author = Mark van Holsteijn
 author_email = mark@binx.io
 license = BSD
 description = reap dangling EC2 machines on AWS
 url = https://github.com/binxio/aws-ec2-instance-reaper
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/__main__.py` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/__main__.py`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/aws.py` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/aws.py`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/click_argument_types.py` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/click_argument_types.py`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/reaper.py` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/reaper.py`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper/schema.py` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper/schema.py`

 * *Files identical despite different names*

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/PKG-INFO` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ec2-instance-reaper
-Version: 0.1.0
+Version: 0.1.4
 Summary: reap dangling EC2 machines on AWS
 Home-page: https://github.com/binxio/aws-ec2-instance-reaper
 Author: Mark van Holsteijn
 Author-email: mark@binx.io
 License: BSD
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `aws_ec2_instance_reaper-0.1.0/src/aws_ec2_instance_reaper.egg-info/SOURCES.txt` & `aws_ec2_instance_reaper-0.1.4/src/aws_ec2_instance_reaper.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 src/aws_ec2_instance_reaper/schema.py
 src/aws_ec2_instance_reaper.egg-info/PKG-INFO
 src/aws_ec2_instance_reaper.egg-info/SOURCES.txt
 src/aws_ec2_instance_reaper.egg-info/dependency_links.txt
 src/aws_ec2_instance_reaper.egg-info/entry_points.txt
 src/aws_ec2_instance_reaper.egg-info/not-zip-safe
 src/aws_ec2_instance_reaper.egg-info/requires.txt
-src/aws_ec2_instance_reaper.egg-info/top_level.txt
+src/aws_ec2_instance_reaper.egg-info/top_level.txt
+tests/.gitignore
```

