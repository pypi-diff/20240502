# Comparing `tmp/dbt_platform_helper-8.0.0.tar.gz` & `tmp/dbt_platform_helper-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_platform_helper-8.0.0.tar", max compression
+gzip compressed data, was "dbt_platform_helper-8.1.0.tar", max compression
```

## Comparing `dbt_platform_helper-8.0.0.tar` & `dbt_platform_helper-8.1.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1090 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/LICENSE
--rw-r--r--   0        0        0    17094 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/COMMANDS.md
--rw-r--r--   0        0        0     1762 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/README.md
--rw-r--r--   0        0        0        0 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/__init__.py
--rw-r--r--   0        0        0     4522 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/addon-plans.yml
--rw-r--r--   0        0        0     1315 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/addons-template-map.yml
--rw-r--r--   0        0        0        0 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/__init__.py
--rw-r--r--   0        0        0     9957 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/application.py
--rwxr-xr-x   0        0        0     3226 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/check_cloudformation.py
--rw-r--r--   0        0        0    11192 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/codebase.py
--rw-r--r--   0        0        0    12871 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/conduit.py
--rw-r--r--   0        0        0     7953 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/config.py
--rwxr-xr-x   0        0        0    15859 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/copilot.py
--rwxr-xr-x   0        0        0    35037 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/dns.py
--rw-r--r--   0        0        0     8670 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/environment.py
--rw-r--r--   0        0        0      853 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/generate.py
--rw-r--r--   0        0        0     6218 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/pipeline.py
--rwxr-xr-x   0        0        0     3860 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/commands/secrets.py
--rw-r--r--   0        0        0        0 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/custom_resources/__init__.py
--rw-r--r--   0        0        0     2396 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/custom_resources/s3_object.py
--rw-r--r--   0        0        0      342 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/default-extensions.yml
--rw-r--r--   0        0        0      499 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/exceptions.py
--rw-r--r--   0        0        0      369 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/jinja2_tags.py
--rw-r--r--   0        0        0      158 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/config.yml
--rwxr-xr-x   0        0        0      164 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
--rwxr-xr-x   0        0        0      121 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/build.sh
--rwxr-xr-x   0        0        0      123 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/install.sh
--rwxr-xr-x   0        0        0      126 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
--rwxr-xr-x   0        0        0      125 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
--rw-r--r--   0        0        0     1081 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja
--rw-r--r--   0        0        0      618 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addon-instructions.txt
--rw-r--r--   0        0        0      412 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/README.md
--rw-r--r--   0        0        0      734 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
--rw-r--r--   0        0        0    26381 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
--rw-r--r--   0        0        0     6064 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml
--rw-r--r--   0        0        0    10853 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml
--rw-r--r--   0        0        0    25624 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
--rw-r--r--   0        0        0     7613 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
--rw-r--r--   0        0        0     7626 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/s3.yml
--rw-r--r--   0        0        0     3658 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/vpc.yml
--rw-r--r--   0        0        0      956 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
--rw-r--r--   0        0        0     2403 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
--rw-r--r--   0        0        0      893 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
--rw-r--r--   0        0        0     1836 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
--rw-r--r--   0        0        0      197 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/create-codebuild-role.json
--rw-r--r--   0        0        0     1180 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
--rw-r--r--   0        0        0      691 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/manifest.yml
--rw-r--r--   0        0        0      169 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/.gitignore
--rw-r--r--   0        0        0      443 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/README.md
--rw-r--r--   0        0        0      284 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
--rw-r--r--   0        0        0      339 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/cdk.json
--rw-r--r--   0        0        0     1760 2024-04-25 12:44:20.756892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
--rw-r--r--   0        0        0   155387 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package.json
--rw-r--r--   0        0        0     1910 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/stack.ts
--rw-r--r--   0        0        0      710 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
--rw-r--r--   0        0        0      208 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
--rw-r--r--   0        0        0     1959 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
--rw-r--r--   0        0        0      169 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
--rw-r--r--   0        0        0      227 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
--rw-r--r--   0        0        0      287 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
--rw-r--r--   0        0        0      781 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
--rw-r--r--   0        0        0      339 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
--rw-r--r--   0        0        0   152518 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
--rw-r--r--   0        0        0      536 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
--rw-r--r--   0        0        0    20142 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
--rw-r--r--   0        0        0      651 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
--rw-r--r--   0        0        0     1205 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
--rw-r--r--   0        0        0     3178 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
--rw-r--r--   0        0        0     1778 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
--rw-r--r--   0        0        0      617 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
--rw-r--r--   0        0        0      741 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
--rw-r--r--   0        0        0      783 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
--rw-r--r--   0        0        0     2881 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml
--rw-r--r--   0        0        0     3921 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-public.yml
--rw-r--r--   0        0        0      386 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
--rw-r--r--   0        0        0        0 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/__init__.py
--rw-r--r--   0        0        0     3555 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/application.py
--rw-r--r--   0        0        0    10704 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/aws.py
--rw-r--r--   0        0        0     2943 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/click.py
--rw-r--r--   0        0        0     1053 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/cloudformation.py
--rw-r--r--   0        0        0      484 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/cloudfoundry.py
--rw-r--r--   0        0        0     1720 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/files.py
--rw-r--r--   0        0        0      304 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/git.py
--rw-r--r--   0        0        0      507 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/manifests.py
--rw-r--r--   0        0        0      115 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/messages.py
--rw-r--r--   0        0        0      469 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/template.py
--rw-r--r--   0        0        0    17799 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/validation.py
--rw-r--r--   0        0        0     6695 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/dbt_platform_helper/utils/versioning.py
--rwxr-xr-x   0        0        0     1930 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/platform_helper.py
--rw-r--r--   0        0        0     1392 2024-04-25 12:44:20.766892 dbt_platform_helper-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/LICENSE
+-rw-r--r--   0        0        0    17094 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/COMMANDS.md
+-rw-r--r--   0        0        0     1762 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/__init__.py
+-rw-r--r--   0        0        0     4522 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/addon-plans.yml
+-rw-r--r--   0        0        0     1315 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/addons-template-map.yml
+-rw-r--r--   0        0        0        0 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/__init__.py
+-rw-r--r--   0        0        0     9957 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/application.py
+-rwxr-xr-x   0        0        0     3226 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/check_cloudformation.py
+-rw-r--r--   0        0        0    11192 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/codebase.py
+-rw-r--r--   0        0        0    14847 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/conduit.py
+-rw-r--r--   0        0        0     7953 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/config.py
+-rwxr-xr-x   0        0        0    15859 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/copilot.py
+-rwxr-xr-x   0        0        0    35037 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/dns.py
+-rw-r--r--   0        0        0     8670 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/environment.py
+-rw-r--r--   0        0        0      853 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/generate.py
+-rw-r--r--   0        0        0     6218 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/pipeline.py
+-rwxr-xr-x   0        0        0     3860 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/commands/secrets.py
+-rw-r--r--   0        0        0        0 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/custom_resources/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/custom_resources/s3_object.py
+-rw-r--r--   0        0        0      342 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/default-extensions.yml
+-rw-r--r--   0        0        0      499 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/exceptions.py
+-rw-r--r--   0        0        0      369 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/jinja2_tags.py
+-rw-r--r--   0        0        0      158 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/.copilot/config.yml
+-rwxr-xr-x   0        0        0      164 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/.copilot/image_build_run.sh
+-rwxr-xr-x   0        0        0      121 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/.copilot/phases/build.sh
+-rwxr-xr-x   0        0        0      123 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/.copilot/phases/install.sh
+-rwxr-xr-x   0        0        0      126 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/.copilot/phases/post_build.sh
+-rwxr-xr-x   0        0        0      125 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/.copilot/phases/pre_build.sh
+-rw-r--r--   0        0        0     1081 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/COMMANDS.md.jinja
+-rw-r--r--   0        0        0      618 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addon-instructions.txt
+-rw-r--r--   0        0        0      412 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/README.md
+-rw-r--r--   0        0        0      734 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml
+-rw-r--r--   0        0        0    26381 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml
+-rw-r--r--   0        0        0     6064 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/monitoring.yml
+-rw-r--r--   0        0        0    10853 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/opensearch.yml
+-rw-r--r--   0        0        0    25624 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml
+-rw-r--r--   0        0        0     7613 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml
+-rw-r--r--   0        0        0     7626 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/s3.yml
+-rw-r--r--   0        0        0     3658 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/vpc.yml
+-rw-r--r--   0        0        0      956 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml
+-rw-r--r--   0        0        0     2403 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml
+-rw-r--r--   0        0        0      893 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml
+-rw-r--r--   0        0        0     1836 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json
+-rw-r--r--   0        0        0      197 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/create-codebuild-role.json
+-rw-r--r--   0        0        0     1180 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json
+-rw-r--r--   0        0        0      691 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/.gitignore
+-rw-r--r--   0        0        0      443 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/README.md
+-rw-r--r--   0        0        0      284 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/bin/override.ts
+-rw-r--r--   0        0        0      339 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/cdk.json
+-rw-r--r--   0        0        0     1760 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json
+-rw-r--r--   0        0        0   155387 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/package.json
+-rw-r--r--   0        0        0     1910 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/stack.ts
+-rw-r--r--   0        0        0      710 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/tsconfig.json
+-rw-r--r--   0        0        0      208 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/terraform-overrides/cfn.patches.yml
+-rw-r--r--   0        0        0     1959 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml
+-rw-r--r--   0        0        0      169 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/.gitignore
+-rw-r--r--   0        0        0      227 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/bin/override.ts
+-rw-r--r--   0        0        0      287 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.deploy.yml
+-rw-r--r--   0        0        0      781 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml
+-rw-r--r--   0        0        0      339 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/cdk.json
+-rw-r--r--   0        0        0   152518 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json
+-rw-r--r--   0        0        0      536 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json
+-rw-r--r--   0        0        0    20142 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts
+-rw-r--r--   0        0        0      651 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json
+-rw-r--r--   0        0        0     1205 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts
+-rw-r--r--   0        0        0     3178 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml
+-rw-r--r--   0        0        0     1778 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml
+-rw-r--r--   0        0        0      617 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0      741 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html
+-rw-r--r--   0        0        0      783 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html
+-rw-r--r--   0        0        0     2881 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/manifest-backend.yml
+-rw-r--r--   0        0        0     3921 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/manifest-public.yml
+-rw-r--r--   0        0        0      386 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/overrides/cfn.patches.yml
+-rw-r--r--   0        0        0        0 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/__init__.py
+-rw-r--r--   0        0        0     3555 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/application.py
+-rw-r--r--   0        0        0    10297 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/aws.py
+-rw-r--r--   0        0        0     2943 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/click.py
+-rw-r--r--   0        0        0     1053 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/cloudformation.py
+-rw-r--r--   0        0        0      484 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/cloudfoundry.py
+-rw-r--r--   0        0        0     1720 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/files.py
+-rw-r--r--   0        0        0      304 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/git.py
+-rw-r--r--   0        0        0      507 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/manifests.py
+-rw-r--r--   0        0        0      115 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/messages.py
+-rw-r--r--   0        0        0      469 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/template.py
+-rw-r--r--   0        0        0    17799 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/validation.py
+-rw-r--r--   0        0        0     6695 2024-05-02 09:02:35.148631 dbt_platform_helper-8.1.0/dbt_platform_helper/utils/versioning.py
+-rwxr-xr-x   0        0        0     1930 2024-05-02 09:02:35.158631 dbt_platform_helper-8.1.0/platform_helper.py
+-rw-r--r--   0        0        0     1392 2024-05-02 09:02:35.158631 dbt_platform_helper-8.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 dbt_platform_helper-8.1.0/PKG-INFO
```

### Comparing `dbt_platform_helper-8.0.0/LICENSE` & `dbt_platform_helper-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/COMMANDS.md` & `dbt_platform_helper-8.1.0/dbt_platform_helper/COMMANDS.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/README.md` & `dbt_platform_helper-8.1.0/dbt_platform_helper/README.md`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/addon-plans.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/addon-plans.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/addons-template-map.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/addons-template-map.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/application.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/check_cloudformation.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/check_cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/codebase.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/codebase.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/conduit.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/conduit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 import random
 import string
 import subprocess
 import time
+import urllib.parse
 
 import click
 from cfn_tools import dump_yaml
 from cfn_tools import load_yaml
 
+from dbt_platform_helper.commands.copilot import is_terraform_project
 from dbt_platform_helper.utils.application import Application
 from dbt_platform_helper.utils.application import load_application
 from dbt_platform_helper.utils.click import ClickDocOptCommand
 from dbt_platform_helper.utils.versioning import (
     check_platform_helper_version_needs_update,
 )
 
@@ -81,15 +83,15 @@
         if name == addon_name:
             addon_type = config["type"]
 
     if not addon_type or addon_type not in CONDUIT_ADDON_TYPES:
         raise InvalidAddonTypeConduitError(addon_type)
 
     if "postgres" in addon_type:
-        addon_type = addon_type.split("-")[1]
+        addon_type = "postgres"
 
     return addon_type
 
 
 def get_parameter_name(
     app: Application, env: str, addon_type: str, addon_name: str, access: str
 ) -> str:
@@ -149,14 +151,58 @@
         return secrets_manager.describe_secret(SecretId=secret_name)["ARN"]
     except secrets_manager.exceptions.ResourceNotFoundException:
         pass
 
     raise SecretNotFoundConduitError(secret_name)
 
 
+def update_parameter_with_secret(session, parameter_name, secret_arn):
+    ssm_client = session.client("ssm")
+    secrets_manager_client = session.client("secretsmanager")
+    response = ssm_client.get_parameter(Name=parameter_name, WithDecryption=True)
+    parameter_value = response["Parameter"]["Value"]
+
+    parameter_data = json.loads(parameter_value)
+
+    secret_response = secrets_manager_client.get_secret_value(SecretId=secret_arn)
+    secret_value = json.loads(secret_response["SecretString"])
+
+    parameter_data["username"] = urllib.parse.quote(secret_value["username"])
+    parameter_data["password"] = urllib.parse.quote(secret_value["password"])
+
+    updated_parameter_value = json.dumps(parameter_data)
+
+    return updated_parameter_value
+
+
+def create_postgres_admin_task(
+    app: Application, env: str, secret_name: str, task_name: str, addon_type: str, addon_name: str
+):
+    session = app.environments[env].session
+    read_only_secret_name = secret_name + "_READ_ONLY_USER"
+    master_secret_name = (
+        f"/copilot/{app.name}/{env}/secrets/{normalise_secret_name(addon_name)}_RDS_MASTER_ARN"
+    )
+    master_secret_arn = session.client("ssm").get_parameter(
+        Name=master_secret_name, WithDecryption=True
+    )["Parameter"]["Value"]
+    connection_string = update_parameter_with_secret(
+        session, read_only_secret_name, master_secret_arn
+    )
+    subprocess.call(
+        f"copilot task run --app {app.name} --env {env} "
+        f"--task-group-name {task_name} "
+        f"--image {CONDUIT_DOCKER_IMAGE_LOCATION}:{addon_type} "
+        f"--env-vars CONNECTION_SECRET='{connection_string}' "
+        "--platform-os linux "
+        "--platform-arch arm64",
+        shell=True,
+    )
+
+
 def create_addon_client_task(
     app: Application,
     env: str,
     addon_type: str,
     addon_name: str,
     task_name: str,
     access: str,
@@ -164,14 +210,17 @@
     secret_name = f"/copilot/{app.name}/{env}/secrets/{normalise_secret_name(addon_name)}"
 
     if addon_type == "postgres":
         if access == "read":
             secret_name += "_READ_ONLY_USER"
         elif access == "write":
             secret_name += "_APPLICATION_USER"
+        elif access == "admin" and is_terraform_project():
+            create_postgres_admin_task(app, env, secret_name, task_name, addon_type, addon_name)
+            return
 
     subprocess.call(
         f"copilot task run --app {app.name} --env {env} "
         f"--task-group-name {task_name} "
         f"--image {CONDUIT_DOCKER_IMAGE_LOCATION}:{addon_type} "
         f"--secrets CONNECTION_SECRET={get_connection_secret_arn(app, env, secret_name)} "
         "--platform-os linux "
```

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/config.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/config.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/copilot.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/copilot.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/dns.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/dns.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/environment.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/environment.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/generate.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/generate.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/pipeline.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/pipeline.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/commands/secrets.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/custom_resources/s3_object.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/custom_resources/s3_object.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/COMMANDS.md.jinja` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/COMMANDS.md.jinja`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addon-instructions.txt` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addon-instructions.txt`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/addons.parameters.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/aurora-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/monitoring.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/monitoring.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/opensearch.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/opensearch.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/rds-postgres.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/redis-cluster.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/s3.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/s3.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/env/vpc.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/env/vpc.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/svc/appconfig-ipfilter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/svc/s3-policy.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/addons/svc/subscription-filter.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/ci-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/custom-codebuild-role-policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/manifest.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/log_resource_policy.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package-lock.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/package.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/stack.ts` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/env/overrides/tsconfig.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/env/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/buildspec.image.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package-lock.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/package.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/stack.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/tsconfig.json`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/codebase/overrides/types.ts`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/environments/buildspec.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/environments/manifest.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/pipelines/environments/overrides/cfn.patches.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/maintenance_pages/default.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/maintenance_pages/migration.html`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-backend.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/manifest-backend.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/templates/svc/manifest-public.yml` & `dbt_platform_helper-8.1.0/dbt_platform_helper/templates/svc/manifest-public.yml`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/application.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/application.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/aws.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,47 +24,38 @@
     # Check that the aws profile exists and is set.
     click.secho(f"""Checking AWS connection for profile "{aws_profile}"...""", fg="cyan")
 
     try:
         session = boto3.session.Session(profile_name=aws_profile)
     except botocore.exceptions.ProfileNotFound:
         click.secho(f"""AWS profile "{aws_profile}" is not configured.""", fg="red")
-        exit()
-    except botocore.errorfactory.UnauthorizedException:
-        click.secho(
-            "The SSO session associated with this profile has expired or is otherwise invalid.  "
-            "To refresh this SSO session run aws sso login with the corresponding profile",
-            fg="red",
-        )
-        exit()
+        exit(1)
+    except botocore.exceptions.ClientError as e:
+        if e.response["Error"]["Code"] == "ExpiredToken":
+            click.secho(
+                f"Credentials are NOT valid.  \nPlease login with: aws sso login --profile {aws_profile}",
+                fg="red",
+            )
+            exit(1)
 
     sts = session.client("sts")
     try:
         account_id, user_id = get_account_details(sts)
         click.secho("Credentials are valid.", fg="green")
-    except botocore.exceptions.SSOTokenLoadError:
-        click.secho(
-            f"Credentials are NOT valid.  \nPlease login with: aws sso login --profile {aws_profile}",
-            fg="red",
-        )
-        exit()
-    except botocore.exceptions.UnauthorizedSSOTokenError:
-        click.secho(
-            "The SSO session associated with this profile has expired or is otherwise invalid.  "
-            "To refresh this SSO session run aws sso login with the corresponding profile",
-            fg="red",
-        )
-        exit()
-    except botocore.exceptions.TokenRetrievalError:
+    except (
+        botocore.exceptions.UnauthorizedSSOTokenError,
+        botocore.exceptions.TokenRetrievalError,
+        botocore.exceptions.SSOTokenLoadError,
+    ):
         click.secho(
-            "The SSO Token associated with this profile has expired.  "
+            "The SSO session associated with this profile has expired or is otherwise invalid."
             "To refresh this SSO session run `aws sso login` with the corresponding profile",
             fg="red",
         )
-        exit()
+        exit(1)
 
     alias_client = session.client("iam")
     account_name = alias_client.list_account_aliases()["AccountAliases"]
     if account_name:
         click.echo(
             click.style("Logged in with AWS account: ", fg="yellow")
             + click.style(f"{account_name[0]}/{account_id}", fg="white", bold=True),
```

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/click.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/click.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/cloudformation.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/cloudformation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/files.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/files.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/validation.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/dbt_platform_helper/utils/versioning.py` & `dbt_platform_helper-8.1.0/dbt_platform_helper/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/platform_helper.py` & `dbt_platform_helper-8.1.0/platform_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_platform_helper-8.0.0/pyproject.toml` & `dbt_platform_helper-8.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 100
 
 [tool.poetry]
 name = "dbt-platform-helper"
-version = "8.0.0"
+version = "8.1.0"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "dbt_platform_helper/README.md"
 packages = [
     { include = "dbt_platform_helper" },
     { include = "platform_helper.py" }
```

### Comparing `dbt_platform_helper-8.0.0/PKG-INFO` & `dbt_platform_helper-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-platform-helper
-Version: 8.0.0
+Version: 8.1.0
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

