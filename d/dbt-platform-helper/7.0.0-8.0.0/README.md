# Comparing `tmp/dbt_platform_helper-7.0.0.tar.gz` & `tmp/dbt_platform_helper-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-7.0.0.tar", max compression
+gzip compressed data, was "dbt_platform_helper-8.0.0.tar", max compression
```

## Comparing `dbt_platform_helper-7.0.0.tar` & `dbt_platform_helper-8.0.0.tar`

### file list

```diff
@@ -1,91 +1,92 @@
--rw-r--r--   0        0        0     1090 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/LICENSE
--rw-r--r--   0        0        0    19003 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     4522 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1315 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0    10582 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/bootstrap.py
--rwxr-xr-x   0        0        0     3226 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    12855 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0     7949 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    16324 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0     8670 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      722 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6218 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/commands/pipeline.py
--rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      342 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/default-addons.yml
--rw-r--r--   0        0        0      499 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      618 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3658 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2403 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      691 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      439 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   150965 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1906 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0     1959 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   148134 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      534 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3908 2024-04-15 16:31:17.930914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10704 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      304 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    17799 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6408 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1936 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/platform_helper.py
--rw-r--r--   0        0        0     1393 2024-04-15 16:31:17.940914 dbt_platform_helper-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/LICENSE
+-rw-r--r--   0        0        0    17094 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     4522 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1315 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0     3226 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    12871 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0     7953 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    15859 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0     8670 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      853 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6218 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/pipeline.py
+-rwxr-xr-x   0        0        0     3860 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/secrets.py
+-rw-r--r--   0        0        0        0 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      342 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/default-extensions.yml
+-rw-r--r--   0        0        0      499 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      618 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3658 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2403 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      691 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      443 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   155387 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1910 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0      208 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
+-rw-r--r--   0        0        0     1959 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   152518 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3555 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10704 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      304 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    17799 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6695 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1930 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/platform_helper.py
+-rw-r--r--   0        0        0     1392 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.0.0/PKG-INFO
```

### Comparing `dbt_platform_helper-7.0.0/LICENSE` & `dbt_platform_helper-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-8.0.0/dbt_platform_helper/COMMANDS.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 # Commands Reference
 
 - [platform-helper](#platform-helper)
-- [platform-helper bootstrap](#platform-helper-bootstrap)
-- [platform-helper bootstrap make-config](#platform-helper-bootstrap-make-config)
-- [platform-helper bootstrap migrate-secrets](#platform-helper-bootstrap-migrate-secrets)
-- [platform-helper bootstrap copy-secrets](#platform-helper-bootstrap-copy-secrets)
+- [platform-helper application](#platform-helper-application)
+- [platform-helper application container-stats](#platform-helper-application-container-stats)
+- [platform-helper application task-stats](#platform-helper-application-task-stats)
+- [platform-helper cdn](#platform-helper-cdn)
+- [platform-helper cdn assign](#platform-helper-cdn-assign)
+- [platform-helper cdn delete](#platform-helper-cdn-delete)
+- [platform-helper cdn list](#platform-helper-cdn-list)
 - [platform-helper check-cloudformation](#platform-helper-check-cloudformation)
 - [platform-helper check-cloudformation lint](#platform-helper-check-cloudformation-lint)
 - [platform-helper check-cloudformation check-security](#platform-helper-check-cloudformation-check-security)
 - [platform-helper codebase](#platform-helper-codebase)
 - [platform-helper codebase prepare](#platform-helper-codebase-prepare)
 - [platform-helper codebase list](#platform-helper-codebase-list)
 - [platform-helper codebase build](#platform-helper-codebase-build)
 - [platform-helper codebase deploy](#platform-helper-codebase-deploy)
 - [platform-helper conduit](#platform-helper-conduit)
 - [platform-helper config](#platform-helper-config)
 - [platform-helper config validate](#platform-helper-config-validate)
 - [platform-helper copilot](#platform-helper-copilot)
 - [platform-helper copilot make-addons](#platform-helper-copilot-make-addons)
-- [platform-helper copilot get-env-secrets](#platform-helper-copilot-get-env-secrets)
 - [platform-helper domain](#platform-helper-domain)
 - [platform-helper domain configure](#platform-helper-domain-configure)
 - [platform-helper domain assign](#platform-helper-domain-assign)
-- [platform-helper cdn](#platform-helper-cdn)
-- [platform-helper cdn assign](#platform-helper-cdn-assign)
-- [platform-helper cdn delete](#platform-helper-cdn-delete)
-- [platform-helper cdn list](#platform-helper-cdn-list)
 - [platform-helper environment](#platform-helper-environment)
 - [platform-helper environment offline](#platform-helper-environment-offline)
 - [platform-helper environment online](#platform-helper-environment-online)
 - [platform-helper generate](#platform-helper-generate)
 - [platform-helper pipeline](#platform-helper-pipeline)
 - [platform-helper pipeline generate](#platform-helper-pipeline-generate)
-- [platform-helper application](#platform-helper-application)
-- [platform-helper application container-stats](#platform-helper-application-container-stats)
-- [platform-helper application task-stats](#platform-helper-application-task-stats)
+- [platform-helper secrets](#platform-helper-secrets)
+- [platform-helper secrets copy](#platform-helper-secrets-copy)
+- [platform-helper secrets list](#platform-helper-secrets-list)
 
 # platform-helper
 
 ## Usage
 
 ```
 platform-helper <command> [--version] 
@@ -50,125 +48,198 @@
   - Show the version and exit.
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 ## Commands
 
 - [`application` ↪](#platform-helper-application)
-- [`bootstrap` ↪](#platform-helper-bootstrap)
 - [`cdn` ↪](#platform-helper-cdn)
 - [`check-cloudformation` ↪](#platform-helper-check-cloudformation)
 - [`codebase` ↪](#platform-helper-codebase)
 - [`conduit` ↪](#platform-helper-conduit)
 - [`config` ↪](#platform-helper-config)
 - [`copilot` ↪](#platform-helper-copilot)
 - [`domain` ↪](#platform-helper-domain)
 - [`environment` ↪](#platform-helper-environment)
 - [`generate` ↪](#platform-helper-generate)
 - [`pipeline` ↪](#platform-helper-pipeline)
+- [`secrets` ↪](#platform-helper-secrets)
 
-# platform-helper bootstrap
+# platform-helper application
 
 [↩ Parent](#platform-helper)
 
+    Application metrics.
+
 ## Usage
 
 ```
-platform-helper bootstrap (make-config|migrate-secrets|copy-secrets) 
+platform-helper application (container-stats|task-stats) 
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 ## Commands
 
-- [`copy-secrets` ↪](#platform-helper-bootstrap-copy-secrets)
-- [`make-config` ↪](#platform-helper-bootstrap-make-config)
-- [`migrate-secrets` ↪](#platform-helper-bootstrap-migrate-secrets)
+- [`container-stats` ↪](#platform-helper-application-container-stats)
+- [`task-stats` ↪](#platform-helper-application-task-stats)
 
-# platform-helper bootstrap make-config
+# platform-helper application container-stats
 
-[↩ Parent](#platform-helper-bootstrap)
+[↩ Parent](#platform-helper-application)
 
-    Generate Copilot boilerplate code.
+    Command to get application container level metrics.
 
 ## Usage
 
 ```
-platform-helper bootstrap make-config [-d <directory>] 
+platform-helper application container-stats --env <environment> --app <application> 
+                                            [--storage] [--network] 
 ```
 
 ## Options
 
-- `-d
---directory <text>` _Defaults to .._
+- `--env <text>`
+
+- `--app <text>`
+
+- `--storage <boolean>` _Defaults to False._
+
+- `--network <boolean>` _Defaults to False._
+
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
+
+# platform-helper application task-stats
+
+[↩ Parent](#platform-helper-application)
+
+    Command to get application task level metrics.
+
+## Usage
+
+```
+platform-helper application task-stats --env <environment> --app <application> [--disk] 
+                                       [--storage] [--network] 
+```
+
+## Options
+
+- `--env <text>`
+
+- `--app <text>`
+
+- `--disk <boolean>` _Defaults to False._
+
+- `--storage <boolean>` _Defaults to False._
+
+- `--network <boolean>` _Defaults to False._
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
-# platform-helper bootstrap migrate-secrets
+# platform-helper cdn
+
+[↩ Parent](#platform-helper)
+
+## Usage
+
+```
+platform-helper cdn (assign|delete|list) 
+```
+
+## Options
+
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
 
-[↩ Parent](#platform-helper-bootstrap)
+## Commands
 
-    Migrate secrets from your GOV.UK PaaS application to DBT PaaS.
+- [`assign` ↪](#platform-helper-cdn-assign)
+- [`delete` ↪](#platform-helper-cdn-delete)
+- [`list` ↪](#platform-helper-cdn-list)
 
-    You need to be authenticated via Cloud Foundry CLI and the AWS CLI to use this command.
+# platform-helper cdn assign
 
-    If you're using AWS profiles, use the AWS_PROFILE environment variable to indicate the which
-    profile to use, e.g.:
+[↩ Parent](#platform-helper-cdn)
 
-    AWS_PROFILE=myaccount copilot-bootstrap.py ...
+    Assigns a CDN domain name to application loadbalancer.
 
 ## Usage
 
 ```
-platform-helper bootstrap migrate-secrets --project-profile <project_profile> 
-                                          --env <environment> [--svc <service>] 
-                                          [--overwrite] [--dry-run] 
+platform-helper cdn assign --project-profile <project_profile> --env <environment> 
+                           --app <application> --svc <service> 
 ```
 
 ## Options
 
 - `--project-profile <text>`
-  - AWS account profile name
+  - AWS account profile name for certificates account
 - `--env <text>`
-  - Migrate secrets from a specific environment
+  - AWS Copilot environment name
+- `--app <text>`
+  - Application Name
 - `--svc <text>`
-  - Migrate secrets from a specific service
-- `--overwrite <boolean>` _Defaults to False._
-  - Overwrite existing secrets?
-- `--dry-run <boolean>` _Defaults to False._
-  - dry run
+  - Service Name
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
-# platform-helper bootstrap copy-secrets
+# platform-helper cdn delete
 
-[↩ Parent](#platform-helper-bootstrap)
+[↩ Parent](#platform-helper-cdn)
 
-    Copy secrets from one environment to a new environment.
+    Assigns a CDN domain name to application loadbalancer.
 
 ## Usage
 
 ```
-platform-helper bootstrap copy-secrets <source_environment> <target_environment> 
-                                       --project-profile <project_profile> 
+platform-helper cdn delete --project-profile <project_profile> --env <environment> 
+                           --app <application> --svc <service> 
 ```
 
-## Arguments
+## Options
 
-- `source_environment <text>`
-- `target_environment <text>`
+- `--project-profile <text>`
+  - AWS account profile name for certificates account
+- `--env <text>`
+  - AWS Copilot environment name
+- `--app <text>`
+  - Application Name
+- `--svc <text>`
+  - Service Name
+- `--help <boolean>` _Defaults to False._
+  - Show this message and exit.
+
+# platform-helper cdn list
+
+[↩ Parent](#platform-helper-cdn)
+
+    List CDN domain name attached to application loadbalancer.
+
+## Usage
+
+```
+platform-helper cdn list --project-profile <project_profile> --env <environment> 
+                         --app <application> --svc <service> 
+```
 
 ## Options
 
 - `--project-profile <text>`
-  - AWS account profile name
+  - AWS account profile name for certificates account
+- `--env <text>`
+  - AWS Copilot environment name
+- `--app <text>`
+  - Application Name
+- `--svc <text>`
+  - Service Name
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 # platform-helper check-cloudformation
 
 [↩ Parent](#platform-helper)
 
@@ -415,25 +486,24 @@
 # platform-helper copilot
 
 [↩ Parent](#platform-helper)
 
 ## Usage
 
 ```
-platform-helper copilot (make-addons|get-env-secrets) 
+platform-helper copilot make-addons 
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 ## Commands
 
-- [`get-env-secrets` ↪](#platform-helper-copilot-get-env-secrets)
 - [`make-addons` ↪](#platform-helper-copilot-make-addons)
 
 # platform-helper copilot make-addons
 
 [↩ Parent](#platform-helper-copilot)
 
     WARNING: this command should not be used as a stand-alone.
@@ -448,36 +518,14 @@
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
-# platform-helper copilot get-env-secrets
-
-[↩ Parent](#platform-helper-copilot)
-
-    List secret names and values for an environment.
-
-## Usage
-
-```
-platform-helper copilot get-env-secrets <application> <environment> 
-```
-
-## Arguments
-
-- `app <text>`
-- `env <text>`
-
-## Options
-
-- `--help <boolean>` _Defaults to False._
-  - Show this message and exit.
-
 # platform-helper domain
 
 [↩ Parent](#platform-helper)
 
 ## Usage
 
 ```
@@ -541,113 +589,14 @@
 - `--domain-profile <choice>`
   - AWS account profile name for Route53 domains account
 - `--project-profile <text>`
   - AWS account profile name for application account
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
-# platform-helper cdn
-
-[↩ Parent](#platform-helper)
-
-## Usage
-
-```
-platform-helper cdn (assign|delete|list) 
-```
-
-## Options
-
-- `--help <boolean>` _Defaults to False._
-  - Show this message and exit.
-
-## Commands
-
-- [`assign` ↪](#platform-helper-cdn-assign)
-- [`delete` ↪](#platform-helper-cdn-delete)
-- [`list` ↪](#platform-helper-cdn-list)
-
-# platform-helper cdn assign
-
-[↩ Parent](#platform-helper-cdn)
-
-    Assigns a CDN domain name to application loadbalancer.
-
-## Usage
-
-```
-platform-helper cdn assign --project-profile <project_profile> --env <environment> 
-                           --app <application> --svc <service> 
-```
-
-## Options
-
-- `--project-profile <text>`
-  - AWS account profile name for certificates account
-- `--env <text>`
-  - AWS Copilot environment name
-- `--app <text>`
-  - Application Name
-- `--svc <text>`
-  - Service Name
-- `--help <boolean>` _Defaults to False._
-  - Show this message and exit.
-
-# platform-helper cdn delete
-
-[↩ Parent](#platform-helper-cdn)
-
-    Assigns a CDN domain name to application loadbalancer.
-
-## Usage
-
-```
-platform-helper cdn delete --project-profile <project_profile> --env <environment> 
-                           --app <application> --svc <service> 
-```
-
-## Options
-
-- `--project-profile <text>`
-  - AWS account profile name for certificates account
-- `--env <text>`
-  - AWS Copilot environment name
-- `--app <text>`
-  - Application Name
-- `--svc <text>`
-  - Service Name
-- `--help <boolean>` _Defaults to False._
-  - Show this message and exit.
-
-# platform-helper cdn list
-
-[↩ Parent](#platform-helper-cdn)
-
-    List CDN domain name attached to application loadbalancer.
-
-## Usage
-
-```
-platform-helper cdn list --project-profile <project_profile> --env <environment> 
-                         --app <application> --svc <service> 
-```
-
-## Options
-
-- `--project-profile <text>`
-  - AWS account profile name for certificates account
-- `--env <text>`
-  - AWS Copilot environment name
-- `--app <text>`
-  - Application Name
-- `--svc <text>`
-  - Service Name
-- `--help <boolean>` _Defaults to False._
-  - Show this message and exit.
-
 # platform-helper environment
 
 [↩ Parent](#platform-helper)
 
     Commands affecting environments.
 
 ## Usage
@@ -768,82 +717,73 @@
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
-# platform-helper application
+# platform-helper secrets
 
 [↩ Parent](#platform-helper)
 
-    Application metrics.
-
 ## Usage
 
 ```
-platform-helper application (container-stats|task-stats) 
+platform-helper secrets (copy|list) 
 ```
 
 ## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
 ## Commands
 
-- [`container-stats` ↪](#platform-helper-application-container-stats)
-- [`task-stats` ↪](#platform-helper-application-task-stats)
+- [`copy` ↪](#platform-helper-secrets-copy)
+- [`list` ↪](#platform-helper-secrets-list)
 
-# platform-helper application container-stats
+# platform-helper secrets copy
 
-[↩ Parent](#platform-helper-application)
+[↩ Parent](#platform-helper-secrets)
 
-    Command to get application container level metrics.
+    Copy secrets from one environment to a new environment.
 
 ## Usage
 
 ```
-platform-helper application container-stats --env <environment> --app <application> 
-                                            [--storage] [--network] 
+platform-helper secrets copy <source_environment> <target_environment> 
+                             --project-profile <project_profile> 
 ```
 
-## Options
-
-- `--env <text>`
-
-- `--app <text>`
+## Arguments
 
-- `--storage <boolean>` _Defaults to False._
+- `source_environment <text>`
+- `target_environment <text>`
 
-- `--network <boolean>` _Defaults to False._
+## Options
 
+- `--project-profile <text>`
+  - AWS account profile name
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
 
-# platform-helper application task-stats
+# platform-helper secrets list
 
-[↩ Parent](#platform-helper-application)
+[↩ Parent](#platform-helper-secrets)
 
-    Command to get application task level metrics.
+    List secret names and values for an environment.
 
 ## Usage
 
 ```
-platform-helper application task-stats --env <environment> --app <application> [--disk] 
-                                       [--storage] [--network] 
+platform-helper secrets list <application> <environment> 
 ```
 
-## Options
-
-- `--env <text>`
-
-- `--app <text>`
-
-- `--disk <boolean>` _Defaults to False._
+## Arguments
 
-- `--storage <boolean>` _Defaults to False._
+- `app <text>`
+- `env <text>`
 
-- `--network <boolean>` _Defaults to False._
+## Options
 
 - `--help <boolean>` _Defaults to False._
   - Show this message and exit.
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/README.md` & `dbt_platform_helper-8.0.0/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/conduit.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 
 CONDUIT_DOCKER_IMAGE_LOCATION = "public.ecr.aws/uktrade/tunnel"
 CONDUIT_ADDON_TYPES = [
     "opensearch",
     "rds-postgres",
     "aurora-postgres",
+    "postgres",
     "redis",
 ]
 CONDUIT_ACCESS_OPTIONS = ["read", "write", "admin"]
 
 
 def normalise_secret_name(addon_name: str) -> str:
     return addon_name.replace("-", "_").upper()
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     recommendations = {}
 
     if Path("storage.yml").exists():
         recommendations["storage.yml"] = (
             "The file `storage.yml` is incompatible with version "
             f"{versioning.string_version(app_released_version)} of "
-            "dbt-platform-helper, move contents to `addons.yml` and "
+            "dbt-platform-helper, move contents to `extensions.yml` and "
             "delete `storage.yml`."
         )
 
     for template_file in addons_templates:
         generated_with_version = maybe
         local_compatible_symbol = yes
         latest_compatible_symbol = yes
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/copilot.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pathlib import PosixPath
 
 import click
 import yaml
 
 from dbt_platform_helper.utils.application import get_application_name
 from dbt_platform_helper.utils.application import load_application
-from dbt_platform_helper.utils.aws import SSM_BASE_PATH
 from dbt_platform_helper.utils.aws import get_aws_session_or_abort
 from dbt_platform_helper.utils.click import ClickDocOptGroup
 from dbt_platform_helper.utils.files import ensure_cwd_is_repo_root
 from dbt_platform_helper.utils.files import generate_override_files
 from dbt_platform_helper.utils.files import mkfile
 from dbt_platform_helper.utils.template import camel_case
 from dbt_platform_helper.utils.template import setup_templates
@@ -221,39 +220,40 @@
 def make_addons():
     """
     WARNING: this command should not be used as a stand-alone.
     Use `platform-helper generate` instead.
 
     Generate addons CloudFormation for each environment.
     """
-
     output_dir = Path(".").absolute()
     ensure_cwd_is_repo_root()
     is_terraform = is_terraform_project()
 
     templates = setup_templates()
     config = _get_config()
     session = get_aws_session_or_abort()
 
     application_name = get_application_name()
 
     with open(PACKAGE_DIR / "addons-template-map.yml") as fd:
         addon_template_map = yaml.safe_load(fd)
 
-    _generate_env_overrides(output_dir)
-
     if is_terraform:
         click.echo("\n>>> Generating Terraform compatible addons CloudFormation\n")
     else:
         click.echo("\n>>> Generating addons CloudFormation\n")
 
-    env_addons_path = Path(f"copilot/environments/addons/")
+    env_path = Path(f"copilot/environments/")
+    env_addons_path = env_path / "addons"
+    env_overrides_path = env_path / "overrides"
+
     (output_dir / env_addons_path).mkdir(parents=True, exist_ok=True)
 
-    _cleanup_old_files(config, output_dir, env_addons_path)
+    _cleanup_old_files(config, output_dir, env_addons_path, env_overrides_path)
+    _generate_env_overrides(output_dir, is_terraform)
     custom_resources = _get_custom_resources()
 
     svc_names = list_copilot_local_services()
     base_path = Path(".")
     for svc_name in svc_names:
         _generate_svc_overrides(base_path, templates, svc_name)
 
@@ -345,25 +345,26 @@
             mkfile(output_dir, env_addons_path / "addons.parameters.yml", contents, overwrite=True)
         )
 
     click.echo(templates.get_template("addon-instructions.txt").render(services=services))
 
 
 def _get_config():
-    config = _validate_and_normalise_config(PACKAGE_DIR / "default-addons.yml")
-    project_config = _validate_and_normalise_config("addons.yml")
+    config = _validate_and_normalise_config(PACKAGE_DIR / "default-extensions.yml")
+    project_config = _validate_and_normalise_config("extensions.yml")
     config.update(project_config)
     return config
 
 
-def _generate_env_overrides(output_dir):
+def _generate_env_overrides(output_dir, is_terraform):
+    path = "templates/env/terraform-overrides" if is_terraform else "templates/env/overrides"
     click.echo("\n>>> Generating Environment overrides\n")
     overrides_path = output_dir.joinpath(f"copilot/environments/overrides")
     overrides_path.mkdir(parents=True, exist_ok=True)
-    template_overrides_path = Path(__file__).parent.parent.joinpath("templates/env/overrides")
+    template_overrides_path = Path(__file__).parent.parent.joinpath(path)
     generate_override_files(Path("."), template_overrides_path, overrides_path)
 
 
 def _generate_env_addons(
     addon_name,
     addon_template_map,
     addons,
@@ -437,52 +438,32 @@
                 ]
                 return "".join(lines)
 
             custom_resources[file_path.name.rstrip(".py")] = file_with_formatting_options
     return custom_resources
 
 
-def _cleanup_old_files(config, output_dir, env_addons_path):
-    for f in (output_dir / env_addons_path).iterdir():
-        if f.is_file():
-            f.unlink()
+def _cleanup_old_files(config, output_dir, env_addons_path, env_overrides_path):
+    def _rmdir(path):
+        if not path.exists():
+            return
+        for f in path.iterdir():
+            if f.is_file():
+                f.unlink()
+            if f.is_dir():
+                _rmdir(f)
+                f.rmdir()
+
+    _rmdir(output_dir / env_addons_path)
+    _rmdir(output_dir / env_overrides_path)
 
     all_services = set()
     for services in [v["services"] for v in config.values() if "services" in v]:
         all_services.update(services)
 
     for service in all_services:
         svc_addons_dir = Path(output_dir, "copilot", service, "addons")
         if not svc_addons_dir.exists():
             continue
         for f in svc_addons_dir.iterdir():
             if f.is_file():
                 f.unlink()
-
-
-@copilot.command()
-@click.argument("app", type=str, required=True)
-@click.argument("env", type=str, required=True)
-def get_env_secrets(app, env):
-    """List secret names and values for an environment."""
-
-    session = get_aws_session_or_abort()
-    client = session.client("ssm")
-
-    path = SSM_BASE_PATH.format(app=app, env=env)
-
-    params = dict(Path=path, Recursive=False, WithDecryption=True, MaxResults=10)
-    secrets = []
-
-    # TODO: refactor shared code with get_ssm_secret_names
-    while True:
-        response = client.get_parameters_by_path(**params)
-
-        for secret in response["Parameters"]:
-            secrets.append(f"{secret['Name']:<8}: {secret['Value']:<15}")
-
-        if "NextToken" in response:
-            params["NextToken"] = response["NextToken"]
-        else:
-            break
-
-    print("\n".join(sorted(secrets)))
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936813146344396%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'aws-cdk-lib': '2.137.0'}, 'devDependencies': {'aws-cdk': "*

 * *               "'2.137.0'}}, 'node_modules/aws-cdk': {'version': '2.137.0', 'resolved': "*

 * *               "'https://registry.npmjs.org/aws-cdk/-/aws-cdk-2.137.0.tgz', 'integrity': "*

 * *               "'sha512-3pf3SVDwNZvo3EfhO3yl1B+KbRHz7T4UmPifUEKfOwk7ABAFLRSNddZuUlF560XSBTFLkrZoeBDa0/MLJT6F4g=='}, "*

 * *               "'node_modules/aws-cdk-lib': {'version': '2.137.0', 'resolved': "*

 * *               "'https://registry […]*

```diff
@@ -3,23 +3,23 @@
     "name": "override",
     "packages": {
         "": {
             "bin": {
                 "override": "bin/override.js"
             },
             "dependencies": {
-                "aws-cdk-lib": "2.56.0",
+                "aws-cdk-lib": "2.137.0",
                 "constructs": "^10.0.0",
                 "source-map-support": "^0.5.21",
                 "yaml": "^2.3.4"
             },
             "devDependencies": {
                 "@types/jest": "^29.2.4",
                 "@types/node": "18.11.15",
-                "aws-cdk": "2.56.0",
+                "aws-cdk": "2.137.0",
                 "jest": "^29.3.1",
                 "ts-jest": "^29.0.3",
                 "ts-node": "^10.9.1",
                 "typescript": "~4.9.4"
             },
             "name": "override",
             "version": "0.1.0"
@@ -43,18 +43,18 @@
             "version": "2.2.202"
         },
         "node_modules/@aws-cdk/asset-kubectl-v20": {
             "integrity": "sha512-3M2tELJOxQv0apCIiuKQ4pAbncz9GuLwnKFqxifWfe77wuMxyTRPmxssYHs42ePqzap1LT6GDcPygGs+hHstLg==",
             "resolved": "https://registry.npmjs.org/@aws-cdk/asset-kubectl-v20/-/asset-kubectl-v20-2.1.2.tgz",
             "version": "2.1.2"
         },
-        "node_modules/@aws-cdk/asset-node-proxy-agent-v5": {
-            "integrity": "sha512-j0xnccpUQHXJKPgCwQcGGNu4lRiC1PptYfdxBIH1L4dRK91iBxtSQHESRQX+yB47oGLaF/WfNN/aF3WXwlhikg==",
-            "resolved": "https://registry.npmjs.org/@aws-cdk/asset-node-proxy-agent-v5/-/asset-node-proxy-agent-v5-2.0.166.tgz",
-            "version": "2.0.166"
+        "node_modules/@aws-cdk/asset-node-proxy-agent-v6": {
+            "integrity": "sha512-twhuEG+JPOYCYPx/xy5uH2+VUsIEhPTzDY0F1KuB+ocjWWB/KEDiOVL19nHvbPCB6fhWnkykXEMJ4HHcKvjtvg==",
+            "resolved": "https://registry.npmjs.org/@aws-cdk/asset-node-proxy-agent-v6/-/asset-node-proxy-agent-v6-2.0.3.tgz",
+            "version": "2.0.3"
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
                 "@babel/highlight": "^7.23.4",
                 "chalk": "^2.4.2"
             },
             "dev": true,
@@ -1298,69 +1298,110 @@
             "bin": {
                 "cdk": "bin/cdk"
             },
             "dev": true,
             "engines": {
                 "node": ">= 14.15.0"
             },
-            "integrity": "sha512-UjzCnuW5uw10MrzlOqp/cc8dGfTw5Og9YpMWBlCrYA+kVSSS2ikc6aWnk0IM07RQLr9RTvAzXkT2IfVivY3baQ==",
+            "integrity": "sha512-3pf3SVDwNZvo3EfhO3yl1B+KbRHz7T4UmPifUEKfOwk7ABAFLRSNddZuUlF560XSBTFLkrZoeBDa0/MLJT6F4g==",
             "optionalDependencies": {
                 "fsevents": "2.3.2"
             },
-            "resolved": "https://registry.npmjs.org/aws-cdk/-/aws-cdk-2.56.0.tgz",
-            "version": "2.56.0"
+            "resolved": "https://registry.npmjs.org/aws-cdk/-/aws-cdk-2.137.0.tgz",
+            "version": "2.137.0"
         },
         "node_modules/aws-cdk-lib": {
             "bundleDependencies": [
                 "@balena/dockerignore",
                 "case",
                 "fs-extra",
                 "ignore",
                 "jsonschema",
                 "minimatch",
                 "punycode",
                 "semver",
-                "yaml"
+                "table",
+                "yaml",
+                "mime-types"
             ],
             "dependencies": {
-                "@aws-cdk/asset-awscli-v1": "^2.2.30",
-                "@aws-cdk/asset-kubectl-v20": "^2.1.1",
-                "@aws-cdk/asset-node-proxy-agent-v5": "^2.0.38",
+                "@aws-cdk/asset-awscli-v1": "^2.2.202",
+                "@aws-cdk/asset-kubectl-v20": "^2.1.2",
+                "@aws-cdk/asset-node-proxy-agent-v6": "^2.0.1",
                 "@balena/dockerignore": "^1.0.2",
                 "case": "1.6.3",
-                "fs-extra": "^9.1.0",
-                "ignore": "^5.2.1",
+                "fs-extra": "^11.2.0",
+                "ignore": "^5.3.1",
                 "jsonschema": "^1.4.1",
+                "mime-types": "^2.1.35",
                 "minimatch": "^3.1.2",
-                "punycode": "^2.1.1",
-                "semver": "^7.3.8",
+                "punycode": "^2.3.1",
+                "semver": "^7.6.0",
+                "table": "^6.8.2",
                 "yaml": "1.10.2"
             },
             "engines": {
                 "node": ">= 14.15.0"
             },
-            "integrity": "sha512-WFcqPzqiVsRCDGWq+rW2RRKsqg6ijCsDGwPWZmRyTkWurHEFk6BUbU4peRaUw5xeSP/qH9WcL17Tt7CF5Z1UVg==",
+            "integrity": "sha512-pD3AGdKBa8q1+vVWRabiDHuecVMlP8ERGPHc9Pb0dVlpbC/ODC6XXC1S0TAMsr0JI5Lh6pk4vL5cC+spsMeotw==",
             "peerDependencies": {
                 "constructs": "^10.0.0"
             },
-            "resolved": "https://registry.npmjs.org/aws-cdk-lib/-/aws-cdk-lib-2.56.0.tgz",
-            "version": "2.56.0"
+            "resolved": "https://registry.npmjs.org/aws-cdk-lib/-/aws-cdk-lib-2.137.0.tgz",
+            "version": "2.137.0"
         },
         "node_modules/aws-cdk-lib/node_modules/@balena/dockerignore": {
             "inBundle": true,
             "license": "Apache-2.0",
             "version": "1.0.2"
         },
-        "node_modules/aws-cdk-lib/node_modules/at-least-node": {
+        "node_modules/aws-cdk-lib/node_modules/ajv": {
+            "dependencies": {
+                "fast-deep-equal": "^3.1.1",
+                "json-schema-traverse": "^1.0.0",
+                "require-from-string": "^2.0.2",
+                "uri-js": "^4.2.2"
+            },
+            "funding": {
+                "type": "github",
+                "url": "https://github.com/sponsors/epoberezkin"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "8.12.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/ansi-regex": {
             "engines": {
-                "node": ">= 4.0.0"
+                "node": ">=8"
             },
             "inBundle": true,
-            "license": "ISC",
-            "version": "1.0.0"
+            "license": "MIT",
+            "version": "5.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/ansi-styles": {
+            "dependencies": {
+                "color-convert": "^2.0.1"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/ansi-styles?sponsor=1"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.3.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/astral-regex": {
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.0.0"
         },
         "node_modules/aws-cdk-lib/node_modules/balanced-match": {
             "inBundle": true,
             "license": "MIT",
             "version": "1.0.2"
         },
         "node_modules/aws-cdk-lib/node_modules/brace-expansion": {
@@ -1376,45 +1417,83 @@
             "engines": {
                 "node": ">= 0.8.0"
             },
             "inBundle": true,
             "license": "(MIT OR GPL-3.0-or-later)",
             "version": "1.6.3"
         },
+        "node_modules/aws-cdk-lib/node_modules/color-convert": {
+            "dependencies": {
+                "color-name": "~1.1.4"
+            },
+            "engines": {
+                "node": ">=7.0.0"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/color-name": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "1.1.4"
+        },
         "node_modules/aws-cdk-lib/node_modules/concat-map": {
             "inBundle": true,
             "license": "MIT",
             "version": "0.0.1"
         },
+        "node_modules/aws-cdk-lib/node_modules/emoji-regex": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "8.0.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/fast-deep-equal": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "3.1.3"
+        },
         "node_modules/aws-cdk-lib/node_modules/fs-extra": {
             "dependencies": {
-                "at-least-node": "^1.0.0",
                 "graceful-fs": "^4.2.0",
                 "jsonfile": "^6.0.1",
                 "universalify": "^2.0.0"
             },
             "engines": {
-                "node": ">=10"
+                "node": ">=14.14"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "9.1.0"
+            "version": "11.2.0"
         },
         "node_modules/aws-cdk-lib/node_modules/graceful-fs": {
             "inBundle": true,
             "license": "ISC",
-            "version": "4.2.10"
+            "version": "4.2.11"
         },
         "node_modules/aws-cdk-lib/node_modules/ignore": {
             "engines": {
                 "node": ">= 4"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "5.2.1"
+            "version": "5.3.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/is-fullwidth-code-point": {
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "3.0.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/json-schema-traverse": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "1.0.0"
         },
         "node_modules/aws-cdk-lib/node_modules/jsonfile": {
             "dependencies": {
                 "universalify": "^2.0.0"
             },
             "inBundle": true,
             "license": "MIT",
@@ -1427,25 +1506,49 @@
             "engines": {
                 "node": "*"
             },
             "inBundle": true,
             "license": "MIT",
             "version": "1.4.1"
         },
+        "node_modules/aws-cdk-lib/node_modules/lodash.truncate": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.4.2"
+        },
         "node_modules/aws-cdk-lib/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
             "inBundle": true,
             "license": "ISC",
             "version": "6.0.0"
         },
+        "node_modules/aws-cdk-lib/node_modules/mime-db": {
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "1.52.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/mime-types": {
+            "dependencies": {
+                "mime-db": "1.52.0"
+            },
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.1.35"
+        },
         "node_modules/aws-cdk-lib/node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^1.1.7"
             },
             "engines": {
                 "node": "*"
             },
@@ -1455,37 +1558,108 @@
         },
         "node_modules/aws-cdk-lib/node_modules/punycode": {
             "engines": {
                 "node": ">=6"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "2.1.1"
+            "version": "2.3.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/require-from-string": {
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.0.2"
         },
         "node_modules/aws-cdk-lib/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
             "inBundle": true,
             "license": "ISC",
-            "version": "7.3.8"
+            "version": "7.6.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/slice-ansi": {
+            "dependencies": {
+                "ansi-styles": "^4.0.0",
+                "astral-regex": "^2.0.0",
+                "is-fullwidth-code-point": "^3.0.0"
+            },
+            "engines": {
+                "node": ">=10"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/slice-ansi?sponsor=1"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.0.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/string-width": {
+            "dependencies": {
+                "emoji-regex": "^8.0.0",
+                "is-fullwidth-code-point": "^3.0.0",
+                "strip-ansi": "^6.0.1"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.2.3"
+        },
+        "node_modules/aws-cdk-lib/node_modules/strip-ansi": {
+            "dependencies": {
+                "ansi-regex": "^5.0.1"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "6.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/table": {
+            "dependencies": {
+                "ajv": "^8.0.1",
+                "lodash.truncate": "^4.4.2",
+                "slice-ansi": "^4.0.0",
+                "string-width": "^4.2.3",
+                "strip-ansi": "^6.0.1"
+            },
+            "engines": {
+                "node": ">=10.0.0"
+            },
+            "inBundle": true,
+            "license": "BSD-3-Clause",
+            "version": "6.8.2"
         },
         "node_modules/aws-cdk-lib/node_modules/universalify": {
             "engines": {
                 "node": ">= 10.0.0"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "2.0.0"
+            "version": "2.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/uri-js": {
+            "dependencies": {
+                "punycode": "^2.1.0"
+            },
+            "inBundle": true,
+            "license": "BSD-2-Clause",
+            "version": "4.4.1"
         },
         "node_modules/aws-cdk-lib/node_modules/yallist": {
             "inBundle": true,
             "license": "ISC",
             "version": "4.0.0"
         },
         "node_modules/aws-cdk-lib/node_modules/yaml": {
@@ -3574,15 +3748,14 @@
             "resolved": "https://registry.npmjs.org/resolve.exports/-/resolve.exports-2.0.2.tgz",
             "version": "2.0.2"
         },
         "node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
-            "dev": true,
             "integrity": "sha512-BR7VvDCVHO+q2xBEWskxS6DJE1qRnb7DxzUrogb71CWoSficBxYsiAGd+Kl0mmq/MprG9yArRkyrQxTO6XjMzA==",
             "resolved": "https://registry.npmjs.org/semver/-/semver-6.3.1.tgz",
             "version": "6.3.1"
         },
         "node_modules/shebang-command": {
             "dependencies": {
                 "shebang-regex": "^3.0.0"
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9836309523809524%*

 * *Differences: {"'dependencies'": "{'aws-cdk-lib': '2.137.0'}", "'devDependencies'": "{'aws-cdk': '2.137.0'}"}*

```diff
@@ -1,21 +1,21 @@
 {
     "bin": {
         "override": "bin/override.js"
     },
     "dependencies": {
-        "aws-cdk-lib": "2.56.0",
+        "aws-cdk-lib": "2.137.0",
         "constructs": "^10.0.0",
         "source-map-support": "^0.5.21",
         "yaml": "^2.3.4"
     },
     "devDependencies": {
         "@types/jest": "^29.2.4",
         "@types/node": "18.11.15",
-        "aws-cdk": "2.56.0",
+        "aws-cdk": "2.137.0",
         "jest": "^29.3.1",
         "ts-jest": "^29.0.3",
         "ts-node": "^10.9.1",
         "typescript": "~4.9.4"
     },
     "name": "override",
     "scripts": {
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         logResourcePolicy.policyDocument = Fn.sub(JSON.stringify(resource_policy));
     }
 
     private uploadAddonConfiguration() {
         const deployRepoRoot = path.join(process.cwd(), '..', '..', '..');
 
         const addonConfig = parse(readFileSync(
-            path.join(deployRepoRoot, 'addons.yml'),
+            path.join(deployRepoRoot, 'extensions.yml'),
         ).toString('utf-8'));
 
         new cdk.aws_ssm.CfnParameter(this, 'AddonConfig', {
             name: `/copilot/applications/${this.appName}/environments/${this.envName}/addons`,
             type: "String",
             value: JSON.stringify(addonConfig),
         });
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8934201050366065%*

 * *Differences: {"'packages'": "{'': {'version': '0.1.1', 'dependencies': {'aws-cdk-lib': '2.137.0'}, "*

 * *               "'devDependencies': {'aws-cdk': '2.137.0'}}, "*

 * *               "'node_modules/@aws-cdk/asset-awscli-v1': {'version': '2.2.202', 'resolved': "*

 * *               "'https://registry.npmjs.org/@aws-cdk/asset-awscli-v1/-/asset-awscli-v1-2.2.202.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-JqlF0D4+EVugnG5dAsNZMqhu3HW7ehOXm5SDMxMbXNDMdsF0pxtQKNHRl52z1U9igsHmaFpUgSGjbhAJ+0JONg=='}, "*

 * *               " […]*

```diff
@@ -3,30 +3,30 @@
     "name": "override",
     "packages": {
         "": {
             "bin": {
                 "override": "bin/override.js"
             },
             "dependencies": {
-                "aws-cdk-lib": "2.56.0",
+                "aws-cdk-lib": "2.137.0",
                 "constructs": "^10.0.0",
                 "source-map-support": "^0.5.21",
                 "yaml": "^2.3.4"
             },
             "devDependencies": {
                 "@types/jest": "^29.2.4",
                 "@types/node": "18.11.15",
-                "aws-cdk": "2.56.0",
+                "aws-cdk": "2.137.0",
                 "jest": "^29.3.1",
                 "ts-jest": "^29.0.3",
                 "ts-node": "^10.9.1",
                 "typescript": "~4.9.4"
             },
             "name": "override",
-            "version": "0.1.0"
+            "version": "0.1.1"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.3.0",
                 "@jridgewell/trace-mapping": "^0.3.9"
             },
             "dev": true,
@@ -34,27 +34,27 @@
                 "node": ">=6.0.0"
             },
             "integrity": "sha512-lFMjJTrFL3j7L9yBxwYfCq2k6qqwHyzuUl/XBnif78PWTJYyL/dfowQHWE3sp6U6ZzqWiiIZnpTMO96zhkjwtg==",
             "resolved": "https://registry.npmjs.org/@ampproject/remapping/-/remapping-2.2.1.tgz",
             "version": "2.2.1"
         },
         "node_modules/@aws-cdk/asset-awscli-v1": {
-            "integrity": "sha512-INZqcwDinNaIdb5CtW3ez5s943nX5stGBQS6VOP2JDlOFP81hM3fds/9NDknipqfUkZM43dx+HgVvkXYXXARCQ==",
-            "resolved": "https://registry.npmjs.org/@aws-cdk/asset-awscli-v1/-/asset-awscli-v1-2.2.201.tgz",
-            "version": "2.2.201"
+            "integrity": "sha512-JqlF0D4+EVugnG5dAsNZMqhu3HW7ehOXm5SDMxMbXNDMdsF0pxtQKNHRl52z1U9igsHmaFpUgSGjbhAJ+0JONg==",
+            "resolved": "https://registry.npmjs.org/@aws-cdk/asset-awscli-v1/-/asset-awscli-v1-2.2.202.tgz",
+            "version": "2.2.202"
         },
         "node_modules/@aws-cdk/asset-kubectl-v20": {
             "integrity": "sha512-3M2tELJOxQv0apCIiuKQ4pAbncz9GuLwnKFqxifWfe77wuMxyTRPmxssYHs42ePqzap1LT6GDcPygGs+hHstLg==",
             "resolved": "https://registry.npmjs.org/@aws-cdk/asset-kubectl-v20/-/asset-kubectl-v20-2.1.2.tgz",
             "version": "2.1.2"
         },
-        "node_modules/@aws-cdk/asset-node-proxy-agent-v5": {
-            "integrity": "sha512-j0xnccpUQHXJKPgCwQcGGNu4lRiC1PptYfdxBIH1L4dRK91iBxtSQHESRQX+yB47oGLaF/WfNN/aF3WXwlhikg==",
-            "resolved": "https://registry.npmjs.org/@aws-cdk/asset-node-proxy-agent-v5/-/asset-node-proxy-agent-v5-2.0.166.tgz",
-            "version": "2.0.166"
+        "node_modules/@aws-cdk/asset-node-proxy-agent-v6": {
+            "integrity": "sha512-twhuEG+JPOYCYPx/xy5uH2+VUsIEhPTzDY0F1KuB+ocjWWB/KEDiOVL19nHvbPCB6fhWnkykXEMJ4HHcKvjtvg==",
+            "resolved": "https://registry.npmjs.org/@aws-cdk/asset-node-proxy-agent-v6/-/asset-node-proxy-agent-v6-2.0.3.tgz",
+            "version": "2.0.3"
         },
         "node_modules/@babel/code-frame": {
             "dependencies": {
                 "@babel/highlight": "^7.22.13",
                 "chalk": "^2.4.2"
             },
             "dev": true,
@@ -1316,69 +1316,110 @@
             "bin": {
                 "cdk": "bin/cdk"
             },
             "dev": true,
             "engines": {
                 "node": ">= 14.15.0"
             },
-            "integrity": "sha512-UjzCnuW5uw10MrzlOqp/cc8dGfTw5Og9YpMWBlCrYA+kVSSS2ikc6aWnk0IM07RQLr9RTvAzXkT2IfVivY3baQ==",
+            "integrity": "sha512-3pf3SVDwNZvo3EfhO3yl1B+KbRHz7T4UmPifUEKfOwk7ABAFLRSNddZuUlF560XSBTFLkrZoeBDa0/MLJT6F4g==",
             "optionalDependencies": {
                 "fsevents": "2.3.2"
             },
-            "resolved": "https://registry.npmjs.org/aws-cdk/-/aws-cdk-2.56.0.tgz",
-            "version": "2.56.0"
+            "resolved": "https://registry.npmjs.org/aws-cdk/-/aws-cdk-2.137.0.tgz",
+            "version": "2.137.0"
         },
         "node_modules/aws-cdk-lib": {
             "bundleDependencies": [
                 "@balena/dockerignore",
                 "case",
                 "fs-extra",
                 "ignore",
                 "jsonschema",
                 "minimatch",
                 "punycode",
                 "semver",
-                "yaml"
+                "table",
+                "yaml",
+                "mime-types"
             ],
             "dependencies": {
-                "@aws-cdk/asset-awscli-v1": "^2.2.30",
-                "@aws-cdk/asset-kubectl-v20": "^2.1.1",
-                "@aws-cdk/asset-node-proxy-agent-v5": "^2.0.38",
+                "@aws-cdk/asset-awscli-v1": "^2.2.202",
+                "@aws-cdk/asset-kubectl-v20": "^2.1.2",
+                "@aws-cdk/asset-node-proxy-agent-v6": "^2.0.1",
                 "@balena/dockerignore": "^1.0.2",
                 "case": "1.6.3",
-                "fs-extra": "^9.1.0",
-                "ignore": "^5.2.1",
+                "fs-extra": "^11.2.0",
+                "ignore": "^5.3.1",
                 "jsonschema": "^1.4.1",
+                "mime-types": "^2.1.35",
                 "minimatch": "^3.1.2",
-                "punycode": "^2.1.1",
-                "semver": "^7.3.8",
+                "punycode": "^2.3.1",
+                "semver": "^7.6.0",
+                "table": "^6.8.2",
                 "yaml": "1.10.2"
             },
             "engines": {
                 "node": ">= 14.15.0"
             },
-            "integrity": "sha512-WFcqPzqiVsRCDGWq+rW2RRKsqg6ijCsDGwPWZmRyTkWurHEFk6BUbU4peRaUw5xeSP/qH9WcL17Tt7CF5Z1UVg==",
+            "integrity": "sha512-pD3AGdKBa8q1+vVWRabiDHuecVMlP8ERGPHc9Pb0dVlpbC/ODC6XXC1S0TAMsr0JI5Lh6pk4vL5cC+spsMeotw==",
             "peerDependencies": {
                 "constructs": "^10.0.0"
             },
-            "resolved": "https://registry.npmjs.org/aws-cdk-lib/-/aws-cdk-lib-2.56.0.tgz",
-            "version": "2.56.0"
+            "resolved": "https://registry.npmjs.org/aws-cdk-lib/-/aws-cdk-lib-2.137.0.tgz",
+            "version": "2.137.0"
         },
         "node_modules/aws-cdk-lib/node_modules/@balena/dockerignore": {
             "inBundle": true,
             "license": "Apache-2.0",
             "version": "1.0.2"
         },
-        "node_modules/aws-cdk-lib/node_modules/at-least-node": {
+        "node_modules/aws-cdk-lib/node_modules/ajv": {
+            "dependencies": {
+                "fast-deep-equal": "^3.1.1",
+                "json-schema-traverse": "^1.0.0",
+                "require-from-string": "^2.0.2",
+                "uri-js": "^4.2.2"
+            },
+            "funding": {
+                "type": "github",
+                "url": "https://github.com/sponsors/epoberezkin"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "8.12.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/ansi-regex": {
             "engines": {
-                "node": ">= 4.0.0"
+                "node": ">=8"
             },
             "inBundle": true,
-            "license": "ISC",
-            "version": "1.0.0"
+            "license": "MIT",
+            "version": "5.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/ansi-styles": {
+            "dependencies": {
+                "color-convert": "^2.0.1"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/ansi-styles?sponsor=1"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.3.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/astral-regex": {
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.0.0"
         },
         "node_modules/aws-cdk-lib/node_modules/balanced-match": {
             "inBundle": true,
             "license": "MIT",
             "version": "1.0.2"
         },
         "node_modules/aws-cdk-lib/node_modules/brace-expansion": {
@@ -1394,45 +1435,83 @@
             "engines": {
                 "node": ">= 0.8.0"
             },
             "inBundle": true,
             "license": "(MIT OR GPL-3.0-or-later)",
             "version": "1.6.3"
         },
+        "node_modules/aws-cdk-lib/node_modules/color-convert": {
+            "dependencies": {
+                "color-name": "~1.1.4"
+            },
+            "engines": {
+                "node": ">=7.0.0"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/color-name": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "1.1.4"
+        },
         "node_modules/aws-cdk-lib/node_modules/concat-map": {
             "inBundle": true,
             "license": "MIT",
             "version": "0.0.1"
         },
+        "node_modules/aws-cdk-lib/node_modules/emoji-regex": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "8.0.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/fast-deep-equal": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "3.1.3"
+        },
         "node_modules/aws-cdk-lib/node_modules/fs-extra": {
             "dependencies": {
-                "at-least-node": "^1.0.0",
                 "graceful-fs": "^4.2.0",
                 "jsonfile": "^6.0.1",
                 "universalify": "^2.0.0"
             },
             "engines": {
-                "node": ">=10"
+                "node": ">=14.14"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "9.1.0"
+            "version": "11.2.0"
         },
         "node_modules/aws-cdk-lib/node_modules/graceful-fs": {
             "inBundle": true,
             "license": "ISC",
-            "version": "4.2.10"
+            "version": "4.2.11"
         },
         "node_modules/aws-cdk-lib/node_modules/ignore": {
             "engines": {
                 "node": ">= 4"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "5.2.1"
+            "version": "5.3.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/is-fullwidth-code-point": {
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "3.0.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/json-schema-traverse": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "1.0.0"
         },
         "node_modules/aws-cdk-lib/node_modules/jsonfile": {
             "dependencies": {
                 "universalify": "^2.0.0"
             },
             "inBundle": true,
             "license": "MIT",
@@ -1445,25 +1524,49 @@
             "engines": {
                 "node": "*"
             },
             "inBundle": true,
             "license": "MIT",
             "version": "1.4.1"
         },
+        "node_modules/aws-cdk-lib/node_modules/lodash.truncate": {
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.4.2"
+        },
         "node_modules/aws-cdk-lib/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
             "inBundle": true,
             "license": "ISC",
             "version": "6.0.0"
         },
+        "node_modules/aws-cdk-lib/node_modules/mime-db": {
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "1.52.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/mime-types": {
+            "dependencies": {
+                "mime-db": "1.52.0"
+            },
+            "engines": {
+                "node": ">= 0.6"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.1.35"
+        },
         "node_modules/aws-cdk-lib/node_modules/minimatch": {
             "dependencies": {
                 "brace-expansion": "^1.1.7"
             },
             "engines": {
                 "node": "*"
             },
@@ -1473,37 +1576,108 @@
         },
         "node_modules/aws-cdk-lib/node_modules/punycode": {
             "engines": {
                 "node": ">=6"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "2.1.1"
+            "version": "2.3.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/require-from-string": {
+            "engines": {
+                "node": ">=0.10.0"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "2.0.2"
         },
         "node_modules/aws-cdk-lib/node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
             "engines": {
                 "node": ">=10"
             },
             "inBundle": true,
             "license": "ISC",
-            "version": "7.3.8"
+            "version": "7.6.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/slice-ansi": {
+            "dependencies": {
+                "ansi-styles": "^4.0.0",
+                "astral-regex": "^2.0.0",
+                "is-fullwidth-code-point": "^3.0.0"
+            },
+            "engines": {
+                "node": ">=10"
+            },
+            "funding": {
+                "url": "https://github.com/chalk/slice-ansi?sponsor=1"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.0.0"
+        },
+        "node_modules/aws-cdk-lib/node_modules/string-width": {
+            "dependencies": {
+                "emoji-regex": "^8.0.0",
+                "is-fullwidth-code-point": "^3.0.0",
+                "strip-ansi": "^6.0.1"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "4.2.3"
+        },
+        "node_modules/aws-cdk-lib/node_modules/strip-ansi": {
+            "dependencies": {
+                "ansi-regex": "^5.0.1"
+            },
+            "engines": {
+                "node": ">=8"
+            },
+            "inBundle": true,
+            "license": "MIT",
+            "version": "6.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/table": {
+            "dependencies": {
+                "ajv": "^8.0.1",
+                "lodash.truncate": "^4.4.2",
+                "slice-ansi": "^4.0.0",
+                "string-width": "^4.2.3",
+                "strip-ansi": "^6.0.1"
+            },
+            "engines": {
+                "node": ">=10.0.0"
+            },
+            "inBundle": true,
+            "license": "BSD-3-Clause",
+            "version": "6.8.2"
         },
         "node_modules/aws-cdk-lib/node_modules/universalify": {
             "engines": {
                 "node": ">= 10.0.0"
             },
             "inBundle": true,
             "license": "MIT",
-            "version": "2.0.0"
+            "version": "2.0.1"
+        },
+        "node_modules/aws-cdk-lib/node_modules/uri-js": {
+            "dependencies": {
+                "punycode": "^2.1.0"
+            },
+            "inBundle": true,
+            "license": "BSD-2-Clause",
+            "version": "4.4.1"
         },
         "node_modules/aws-cdk-lib/node_modules/yallist": {
             "inBundle": true,
             "license": "ISC",
             "version": "4.0.0"
         },
         "node_modules/aws-cdk-lib/node_modules/yaml": {
@@ -3505,36 +3679,33 @@
         "node_modules/semver": {
             "bin": {
                 "semver": "bin/semver.js"
             },
             "dependencies": {
                 "lru-cache": "^6.0.0"
             },
-            "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-1bCSESV6Pv+i21Hvpxp3Dx+pSD8lIPt8uVjRrxAUt/nbswYc+tK6Y2btiULjd4+fnq15PX+nqQDC7Oft7WkwcA==",
             "resolved": "https://registry.npmjs.org/semver/-/semver-7.5.4.tgz",
             "version": "7.5.4"
         },
         "node_modules/semver/node_modules/lru-cache": {
             "dependencies": {
                 "yallist": "^4.0.0"
             },
-            "dev": true,
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-Jo6dJ04CmSjuznwJSS3pUeWmd/H0ffTlkXXgwZi+eq1UCmqQwCh+eLsYOYCwY991i2Fah4h1BEMCx4qThGbsiA==",
             "resolved": "https://registry.npmjs.org/lru-cache/-/lru-cache-6.0.0.tgz",
             "version": "6.0.0"
         },
         "node_modules/semver/node_modules/yallist": {
-            "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         },
         "node_modules/shebang-command": {
             "dependencies": {
                 "shebang-regex": "^3.0.0"
@@ -4045,9 +4216,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9002976190476191%*

 * *Differences: {"'dependencies'": "{'aws-cdk-lib': '2.137.0'}",*

 * * "'devDependencies'": "{'aws-cdk': '2.137.0'}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -1,27 +1,27 @@
 {
     "bin": {
         "override": "bin/override.js"
     },
     "dependencies": {
-        "aws-cdk-lib": "2.56.0",
+        "aws-cdk-lib": "2.137.0",
         "constructs": "^10.0.0",
         "source-map-support": "^0.5.21",
         "yaml": "^2.3.4"
     },
     "devDependencies": {
         "@types/jest": "^29.2.4",
         "@types/node": "18.11.15",
-        "aws-cdk": "2.56.0",
+        "aws-cdk": "2.137.0",
         "jest": "^29.3.1",
         "ts-jest": "^29.0.3",
         "ts-node": "^10.9.1",
         "typescript": "~4.9.4"
     },
     "name": "override",
     "scripts": {
         "build": "tsc",
         "cdk": "cdk",
         "watch": "tsc -w"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/application.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 import boto3
 import yaml
 from boto3 import Session
 from yaml.parser import ParserError
 
 from dbt_platform_helper.utils.aws import get_aws_session_or_abort
 from dbt_platform_helper.utils.aws import get_profile_name_from_account_id
-from dbt_platform_helper.utils.files import load_and_validate_config
 from dbt_platform_helper.utils.messages import abort_with_error
-from dbt_platform_helper.utils.validation import BOOTSTRAP_SCHEMA
 
 
 class Environment:
     name: str
     account_id: str
     sessions: Dict[str, boto3.Session]
 
@@ -107,25 +105,17 @@
     }
 
     return application
 
 
 def get_application_name():
     app_name = None
-
-    try:
-        app_config = load_and_validate_config("bootstrap.yml", BOOTSTRAP_SCHEMA)
-        app_name = app_config["app"]
-    except (FileNotFoundError, ParserError):
-        pass
-
     try:
-        if app_name is None:
-            app_config = yaml.safe_load(Path("copilot/.workspace").read_text())
-            app_name = app_config["application"]
+        app_config = yaml.safe_load(Path("copilot/.workspace").read_text())
+        app_name = app_config["application"]
     except (FileNotFoundError, ParserError):
         pass
 
     if app_name is None:
-        abort_with_error("No valid bootstrap.yml or copilot/.workspace file found")
+        abort_with_error("Cannot get application name. No copilot/.workspace file found")
 
     return app_name
```

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/aws.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-7.0.0/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/versioning.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import click
 import requests
 
 from dbt_platform_helper.exceptions import IncompatibleMajorVersion
 from dbt_platform_helper.exceptions import IncompatibleMinorVersion
 from dbt_platform_helper.exceptions import ValidationException
+from dbt_platform_helper.utils.files import mkfile
 
 
 def string_version(input_version: Union[Tuple[int, int, int], None]) -> str:
     if input_version is None:
         return "unknown"
     major, minor, patch = input_version
     return ".".join([str(s) for s in [major, minor, patch]])
@@ -139,14 +140,20 @@
 def validate_platform_helper_file_version(template_file_path: str):
     validate_version_compatibility(
         get_file_app_versions()[1],
         get_template_generated_with_version(template_file_path),
     )
 
 
+def generate_platform_helper_version_file(directory="."):
+    base_path = Path(directory)
+    copilot_version = string_version(get_app_versions()[0])
+    click.echo(mkfile(base_path, ".platform-helper-version", f"{copilot_version}"))
+
+
 def check_platform_helper_version_needs_update():
     if not running_as_installed_package() or "PLATFORM_TOOLS_SKIP_VERSION_CHECK" in os.environ:
         return
 
     app_version, app_released_version = get_app_versions()
     message = (
         f"You are running platform-helper v{string_version(app_version)}, upgrade to "
```

### Comparing `dbt_platform_helper-7.0.0/platform_helper.py` & `dbt_platform_helper-8.0.0/platform_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 #!/usr/bin/env python
 
 from importlib.metadata import version
 
 import click
 
 from dbt_platform_helper.commands.application import application as application_commands
-from dbt_platform_helper.commands.bootstrap import bootstrap as bootstrap_commands
 from dbt_platform_helper.commands.check_cloudformation import (
-    check_cloudformation as check_cloudformation_command,
+    check_cloudformation as check_cloudformation_commands,
 )
 from dbt_platform_helper.commands.codebase import codebase as codebase_commands
 from dbt_platform_helper.commands.conduit import conduit as conduit_commands
 from dbt_platform_helper.commands.config import config as config_commands
 from dbt_platform_helper.commands.copilot import copilot as copilot_commands
 from dbt_platform_helper.commands.dns import cdn as cdn_commands
 from dbt_platform_helper.commands.dns import domain as domain_commands
 from dbt_platform_helper.commands.environment import environment as environment_commands
 from dbt_platform_helper.commands.generate import generate as generate_commands
 from dbt_platform_helper.commands.pipeline import pipeline as pipeline_commands
+from dbt_platform_helper.commands.secrets import secrets as secrets_commands
 from dbt_platform_helper.utils.click import ClickDocOptGroup
 
 
 @click.group(cls=ClickDocOptGroup)
 @click.version_option(
     version=version("dbt-platform-helper"),
     message=f"dbt-platform-helper %(version)s",
 )
 def platform_helper():
     pass
 
 
-platform_helper.add_command(bootstrap_commands)
-platform_helper.add_command(check_cloudformation_command)
+platform_helper.add_command(application_commands)
+platform_helper.add_command(cdn_commands)
+platform_helper.add_command(check_cloudformation_commands)
 platform_helper.add_command(codebase_commands)
 platform_helper.add_command(conduit_commands)
 platform_helper.add_command(config_commands)
 platform_helper.add_command(copilot_commands)
 platform_helper.add_command(domain_commands)
-platform_helper.add_command(cdn_commands)
 platform_helper.add_command(environment_commands)
 platform_helper.add_command(generate_commands)
 platform_helper.add_command(pipeline_commands)
-platform_helper.add_command(application_commands)
+platform_helper.add_command(secrets_commands)
 
 if __name__ == "__main__":
     platform_helper()
```

### Comparing `dbt_platform_helper-7.0.0/pyproject.toml` & `dbt_platform_helper-8.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "7.0.0"
+version = "8.0.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
@@ -17,15 +17,15 @@
 platform-helper = "platform_helper:platform_helper"
 
 [tool.poetry.dependencies]
 Jinja2 = "^3.1.3"
 PyYAML = "6.0.1"
 boto3 = "^1.28.24"
 boto3-stubs = "^1.26.148"
-botocore = "^1.29.31"
+botocore = "^1.34.85"
 click = "^8.1.3"
 cloudfoundry-client = "1.35.2"
 mypy-boto3-codebuild = "^1.26.0.post1"
 python = "^3.9"
 schema = "0.7.5"
 cfn-flip = "1.3.0"
 aiohttp = "^3.8.4"
@@ -37,15 +37,15 @@
 prettytable = "^3.9.0"
 semver = "^3.0.2"
 tomlkit = "^0.12.2"
 checkov = "^3.1.67"
 slack-sdk = "^3.27.1"
 
 [tool.poetry.group.dev.dependencies]
-moto = {extras = ["all"], version = "^4.1.12"}
+moto = {extras = ["all"], version = "^5.0.5"}
 pyfakefs = "^5.2.2"
 pytest = "^7.3.1"
 pytest-env = "^0.8.1"
 tox = "^4.6.0"
 pre-commit = "^3.3.3"
 freezegun = "^1.2.2"
 parameterized = "^0.9.0"
```

### Comparing `dbt_platform_helper-7.0.0/PKG-INFO` & `dbt_platform_helper-8.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 7.0.0
+Version: 8.0.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: boto3 (>=1.28.24,<2.0.0)
 Requires-Dist: boto3-stubs (>=1.26.148,<2.0.0)
-Requires-Dist: botocore (>=1.29.31,<2.0.0)
+Requires-Dist: botocore (>=1.34.85,<2.0.0)
 Requires-Dist: certifi (>=2023.07.22,<2024.0.0)
 Requires-Dist: cfn-flip (==1.3.0)
 Requires-Dist: cfn-lint (>=0.86.2,<0.87.0)
 Requires-Dist: checkov (>=3.1.67,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cloudfoundry-client (==1.35.2)
 Requires-Dist: cryptography (>=41.0.3,<43.0.0)
```

