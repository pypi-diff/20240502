# Comparing `tmp/laktory-0.1.9.tar.gz` & `tmp/laktory-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laktory-0.1.9.tar", last modified: Wed Apr 17 05:20:29 2024, max compression
+gzip compressed data, was "laktory-0.2.0.tar", last modified: Thu May  2 06:11:56 2024, max compression
```

## Comparing `laktory-0.1.9.tar` & `laktory-0.2.0.tar`

### file list

```diff
@@ -1,337 +1,493 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.630675 laktory-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.570675 laktory-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/ISSUE_TEMPLATE/bug.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/ISSUE_TEMPLATE/feature.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/scripts/bump_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/scripts/write_release_body.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/workflows/publish-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 05:20:21.000000 laktory-0.1.9/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-17 05:20:21.000000 laktory-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-17 05:20:21.000000 laktory-0.1.9/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-17 05:20:21.000000 laktory-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-17 05:20:21.000000 laktory-0.1.9/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-17 05:20:29.626675 laktory-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 05:20:21.000000 laktory-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.570675 laktory-0.1.9/bundles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.578675 laktory-0.1.9/bundles/stocks/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-17 05:20:21.000000 laktory-0.1.9/bundles/stocks/databricks.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:21.000000 laktory-0.1.9/bundles/stocks/template_brz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/cli.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/api/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/apply_changes.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/get_df.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/is_debug.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/is_mocked.md
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/read.md
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/dlt/read_stream.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.582675 laktory-0.1.9/docs/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/basemodel.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/accesscontrol.md
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/cluster.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/directory.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/externallocation.md
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/grants.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/group.md
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/job.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/metastore.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/metastoreassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/metastoredataaccess.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/mwspermissionassignment.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/notebook.md
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/secret.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/secretacl.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/secretscope.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/serviceprincipal.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/serviceprincipalrole.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/sqlquery.md
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/user.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/userrole.md
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/warehouse.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/databricks/workspacefile.md
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/dataeventheader.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/dataproducer.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/datasources/basedatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/datasources/eventdatasource.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/datasources/tabledatasource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/aws.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/azure.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/azurepulumi.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/providers/databricks.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.586675 laktory-0.1.9/docs/api/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/resources/baseresource.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/resources/pulumiresource.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/resources/terraformresource.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/column.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tableaggregation.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tableexpectation.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tablejoin.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/tablewindowfilter.md
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/sql/volume.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/stacks/pulumistack.md
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/stacks/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/models/stacks/terraformstack.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.574675 laktory-0.1.9/docs/api/spark/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/dataframe/has_column.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/dataframe/schema_flat.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/dataframe/show_string.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.590675 laktory-0.1.9/docs/api/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/_constants.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/add.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/convert_units.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/div.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/mul.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/poly1.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/poly2.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/roundp.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/scaled_power.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/string_split.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/sub.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/api/spark/functions/uuid.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.594675 laktory-0.1.9/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/dataevent.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/deployment.md
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/governance.md
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/models.md
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/spark.md
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/stack.md
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/table.md
--rw-r--r--   0 runner    (1001) docker     (127)     9175 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/tablebuilder.md
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/concepts/variables.md
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/demos.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.594675 laktory-0.1.9/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/catalog.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/compute.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/job.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/secrets.md
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/table.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/guides/users.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.602675 laktory-0.1.9/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/databricks.png
--rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/delta_live_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/dlt_debug.png
--rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/kappa.png
--rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/lakehouse.png
--rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sg.png
--rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sg_ltb.png
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sw.png
--rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/logo_sw_ltw.png
--rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/medaillon_complex.png
--rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/medallion.png
--rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/okube.png
--rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pl_quickstart.png
--rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pl_stock_prices.png
--rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pl_stock_prices_simple.png
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/pulumi.png
--rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/stock_prices_lineage.png
--rw-r--r--   0 runner    (1001) docker     (127)    83413 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/table_builder.png
--rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/terraform.png
--rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/images/what_is_laktory.png
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/lakehouseascode.md
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.602675 laktory-0.1.9/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-17 05:20:21.000000 laktory-0.1.9/docs/stylesheets/mkdocstrings.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.602675 laktory-0.1.9/laktory/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/_testing/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_testing/stackvalidator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_testing/stockprices.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/cli/_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    19933 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/cli/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/dlt/
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/dlt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/models/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.606675 laktory-0.1.9/laktory/models/azurenative/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/azurenative/storageblob.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/basemodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.610675 laktory-0.1.9/laktory/models/databricks/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/accesscontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/externallocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/groupmember.py
--rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/metastoreassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/metastoredataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/mwspermissionassignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/secretacl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/secretscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/serviceprincipal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/serviceprincipalrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/sqlquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/userrole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/databricks/workspacefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/dataeventheader.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/dataproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.610675 laktory-0.1.9/laktory/models/datasources/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/basedatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/eventdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/datasources/tabledatasource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.614675 laktory-0.1.9/laktory/models/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/cataloggrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/connectiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/externallocationgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/functiongrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/metastoregrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/registeredmodelgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/schemagrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/sharegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/storagecredentialgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/tablegrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/viewgrant.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/grants/volumegrant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.614675 laktory-0.1.9/laktory/models/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/awsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/azureprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/azurepulumiprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/baseprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/providers/databricksprovider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.614675 laktory-0.1.9/laktory/models/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4021 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/pulumiresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/resources/terraformresource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/models/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tableaggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14918 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tablebuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tableexpectation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tablejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tableunion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/tablewindowfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/sql/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/models/stacks/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/pulumistack.py
--rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/models/stacks/terraformstack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.574675 laktory-0.1.9/laktory/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/resources/data/
--rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/data/stock_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/resources/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_brz_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_gld_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_slv_star_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/resources/notebooks/dlt_slv_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/spark/dataframe/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/has_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/schema_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/dataframe/show_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/laktory/spark/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/logical.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/spark/functions/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-17 05:20:21.000000 laktory-0.1.9/laktory/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.626675 laktory-0.1.9/laktory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 05:20:29.000000 laktory-0.1.9/laktory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-17 05:20:21.000000 laktory-0.1.9/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-17 05:20:21.000000 laktory-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-17 05:20:21.000000 laktory-0.1.9/scripts/test_computed_filed.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-17 05:20:21.000000 laktory-0.1.9/scripts/test_db_connect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.618675 laktory-0.1.9/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 05:20:21.000000 laktory-0.1.9/settings/dev.env
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 05:20:29.630675 laktory-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:29.626675 laktory-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stack_empty.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stockprices0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stockprices1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/stockprices2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_baseresource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_dataevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_dbfsfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_dlt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_spark_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_spark_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    26375 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    17066 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    16683 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_table_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_version_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-17 05:20:21.000000 laktory-0.1.9/tests/test_workspacefile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.869662 laktory-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/ISSUE_TEMPLATE/bug.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/ISSUE_TEMPLATE/feature.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/scripts/bump_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/scripts/update_quickstart_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/scripts/write_release_body.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/publish-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/run_quickstart.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-02 06:11:47.000000 laktory-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-02 06:11:47.000000 laktory-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11423 2024-05-02 06:11:47.000000 laktory-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 06:11:47.000000 laktory-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-02 06:11:47.000000 laktory-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-02 06:11:56.957663 laktory-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-02 06:11:47.000000 laktory-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.881662 laktory-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/datetime.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/dispatcher.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/dispatcherrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/jobrunner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dispatcher/pipelinerunner.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/apply_changes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/get_df.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/is_debug.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/is_mocked.md
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/read.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/dlt/read_stream.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.885662 laktory-0.2.0/docs/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/basemodel.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.889662 laktory-0.2.0/docs/api/models/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/accesscontrol.md
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/cluster.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/directory.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/externallocation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/grants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/group.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/metastore.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/metastoreassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/metastoredataaccess.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/mwspermissionassignment.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/notebook.md
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/secretacl.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/secretscope.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/serviceprincipal.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/serviceprincipalrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/sqlquery.md
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/userrole.md
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/warehouse.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/databricks/workspacefile.md
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/dataeventheader.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/dataproducer.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.889662 laktory-0.2.0/docs/api/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/datasources/basedatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/datasources/eventdatasource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/datasources/tabledatasource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.889662 laktory-0.2.0/docs/api/models/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/aws.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/azure.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/azurepulumi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/providers/databricks.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/resources/baseresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/resources/pulumiresource.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/resources/terraformresource.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/spark/sparkchain.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/spark/sparkchainnode.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/spark/sparkfuncarg.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/tablebuilder.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/tableexpectation.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/sql/volume.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/stacks/pulumistack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/stacks/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/models/stacks/terraformstack.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.869662 laktory-0.2.0/docs/api/spark/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.893662 laktory-0.2.0/docs/api/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/groupby_and_agg.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/has_column.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/schema_flat.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/show_string.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/smart_join.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/dataframe/window_filter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.897662 laktory-0.2.0/docs/api/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/_constants.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/add.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/convert_units.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/div.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/mul.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/poly1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/poly2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/roundp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/scaled_power.md
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/string_split.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/sub.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/api/spark/functions/uuid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.897662 laktory-0.2.0/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/dataevent.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/deployment.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/governance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/models.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/spark.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/stack.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/tablebuilder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/concepts/variables.md
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/demos.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.901662 laktory-0.2.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/catalog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/compute.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/job.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/secrets.md
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/table.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/guides/users.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.905662 laktory-0.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    20095 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/databricks.png
+-rw-r--r--   0 runner    (1001) docker     (127)   588404 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/delta_live_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)   187140 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/dlt_debug.png
+-rw-r--r--   0 runner    (1001) docker     (127)   307164 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/kappa.png
+-rw-r--r--   0 runner    (1001) docker     (127)   118303 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/lakehouse.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24669 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41747 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sg_ltb.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sw.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41214 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/logo_sw_ltw.png
+-rw-r--r--   0 runner    (1001) docker     (127)   644132 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/medaillon_complex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   449508 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/medallion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48171 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/okube.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92500 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pl_quickstart.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168057 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pl_stock_prices.png
+-rw-r--r--   0 runner    (1001) docker     (127)   153436 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pl_stock_prices_simple.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/pulumi.png
+-rw-r--r--   0 runner    (1001) docker     (127)   197565 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/stock_prices_lineage.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13352 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/terraform.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58734 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/images/what_is_laktory.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/lakehouseascode.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.909663 laktory-0.2.0/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 06:11:47.000000 laktory-0.2.0/docs/stylesheets/mkdocstrings.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.909663 laktory-0.2.0/laktory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.909663 laktory-0.2.0/laktory/_testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_testing/stackvalidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_testing/stockprices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/cli/quickstart_stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2702 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/dispatcherrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/jobrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dispatcher/pipelinerunner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/dlt/
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/dlt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.913663 laktory-0.2.0/laktory/models/azurenative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/azurenative/storageblob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/basemodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.921663 laktory-0.2.0/laktory/models/databricks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/accesscontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/externallocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/groupmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24518 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/metastoreassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/metastoredataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/mwspermissionassignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13523 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/secretacl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/secretscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/serviceprincipal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/serviceprincipalrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/sqlquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/userrole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/databricks/workspacefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14591 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/dataeventheader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/dataproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.921663 laktory-0.2.0/laktory/models/datasources/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/basedatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/eventdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/datasources/tabledatasource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.921663 laktory-0.2.0/laktory/models/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/cataloggrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/connectiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/externallocationgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/functiongrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/metastoregrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/registeredmodelgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/schemagrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/sharegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/storagecredentialgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/tablegrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/viewgrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/grants/volumegrant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.925663 laktory-0.2.0/laktory/models/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/awsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6033 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/azureprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/azurepulumiprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/baseprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/providers/databricksprovider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.925663 laktory-0.2.0/laktory/models/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/pulumiresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/resources/terraformresource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.925663 laktory-0.2.0/laktory/models/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/sparkchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/sparkchainnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/spark/sparkfuncarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/tablebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/tableexpectation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/sql/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/models/stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/pulumistack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18667 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/models/stacks/terraformstack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.873662 laktory-0.2.0/laktory/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    10909 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/data/stock_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/resources/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_brz_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_gld_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_slv_star_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/resources/notebooks/dlt_slv_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.929663 laktory-0.2.0/laktory/spark/dataframe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/groupby_and_agg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/has_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/schema_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/show_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/smart_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/dataframe/window_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.933663 laktory-0.2.0/laktory/spark/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/logical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/spark/functions/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-02 06:11:47.000000 laktory-0.2.0/laktory/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/laktory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18899 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:56.000000 laktory-0.2.0/laktory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-05-02 06:11:47.000000 laktory-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-02 06:11:47.000000 laktory-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.933663 laktory-0.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 06:11:47.000000 laktory-0.2.0/scripts/databricks_api_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-02 06:11:47.000000 laktory-0.2.0/scripts/test_computed_filed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-02 06:11:47.000000 laktory-0.2.0/scripts/test_db_connect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.933663 laktory-0.2.0/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 06:11:47.000000 laktory-0.2.0/settings/dev.env
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:11:56.957663 laktory-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.937663 laktory-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/build_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/brz_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/.part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/brz_stock_prices/part-00000-aff20661-c55f-4489-86fc-8336e06ee376-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.877662 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_AMZN_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_GOOGL_20230901T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/01/stock_price_MSFT_20230901T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AAPL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_AMZN_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_GOOGL_20230905T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/05/stock_price_MSFT_20230905T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AAPL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_AMZN_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_GOOGL_20230906T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/06/stock_price_MSFT_20230906T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.941663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AAPL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_AMZN_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_GOOGL_20230907T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/07/stock_price_MSFT_20230907T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AAPL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_AMZN_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_GOOGL_20230908T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/08/stock_price_MSFT_20230908T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AAPL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_AMZN_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_GOOGL_20230911T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/11/stock_price_MSFT_20230911T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AAPL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_AMZN_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_GOOGL_20230912T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/12/stock_price_MSFT_20230912T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AAPL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_AMZN_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_GOOGL_20230913T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/13/stock_price_MSFT_20230913T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.945663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AAPL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_AMZN_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_GOOGL_20230914T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/14/stock_price_MSFT_20230914T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AAPL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_AMZN_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_GOOGL_20230915T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/15/stock_price_MSFT_20230915T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AAPL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_AMZN_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_GOOGL_20230918T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/18/stock_price_MSFT_20230918T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AAPL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_AMZN_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_GOOGL_20230919T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/19/stock_price_MSFT_20230919T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AAPL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_AMZN_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_GOOGL_20230920T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/20/stock_price_MSFT_20230920T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.949663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AAPL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_AMZN_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_GOOGL_20230921T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/21/stock_price_MSFT_20230921T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AAPL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_AMZN_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_GOOGL_20230922T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/22/stock_price_MSFT_20230922T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AAPL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_AMZN_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_GOOGL_20230925T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/25/stock_price_MSFT_20230925T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AAPL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_AMZN_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_GOOGL_20230926T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/26/stock_price_MSFT_20230926T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AAPL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_AMZN_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_GOOGL_20230927T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/27/stock_price_MSFT_20230927T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AAPL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_AMZN_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_GOOGL_20230928T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/28/stock_price_MSFT_20230928T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.953663 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AAPL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_AMZN_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_GOOGL_20230929T000000000Z.json
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/events/yahoo-finance/stock_price/2023/09/29/stock_price_MSFT_20230929T000000000Z.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/tests/data/slv_stock_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/.part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_meta/part-00000-d86fbfe6-5d98-43f6-827b-c18d9f79622f-c000.snappy.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:56.957663 laktory-0.2.0/tests/data/slv_stock_prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/.part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/slv_stock_prices/part-00000-d12f5de4-d8dd-46fc-b00a-c3c7dc6edc32-c000.snappy.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stack_empty.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stockprices0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stockprices1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/data/stockprices2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_baseresource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dataevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dbfsfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_dlt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_spark_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_spark_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_spark_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26494 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_table_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-02 06:11:47.000000 laktory-0.2.0/tests/test_workspacefile.py
```

### Comparing `laktory-0.1.9/.github/ISSUE_TEMPLATE/bug.yaml` & `laktory-0.2.0/.github/ISSUE_TEMPLATE/bug.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/.github/ISSUE_TEMPLATE/feature.yaml` & `laktory-0.2.0/.github/ISSUE_TEMPLATE/feature.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/.github/scripts/bump_version.py` & `laktory-0.2.0/.github/scripts/bump_version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/.github/scripts/write_release_body.py` & `laktory-0.2.0/.github/scripts/write_release_body.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/.github/workflows/release.yml` & `laktory-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/.github/workflows/test.yml` & `laktory-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/CHANGELOG.md` & `laktory-0.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,39 @@
 # Release History
 
-## [0.1.9] - Unreleased
+## [0.2.0] - Unreleased
+### Added
+* `SparkChain` a high level class allowing to declare and execute spark operations on a dataframe 
+* `SparkColumnNode` the node of a `SparkChain` that builds a new column
+* `SparkTableNode` the node of a `SparkChain` that returns a new DataFrame
+* Moved `filter`, `selects` and `watermarks` properties to `models.BaseDataSource` so that it can be used for all source types
+* `models.BaseDataSource` `renames` attribute for renaming columns of the source table
+* `models.BaseDataSource` `drops` attribute for dropping columns of the source table
+* spark DataFrame `watermark` returns the watermark column and threshold if any 
+* spark DataFrame `smart_join` joins, cleans duplicated columns and supports watermarking 
+* spark DataFrame `groupby_and_agg` groupby and aggregates in a single function 
+* spark DataFrame `window_filter` takes the first n rows over a window 
+### Updated
+* n/a
+### Breaking changes
+* Refactored table builder to use SparkChain instead of direct definitions of joins, unions, columns building, etc.
+
+## [0.1.10] - 2024-04-23
+### Added
+* CLI `run` command to execute remote jobs and pipelines and monitor errors until completion
+* `Dispatcher` class to manage and run remote jobs
+* `JobRunner` class to run remote jobs
+* `PipelineRunner` class to run remote pipelines
+* datetime utilities
+### Updated
+* Environment variables `DATABRICKS_SDK_UPSTREAM` and `DATABRICKS_SDK_UPSTREAM_VERSION` to track laktory metrics as a Databricks partner
+### Fixed
+* Permissions resource dependencies on `DbfsFile` and `WorkspaceFile`.
+
+## [0.1.9] - 2024-04-17
 ### Added
 * Support for table unions in table builder
 * New column property `raise_missing_arg_exception` to allow for some spark function inputs to be missing
 * `add`, `sub`, `mul` and `div` spark functions
 
 ### Breaking Change
 * Renamed `power` spark function to `scaled_power` to prevent conflict with native spark function
```

### Comparing `laktory-0.1.9/LICENSE` & `laktory-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/PKG-INFO` & `laktory-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.1.9
+Version: 0.2.0
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
@@ -14,22 +14,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: databricks-sdk
 Requires-Dist: inflect
 Requires-Dist: planck
 Requires-Dist: prompt_toolkit
 Requires-Dist: pulumi
-Requires-Dist: pulumi_databricks
+Requires-Dist: pulumi_databricks>=1.36
 Requires-Dist: pulumi_random
 Requires-Dist: pyyaml
 Requires-Dist: pydantic>=2
+Requires-Dist: python-dateutil
 Requires-Dist: settus
 Requires-Dist: typer[all]
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flit; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
@@ -99,23 +101,25 @@
     catalog_name="prod",
     schema_name="finance",
     timestamp_key="data.created_at",
     builder={
         "layer": "SILVER",
         "table_source": {
             "name": "brz_stock_prices",
+        },
+        "spark_chain": {
+            "nodes": [
+                {
+                    "column": {"name": "symbol"},
+                    "type": "string",
+                    "sql_expression": "data.symbol"
+                }
+            ]
         }
     },
-    columns=[
-        {
-            "name": "symbol",
-            "type": "string",
-            "sql_expression": "data.symbol"
-        }
-    ]
 )
 
 print(table)
 #> catalog_name='prod' columns=[Column(catalog_name='prod', comment=None, name='symbol', pii=None, schema_name='finance', spark_func_args=[], spark_func_kwargs={}, spark_func_name=None, sql_expression='data.symbol', table_name='brz_stock_prices', type='string', unit=None)] comment=None data=None grants=None name='brz_stock_prices' primary_key=None schema_name='finance' timestamp_key='data.created_at' builder=TableBuilder(drop_source_columns=True, drop_duplicates=None, event_source=None, joins=[], pipeline_name=None, table_source=TableDataSource(read_as_stream=True, catalog_name='prod', cdc=None, selects=None, filter=None, from_pipeline=True, name='brz_stock_prices', schema_name='finance', watermark=None), layer='SILVER')
 ```
 
 To get started with a more useful example, jump into the [Quickstart](https://www.laktory.ai/quickstart/).
```

### Comparing `laktory-0.1.9/README.md` & `laktory-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,23 +40,25 @@
     catalog_name="prod",
     schema_name="finance",
     timestamp_key="data.created_at",
     builder={
         "layer": "SILVER",
         "table_source": {
             "name": "brz_stock_prices",
+        },
+        "spark_chain": {
+            "nodes": [
+                {
+                    "column": {"name": "symbol"},
+                    "type": "string",
+                    "sql_expression": "data.symbol"
+                }
+            ]
         }
     },
-    columns=[
-        {
-            "name": "symbol",
-            "type": "string",
-            "sql_expression": "data.symbol"
-        }
-    ]
 )
 
 print(table)
 #> catalog_name='prod' columns=[Column(catalog_name='prod', comment=None, name='symbol', pii=None, schema_name='finance', spark_func_args=[], spark_func_kwargs={}, spark_func_name=None, sql_expression='data.symbol', table_name='brz_stock_prices', type='string', unit=None)] comment=None data=None grants=None name='brz_stock_prices' primary_key=None schema_name='finance' timestamp_key='data.created_at' builder=TableBuilder(drop_source_columns=True, drop_duplicates=None, event_source=None, joins=[], pipeline_name=None, table_source=TableDataSource(read_as_stream=True, catalog_name='prod', cdc=None, selects=None, filter=None, from_pipeline=True, name='brz_stock_prices', schema_name='finance', watermark=None), layer='SILVER')
 ```
 
 To get started with a more useful example, jump into the [Quickstart](https://www.laktory.ai/quickstart/).
```

### Comparing `laktory-0.1.9/docs/api/models/databricks/cluster.md` & `laktory-0.2.0/docs/api/models/databricks/cluster.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/api/models/databricks/grants.md` & `laktory-0.2.0/docs/api/models/databricks/grants.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/api/models/databricks/job.md` & `laktory-0.2.0/docs/api/models/databricks/job.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/api/models/databricks/metastoredataaccess.md` & `laktory-0.2.0/docs/api/models/databricks/metastoredataaccess.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/dataevent.md` & `laktory-0.2.0/docs/concepts/dataevent.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/deployment.md` & `laktory-0.2.0/docs/concepts/deployment.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/design.md` & `laktory-0.2.0/docs/concepts/design.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/governance.md` & `laktory-0.2.0/docs/concepts/governance.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/models.md` & `laktory-0.2.0/docs/concepts/models.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/pipeline.md` & `laktory-0.2.0/docs/concepts/pipeline.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ![dlt](../images/delta_live_tables.png)
 
 ## Tables
 The added value of using Laktory for setting up Delta Live Tables is the ability to not only select the notebooks associated with the pipeline, but also directly declares the expected tables and columns.
 Each bronze and silver table will be built using a definition from the configuration file and a template notebook.
 
 First, let's have a look at the notebook template for silver tables:
+
 ```py title="dlt_slv_template.py"
 from laktory import dlt
 from laktory import read_metadata
 from laktory import get_logger
 
 dlt.spark = spark
 logger = get_logger(__name__)
@@ -111,38 +112,43 @@
   - name: slv_stock_prices
     timestamp_key: created_at
     builder:
       layer: SILVER
       table_source:
         name: brz_stock_prices
         read_as_stream: True
-    columns:
-      - name: created_at
-        type: timestamp
-        spark_func_name: coalesce
-        spark_func_args:
-          - data._created_at
-
-      - name: symbol
-        type: string
-        spark_func_name: coalesce
-        spark_func_args:
-          - data.symbol
-
-      - name: open
-        type: double
-        spark_func_name: coalesce
-        spark_func_args:
-          - data.open
-
-      - name: close
-        type: double
-        spark_func_name: coalesce
-        spark_func_args:
-          - data.close
+      spark_chain:
+        nodes:
+          - column:
+              name: created_at
+              type: timestamp
+            spark_func_name: coalesce
+            spark_func_args:
+              - data._created_at
+    
+          - column:
+              name: symbol
+              type: string
+            spark_func_name: coalesce
+            spark_func_args:
+              - data.symbol
+    
+          - column:
+              name: open
+              type: double
+            spark_func_name: coalesce
+            spark_func_args:
+              - data.open
+    
+          - column:
+              name: close
+              type: double
+            spark_func_name: coalesce
+            spark_func_args:
+              - data.close
 ```
  
 As you can see:
 
 * Each bronze and silver table is explicitly defined, including:
     * The source of data
     * The desired output columns
```

### Comparing `laktory-0.1.9/docs/concepts/spark.md` & `laktory-0.2.0/docs/concepts/spark.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import laktory.spark.functions as LF
 
 df = spark.createDataFrame(pd.DataFrame({"x": [1, 2, 3]}))
 df = df.withColumn("y", LF.poly1("x", -1, 1.0))
 ```
 These functions are by default available when declaring a column in a pipeline `Table` model.
 
-## DataFrame
+## DataFrame methods
 In this case the methods are designed to be applied directly on a spark dataframe.
 ```py
 import pandas as pd
 from laktory.spark.dataframe import has_column
 
 df = spark.createDataFrame(pd.DataFrame({"x": [1, 2, 3]}))
 has_column(df, "x")
@@ -33,7 +33,13 @@
 you can also do the following to get the same results
 ```py
 import pandas as pd
 
 df = spark.createDataFrame(pd.DataFrame({"x": [1, 2, 3]}))
 df.has_column("x")
 ```
+
+Some methods of interest are:
+
+- [`laktory.spark.dataframe.groupby_and_agg`](../api/spark/dataframe/groupby_and_agg.md): Apply a groupby and create aggregation columns.
+- [`laktory.spark.dataframe.smart_join`](../api/spark/dataframe/smart_join.md): Join tables, clean up duplicated columns and support watermarking for streaming joins. This is the recommended spark function for all joins defined in pipelines.
+- [`laktory.spark.dataframe.window_filter`](../api/spark/dataframe/window_filter.md): Apply spark window-based filtering
```

### Comparing `laktory-0.1.9/docs/concepts/stack.md` & `laktory-0.2.0/docs/concepts/stack.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/table.md` & `laktory-0.2.0/docs/concepts/table.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/concepts/variables.md` & `laktory-0.2.0/docs/concepts/variables.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/databricks.png` & `laktory-0.2.0/docs/images/databricks.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/delta_live_tables.png` & `laktory-0.2.0/docs/images/delta_live_tables.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/dlt_debug.png` & `laktory-0.2.0/docs/images/dlt_debug.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/kappa.png` & `laktory-0.2.0/docs/images/kappa.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/lakehouse.png` & `laktory-0.2.0/docs/images/lakehouse.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/logo_sg.png` & `laktory-0.2.0/docs/images/logo_sg.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/logo_sg_ltb.png` & `laktory-0.2.0/docs/images/logo_sg_ltb.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/logo_sw.png` & `laktory-0.2.0/docs/images/logo_sw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/logo_sw_ltw.png` & `laktory-0.2.0/docs/images/logo_sw_ltw.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/medaillon_complex.png` & `laktory-0.2.0/docs/images/medaillon_complex.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/medallion.png` & `laktory-0.2.0/docs/images/medallion.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/okube.png` & `laktory-0.2.0/docs/images/okube.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/pl_quickstart.png` & `laktory-0.2.0/docs/images/pl_quickstart.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/pl_stock_prices.png` & `laktory-0.2.0/docs/images/pl_stock_prices.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/pl_stock_prices_simple.png` & `laktory-0.2.0/docs/images/pl_stock_prices_simple.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/pulumi.png` & `laktory-0.2.0/docs/images/pulumi.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/stock_prices_lineage.png` & `laktory-0.2.0/docs/images/stock_prices_lineage.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/terraform.png` & `laktory-0.2.0/docs/images/terraform.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/images/what_is_laktory.png` & `laktory-0.2.0/docs/images/what_is_laktory.png`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/index.md` & `laktory-0.2.0/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 ```yaml
 name: slv_stock_prices
 timestamp_key: created_at
 builder:
   layer: SILVER
   table_source:
     name: brz_stock_prices
-columns:
-  - name: symbol
-    type: string
-    spark_func_name: coalesce
-    spark_func_args:
-      - data.symbol
+  spark_chain:
+    nodes:
+      - column:
+          name: symbol
+          type: string
+        spark_func_name: coalesce
+        spark_func_args:
+          - data.symbol
   ...
 ```
 
 ### Validate
 Validation and augmentation of configuration models with laktory default properties, templates and custom spark functions.
 ```py
 from laktory import models
```

### Comparing `laktory-0.1.9/docs/install.md` & `laktory-0.2.0/docs/install.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 ```bash
 pip install laktory
 ```
 
 The main dependencies are:
 
+* [`databricks-sdk`](https://pypi.org/project/databricks-sdk/): The Databricks SDK for Python includes functionality to accelerate development with Python for the Databricks Lakehouse.
+* [`pulumi`](https://pypi.org/project/pulumi/): Infrastructure as code tool used to deploy resources.
 * [`pydantic`](https://pypi.org/project/pydantic/): All laktory models derived from Pydantic `BaseModel`.
 * [`settus`](https://pypi.org/project/settus/): Cloud-based settings management system.
-* [`pulumi`](https://pypi.org/project/pulumi/): Infrastructure as code tool used to deploy resources.
 * [`typer`](https://pypi.org/project/typer/): Library for building CLI applications. 
  
 
 If you've got Python 3.8+ and `pip` installed, you're good to go. 
 It is generally recommended to use a virtual environment for the installation. 
 
 The pip installation not only install the python package, but also Laktory CLI that can be invoked with
```

### Comparing `laktory-0.1.9/docs/lakehouseascode.md` & `laktory-0.2.0/docs/lakehouseascode.md`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/docs/quickstart.md` & `laktory-0.2.0/docs/quickstart.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 laktory quickstart
 ```
 You will be asked 2 questions:
 
 - Infrastructure as Code backend (terraform or pulumi)
 - Node type for compute (cloud specific, e.g. Standard_DS3_v2, c5.2xlarge, etc.)
 
-Once completed, a files have been created.
+Once completed, the stack files and resources have been created.
 
 #### Stack File
 ??? "API Documentation"
     [`laktory.models.Stack`][laktory.models.Stack]<br>
 
 The `stack.yaml` file is the main entry point defining the `name` of the stack, the selected `backend` and the list
 of `resources` to be deployed.
```

### Comparing `laktory-0.1.9/docs/stylesheets/mkdocstrings.css` & `laktory-0.2.0/docs/stylesheets/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/__init__.py` & `laktory-0.2.0/laktory/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,44 @@
+import os
 from ._version import VERSION
 
 __version__ = VERSION
 
 # Need to be imported first
 from ._settings import settings
 
 # --------------------------------------------------------------------------- #
+# User-agent                                                                  #
+# --------------------------------------------------------------------------- #
+
+from ._useragent import set_databricks_sdk_upstream
+
+set_databricks_sdk_upstream()
+
+
+# --------------------------------------------------------------------------- #
 # Packages                                                                    #
 # --------------------------------------------------------------------------- #
 
 import laktory._parsers
 import laktory.models
 import laktory.spark
 
 # --------------------------------------------------------------------------- #
 # Classes                                                                     #
 # --------------------------------------------------------------------------- #
 
 from ._settings import Settings
+from .dispatcher.dispatcher import Dispatcher
 
 # --------------------------------------------------------------------------- #
 # Objects                                                                     #
 # --------------------------------------------------------------------------- #
 
 from ._logger import get_logger
 from .metadata import read_metadata
 from .models.resources.pulumiresource import pulumi_outputs
 from .models.resources.pulumiresource import pulumi_resources
 from .cli.app import app
 from .version import show_version_info
+from .datetime import unix_timestamp
+from .datetime import utc_datetime
```

### Comparing `laktory-0.1.9/laktory/_logger.py` & `laktory-0.2.0/laktory/_logger.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/_parsers.py` & `laktory-0.2.0/laktory/_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/_settings.py` & `laktory-0.2.0/laktory/_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/_testing/stackvalidator.py` & `laktory-0.2.0/laktory/_testing/stackvalidator.py`

 * *Files 14% similar despite different names*

```diff
@@ -61,12 +61,14 @@
         self.validate_pulumi()
         self.validate_terraform()
         os.chdir(cwd)
         shutil.rmtree(dirpath)
         settings.cli_raise_external_exceptions = c0
 
     def validate_pulumi(self):
-        self.pstack.preview(stack="okube/dev")
+        pass
+        # self.pstack.preview(stack="okube/dev")
+        # TODO: Re-enable
 
     def validate_terraform(self):
         self.tstack.init()
         self.tstack.plan()
```

### Comparing `laktory-0.1.9/laktory/constants.py` & `laktory-0.2.0/laktory/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "struct<>",
     "udt",
 ]
 
 # CACHE_ROOT = "./laktory"
 CACHE_ROOT = "./"
 LAKTORY_WORKSPACE_ROOT = "/.laktory/"
+
 # for k in vars(types):
 #     o = getattr(types, k)
 #     if "Type" in k and inspect.isclass(o):
 #         try:
 #             typ = o()
 #         except TypeError:
 #             continue
```

### Comparing `laktory-0.1.9/laktory/dlt/__init__.py` & `laktory-0.2.0/laktory/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/azurenative/storageblob.py` & `laktory-0.2.0/laktory/models/azurenative/storageblob.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/basemodel.py` & `laktory-0.2.0/laktory/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/__init__.py` & `laktory-0.2.0/laktory/models/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/accesscontrol.py` & `laktory-0.2.0/laktory/models/databricks/accesscontrol.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/cluster.py` & `laktory-0.2.0/laktory/models/databricks/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,17 +283,17 @@
     # aws_attributes
     # azure_attributes
     cluster_id: str = None
     # cluster_log_conf
     # cluster_source
     # cluster_mount_infos
     custom_tags: dict[str, str] = None
-    data_security_mode: Literal[
-        "NONE", "SINGLE_USER", "USER_ISOLATION"
-    ] = "USER_ISOLATION"
+    data_security_mode: Literal["NONE", "SINGLE_USER", "USER_ISOLATION"] = (
+        "USER_ISOLATION"
+    )
     # docker_image
     driver_instance_pool_id: str = None
     driver_node_type_id: str = None
     enable_elastic_disk: bool = None
     enable_local_disk_encryption: bool = None
     # gcp_attributes
     idempotency_token: str = None
```

### Comparing `laktory-0.1.9/laktory/models/databricks/dbfsfile.py` & `laktory-0.2.0/laktory/models/databricks/dbfsfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def additional_core_resources(self) -> list[PulumiResource]:
         resources = []
         if self.access_controls:
             resources += [
                 Permissions(
                     resource_name=f"permissions-{self.resource_name}",
                     access_controls=self.access_controls,
-                    workspace_file_path=self.path,
+                    workspace_file_path=f"${{resources.{self.resource_name}.path}}",
                 )
             ]
         return resources
 
     # ----------------------------------------------------------------------- #
     # Pulumi Properties                                                       #
     # ----------------------------------------------------------------------- #
```

### Comparing `laktory-0.1.9/laktory/models/databricks/directory.py` & `laktory-0.2.0/laktory/models/databricks/directory.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/externallocation.py` & `laktory-0.2.0/laktory/models/databricks/externallocation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/grants.py` & `laktory-0.2.0/laktory/models/databricks/grants.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/group.py` & `laktory-0.2.0/laktory/models/databricks/group.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/groupmember.py` & `laktory-0.2.0/laktory/models/databricks/groupmember.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/job.py` & `laktory-0.2.0/laktory/models/databricks/job.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/metastore.py` & `laktory-0.2.0/laktory/models/databricks/metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/metastoreassignment.py` & `laktory-0.2.0/laktory/models/databricks/metastoreassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/metastoredataaccess.py` & `laktory-0.2.0/laktory/models/databricks/metastoredataaccess.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/mwspermissionassignment.py` & `laktory-0.2.0/laktory/models/databricks/mwspermissionassignment.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/notebook.py` & `laktory-0.2.0/laktory/models/databricks/notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/permissions.py` & `laktory-0.2.0/laktory/models/databricks/permissions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/pipeline.py` & `laktory-0.2.0/laktory/models/databricks/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,38 +253,43 @@
       - name: slv_stock_prices
         timestamp_key: created_at
         builder:
           layer: SILVER
           table_source:
             name: brz_stock_prices
             read_as_stream: True
-        columns:
-          - name: created_at
-            type: timestamp
-            spark_func_name: coalesce
-            spark_func_args:
-              - data._created_at
+          spark_chain:
+            nodes:
+              - column:
+                    name: created_at
+                    type: timestamp
+                spark_func_name: coalesce
+                spark_func_args:
+                  - data._created_at
 
-          - name: symbol
-            type: string
-            spark_func_name: coalesce
-            spark_func_args:
-              - data.symbol
+              - column:
+                    name: symbol
+                    type: string
+                spark_func_name: coalesce
+                spark_func_args:
+                  - data.symbol
 
-          - name: open
-            type: double
-            spark_func_name: coalesce
-            spark_func_args:
-              - data.open
+              - column:
+                    name: open
+                    type: double
+                spark_func_name: coalesce
+                spark_func_args:
+                  - data.open
 
-          - name: close
-            type: double
-            spark_func_name: coalesce
-            spark_func_args:
-              - data.close
+              - column:
+                    name: close
+                    type: double
+                spark_func_name: coalesce
+                spark_func_args:
+                  - data.close
     '''
     pipeline = models.Pipeline.model_validate_yaml(io.StringIO(pipeline_yaml))
     ```
 
     References
     ----------
```

### Comparing `laktory-0.1.9/laktory/models/databricks/secret.py` & `laktory-0.2.0/laktory/models/databricks/secret.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/secretacl.py` & `laktory-0.2.0/laktory/models/databricks/secretacl.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/secretscope.py` & `laktory-0.2.0/laktory/models/databricks/secretscope.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/serviceprincipal.py` & `laktory-0.2.0/laktory/models/databricks/serviceprincipal.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/serviceprincipalrole.py` & `laktory-0.2.0/laktory/models/databricks/serviceprincipalrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/sqlquery.py` & `laktory-0.2.0/laktory/models/databricks/sqlquery.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/user.py` & `laktory-0.2.0/laktory/models/databricks/user.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/userrole.py` & `laktory-0.2.0/laktory/models/databricks/userrole.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/warehouse.py` & `laktory-0.2.0/laktory/models/databricks/warehouse.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/databricks/workspacefile.py` & `laktory-0.2.0/laktory/models/databricks/workspacefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     def additional_core_resources(self) -> list[PulumiResource]:
         resources = []
         if self.access_controls:
             resources += [
                 Permissions(
                     resource_name=f"permissions-{self.resource_name}",
                     access_controls=self.access_controls,
-                    workspace_file_path=self.path,
+                    workspace_file_path=f"${{resources.{self.resource_name}.path}}",
                 )
             ]
         return resources
 
     # ----------------------------------------------------------------------- #
     # Pulumi Properties                                                       #
     # ----------------------------------------------------------------------- #
```

### Comparing `laktory-0.1.9/laktory/models/dataevent.py` & `laktory-0.2.0/laktory/models/dataevent.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/dataeventheader.py` & `laktory-0.2.0/laktory/models/dataeventheader.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,7 @@
             return self.event_root_
 
         producer = ""
         if self.producer is not None:
             producer = self.producer.name + "/"
         v = f"{self.events_root}{producer}{self.name}/"
         return v
-
-
-if __name__ == "__main__":
-    from laktory import models
-
-    event = models.DataEventHeader(
-        name="stock_price",
-        producer={"name": "yahoo-finance"},
-    )
-    print(event)
-
-    print(event.event_root)
```

### Comparing `laktory-0.1.9/laktory/models/dataproducer.py` & `laktory-0.2.0/laktory/models/dataproducer.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/datasources/eventdatasource.py` & `laktory-0.2.0/laktory/models/datasources/eventdatasource.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pydantic import model_validator
 from laktory.spark import DataFrame
 from typing import Literal
-from typing import Any
 
 from laktory.models.dataeventheader import DataEventHeader
 from laktory.models.datasources.basedatasource import BaseDataSource
 from laktory._logger import get_logger
 
 logger = get_logger(__name__)
 
@@ -54,14 +53,23 @@
     schema_location: str = None
     type: Literal["STORAGE_EVENTS", "STREAM_KINESIS", "STREAM_KAFKA"] = "STORAGE_EVENTS"
 
     # ----------------------------------------------------------------------- #
     # Readers                                                                 #
     # ----------------------------------------------------------------------- #
 
+    def _read(self, spark) -> DataFrame:
+        if self.mock_df is not None:
+            logger.info(f"Reading event data source ({self.name}) from memory")
+            return self.mock_df
+        if self.type == "STORAGE_EVENTS":
+            return self._read_storage(spark)
+        else:
+            raise NotImplementedError()
+
     def _read_storage(self, spark) -> DataFrame:
         if self.read_as_stream:
             logger.info(f"Reading {self.event_root} as stream")
 
             schema_location = self.schema_location
             if schema_location is None:
                 schema_location = self.event_root
@@ -94,26 +102,7 @@
         # Load
         df = reader.load(self.event_root)
 
         # Not supported by UC
         # .withColumn("file", F.input_file_name())
 
         return df
-
-    def read(self, spark) -> DataFrame:
-        """
-        Read data with options specified in attributes.
-
-        Parameters
-        ----------
-        spark
-            Spark context
-
-        Returns
-        -------
-        : DataFrame
-            Resulting park dataframe
-        """
-        if self.type == "STORAGE_EVENTS":
-            return self._read_storage(spark)
-        else:
-            raise NotImplementedError()
```

### Comparing `laktory-0.1.9/laktory/models/datasources/tabledatasource.py` & `laktory-0.2.0/laktory/models/datasources/tabledatasource.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,36 +7,14 @@
 from laktory.models.basemodel import BaseModel
 from laktory.models.datasources.basedatasource import BaseDataSource
 from laktory._logger import get_logger
 
 logger = get_logger(__name__)
 
 
-class Watermark(BaseModel):
-    """
-    Definition of a spark structured streaming watermark for joining data
-    streams.
-
-    Attributes
-    ----------
-    column:
-        Event time column name
-    threshold:
-        How late, expressed in seconds, the data is expected to be with
-        respect to event time.
-
-    References
-    ----------
-    https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html#handling-late-data-and-watermarking
-    """
-
-    column: str
-    threshold: str
-
-
 class TableDataSourceCDC(BaseModel):
     """
     Defines the change data capture (CDC) properties of a table data source.
     They are used to build the target using `apply_changes` method from
     Databricks DLT.
 
     Attributes
@@ -102,32 +80,25 @@
 
     Attributes
     ----------
     catalog_name:
         Name of the catalog of the source table
     cdc:
         Change data capture specifications
-    selects:
-        Columns to select from the source table. Can be specified as a list
-        or as a dictionary to rename the source columns
-    filter:
-        SQL expression used to select specific rows from the source table
     fmt:
         Table format
     from_pipeline:
         If `True` the source table will be read using `dlt.read` instead of
         `spark.read`
     name:
         Name of the source table
     path:
         Path of the source table
     schema_name:
         Name of the schema of the source table
-    watermark
-        Spark structured streaming watermark specifications
 
     Examples
     ---------
     ```python
     from laktory import models
 
     source = models.TableDataSource(
@@ -137,25 +108,21 @@
         from_pipeline=False,
         read_as_stream=True,
     )
     # df = source.read(spark)
     ```
     """
 
-    _df: Any = None
     catalog_name: Union[str, None] = None
     cdc: Union[TableDataSourceCDC, None] = None
-    selects: Union[list[str], dict[str, str], None] = None
     fmt: Literal["PARQUET", "DELTA"] = "DELTA"
-    filter: Union[str, None] = None
     from_pipeline: Union[bool, None] = True
     name: Union[str, None] = None
     path: Union[str, None] = None
     schema_name: Union[str, None] = None
-    watermark: Union[Watermark, None] = None
 
     @model_validator(mode="after")
     def set_source(self) -> Any:
         """Source Definition"""
 
         if self.name and self.path:
             raise ValueError("Either path or name must be specified, but not both")
@@ -205,17 +172,17 @@
     # Readers                                                                 #
     # ----------------------------------------------------------------------- #
 
     def _read(self, spark) -> DataFrame:
         from laktory.dlt import read
         from laktory.dlt import read_stream
 
-        if self._df is not None:
+        if self.mock_df is not None:
             logger.info(f"Reading {self.path_or_full_name} from memory")
-            df = self._df
+            df = self.mock_df
         elif self.read_as_stream:
             logger.info(f"Reading {self.path_or_full_name} as stream")
             if self.from_pipeline:
                 df = read_stream(self.full_name)
             elif self.from_path:
                 df = spark.readStream.format(self.fmt).load(self.path)
             else:
@@ -227,41 +194,14 @@
             elif self.from_path:
                 df = spark.read.format(self.fmt).load(self.path)
             else:
                 df = spark.read.format(self.fmt).table(self.full_name)
 
         return df
 
-    def read(self, spark) -> DataFrame:
-        import pyspark.sql.functions as F
-
-        df = self._read(spark)
-
-        # Apply filter
-        if self.filter:
-            df = df.filter(self.filter)
-
-        # Columns
-        cols = []
-        if self.selects:
-            if isinstance(self.selects, list):
-                cols += [F.col(c) for c in self.selects]
-            elif isinstance(self.selects, dict):
-                cols += [F.col(k).alias(v) for k, v in self.selects.items()]
-            df = df.select(cols)
-
-        # Apply Watermark
-        if self.watermark:
-            df = df.withWatermark(
-                self.watermark.column,
-                self.watermark.threshold,
-            )
-
-        return df
-
 
 if __name__ == "__main__":
     from laktory import models
 
     source = models.TableDataSource(
         name="brz_stock_prices",
         selects=["symbol", "open", "close"],
```

### Comparing `laktory-0.1.9/laktory/models/grants/__init__.py` & `laktory-0.2.0/laktory/models/grants/__init__.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/cataloggrant.py` & `laktory-0.2.0/laktory/models/grants/cataloggrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/connectiongrant.py` & `laktory-0.2.0/laktory/models/grants/connectiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/externallocationgrant.py` & `laktory-0.2.0/laktory/models/grants/externallocationgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/functiongrant.py` & `laktory-0.2.0/laktory/models/grants/functiongrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/metastoregrant.py` & `laktory-0.2.0/laktory/models/grants/metastoregrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/registeredmodelgrant.py` & `laktory-0.2.0/laktory/models/grants/registeredmodelgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/schemagrant.py` & `laktory-0.2.0/laktory/models/grants/schemagrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/sharegrant.py` & `laktory-0.2.0/laktory/models/grants/sharegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/storagecredentialgrant.py` & `laktory-0.2.0/laktory/models/grants/storagecredentialgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/tablegrant.py` & `laktory-0.2.0/laktory/models/grants/tablegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/viewgrant.py` & `laktory-0.2.0/laktory/models/grants/viewgrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/grants/volumegrant.py` & `laktory-0.2.0/laktory/models/grants/volumegrant.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/providers/awsprovider.py` & `laktory-0.2.0/laktory/models/providers/awsprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/providers/azureprovider.py` & `laktory-0.2.0/laktory/models/providers/azureprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/providers/azurepulumiprovider.py` & `laktory-0.2.0/laktory/models/providers/azurepulumiprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/providers/baseprovider.py` & `laktory-0.2.0/laktory/models/providers/baseprovider.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/providers/databricksprovider.py` & `laktory-0.2.0/laktory/models/providers/databricksprovider.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         host="adb-4623853922539974.14.azuredatabricks.net",
         token="${vars.DATABRICKS_TOKEN}",
     )
     ```
     """
 
     source: str = Field("databricks/databricks", exclude=True)
+    version: str = Field(">=1.39", exclude=True)  # Required to monitor laktory usage
 
     account_id: str = None
     auth_type: str = None
     azure_client_id: str = None
     azure_client_secret: str = None
     azure_environment: str = None
     azure_login_app_id: str = None
```

### Comparing `laktory-0.1.9/laktory/models/resources/baseresource.py` & `laktory-0.2.0/laktory/models/resources/baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/resources/pulumiresource.py` & `laktory-0.2.0/laktory/models/resources/pulumiresource.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from abc import abstractmethod
 from typing import Union
 from typing import Any
+
+from laktory._useragent import set_databricks_sdk_upstream
 from laktory._settings import settings
 from laktory._parsers import _snake_to_camel
 from laktory.models.resources.baseresource import BaseResource
 
 # TODO: Review pulumi_outputs and pulumi_resources as they cause issues when
 # running multiple tests in parallel
 
@@ -90,14 +92,17 @@
         :
             Deployed pulumi resources
         """
         from pulumi import ResourceOptions
 
         self._pulumi_resources = {}
 
+        # Inject user-agent value for monitoring usage as a Databricks partner
+        set_databricks_sdk_upstream()
+
         for r in self.core_resources:
             # Properties
             properties = r.pulumi_properties
             properties = self.inject_vars(properties)
 
             # Options
             _opts = r.options.model_dump()
```

### Comparing `laktory-0.1.9/laktory/models/resources/terraformresource.py` & `laktory-0.2.0/laktory/models/resources/terraformresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/sql/catalog.py` & `laktory-0.2.0/laktory/models/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/sql/column.py` & `laktory-0.2.0/laktory/models/spark/sparkchainnode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,363 +1,323 @@
 from pydantic import field_validator
-from pydantic import model_validator
 from typing import Any
-from typing import Callable
 from typing import Union
+from typing import Callable
 
 from laktory._logger import get_logger
 from laktory.constants import SUPPORTED_TYPES
 from laktory.models.basemodel import BaseModel
-from laktory.spark import Column as SparkColumn
+from laktory.models.spark.sparkfuncarg import SparkFuncArg
 from laktory.spark import DataFrame
+from laktory.spark import Column
+from laktory.models.spark._common import parse_args
+from laktory.models.spark._common import parse_kwargs
+from laktory.exceptions import MissingColumnError
+from laktory.exceptions import MissingColumnsError
 
 logger = get_logger(__name__)
 
 
-class SparkFuncArg(BaseModel):
+# --------------------------------------------------------------------------- #
+# Main Class                                                                  #
+# --------------------------------------------------------------------------- #
+
+
+class SparkChainNodeColumn(BaseModel):
     """
-    Spark function argument
+    Spark chain node column definition
 
     Attributes
     ----------
-    value:
-        Value of the argument
-    is_column:
-        If `True`, the value is also the name of a column
-    to_lit:
-        If `True`, the value is converted to a spark column using
-        `F.lit({value})`
-    to_expr:
-        If `True`, the value is converted to a spark column using
-        `F.expr({value})`
+    name:
+        Column name
+    type:
+        Column data type
+    unit:
+        Column units
     """
 
-    value: Any
-    is_column: bool = None
-    to_lit: bool = None
-    to_expr: bool = None
-
-    @model_validator(mode="after")
-    def set_defaults(self) -> Any:
-        """Default options"""
-
-        # If only value is provided and value is a string, assume value is column
-        if self.is_column is None and self.to_expr is None and self.to_lit is None:
-            if isinstance(self.value, str):
-                self.is_column = True
-
-        if self.is_column:
-            if self.to_lit:
-                raise ValueError(
-                    "If `to_column` is `True`, `to_lit` must be `None` or `False`"
-                )
+    name: str
+    type: str = "string"
+    unit: Union[str, None] = None
 
-            if self.to_expr == False:
+    @field_validator("type")
+    def check_type(cls, v: str) -> str:
+        if "<" in v:
+            return v
+        else:
+            if v not in SUPPORTED_TYPES:
                 raise ValueError(
-                    "If `to_column` is `True`, `to_expr` must be `None` or `True`"
+                    f"Type {v} is not supported. Select one of {SUPPORTED_TYPES}"
                 )
-
-            self.to_expr = True
-            self.to_lit = False
-
-        else:
-            self.is_column = False
-
-            if self.to_lit is None and self.to_expr is None:
-                self.to_lit = True
-                self.to_expr = False
-
-            if self.to_lit is None:
-                self.to_lit = False
-
-            if self.to_expr is None:
-                self.to_expr = False
-
-        return self
-
-    def to_spark(self):
-        import pyspark.sql.functions as F
-
-        v = self.value
-        if self.to_lit:
-            v = F.lit(v)
-        elif self.to_expr:
-            v = F.expr(v)
         return v
 
 
-class Column(BaseModel):
+class SparkChainNode(BaseModel):
     """
-    Definition of a table column, including instructions on how to build the
-    column using spark and an input dataframe.
+    SparkChain node that output a DataFrame upon execution. As a convenience,
+    `column` can be specified to create a new column. In this case, the spark
+    function or sql expression is expected to return a column instead of a
+    DataFrame. Each node is executed sequentially in the provided order. A node
+    may also be another Spark Chain.
 
     Attributes
     ----------
-    catalog_name:
-        Name of the catalog string the column table
-    comment:
-        Text description of the column
-    name:
-        Name of the column
-    pii:
-        If `True`, the column is flagged as Personally Identifiable Information
-    raise_missing_arg_exception:
-        If `True`, an exception is raised when one of the spark function
-        argument is missing. Otherwise, only warning is issued.
-    schema_name:
-        Name of the schema storing the column table
+    allow_missing_column_args:
+        If `True`, spark func column arguments are allowed to be missing
+        without raising an exception.
+    column:
+        Column definition. If not `None`, the spark function or sql expression
+        is expected to return a column instead of a dataframe.
     spark_func_args:
-        List of arguments to be passed to the spark function to build the
-        column.
+        List of arguments to be passed to the spark function.
+        To support spark functions expecting column argument, col("x"),
+        lit("3") and expr("x*2") can be provided.
     spark_func_kwargs:
-        List of keyword arguments to be passed to the spark function to build
-        the column.
+        List of keyword arguments to be passed to the spark function.
+        To support spark functions expecting column argument, col("x"),
+        lit("3") and expr("x*2") can be provided.
     spark_func_name:
-        Name of the spark function to build the column. Mutually exclusive to
-        `sql_expression`
+        Name of the spark function to build the dataframe. If `column` is
+        specified, the spark function should return a column instead. Mutually
+         exclusive to `sql_expression`.
     sql_expression:
-        Expression defining how to build the column. Mutually exclusive to
-        `spark_func_name`
-    table_name:
-        Name of the table storing the column.
-    type:
-        Column data type
-    unit:
-        Column units
+        Expression defining how to build the column. If `column` is
+        specified, the sql expression should define a column instead. Mutually
+         exclusive to `spark_func_name`
 
     Examples
     --------
     ```py
+    import pandas as pd
     from laktory import models
 
-    df = spark.createDataFrame(
-        [
-            [200.0],
-            [202.0],
-            [201.5],
-        ],
-        ["data.open"],
+    df0 = spark.createDataFrame(pd.DataFrame({"x": [1, 2, 2, 3]}))
+
+    node = models.SparkChainNode(
+        column={
+            "name": "cosx",
+            "type": "double",
+        },
+        spark_func_name="cos",
+        spark_func_args=["x"],
     )
+    df = node.execute(df0)
 
-    col = models.Column(
-        name="open",
-        spark_func_name="poly1",
-        spark_func_args=[
-            "data.open",
-        ],
-        spark_func_kwargs={"a": {"value": 2.0, "to_lit": True}},
-        type="double",
+    node = models.SparkChainNode(
+        column={
+            "name": "xy",
+            "type": "double",
+        },
+        spark_func_name="coalesce",
+        spark_func_args=["col('x')", "F.col('y')"],
+        allow_missing_column_args=True,
     )
+    df = node.execute(df)
 
-    spark_col = col.to_spark(df)
+    print(df.toPandas().to_string())
+    '''
+       x      cosx   xy
+    0  1  0.540302  1.0
+    1  2 -0.416147  2.0
+    2  2 -0.416147  2.0
+    3  3 -0.989992  3.0
+    '''
+
+    node = models.SparkChainNode(
+        spark_func_name="drop_duplicates",
+        spark_func_args=[["x"]],
+    )
+    df = node.execute(df0, spark=spark)
+
+    print(df.toPandas().to_string())
+    '''
+       x
+    0  1
+    1  2
+    2  3
+    '''
     ```
     """
 
-    catalog_name: Union[str, None] = None
-    comment: Union[str, None] = None
-    name: str
-    pii: Union[bool, None] = None
-    raise_missing_arg_exception: Union[bool, None] = True
-    schema_name: Union[str, None] = None
-    spark_func_args: list[Union[str, SparkFuncArg]] = []
+    allow_missing_column_args: Union[bool, None] = False
+    column: Union[SparkChainNodeColumn, None] = None
+    spark_func_args: list[Union[Any, SparkFuncArg]] = []
     spark_func_kwargs: dict[str, Union[Any, SparkFuncArg]] = {}
     spark_func_name: Union[str, None] = None
     sql_expression: Union[str, None] = None
-    table_name: Union[str, None] = None
-    type: str = "string"
-    unit: Union[str, None] = None
-
-    @field_validator("spark_func_args")
-    def parse_args(cls, args: list[Union[str, SparkFuncArg]]) -> list[SparkFuncArg]:
-        _args = []
-        for a in args:
-            if isinstance(a, SparkFuncArg):
-                pass
-            elif isinstance(a, dict):
-                a = SparkFuncArg(**a)
-            else:
-                a = SparkFuncArg(value=a)
-            _args += [a]
-        return _args
-
-    @field_validator("spark_func_kwargs")
-    def parse_kwargs(
-        cls, kwargs: dict[str, Union[str, SparkFuncArg]]
-    ) -> dict[str, SparkFuncArg]:
-        _kwargs = {}
-        for k, a in kwargs.items():
-            if isinstance(a, SparkFuncArg):
-                pass
-            elif isinstance(a, dict):
-                a = SparkFuncArg(**a)
-            else:
-                a = SparkFuncArg(value=a)
-            _kwargs[k] = a
-        return _kwargs
-
-    @field_validator("type")
-    def default_load_path(cls, v: str) -> str:
-        if "<" in v:
-            return v
-        else:
-            if v not in SUPPORTED_TYPES:
-                raise ValueError(
-                    f"Type {v} is not supported. Select one of {SUPPORTED_TYPES}"
-                )
-        return v
 
-    # ----------------------------------------------------------------------- #
-    # Computed fields                                                         #
-    # ----------------------------------------------------------------------- #
+    parse_args = parse_args
+    parse_kwargs = parse_kwargs
 
     @property
-    def parent_full_name(self) -> str:
-        """Table full name `{catalog_name}.{schema_name}.{table_name}`"""
-        _id = ""
-        if self.catalog_name:
-            _id += self.catalog_name
-
-        if self.schema_name:
-            if _id == "":
-                _id = self.schema_name
-            else:
-                _id += f".{self.schema_name}"
-
-        if self.table_name:
-            if _id == "":
-                _id = self.table_name
-            else:
-                _id += f".{self.table_name}"
-
-        return _id
+    def is_column(self):
+        return self.column is not None
 
     @property
-    def full_name(self) -> str:
-        """Column full name `{catalog_name}.{schema_name}.{table_name}.{column_name}`"""
-        _id = self.name
-        if self.parent_full_name is not None:
-            _id = f"{self.parent_full_name}.{_id}"
-        return _id
+    def id(self):
+        if self.is_column:
+            return self.column.name
+        return "df"
+
+    def add_column(self, df, col):
+        return df.withColumn(self.column.name, col)
 
     # ----------------------------------------------------------------------- #
     # Class Methods                                                           #
     # ----------------------------------------------------------------------- #
 
-    def to_spark(
+    def execute(
         self,
         df: DataFrame,
-        udfs: list[Callable[[...], SparkColumn]] = None,
-        raise_exception: bool = True,
-    ) -> SparkColumn:
+        udfs: list[Callable[[...], Union[Column, DataFrame]]] = None,
+        return_col: bool = False,
+        spark=None,
+    ) -> Union[DataFrame, Column]:
         """
         Build Spark Column
 
         Parameters
         ----------
         df:
             Input DataFrame
         udfs:
             User-defined functions
-        raise_exception
-            If `True`, raise exception when input columns are not available,
-            else, skip.
+        return_col
+            If `True` and column specified, function returns `Column` object
+            instead of DataFrame.
+        spark:
+            Spark Session
+
+        Returns
+        -------
+            Output DataFrame
         """
         import pyspark.sql.functions as F
-        from laktory.spark import functions as LF
+        from pyspark.sql.dataframe import DataFrame
+        from pyspark.sql import Column
         from laktory.spark.dataframe import has_column
+        from laktory.spark import functions as LF
+        from laktory.spark import DataFrame as LDF
 
         if udfs is None:
             udfs = []
         udfs = {f.__name__: f for f in udfs}
 
         # From SQL expression
         if self.sql_expression:
-            logger.info(f"   {self.name}[{self.type}] as `{self.sql_expression}`)")
-            col = F.expr(self.sql_expression).alias(self.name)
-            if self.type not in ["_any"]:
-                col = col.cast(self.type)
-            return col
+            if self.is_column:
+                logger.info(
+                    f"{self.column.name}[{self.column.type}] as `{self.sql_expression}`)"
+                )
+                col = F.expr(self.sql_expression).alias(self.column.name)
+                if self.column.type not in ["_any"]:
+                    col = col.cast(self.column.type)
+                if return_col:
+                    return col
+                return self.add_column(df, col)
+            else:
+                raise NotImplementedError("sql_expression not supported yet")
+                #     df.createOrReplaceTempView("_df")
+                #     df = spark.sql(self.sql_expression)
+                #     return df
 
         # From Spark Function
         func_name = self.spark_func_name
-        if func_name is None:
-            func_name = "coalesce"
+        if self.spark_func_name is None:
+            if self.is_column:
+                func_name = "coalesce"
+            else:
+                raise ValueError(
+                    "`spark_func_name` must be specified if `sql_expression` is not specified"
+                )
 
         # Get from UDFs
         f = udfs.get(func_name, None)
         if f is None:
             # Get from built-in spark functions
-            f = getattr(F, func_name, None)
+            if self.is_column:
+                f = getattr(F, func_name, None)
+            else:
+                f = getattr(DataFrame, func_name, None)
 
             if f is None:
                 # Get from laktory functions
-                f = getattr(LF, func_name, None)
+                if self.is_column:
+                    f = getattr(LF, func_name, None)
+                else:
+                    f = getattr(LDF, func_name, None)
 
         if f is None:
             raise ValueError(f"Function {func_name} is not available")
 
         _args = self.spark_func_args
         _kwargs = self.spark_func_kwargs
 
-        logger.info(f"   {self.name}[{self.type}] as {func_name}({_args}, {_kwargs})")
+        # Build log
+        func_log = f"{func_name}("
+        for a in _args:
+            func_log += f"{a.value},"
+        for k, a in _kwargs.items():
+            func_log += f"{k}={a.value},"
+        if func_log.endswith(","):
+            func_log = func_log[:-1]
+        func_log += ")"
+        if self.is_column:
+            logger.info(f"Column {self.id}[{self.column.type}] as {func_log}")
+        else:
+            logger.info(f"DataFrame {self.id} as {func_log}")
 
         # Build args
         args = []
+        missing_column_names = []
         for i, _arg in enumerate(_args):
-            if df is not None:
-                if _arg.is_column and not has_column(df, _arg.value):
-                    logger.info(f"Column '{_arg.value}' not available")
+            parg = _arg.eval()
+            cname = _arg.value
 
-                    if self.raise_missing_arg_exception:
-                        if raise_exception:
-                            raise ValueError(
-                                f"Input column {_arg.value} missing. Abort building {self.name}."
+            if df is not None:
+                # Check if explicitly defined columns are available
+                if isinstance(parg, Column):
+                    cname = str(parg).split("'")[1]
+                    if not has_column(df, cname):
+                        missing_column_names += [cname]
+                        if not self.allow_missing_column_args:
+                            logger.error(
+                                f"Input column {cname} is missing. Abort building {self.id}"
                             )
+                            raise MissingColumnError(cname)
                         else:
-                            logger.info(
-                                f"Input column {_arg.value} missing. Skip building {self.name}"
+                            logger.warn(
+                                f"Input column {cname} is missing for building {self.id}"
                             )
-                            return None
-                    else:
-                        continue
+                            continue
+
+                else:
+                    pass
+                    # TODO: We could try to check if the function expect columns and if it's the case assume
+                    # that a string argument is intended to be a column name, but I feel this will be a rabbit
+                    # hole with tons of exceptions.
 
-            args += [_arg.to_spark()]
+            args += [parg]
 
         if len(_args) > 0 and len(args) < 1:
-            if raise_exception:
-                raise ValueError(
-                    f"All input columns are  missing. Abort building {self.name}"
-                )
-            else:
-                logger.info(f"All input columns are missing. Skip building {self.name}")
-                return None
+            raise MissingColumnsError(missing_column_names)
 
         # Build kwargs
         kwargs = {}
         for k, _arg in _kwargs.items():
-            kwargs[k] = _arg.to_spark()
+            kwargs[k] = _arg.eval(spark)
 
         # Function call
-        logger.info(f"   {self.name}[{self.type}] as {func_name}({args}, {kwargs})")
-        col = f(*args, **kwargs)
-
-        # Type Casting
-        if self.type not in ["_any"]:
-            col = col.cast(self.type)
-
-        return col
-
+        logger.info(f"{self.id} as {func_name}({args}, {kwargs})")
 
-if __name__ == "__main__":
-    from laktory import models
-
-    col = models.Column(
-        name="open",
-        spark_func_name="poly1",
-        spark_func_args=[
-            "data.open",
-        ],
-        spark_func_kwargs={"a": {"value": 2.0, "to_lit": True}},
-        type="double",
-    )
+        if self.is_column:
+            col = f(*args, **kwargs)
+            if self.column.type not in ["_any"]:
+                col = col.cast(self.column.type)
+            if return_col:
+                return col
+            df = self.add_column(df, col)
+        else:
+            df = f(df, *args, **kwargs)
 
-    spark_col = col.to_spark(df)
+        return df
```

### Comparing `laktory-0.1.9/laktory/models/sql/schema.py` & `laktory-0.2.0/laktory/models/sql/schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/sql/table.py` & `laktory-0.2.0/laktory/models/sql/table.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from laktory.models.databricks.grants import Grants
 from laktory.models.grants.tablegrant import TableGrant
 from laktory.models.resources.pulumiresource import PulumiResource
 from laktory.models.resources.terraformresource import TerraformResource
 from laktory.models.sql.column import Column
 from laktory.models.sql.tablebuilder import TableBuilder
 from laktory.models.sql.tableexpectation import TableExpectation
+from laktory.models.datasources.tabledatasource import TableDataSource
 
 logger = get_logger(__name__)
 
 
 class Table(BaseModel, PulumiResource, TerraformResource):
     """
     A table resides in the third layer of Unity Catalog’s three-level
@@ -69,34 +70,43 @@
     from laktory import dlt
     from laktory import models
 
     dlt.spark = spark
 
     table = models.Table(
         name="slv_stock_prices",
-        columns=[
-            {"name": "symbol", "type": "string", "sql_expression": "data.symbol"},
-            {
-                "name": "open",
-                "type": "double",
-                "spark_func_name": "coalesce",
-                "spark_func_args": ["daa.open"],
-            },
-            {
-                "name": "close",
-                "type": "double",
-                "spark_func_name": "coalesce",
-                "spark_func_args": ["daa.close"],
-            },
-        ],
         builder={
             "layer": "SILVER",
             "table_source": {
                 "name": "brz_stock_prices",
             },
+            "spark_chain": {
+                "nodes": [
+                    {
+                        "column": {"name": "symbol", "type": "string"},
+                        "sql_expression": "data.symbol",
+                    },
+                    {
+                        "column": {
+                            "name": "open",
+                            "type": "double",
+                        },
+                        "spark_func_name": "coalesce",
+                        "spark_func_args": ["daa.open"],
+                    },
+                    {
+                        "column": {
+                            "name": "close",
+                            "type": "double",
+                        },
+                        "spark_func_name": "coalesce",
+                        "spark_func_args": ["daa.close"],
+                    },
+                ]
+            },
         },
     )
 
     # Read
     # df = table.builder.read_source(spark)
 
     # Process
@@ -137,27 +147,34 @@
             c.table_name = self.name
             c.catalog_name = self.catalog_name
             c.schema_name = self.schema_name
 
         # Set builder table
         self.builder._table = self
 
-        # Assign to sources
+        # Find table sources
+        sources = []
         if self.builder.table_source is not None:
-            if self.builder.table_source.catalog_name is None:
-                self.builder.table_source.catalog_name = self.catalog_name
-            if self.builder.table_source.schema_name is None:
-                self.builder.table_source.schema_name = self.schema_name
-
-        # Assign to joins
-        for join in self.builder.joins:
-            if join.other.catalog_name is None:
-                join.other.catalog_name = self.catalog_name
-            if join.other.schema_name is None:
-                join.other.schema_name = self.schema_name
+            sources += [self.builder.table_source]
+
+        if self.builder.spark_chain:
+            for n in self.builder.spark_chain.nodes:
+                for a in n.spark_func_args:
+                    if isinstance(a.value, TableDataSource):
+                        sources += [a.value]
+                for a in n.spark_func_kwargs.values():
+                    if isinstance(a.value, TableDataSource):
+                        sources += [a.value]
+
+        # Assign catalog and schema to sources
+        for s in sources:
+            if s.catalog_name is None:
+                s.catalog_name = self.catalog_name
+            if s.schema_name is None:
+                s.schema_name = self.schema_name
 
         # Warehouse ID
         if self.warehouse_id is None:
             self.warehouse_id = settings.databricks_warehouse_id
 
         return self
```

### Comparing `laktory-0.1.9/laktory/models/sql/tableaggregation.py` & `laktory-0.2.0/laktory/spark/dataframe/groupby_and_agg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-from pydantic import field_validator
-from pydantic import model_validator
+from pydantic import BaseModel
 from typing import Union
-from typing import Any
-from typing import Callable
+from pyspark.sql.dataframe import DataFrame
 
 from laktory._logger import get_logger
-from laktory.models.basemodel import BaseModel
-from laktory.spark import DataFrame
-from laktory.spark import Column as SparkColumn
-from laktory.models.sql.column import Column
+from laktory.models.spark.sparkchainnode import SparkChainNode
+
 
 logger = get_logger(__name__)
 
 
 class TimeWindow(BaseModel):
     """
     Specifications for Time Window Aggregation
@@ -40,147 +36,113 @@
 
     time_column: str
     window_duration: str
     slide_duration: Union[str, None] = None
     start_time: Union[str, None] = None
 
 
-# TODO: Add support for partition by and drop
-"""
-w = Window.partitionBy("account_id").orderBy(F.col("created_at").desc())
-df = df.withColumn("_row", F.row_number().over(w)).filter(F.col("_row") == 1)
-df = df.drop("_row")
-"""
-
-
-class TableAggregation(BaseModel):
+def groupby_and_agg(
+    df,
+    groupby_window: TimeWindow = None,
+    groupby_columns: list[str] = None,
+    agg_expressions: list[SparkChainNode] = None,
+) -> DataFrame:
     """
-    Specifications for aggregation by group or time window.
+    Apply a groupby and create aggregation columns.
 
-    Attributes
+    Parameters
     ----------
+    df:
+        DataFrame
     groupby_window:
         Aggregation window definition
     groupby_columns:
         List of column names to group by
     agg_expressions:
         List of columns defining the aggregations
 
     Examples
     --------
     ```py
-    from laktory import models
+    import pandas as pd
 
-    table = models.Table(
-        name="gld_stock_prices_by_1d",
-        builder={
-            "layer": "GOLD",
-            "table_source": {
-                "name": "slv_star_stock_prices",
-            },
-            "aggregation": {
-                "groupby_columns": ["symbol"],
-                "groupby_window": {
-                    "time_column": "_tstamp",
-                    "window_duration": "1 day",
-                },
-                "agg_expressions": [
-                    {"name": "low", "spark_func_name": "min", "spark_func_args": ["low"]},
-                    {"name": "high", "spark_func_name": "max", "spark_func_args": ["high"]},
-                ],
-            },
+    df0 = spark.createDataFrame(
+        pd.DataFrame(
+            {
+                "symbol": ["AAPL", "GOOGL"],
+                "price": [200.0, 205.0],
+                "tstamp": ["2023-09-01", "2023-09-01"],
+            }
+        )
+    )
+
+    df = df0.groupby_and_agg(
+        groupby_window={
+            "time_column": "tstamp",
+            "window_duration": "1 day",
         },
+        agg_expressions=[
+            {
+                "column": {"name": "mean_price"},
+                "spark_func_name": "mean",
+                "spark_func_args": ["price"],
+            },
+        ],
     )
-    ```
 
+    print(df.toPandas().to_string())
+    '''
+                                           window  mean_price
+    0  (2023-09-01 00:00:00, 2023-09-02 00:00:00)       202.5
+    '''
+    ```
 
     References
     ----------
 
     * [pyspark window](https://spark.apache.org/docs/3.1.3/api/python/reference/api/pyspark.sql.functions.window.html)
     """
+    import pyspark.sql.functions as F
+
+    # Parse inputs
+    if groupby_window and not isinstance(groupby_window, TimeWindow):
+        groupby_window = TimeWindow(**groupby_window)
+    if agg_expressions is None:
+        raise ValueError("`agg_expressions` must be specified")
+    if groupby_columns is None:
+        groupby_columns = []
 
-    groupby_window: Union[TimeWindow, None] = None
-    groupby_columns: Union[list[str], None] = []
-    agg_expressions: list[Column] = []
-
-    @model_validator(mode="after")
-    def groupby(self) -> Any:
-        if self.groupby_window is None and len(self.groupby_columns) == 0:
-            raise ValueError(
-                "Either `groupby_window` or `groupby_columns` must be specified."
+    logger.info(
+        f"Executing groupby ({groupby_window} & {groupby_columns}) with {agg_expressions}"
+    )
+
+    # Groupby arguments
+    groupby = []
+    if groupby_window:
+        groupby += [
+            F.window(
+                timeColumn=groupby_window.time_column,
+                windowDuration=groupby_window.window_duration,
+                slideDuration=groupby_window.slide_duration,
+                startTime=groupby_window.start_time,
             )
+        ]
 
-        return self
+    for c in groupby_columns:
+        groupby += [c]
 
-    # ----------------------------------------------------------------------- #
-    # Methods                                                                 #
-    # ----------------------------------------------------------------------- #
-
-    def execute(
-        self,
-        df,
-        udfs: list[Callable[[...], SparkColumn]] = None,
-    ) -> DataFrame:
-        import pyspark.sql.functions as F
-
-        # Groupby arguments
-        groupby = []
-        if self.groupby_window:
-            groupby += [
-                F.window(
-                    timeColumn=self.groupby_window.time_column,
-                    windowDuration=self.groupby_window.window_duration,
-                    slideDuration=self.groupby_window.slide_duration,
-                    startTime=self.groupby_window.start_time,
-                )
-            ]
-
-        for c in self.groupby_columns:
-            groupby += [c]
-
-        # Agg arguments
-        aggs = []
-        for expr in self.agg_expressions:
-            expr.type = "_any"
-            aggs += [
-                expr.to_spark(
-                    df=df,
-                    udfs=udfs,
-                    raise_exception=True,
-                ).alias(expr.name)
-            ]
-
-        return df.groupby(groupby).agg(*aggs)
-
-
-if __name__ == "__main__":
-    from laktory import models
-
-    table = models.Table(
-        name="gld_stock_prices_by_1d",
-        builder={
-            "layer": "GOLD",
-            "table_source": {
-                "name": "slv_star_stock_prices",
-            },
-            "aggregation": {
-                "groupby_columns": ["symbol"],
-                "groupby_window": {
-                    "time_column": "_tstamp",
-                    "window_duration": "1 day",
-                },
-                "agg_expressions": [
-                    {
-                        "name": "low",
-                        "spark_func_name": "min",
-                        "spark_func_args": ["low"],
-                    },
-                    {
-                        "name": "high",
-                        "spark_func_name": "max",
-                        "spark_func_args": ["high"],
-                    },
-                ],
-            },
-        },
-    )
+    # Agg arguments
+    aggs = []
+    for expr in agg_expressions:
+        if not isinstance(expr, SparkChainNode):
+            expr = SparkChainNode(**expr)
+
+        expr.column.type = "_any"
+        aggs += [
+            expr.execute(
+                df=df,
+                # udfs=udfs,
+                return_col=True,
+            ).alias(expr.column.name)
+        ]
+
+    return df.groupby(groupby).agg(*aggs)
```

### Comparing `laktory-0.1.9/laktory/models/sql/tableexpectation.py` & `laktory-0.2.0/laktory/models/sql/tableexpectation.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/sql/tablejoin.py` & `laktory-0.2.0/laktory/spark/dataframe/smart_join.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,217 +1,216 @@
-from typing import Union
 from collections import defaultdict
+from pyspark.sql.dataframe import DataFrame
 
 from laktory._logger import get_logger
-from laktory.models.basemodel import BaseModel
-from laktory.models.datasources.tabledatasource import TableDataSource
-from laktory.spark import DataFrame
+from laktory.spark.dataframe.watermark import watermark
+from laktory.spark.dataframe.watermark import Watermark
+
 
 logger = get_logger(__name__)
 
 
-class TableJoin(BaseModel):
+def smart_join(
+    left: DataFrame,
+    other: DataFrame,
+    how: str = "left",
+    on: list[str] = None,
+    on_expression: str = None,
+    left_watermark: Watermark = None,
+    other_watermark: Watermark = None,
+    time_constraint_interval_lower: str = "60 seconds",
+    time_constraint_interval_upper: str = None,
+) -> DataFrame:
     """
-    Specifications of a tables join.
+    Join tables, clean up duplicated columns and support watermarking for
+    streaming joins.
 
-    Attributes
+    Parameters
     ----------
-    how:
-        Type of join (left, outer, full, etc.)
     left:
         Left side of the join
+    other:
+        Right side of the join
+    how:
+        Type of join (left, outer, full, etc.)
     on:
         A list of strings for the columns to join on. The columns must exist
         on both sides.
     on_expression:
         String expression the join on condition. The expression can include
         `left` and `other` dataframe references.
-    other:
-        Right side of the join
+    left_watermark
+        Watermark for left dataframe
+    other_watermark
+        Watermark for other dataframe
     time_constraint_interval_lower:
         Lower bound for a spark streaming event-time constraint
     time_constraint_interval_upper:
         Upper bound for a spark streaming event-time constraint
 
     Examples
     --------
     ```py
-    from laktory import models
+    import pandas as pd
+
+    df_prices = spark.createDataFrame(
+        pd.DataFrame(
+            {
+                "symbol": ["AAPL", "GOOGL"],
+                "price": [200.0, 205.0],
+            }
+        )
+    )
+
+    df_meta = spark.createDataFrame(
+        pd.DataFrame(
+            {
+                "symbol": ["AAPL", "GOOGL"],
+                "name": ["Apple", "Google"],
+            }
+        )
+    )
 
-    table = models.Table(
-        name="slv_star_stock_prices",
-        builder={
-            "layer": "SILVER",
-            "table_source": {
-                "name": "slv_stock_prices",
-            },
-            "joins": [
-                {
-                    "other": {
-                        "name": "slv_stock_metadata",
-                        "read_as_stream": False,
-                        "selects": ["symbol", "currency", "first_trader"],
-                    },
-                    "on": ["symbol"],
-                }
-            ],
-        },
-    )
-
-    table = models.Table(
-        name="slv_star_stock_prices",
-        builder={
-            "layer": "SILVER",
-            "table_source": {
-                "name": "slv_stock_prices",
-            },
-            "joins": [
-                {
-                    "other": {
-                        "name": "slv_stock_metadata",
-                        "read_as_stream": False,
-                        "selects": ["symbol", "currency", "first_trader"],
-                    },
-                    "on_expression": "left.symbol == other.symbol",
-                }
-            ],
-        },
+    df = df_prices.smart_join(
+        other=df_meta,
+        on=["symbol"],
     )
+
+    print(df.toPandas().to_string())
+    '''
+       price    name symbol
+    0  200.0   Apple   AAPL
+    1  205.0  Google  GOOGL
+    '''
     ```
 
     References
     ----------
 
     * [pyspark join](https://spark.apache.org/docs/3.1.2/api/python/reference/api/pyspark.sql.DataFrame.join.html)
     * [spark streaming join](https://spark.apache.org/docs/latest/structured-streaming-programming-guide.html#inner-joins-with-optional-watermarking)
     """
+    import pyspark.sql.functions as F
+
+    logger.info(f"Executing {left} {how} JOIN {other}")
 
-    how: str = "left"
-    left: TableDataSource = None
-    on: list[str] = []
-    on_expression: str = None
-    other: TableDataSource
-    time_constraint_interval_lower: str = "60 seconds"
-    time_constraint_interval_upper: str = None
-
-    # ----------------------------------------------------------------------- #
-    # Readers                                                                 #
-    # ----------------------------------------------------------------------- #
-
-    def execute(self, spark) -> DataFrame:
-        """
-        Execute join
-
-        Parameters
-        ----------
-        spark: SparkSession
-            Spark session
-
-        Returns
-        -------
-        : DataFrame
-            Output DataFrame
-        """
-        import pyspark.sql.functions as F
-
-        logger.info(f"Executing {self.left.name} {self.how} JOIN {self.other.name}")
-
-        left_df = self.left.read(spark)
-        other_df = self.other.read(spark)
-
-        # Add watermark
-        other_cols = []
-        if self.other.watermark is not None:
-            other_cols += [F.col(self.other.watermark.column).alias("_other_wc")]
-        other_cols += [F.col(c) for c in other_df.columns]
-        other_df = other_df.select(other_cols)
-
-        # Drop duplicates to prevent adding rows to left
-        if self.on:
-            other_df = other_df.dropDuplicates(self.on)
-
-        _join = []
-        for c in self.on:
-            _join += [f"left.{c} == other.{c}"]
-        if self.on_expression:
-            _join += [self.on_expression]
-
-        if self.other.watermark is not None:
-            if self.time_constraint_interval_lower:
-                _join += [
-                    f"left.{self.left.watermark.column} >= other._other_wc - interval {self.time_constraint_interval_lower}"
-                ]
-            if self.time_constraint_interval_upper:
-                _join += [
-                    f"left.{self.left.watermark.column} <= other._other_wc + interval {self.time_constraint_interval_upper}"
-                ]
-        _join = " AND ".join(_join)
-
-        logger.info(f"   ON {_join}")
-
-        logger.info(f"Left Schema:")
-        left_df.printSchema()
-
-        logger.info(f"Other Schema:")
-        other_df.printSchema()
-
-        df = (
-            left_df.alias("left")
-            .join(
-                other=other_df.alias("other"),
-                on=F.expr(_join),
-                how=self.how,
-            )
-            .drop()
+    # Parse inputs
+    if on is None:
+        on = []
+    wml = left_watermark
+    wmo = other_watermark
+    if wml is not None and not isinstance(wml, Watermark):
+        wml = Watermark(**wml)
+    if wmo is not None and not isinstance(wmo, Watermark):
+        wmo = Watermark(**wmo)
+
+    # Set watermarks
+    if wml is None:
+        try:
+            wml = watermark(left)
+        except Exception as e:
+            logger.warn(f"Could not fetch wartermark from left dataframe: {e}")
+    else:
+        left = left.withWatermark(wml.column, wml.threshold)
+    if wmo is None:
+        try:
+            wmo = watermark(other)
+        except Exception as e:
+            logger.warn(f"Could not fetch wartermark from other dataframe: {e}")
+    else:
+        other = other.withWatermark(wmo.column, wmo.threshold)
+
+    # Add watermark
+    other_cols = []
+    if wmo is not None:
+        other_cols += [F.col(wmo.column).alias("_other_wc")]
+    other_cols += [F.col(c) for c in other.columns]
+    other = other.select(other_cols)
+
+    # Drop duplicates to prevent adding rows to left
+    if on:
+        other = other.dropDuplicates(on)
+
+    _join = []
+    for c in on:
+        _join += [f"left.{c} == other.{c}"]
+    if on_expression:
+        _join += [on_expression]
+
+    if wmo is not None:
+        if time_constraint_interval_lower:
+            _join += [
+                f"left.{wml.column} >= other._other_wc - interval {time_constraint_interval_lower}"
+            ]
+        if time_constraint_interval_upper:
+            _join += [
+                f"left.{wml.column} <= other._other_wc + interval {time_constraint_interval_upper}"
+            ]
+    _join = " AND ".join(_join)
+
+    logger.info(f"   ON {_join}")
+
+    logger.info(f"Left Schema:")
+    left.printSchema()
+
+    logger.info(f"Other Schema:")
+    other.printSchema()
+
+    df = (
+        left.alias("left")
+        .join(
+            other=other.alias("other"),
+            on=F.expr(_join),
+            how=how,
         )
+        .drop()
+    )
 
-        # Find duplicated columns (because of join)
-        d = defaultdict(lambda: 0)
-        for c in df.columns:
-            d[c] += 1
-
-        # Drop duplicated columns
-        for c, v in d.items():
-            if v < 2 or c not in _join:
-                continue
-            df = df.withColumn("__tmp", F.coalesce(f"left.{c}", f"other.{c}"))
-            df = df.drop(c)
-            df = df.withColumn(c, F.col("__tmp"))
-            df = df.drop("__tmp")
-
-        # Drop watermark column
-        if self.other.watermark is not None:
-            df = df.drop(F.col(f"other._other_wc"))
-        logger.info(f"Joined Schema:")
-        df.printSchema()
+    # Find duplicated columns (because of join)
+    d = defaultdict(lambda: 0)
+    for c in df.columns:
+        d[c] += 1
+
+    # Drop duplicated columns
+    for c, v in d.items():
+        if v < 2 or c not in _join:
+            continue
+        df = df.withColumn("__tmp", F.coalesce(f"left.{c}", f"other.{c}"))
+        df = df.drop(c)
+        df = df.withColumn(c, F.col("__tmp"))
+        df = df.drop("__tmp")
+
+    # Drop watermark column
+    if wmo is not None:
+        df = df.drop(F.col(f"other._other_wc"))
+    logger.info(f"Joined Schema:")
+    df.printSchema()
 
-        return df
+    return df
 
 
 if __name__ == "__main__":
-    from laktory import models
+    from laktory._testing.stockprices import spark
+    import pandas as pd
 
-    table = models.Table(
-        name="slv_star_stock_prices",
-        builder={
-            "layer": "SILVER",
-            "table_source": {
-                "name": "slv_stock_prices",
-            },
-            "joins": [
-                {
-                    "other": {
-                        "name": "slv_stock_metadata",
-                        "read_as_stream": False,
-                        "selects": ["symbol", "currency", "first_trader"],
-                    },
-                    "on": ["symbol"],
-                }
-            ],
-        },
+    df_prices = spark.createDataFrame(
+        pd.DataFrame(
+            {
+                "symbol": ["AAPL", "GOOGL"],
+                "price": [200.0, 205.0],
+            }
+        )
     )
 
-    # Read
-    df = table.builder.read_source(spark)
+    df_meta = spark.createDataFrame(
+        pd.DataFrame(
+            {
+                "symbol": ["AAPL", "GOOGL"],
+                "name": ["Apple", "Google"],
+            }
+        )
+    )
 
-    # Process
-    df = table.builder.process(df, spark)
+    df = df_prices.smart_join(
+        other=df_meta,
+        on=["symbol"],
+    )
```

### Comparing `laktory-0.1.9/laktory/models/sql/tablewindowfilter.py` & `laktory-0.2.0/laktory/spark/dataframe/window_filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,127 +1,138 @@
+from pydantic import BaseModel
 from typing import Union
+from pyspark.sql.dataframe import DataFrame
 
 from laktory._logger import get_logger
-from laktory.models.basemodel import BaseModel
+
 
 logger = get_logger(__name__)
 
 
 class OrderBy(BaseModel):
     sql_expression: str
     desc: bool = False
 
 
-class TableWindowFilter(BaseModel):
+def window_filter(
+    df,
+    partition_by: Union[list[str], None],
+    order_by: Union[list[OrderBy], None] = None,
+    drop_row_index: bool = True,
+    row_index_name: str = "_row_index",
+    rows_to_keep: int = 1,
+) -> DataFrame:
     """
-    Specifications of a window-based filtering.
+    Apply spark window-based filtering
 
-    Attributes
+    Parameters
     ----------
-    descending:
-        If `True` rows are sorted in descending order before dropping rows
-        from each window.
-    drop_row_index:
-        If `True`, the row index column is dropped
-    order_by:
-        Defines the column used for sorting before dropping rows
+    df:
+        DataFrame
     partition_by
         Defines the columns used for grouping into Windows
+    order_by:
+        Defines the column used for sorting before dropping rows
+    drop_row_index:
+        If `True`, the row index column is dropped
     row_index_name:
         Group-specific and sorted rows index name
     rows_to_keep:
         How many rows to keep per window
 
+
     Examples
     --------
     ```py
-    from datetime import datetime
-    from laktory import models
+    import pyspark.sql.functions as F
+
+    from laktory._testing import spark
 
     df0 = spark.createDataFrame(
         [
-            [datetime(2023, 1, 1), "APPL", 200.0],
-            [datetime(2023, 1, 2), "APPL", 202.0],
-            [datetime(2023, 1, 3), "APPL", 201.5],
-            [datetime(2023, 1, 1), "GOOL", 200.0],
-            [datetime(2023, 1, 2), "GOOL", 202.0],
-            [datetime(2023, 1, 3), "GOOL", 201.5],
+            ["2023-01-01T00:00:00Z", "APPL", 200.0],
+            ["2023-01-02T00:00:00Z", "APPL", 202.0],
+            ["2023-01-03T00:00:00Z", "APPL", 201.5],
+            ["2023-01-01T00:00:00Z", "GOOL", 200.0],
+            ["2023-01-02T00:00:00Z", "GOOL", 202.0],
+            ["2023-01-03T00:00:00Z", "GOOL", 201.5],
         ],
         ["created_at", "symbol", "price"],
-    )
+    ).withColumn("created_at", F.col("created_at").cast("timestamp"))
 
-    f = models.TableWindowFilter(
+    df = df0.window_filter(
         partition_by=["symbol"],
         order_by=[
             {"sql_expression": "created_at", "desc": True},
         ],
         drop_row_index=False,
         rows_to_keep=1,
     )
-    df1 = f.execute(df0)
+
+    print(df.toPandas())
+    '''
+      created_at symbol  price  _row_index
+    0 2023-01-03   APPL  201.5           1
+    1 2023-01-03   GOOL  201.5           1
+    '''
     ```
 
     References
     ----------
 
-    * [pyspark Window](https://spark.apache.org/docs/latest/api/python/reference/pyspark.sql/api/pyspark.sql.Window.html)
+    * [pyspark window](https://spark.apache.org/docs/3.1.3/api/python/reference/api/pyspark.sql.functions.window.html)
     """
+    from pyspark.sql import Window
+    import pyspark.sql.functions as F
+
+    # Partition by
+    w = Window.partitionBy(*partition_by)
 
-    descending: bool = True
-    drop_row_index: bool = True
-    order_by: Union[list[OrderBy], None] = None
-    partition_by: Union[list[str], None]
-    row_index_name: str = "_row_index"
-    rows_to_keep: int = 1
-
-    def execute(self, df):
-        """
-        Execute window filtering
-
-        Parameters
-        ----------
-        df: DataFrame
-            Spark DataFrame
-
-        Returns
-        -------
-        : DataFrame
-            Output DataFrame
-        """
-        from pyspark.sql import Window
-        import pyspark.sql.functions as F
-
-        # Partition by
-        w = Window.partitionBy(*self.partition_by)
-
-        # Order by
-        if self.order_by:
-            order_bys = []
-            for o in self.order_by:
-                order_bys += [F.expr(o.sql_expression)]
-                if o.desc:
-                    order_bys[-1] = order_bys[-1].desc()
-            w = w.orderBy(*order_bys)
-
-        # Set rows index
-        df = df.withColumn(self.row_index_name, F.row_number().over(w))
-
-        # Filter
-        df = df.filter(F.col(self.row_index_name) <= self.rows_to_keep)
-        if self.drop_row_index:
-            df = df.drop(self.row_index_name)
+    # Order by
+    if order_by:
+        order_bys = []
+        for o in order_by:
+            if not isinstance(o, OrderBy):
+                o = OrderBy(**o)
+            order_bys += [F.expr(o.sql_expression)]
+            if o.desc:
+                order_bys[-1] = order_bys[-1].desc()
+        w = w.orderBy(*order_bys)
+
+    # Set rows index
+    df = df.withColumn(row_index_name, F.row_number().over(w))
+
+    # Filter
+    df = df.filter(F.col(row_index_name) <= rows_to_keep)
+    if drop_row_index:
+        df = df.drop(row_index_name)
 
-        return df
+    return df
 
 
 if __name__ == "__main__":
-    from laktory import models
+    import pyspark.sql.functions as F
+
+    from laktory._testing import spark
+
+    df0 = spark.createDataFrame(
+        [
+            ["2023-01-01T00:00:00Z", "APPL", 200.0],
+            ["2023-01-02T00:00:00Z", "APPL", 202.0],
+            ["2023-01-03T00:00:00Z", "APPL", 201.5],
+            ["2023-01-01T00:00:00Z", "GOOL", 200.0],
+            ["2023-01-02T00:00:00Z", "GOOL", 202.0],
+            ["2023-01-03T00:00:00Z", "GOOL", 201.5],
+        ],
+        ["created_at", "symbol", "price"],
+    ).withColumn("created_at", F.col("created_at").cast("timestamp"))
 
-    f = models.TableWindowFilter(
+    df = df0.window_filter(
         partition_by=["symbol"],
         order_by=[
             {"sql_expression": "created_at", "desc": True},
         ],
         drop_row_index=False,
         rows_to_keep=1,
     )
-    df1 = f.execute(df0)
+
+    print(df.toPandas())
```

### Comparing `laktory-0.1.9/laktory/models/sql/volume.py` & `laktory-0.2.0/laktory/models/sql/volume.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/stacks/pulumistack.py` & `laktory-0.2.0/laktory/models/stacks/pulumistack.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import yaml
 from typing import Any
 from typing import Union
 from pydantic import Field
 
+from laktory._useragent import set_databricks_sdk_upstream
 from laktory._logger import get_logger
 from laktory._settings import settings
 from laktory.constants import CACHE_ROOT
 from laktory.models.basemodel import BaseModel
 
 logger = get_logger(__name__)
 
@@ -83,25 +84,28 @@
 
         with open(filepath, "w") as fp:
             yaml.dump(self.model_dump(), fp)
 
         return filepath
 
     def _call(self, command: str, stack: str, flags: list[str] = None):
-        from laktory.cli._worker import Worker
+        from laktory.cli._common import Worker
 
         self.write()
         worker = Worker()
 
         cmd = ["pulumi", command]
         cmd += ["-s", stack]
 
         if flags is not None:
             cmd += flags
 
+        # Inject user-agent value for monitoring usage as a Databricks partner
+        set_databricks_sdk_upstream()
+
         worker.run(
             cmd=cmd,
             cwd=CACHE_ROOT,
             raise_exceptions=settings.cli_raise_external_exceptions,
         )
 
     def preview(self, stack: str = None, flags: list[str] = None) -> None:
```

### Comparing `laktory-0.1.9/laktory/models/stacks/stack.py` & `laktory-0.2.0/laktory/models/stacks/stack.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/models/stacks/terraformstack.py` & `laktory-0.2.0/laktory/models/stacks/terraformstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import json
 from collections import defaultdict
 from typing import Any
 from typing import Union
 from pydantic import model_validator
+
+from laktory._useragent import set_databricks_sdk_upstream
 from laktory._logger import get_logger
 from laktory._settings import settings
 from laktory.constants import CACHE_ROOT
 from laktory.models.basemodel import BaseModel
 
 logger = get_logger(__name__)
 
@@ -122,24 +124,27 @@
 
         with open(filepath, "w") as fp:
             json.dump(self.model_dump(), fp, indent=4)
 
         return filepath
 
     def _call(self, command: str, flags: list[str] = None):
-        from laktory.cli._worker import Worker
+        from laktory.cli._common import Worker
 
         self.write()
         worker = Worker()
 
         cmd = ["terraform", command]
 
         if flags is not None:
             cmd += flags
 
+        # Inject user-agent value for monitoring usage as a Databricks partner
+        set_databricks_sdk_upstream()
+
         worker.run(
             cmd=cmd,
             cwd=CACHE_ROOT,
             raise_exceptions=settings.cli_raise_external_exceptions,
         )
 
     def init(self, flags: list[str] = None) -> None:
```

### Comparing `laktory-0.1.9/laktory/resources/data/stock_prices.json` & `laktory-0.2.0/laktory/resources/data/stock_prices.json`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/resources/notebooks/dlt_brz_template.py` & `laktory-0.2.0/laktory/resources/notebooks/dlt_brz_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/resources/notebooks/dlt_gld_template.py` & `laktory-0.2.0/laktory/resources/notebooks/dlt_gld_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/resources/notebooks/dlt_slv_star_template.py` & `laktory-0.2.0/laktory/resources/notebooks/dlt_slv_star_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/resources/notebooks/dlt_slv_template.py` & `laktory-0.2.0/laktory/resources/notebooks/dlt_slv_template.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/dataframe/has_column.py` & `laktory-0.2.0/laktory/spark/dataframe/has_column.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/dataframe/schema_flat.py` & `laktory-0.2.0/laktory/spark/dataframe/schema_flat.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/dataframe/show_string.py` & `laktory-0.2.0/laktory/spark/dataframe/show_string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/functions/_common.py` & `laktory-0.2.0/laktory/spark/functions/_common.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/functions/logical.py` & `laktory-0.2.0/laktory/spark/functions/logical.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/functions/math.py` & `laktory-0.2.0/laktory/spark/functions/math.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/functions/string.py` & `laktory-0.2.0/laktory/spark/functions/string.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/spark/functions/units.py` & `laktory-0.2.0/laktory/spark/functions/units.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory/version.py` & `laktory-0.2.0/laktory/version.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/laktory.egg-info/PKG-INFO` & `laktory-0.2.0/laktory.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laktory
-Version: 0.1.9
+Version: 0.2.0
 Summary: A DataOps framework for building a lakehouse
 Author-email: Olivier Soucy <olivier.soucy@okube.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/opencubes-ai/laktory
 Project-URL: Bug Tracker, https://github.com/opencubes-ai/laktory/issues
 Keywords: one,two
 Classifier: Development Status :: 4 - Beta
@@ -14,22 +14,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: databricks-sdk
 Requires-Dist: inflect
 Requires-Dist: planck
 Requires-Dist: prompt_toolkit
 Requires-Dist: pulumi
-Requires-Dist: pulumi_databricks
+Requires-Dist: pulumi_databricks>=1.36
 Requires-Dist: pulumi_random
 Requires-Dist: pyyaml
 Requires-Dist: pydantic>=2
+Requires-Dist: python-dateutil
 Requires-Dist: settus
 Requires-Dist: typer[all]
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flit; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
@@ -99,23 +101,25 @@
     catalog_name="prod",
     schema_name="finance",
     timestamp_key="data.created_at",
     builder={
         "layer": "SILVER",
         "table_source": {
             "name": "brz_stock_prices",
+        },
+        "spark_chain": {
+            "nodes": [
+                {
+                    "column": {"name": "symbol"},
+                    "type": "string",
+                    "sql_expression": "data.symbol"
+                }
+            ]
         }
     },
-    columns=[
-        {
-            "name": "symbol",
-            "type": "string",
-            "sql_expression": "data.symbol"
-        }
-    ]
 )
 
 print(table)
 #> catalog_name='prod' columns=[Column(catalog_name='prod', comment=None, name='symbol', pii=None, schema_name='finance', spark_func_args=[], spark_func_kwargs={}, spark_func_name=None, sql_expression='data.symbol', table_name='brz_stock_prices', type='string', unit=None)] comment=None data=None grants=None name='brz_stock_prices' primary_key=None schema_name='finance' timestamp_key='data.created_at' builder=TableBuilder(drop_source_columns=True, drop_duplicates=None, event_source=None, joins=[], pipeline_name=None, table_source=TableDataSource(read_as_stream=True, catalog_name='prod', cdc=None, selects=None, filter=None, from_pipeline=True, name='brz_stock_prices', schema_name='finance', watermark=None), layer='SILVER')
 ```
 
 To get started with a more useful example, jump into the [Quickstart](https://www.laktory.ai/quickstart/).
```

### Comparing `laktory-0.1.9/mkdocs.yml` & `laktory-0.2.0/mkdocs.yml`

 * *Files 9% similar despite different names*

```diff
@@ -184,37 +184,39 @@
         - AzureProvider: api/models/providers/azure.md
         - AzurePulumiProvider: api/models/providers/azurepulumi.md
         - AWSProvider: api/models/providers/aws.md
         - DatabricksProvider: api/models/providers/databricks.md
       - Resources:
         - BaseResource: api/models/resources/baseresource.md
         - PulumiResource: api/models/resources/pulumiresource.md
+      - Spark:
+        - SparkChain: api/models/spark/sparkchain.md
+        - SparkChainNode: api/models/spark/sparkchainnode.md
+        - SparkFuncArg: api/models/spark/sparkfuncarg.md
       - SQL:
           - api/models/sql/catalog.md
           - api/models/sql/column.md
           - api/models/sql/schema.md
           - api/models/sql/table.md
-          - TableAggregation: api/models/sql/tableaggregation.md
+          - TableExpectations: api/models/sql/tableexpectation.md
           - TableBuilder: api/models/sql/tablebuilder.md
-          - TableExpectation: api/models/sql/tableexpectation.md
-          - TableJoin: api/models/sql/tablejoin.md
-          - TableWindowFilter: api/models/sql/tablewindowfilter.md
           - api/models/sql/volume.md
       - Stacks:
           - Stack: api/models/stacks/stack.md
           - PulumiStack: api/models/stacks/pulumistack.md
           - TerraformStack: api/models/stacks/terraformstack.md
-
-
     - CLI: api/cli.md
     - Spark:
       - DataFrame:
+        - groupby_and_agg: api/spark/dataframe/groupby_and_agg.md
         - has_column: api/spark/dataframe/has_column.md
         - schema_flat: api/spark/dataframe/schema_flat.md
+        - smart_join: api/spark/dataframe/smart_join.md
         - show_string: api/spark/dataframe/show_string.md
+        - window_filter: api/spark/dataframe/window_filter.md
       - Functions:
         - constants: api/spark/functions/_constants.md
         - add: api/spark/functions/add.md
         - convert_units: api/spark/functions/convert_units.md
         - div: api/spark/functions/div.md
         - mul: api/spark/functions/mul.md
         - poly1: api/spark/functions/poly1.md
@@ -227,8 +229,15 @@
     - DLT:
       - apply_changes: api/dlt/apply_changes.md
       - get_df: api/dlt/get_df.md
       - is_debug: api/dlt/is_debug.md
       - is_mocked: api/dlt/is_mocked.md
       - read: api/dlt/read.md
       - read_stream: api/dlt/read_stream.md
+    - Dispatcher:
+        - Dispatcher: api/dispatcher/dispatcher.md
+        - DispatcherRunner: api/dispatcher/dispatcherrunner.md
+        - JobRunner: api/dispatcher/jobrunner.md
+        - PipelineRunner: api/dispatcher/pipelinerunner.md
+    - Datetime: api/datetime.md
+
   - Changelog: changelog.md
```

### Comparing `laktory-0.1.9/pyproject.toml` & `laktory-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,22 +31,24 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
+    "databricks-sdk",
     "inflect",
     "planck",
     "prompt_toolkit",
     "pulumi",
-    "pulumi_databricks",
+    "pulumi_databricks>=1.36",  # required to monitor laktory usage
     "pulumi_random",
     "pyyaml",
     "pydantic>=2",
+    "python-dateutil",
     "settus",
     "typer[all]",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
```

### Comparing `laktory-0.1.9/tests/stack.yaml` & `laktory-0.2.0/tests/data/stack.yaml`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_basemodel.py` & `laktory-0.2.0/tests/test_table.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,342 +1,290 @@
-import pulumi
-import os
+import pytest
+from pydantic import ValidationError
 
-from laktory.models import BaseModel
 from laktory.models import Table
-from laktory.models import Schema
-from laktory.models import Job
-from laktory import settings
-from pulumi_random import RandomString
-
-dirpath = os.path.dirname(__file__)
-
-env = RandomString("env", length=3, upper=False, numeric=False, special=False)
-schema_name = RandomString(
-    "schema", length=5, upper=False, numeric=False, special=False
-)
-
-
-schema = Schema(
-    name="${vars.env}.${vars.schema_name}",
-    catalog_name="${vars.env}",
-    tables=[
-        Table(
-            name="AAPL",
-            columns=[
-                {
-                    "name": "open",
-                    "type": "double",
-                    "spark_func_kwargs": {
-                        "window_length": 2
-                    },  # window_length should not be converted to camel
-                },
-                {
-                    "name": "${resources.close.id}",
-                    "type": "double",
-                },
-            ],
-        ),
-        Table(
-            name="GOOGL",
-            columns=[
-                {
-                    "name": "${vars.dynamic_column}",
-                    "type": "double",
-                },
-                {
-                    "name": "high",
-                    "type": "double",
-                },
-            ],
-        ),
-    ],
-    variables={
-        "DYNAMIC_COLUMN": "low",
-        "env": env.id,
-        "schema_name": schema_name.id,
-        # r"\$\{resources\.([\w.]+)\}": r"\1",
-        r"\$\{resources\.([\w.]+)\}": r"${ \1 }",
-    },
-)
-
-
-def test_read_yaml():
-    class OHLC(BaseModel):
-        open: float = None
-        high: float = None
-        low: float = None
-        close: float = None
-
-    class Price(BaseModel):
-        timestamp: float
-        ohlc: OHLC
-
-    class StockPrices(BaseModel):
-        symbol: str
-        prices: list[Price]
-
-    with open(os.path.join(dirpath, "stockprices0.yaml"), "r") as fp:
-        stockprices = StockPrices.model_validate_yaml(fp)
-
-    assert stockprices.model_dump() == {
-        "symbol": "AAPL",
-        "prices": [
+from laktory._testing.stockprices import table_slv
+from laktory._testing.stockprices import table_slv_join
+from laktory._testing.stockprices import spark
+
+
+def test_model():
+    print(table_slv.model_dump())
+    data = table_slv.model_dump()
+    assert data == {
+        "builder": {
+            "add_laktory_columns": True,
+            "as_dlt_view": False,
+            "drop_duplicates": None,
+            "drop_source_columns": True,
+            "event_source": None,
+            "layer": "SILVER",
+            "pipeline_name": None,
+            "table_source": {
+                "drops": None,
+                "filter": None,
+                "read_as_stream": True,
+                "renames": None,
+                "selects": None,
+                "watermark": None,
+                "catalog_name": "dev",
+                "cdc": None,
+                "fmt": "DELTA",
+                "from_pipeline": True,
+                "name": "brz_stock_prices",
+                "path": None,
+                "schema_name": "markets",
+            },
+            "template": "SILVER",
+            "spark_chain": None,
+        },
+        "catalog_name": "dev",
+        "columns": [
             {
-                "timestamp": 1.0,
-                "ohlc": {"open": 0.0, "high": None, "low": None, "close": 1.0},
+                "catalog_name": "dev",
+                "comment": None,
+                "name": "created_at",
+                "pii": None,
+                "raise_missing_arg_exception": True,
+                "schema_name": "markets",
+                "table_name": "slv_stock_prices",
+                "type": "timestamp",
+                "unit": None,
+            },
+            {
+                "catalog_name": "dev",
+                "comment": None,
+                "name": "symbol",
+                "pii": None,
+                "raise_missing_arg_exception": True,
+                "schema_name": "markets",
+                "table_name": "slv_stock_prices",
+                "type": "string",
+                "unit": None,
             },
             {
-                "timestamp": 2.0,
-                "ohlc": {"open": 1.0, "high": None, "low": None, "close": 2.0},
+                "catalog_name": "dev",
+                "comment": None,
+                "name": "open",
+                "pii": None,
+                "raise_missing_arg_exception": True,
+                "schema_name": "markets",
+                "table_name": "slv_stock_prices",
+                "type": "double",
+                "unit": None,
+            },
+            {
+                "catalog_name": "dev",
+                "comment": None,
+                "name": "close",
+                "pii": None,
+                "raise_missing_arg_exception": True,
+                "schema_name": "markets",
+                "table_name": "slv_stock_prices",
+                "type": "double",
+                "unit": None,
             },
+        ],
+        "comment": None,
+        "data": [
+            ["2023-11-01T00:00:00Z", "AAPL", 1, 2],
+            ["2023-11-01T01:00:00Z", "AAPL", 3, 4],
+            ["2023-11-01T00:00:00Z", "GOOGL", 3, 4],
+            ["2023-11-01T01:00:00Z", "GOOGL", 5, 6],
+        ],
+        "data_source_format": "DELTA",
+        "expectations": [
+            {"name": "positive_price", "expression": "open > 0", "action": "FAIL"},
             {
-                "timestamp": 3.0,
-                "ohlc": {"open": None, "high": None, "low": 3.0, "close": 4.0},
+                "name": "recent_price",
+                "expression": "created_at > '2023-01-01'",
+                "action": "DROP",
             },
         ],
+        "grants": None,
+        "name": "slv_stock_prices",
+        "primary_key": None,
+        "schema_name": "markets",
+        "table_type": "MANAGED",
+        "timestamp_key": None,
+        "view_definition": None,
+        "warehouse_id": "08b717ce051a0261",
     }
 
+    assert not table_slv.is_from_cdc
 
-def test_camelize():
-    settings.camel_serialization = True
-    dump = schema.model_dump()
-    print(dump)
-    assert dump == {
-        "comment": None,
-        "grants": None,
-        "name": "${vars.env}.${vars.schema_name}",
-        "tables": [
-            {
-                "builder": {
-                    "aggregation": None,
-                    "filter": None,
-                    "joins": [],
-                    "layer": None,
-                    "selects": None,
-                    "template": None,
-                    "unions": [],
-                    "asDltView": False,
-                    "dropColumns": [],
-                    "dropDuplicates": None,
-                    "dropSourceColumns": None,
-                    "eventSource": None,
-                    "joinsPostAggregation": [],
-                    "pipelineName": None,
-                    "tableSource": None,
-                    "windowFilter": None,
-                },
-                "columns": [
+    assert table_slv.warning_expectations == {}
+    assert table_slv.drop_expectations == {"recent_price": "created_at > '2023-01-01'"}
+    assert table_slv.fail_expectations == {"positive_price": "open > 0"}
+
+    # Invalid layer
+    with pytest.raises(ValidationError):
+        Table(name="googl", layer="ROUGE")
+
+
+def test_data():
+    data = table_slv.to_df().to_dict(orient="records")
+    print(data)
+    assert data == [
+        {"created_at": "2023-11-01T00:00:00Z", "symbol": "AAPL", "open": 1, "close": 2},
+        {"created_at": "2023-11-01T01:00:00Z", "symbol": "AAPL", "open": 3, "close": 4},
+        {
+            "created_at": "2023-11-01T00:00:00Z",
+            "symbol": "GOOGL",
+            "open": 3,
+            "close": 4,
+        },
+        {
+            "created_at": "2023-11-01T01:00:00Z",
+            "symbol": "GOOGL",
+            "open": 5,
+            "close": 6,
+        },
+    ]
+
+
+def test_table_builder():
+    # Test model
+    data = table_slv_join.model_dump()
+    print(data)
+    assert data == {
+        "builder": {
+            "add_laktory_columns": True,
+            "as_dlt_view": False,
+            "drop_duplicates": None,
+            "drop_source_columns": False,
+            "event_source": None,
+            "layer": "SILVER",
+            "pipeline_name": None,
+            "table_source": {
+                "drops": None,
+                "filter": "created_at = '2023-09-01T00:00:00Z'",
+                "read_as_stream": True,
+                "renames": None,
+                "selects": None,
+                "watermark": None,
+                "catalog_name": "dev",
+                "cdc": None,
+                "fmt": "DELTA",
+                "from_pipeline": True,
+                "name": "slv_stock_prices",
+                "path": None,
+                "schema_name": "markets",
+            },
+            "template": "SILVER",
+            "spark_chain": {
+                "nodes": [
                     {
-                        "comment": None,
-                        "name": "open",
-                        "pii": None,
-                        "type": "double",
-                        "unit": None,
-                        "catalogName": None,
-                        "raiseMissingArgException": True,
-                        "schemaName": None,
-                        "sparkFuncArgs": [],
-                        "sparkFuncKwargs": {
-                            "window_length": {
-                                "value": 2,
-                                "isColumn": False,
-                                "toLit": True,
-                                "toExpr": False,
-                            }
+                        "allow_missing_column_args": False,
+                        "column": None,
+                        "spark_func_args": [],
+                        "spark_func_kwargs": {
+                            "other": {
+                                "value": {
+                                    "drops": None,
+                                    "filter": None,
+                                    "read_as_stream": True,
+                                    "renames": {"symbol2": "symbol"},
+                                    "selects": None,
+                                    "watermark": None,
+                                    "catalog_name": "dev",
+                                    "cdc": None,
+                                    "fmt": "DELTA",
+                                    "from_pipeline": True,
+                                    "name": "slv_stockmeta",
+                                    "path": None,
+                                    "schema_name": "markets",
+                                }
+                            },
+                            "on": {"value": ["symbol"]},
                         },
-                        "sparkFuncName": None,
-                        "sqlExpression": None,
-                        "tableName": "AAPL",
+                        "spark_func_name": "smart_join",
+                        "sql_expression": None,
                     },
                     {
-                        "comment": None,
-                        "name": "${resources.close.id}",
-                        "pii": None,
-                        "type": "double",
-                        "unit": None,
-                        "catalogName": None,
-                        "raiseMissingArgException": True,
-                        "schemaName": None,
-                        "sparkFuncArgs": [],
-                        "sparkFuncKwargs": {},
-                        "sparkFuncName": None,
-                        "sqlExpression": None,
-                        "tableName": "AAPL",
+                        "allow_missing_column_args": False,
+                        "column": {"name": "symbol3", "type": "string", "unit": None},
+                        "spark_func_args": [],
+                        "spark_func_kwargs": {},
+                        "spark_func_name": None,
+                        "sql_expression": "symbol",
                     },
-                ],
-                "comment": None,
-                "data": None,
-                "expectations": [],
-                "grants": None,
-                "name": "AAPL",
-                "catalogName": "${vars.env}",
-                "dataSourceFormat": "DELTA",
-                "primaryKey": None,
-                "schemaName": "${vars.env}.${vars.schema_name}",
-                "tableType": "MANAGED",
-                "timestampKey": None,
-                "viewDefinition": None,
-                "warehouseId": "08b717ce051a0261",
-            },
-            {
-                "builder": {
-                    "aggregation": None,
-                    "filter": None,
-                    "joins": [],
-                    "layer": None,
-                    "selects": None,
-                    "template": None,
-                    "unions": [],
-                    "asDltView": False,
-                    "dropColumns": [],
-                    "dropDuplicates": None,
-                    "dropSourceColumns": None,
-                    "eventSource": None,
-                    "joinsPostAggregation": [],
-                    "pipelineName": None,
-                    "tableSource": None,
-                    "windowFilter": None,
-                },
-                "columns": [
                     {
-                        "comment": None,
-                        "name": "${vars.dynamic_column}",
-                        "pii": None,
-                        "type": "double",
-                        "unit": None,
-                        "catalogName": None,
-                        "raiseMissingArgException": True,
-                        "schemaName": None,
-                        "sparkFuncArgs": [],
-                        "sparkFuncKwargs": {},
-                        "sparkFuncName": None,
-                        "sqlExpression": None,
-                        "tableName": "GOOGL",
+                        "allow_missing_column_args": False,
+                        "column": None,
+                        "spark_func_args": [{"value": "symbol"}],
+                        "spark_func_kwargs": {},
+                        "spark_func_name": "drop",
+                        "sql_expression": None,
                     },
                     {
-                        "comment": None,
-                        "name": "high",
-                        "pii": None,
-                        "type": "double",
-                        "unit": None,
-                        "catalogName": None,
-                        "raiseMissingArgException": True,
-                        "schemaName": None,
-                        "sparkFuncArgs": [],
-                        "sparkFuncKwargs": {},
-                        "sparkFuncName": None,
-                        "sqlExpression": None,
-                        "tableName": "GOOGL",
+                        "allow_missing_column_args": False,
+                        "column": None,
+                        "spark_func_args": [],
+                        "spark_func_kwargs": {
+                            "other": {
+                                "value": {
+                                    "drops": None,
+                                    "filter": None,
+                                    "read_as_stream": True,
+                                    "renames": None,
+                                    "selects": None,
+                                    "watermark": None,
+                                    "catalog_name": "dev",
+                                    "cdc": None,
+                                    "fmt": "DELTA",
+                                    "from_pipeline": True,
+                                    "name": "slv_stock_names",
+                                    "path": None,
+                                    "schema_name": "markets",
+                                }
+                            },
+                            "on": {"value": ["symbol3"]},
+                        },
+                        "spark_func_name": "smart_join",
+                        "sql_expression": None,
                     },
-                ],
-                "comment": None,
-                "data": None,
-                "expectations": [],
-                "grants": None,
-                "name": "GOOGL",
-                "catalogName": "${vars.env}",
-                "dataSourceFormat": "DELTA",
-                "primaryKey": None,
-                "schemaName": "${vars.env}.${vars.schema_name}",
-                "tableType": "MANAGED",
-                "timestampKey": None,
-                "viewDefinition": None,
-                "warehouseId": "08b717ce051a0261",
+                ]
             },
-        ],
-        "volumes": [],
-        "catalogName": "${vars.env}",
-        "forceDestroy": True,
-    }
-
-    settings.camel_serialization = False
-
-
-def test_singular():
-    job = Job(
-        name="my-job",
-        clusters=[
-            {
-                "name": "main",
-                "spark_version": "14.0.x-scala2.12",
-                "node_type_id": "${vars.node_type_id}",
-                "spark_env_vars": {
-                    "AZURE_TENANT_ID": "{{secrets/azure/tenant-id}}",
-                    "LAKTORY_WORKSPACE_ENV": "${vars.env}",
-                },
-            }
-        ],
-    )
-
-    settings.singular_serialization = True
-    dump = job.model_dump()
-    print(dump)
-    assert dump == {
-        "continuous": None,
-        "control_run_state": None,
-        "email_notifications": None,
-        "format": None,
-        "health": None,
-        "max_concurrent_runs": None,
-        "max_retries": None,
-        "min_retry_interval_millis": None,
-        "name": "my-job",
-        "notification_settings": None,
-        "retry_on_timeout": None,
-        "run_as": None,
-        "schedule": None,
-        "tags": {},
-        "timeout_seconds": None,
-        "trigger": None,
-        "webhook_notifications": None,
-        "access_control": [],
-        "cluster": [
-            {
-                "apply_policy_default_values": None,
-                "autoscale": None,
-                "autotermination_minutes": None,
-                "cluster_id": None,
-                "custom_tags": None,
-                "data_security_mode": "USER_ISOLATION",
-                "driver_instance_pool_id": None,
-                "driver_node_type_id": None,
-                "enable_elastic_disk": None,
-                "enable_local_disk_encryption": None,
-                "idempotency_token": None,
-                "init_scripts": [],
-                "instance_pool_id": None,
-                "name": "main",
-                "node_type_id": "${vars.node_type_id}",
-                "num_workers": None,
-                "policy_id": None,
-                "runtime_engine": None,
-                "single_user_name": None,
-                "spark_conf": {},
-                "spark_env_vars": {
-                    "AZURE_TENANT_ID": "{{secrets/azure/tenant-id}}",
-                    "LAKTORY_WORKSPACE_ENV": "${vars.env}",
-                },
-                "spark_version": "14.0.x-scala2.12",
-                "ssh_public_keys": [],
-            }
-        ],
-        "parameter": [],
-        "task": [],
+        },
+        "catalog_name": "dev",
+        "columns": [],
+        "comment": None,
+        "data": None,
+        "data_source_format": "DELTA",
+        "expectations": [],
+        "grants": None,
+        "name": "slv_join_stock_prices",
+        "primary_key": None,
+        "schema_name": "markets",
+        "table_type": "MANAGED",
+        "timestamp_key": None,
+        "view_definition": None,
+        "warehouse_id": "08b717ce051a0261",
     }
-    settings.singular_serialization = False
-
 
-def test_inject_vars():
-    d0 = schema.model_dump()
-    d1 = schema.inject_vars(d0)
-    assert d1["tables"][-1]["columns"][0]["name"] == "low"
-    assert isinstance(d1["name"], pulumi.Output)
-    assert isinstance(d1["catalog_name"], pulumi.Output)
-    assert d1["tables"][0]["columns"][1]["name"] == "${ close.id }"
+    # Test process
+    df = table_slv_join.builder.read_source(spark)
+    df = table_slv_join.builder.process(df, spark=spark)
+    df = df.sort("symbol3")
+    pdf = df.toPandas()
+
+    # Test data
+    assert df.columns == [
+        "created_at",
+        "open",
+        "close",
+        "currency",
+        "first_traded",
+        "name",
+        "symbol3",
+        "_silver_at",
+    ]
+    assert df.count() == 4
+    assert pdf["symbol3"].tolist() == ["AAPL", "AMZN", "GOOGL", "MSFT"]
+    assert pdf["name"].tolist() == ["Apple", "Amazon", "Google", None]
 
 
 if __name__ == "__main__":
-    test_read_yaml()
-    test_camelize()
-    test_singular()
-    test_inject_vars()
+    test_model()
+    test_data()
+    test_table_builder()
```

### Comparing `laktory-0.1.9/tests/test_baseresource.py` & `laktory-0.2.0/tests/test_baseresource.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_catalog.py` & `laktory-0.2.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_cli.py` & `laktory-0.2.0/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import os
 from laktory import app
 from laktory import settings
 from laktory import models
+from laktory._testing import Paths
 from typer.testing import CliRunner
 
 runner = CliRunner()
 settings.cli_raise_external_exceptions = True
-dirpath = os.path.dirname(__file__)
+paths = Paths(__file__)
 
 
 def test_preview_pulumi():
-    filepath = os.path.join(dirpath, "stack.yaml")
+    filepath = os.path.join(paths.data, "stack.yaml")
     result = runner.invoke(app, ["preview", "--env", "dev", "--filepath", filepath])
     assert result.exit_code == 0
 
 
 def test_preview_terraform():
-    filepath = os.path.join(dirpath, "stack.yaml")
+    filepath = os.path.join(paths.data, "stack.yaml")
 
     # Ideally, we would run `laktory init`, but the runner does not seem to handle running multiple commands
     with open(filepath, "r") as fp:
         pstack = models.Stack.model_validate_yaml(fp).to_terraform(env="dev")
-        pstack.init(flags=["-migrate-state"])
+        pstack.init(flags=["-migrate-state", "-upgrade"])
 
     result = runner.invoke(
         app,
         ["preview", "--backend", "terraform", "--env", "dev", "--filepath", filepath],
     )
     assert result.exit_code == 0
 
 
 def test_quickstart_pulumi():
-    filepath = os.path.join(dirpath, "stack_quickstart_pulumi.yaml")
+    filepath = os.path.join(paths.tmp, "stack_quickstart_pulumi.yaml")
+    print(filepath)
     result = runner.invoke(
         app,
         [
             "quickstart",
             "--backend",
             "pulumi",
             "-o",
@@ -59,15 +61,15 @@
     assert stack.pulumi.config["databricks:token"] == "${vars.DATABRICKS_TOKEN}"
     assert len(stack.resources.dbfsfiles) == 1
     assert len(stack.resources.notebooks) == 2
     assert len(stack.resources.pipelines) == 1
 
 
 def test_quickstart_terraform():
-    filepath = os.path.join(dirpath, "stack_quickstart_terraform.yaml")
+    filepath = os.path.join(paths.tmp, "stack_quickstart_terraform.yaml")
     result = runner.invoke(
         app,
         [
             "quickstart",
             "--backend",
             "terraform",
             "-o",
@@ -97,15 +99,15 @@
     # TODO: Figure out how to run in isolation. Currently, pulumi up commands
     # are run concurrently because of the multiple python testing environment
     # which result in:  Conflict: Another update is currently in progress
     for filename in [
         "stack.yaml",
         "stack_empty.yaml",
     ]:
-        filepath = os.path.join(dirpath, filename)
+        filepath = os.path.join(paths.data, filename)
         result = runner.invoke(
             app,
             [
                 "deploy",
                 "-e",
                 "dev",
                 "--filepath",
@@ -121,15 +123,15 @@
     # TODO: Figure out how to run in isolation. Currently, pulumi up commands
     # are run concurrently because of the multiple python testing environment
     # which result in:  Conflict: Another update is currently in progress
     for filename in [
         "stack.yaml",
         "stack_empty.yaml",
     ]:
-        filepath = os.path.join(dirpath, filename)
+        filepath = os.path.join(paths.data, filename)
         result = runner.invoke(
             app,
             [
                 "deploy",
                 "-e",
                 "dev",
                 "--backend",
```

### Comparing `laktory-0.1.9/tests/test_dataevent.py` & `laktory-0.2.0/tests/test_dataevent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,38 @@
+import os
+import json
 from datetime import datetime
 from zoneinfo import ZoneInfo
 import pytest
 
-from laktory._testing import StockPriceDataEventHeader
-from laktory._testing import EventsManager
 from laktory import models
 from laktory import settings
+from laktory._testing import Paths
+
+paths = Paths(__file__)
+
+
+# Header
+class StockPriceDataEventHeader(models.DataEventHeader):
+    name: str = "stock_price"
+    producer: models.DataProducer = models.DataProducer(name="yahoo-finance")
+
 
 header = StockPriceDataEventHeader()
-events = EventsManager().build_events()
-event = events[0]
+
+
+# Event
+with open(
+    os.path.join(
+        paths.data,
+        "./events/yahoo-finance/stock_price/2023/09/01/stock_price_AAPL_20230901T000000000Z.json",
+    )
+) as fp:
+    event = json.load(fp)
+event = models.DataEvent(**event)
 
 
 def test_dataeventheader():
     print(header.model_dump())
     assert header.model_dump() == {
         "name": "stock_price",
         "description": None,
@@ -68,18 +87,19 @@
         == "/Volumes/dev/sources/landing/events/yahoo-finance/stock_price/2023/09/01/stock_price_20230901T000000000Z.json"
     )
 
 
 def test_model_dump():
     # Without exclusions
     d = event.model_dump(exclude=[])
+    print(d)
     assert d == {
-        "name": "stock_price",
-        "description": None,
-        "producer": {"name": "yahoo-finance", "description": None, "party": 1},
+        "event_name": "stock_price",
+        "event_description": None,
+        "event_producer": {"name": "yahoo-finance", "description": None, "party": 1},
         "events_root": None,
         "event_root": None,
         "data": {
             "created_at": "2023-09-01T00:00:00",
             "symbol": "AAPL",
             "open": 189.49000549316406,
             "close": 189.4600067138672,
@@ -96,17 +116,17 @@
 
     assert event.events_root == "/Volumes/dev/sources/landing/events/"
 
     # With exclusions
     d = event.model_dump()
     print(d)
     assert d == {
-        "name": "stock_price",
-        "description": None,
-        "producer": {"name": "yahoo-finance", "description": None, "party": 1},
+        "event_name": "stock_price",
+        "event_description": None,
+        "event_producer": {"name": "yahoo-finance", "description": None, "party": 1},
         "event_root": None,
         "data": {
             "created_at": "2023-09-01T00:00:00",
             "symbol": "AAPL",
             "open": 189.49000549316406,
             "close": 189.4600067138672,
             "high": 189.9199981689453,
```

### Comparing `laktory-0.1.9/tests/test_datasources.py` & `laktory-0.2.0/tests/test_datasources.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from pyspark.sql import Row
 from pyspark.sql import SparkSession
 import os
-import pytest
+import pandas as pd
 
 from laktory.models.datasources import EventDataSource
 from laktory.models.datasources import TableDataSource
-from laktory._testing import StockPriceDataEventHeader
-from laktory._testing import EventsManager
+from laktory._testing import Paths
+from laktory._testing import spark
 
+paths = Paths(__file__)
 
-# Build and write events
-data_dir = os.path.join(os.path.dirname(__file__), "data/")
-header = StockPriceDataEventHeader()
-manager = EventsManager()
-manager.build_events(data_dir)
-manager.to_path()
-
-# Spark
-spark = SparkSession.builder.appName("UnitTesting").getOrCreate()
+# DataFrame
+pdf = pd.DataFrame(
+    {
+        "x": [1, 2, 3],
+        "a": [1, -1, 1],
+        "b": [2, 0, 2],
+        "c": [3, 0, 3],
+        "n": [4, 0, 4],
+    },
+)
+df0 = spark.createDataFrame(pdf)
 
 
 def test_event_data_source():
     source = EventDataSource(
         name="stock_price",
         producer={"name": "yahoo_finance"},
     )
@@ -32,42 +34,65 @@
     assert not source.is_cdc
 
 
 def test_event_data_source_read():
     source = EventDataSource(
         name="stock_price",
         producer={"name": "yahoo-finance"},
-        events_root=data_dir,
+        events_root=os.path.join(paths.data, "./events/"),
         read_as_stream=False,
     )
-    df = source.read(spark).toPandas()
-    assert len(df) == 80
-    print(list(df.columns))
-    assert list(df.columns) == [
+    df = source.read(spark)
+    assert df.count() == 80
+    assert df.columns == [
         "data",
         "description",
         "event_root_",
         "name",
         "producer",
     ]
-    df["data"] = df["data"].apply(Row.asDict)
-    df["symbol"] = df["data"].apply(dict.get, args=("symbol",))
-    df["created_at"] = df["data"].apply(dict.get, args=("_created_at",))
-    df = df.sort_values(["symbol", "created_at"])
-    row = df.iloc[0]["data"]
-    assert row["symbol"] == "AAPL"
-    assert row["close"] == pytest.approx(189.46, abs=0.01)
 
 
-def test_table_data_souurce():
+def test_table_data_source(df0=df0):
     source = TableDataSource(
+        mock_df=df0,
         path="/Volumes/tables/stock_prices/",
+        filter="b != 0",
+        selects=["a", "b", "c"],
+        renames={"a": "aa", "b": "bb", "c": "cc"},
     )
+
+    # Test paths
     assert source.path == "/Volumes/tables/stock_prices/"
     assert source.from_path
     assert source.path_or_full_name == "/Volumes/tables/stock_prices/"
 
+    # Test reader
+    df = source.read(spark)
+    assert df.columns == ["aa", "bb", "cc"]
+    assert df.count() == 2
+
+    # Select with rename
+    source = TableDataSource(
+        mock_df=df0,
+        path="/Volumes/tables/stock_prices/",
+        selects={"x": "x1", "n": "n1"},
+    )
+    df = source.read(spark)
+    assert df.columns == ["x1", "n1"]
+    assert df.count() == 3
+
+    # Drop
+    source = TableDataSource(
+        mock_df=df0,
+        path="/Volumes/tables/stock_prices/",
+        drops=["b", "c", "n"],
+    )
+    df = source.read(spark)
+    assert df.columns == ["x", "a"]
+    assert df.count() == 3
+
 
 if __name__ == "__main__":
     test_event_data_source()
     test_event_data_source_read()
-    test_table_data_souurce()
+    test_table_data_source()
```

### Comparing `laktory-0.1.9/tests/test_dbfsfile.py` & `laktory-0.2.0/tests/test_dbfsfile.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_docstrings.py` & `laktory-0.2.0/tests/test_docstrings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,40 @@
 import pytest
 from pytest_examples import find_examples, CodeExample, EvalExample
 from pyspark.sql import SparkSession
 
 spark = SparkSession.builder.getOrCreate()
+spark.conf.set("spark.sql.session.timeZone", "UTC")
+
+
+# --------------------------------------------------------------------------- #
+# Datetime                                                                    #
+# --------------------------------------------------------------------------- #
+
+
+@pytest.mark.parametrize("example", find_examples("./laktory/datetime.py"), ids=str)
+def test_docstrings_datetime(example: CodeExample, eval_example: EvalExample):
+    if eval_example.update_examples:
+        eval_example.format(example)
+        eval_example.run_print_update(
+            example,
+            # module_globals={
+            # "spark": spark,
+            # "display": lambda x: x,
+            # },
+        )
+    else:
+        eval_example.lint(example)
+        eval_example.run_print_check(
+            example,
+            # module_globals={
+            #     "spark": spark,
+            #     "display": lambda x: x,
+            # },
+        )
 
 
 # --------------------------------------------------------------------------- #
 # DLT                                                                         #
 # --------------------------------------------------------------------------- #
```

### Comparing `laktory-0.1.9/tests/test_job.py` & `laktory-0.2.0/tests/test_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import os
 
 from laktory.models import Job
 from laktory import pulumi_outputs
 
-
-root_dir = os.path.dirname(__file__)
-
 job = Job(
     name="job-stock-prices",
     clusters=[
         {
             "name": "main",
             "spark_version": "14.0.x-scala2.12",
             "node_type_id": "Standard_DS3_v2",
```

### Comparing `laktory-0.1.9/tests/test_metastore.py` & `laktory-0.2.0/tests/test_metastore.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_notebook.py` & `laktory-0.2.0/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_parsers.py` & `laktory-0.2.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_pipeline.py` & `laktory-0.2.0/tests/test_pipeline.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,33 @@
-from laktory._testing import StockPricesPipeline
+from laktory import models
 
-pl = StockPricesPipeline()
+from laktory._testing.stockprices import table_slv_pl
+from laktory._testing.stockprices import table_slv_join_pl
+
+
+pl = models.Pipeline(
+    name="pl-stock-prices",
+    catalog="dev1",
+    target="markets1",
+    tables=[table_slv_pl, table_slv_join_pl],
+    udfs=[
+        {
+            "module_name": "stock_functions",
+            "function_name": "high",
+        }
+    ],
+)
 
 
 def test_pipeline():
     print(pl.model_dump())
     assert pl.model_dump() == {
         "access_controls": [],
         "allow_duplicate_names": None,
-        "catalog": None,
+        "catalog": "dev1",
         "channel": "PREVIEW",
         "clusters": [],
         "configuration": {},
         "continuous": None,
         "development": None,
         "edition": None,
         "libraries": None,
@@ -20,169 +35,81 @@
         "notifications": [],
         "photon": None,
         "serverless": None,
         "storage": None,
         "tables": [
             {
                 "builder": {
-                    "aggregation": None,
-                    "as_dlt_view": False,
-                    "drop_columns": [],
-                    "drop_duplicates": None,
-                    "drop_source_columns": False,
-                    "event_source": {
-                        "name": "stock_price",
-                        "description": None,
-                        "producer": None,
-                        "events_root_": None,
-                        "event_root_": None,
-                        "read_as_stream": True,
-                        "fmt": "JSON",
-                        "header": True,
-                        "multiline": False,
-                        "read_options": {},
-                        "schema_location": None,
-                        "type": "STORAGE_EVENTS",
-                    },
-                    "filter": None,
-                    "joins": [],
-                    "joins_post_aggregation": [],
-                    "layer": "BRONZE",
-                    "pipeline_name": "pl-stock-prices",
-                    "selects": None,
-                    "table_source": None,
-                    "template": "BRONZE",
-                    "unions": [],
-                    "window_filter": None,
-                },
-                "catalog_name": None,
-                "columns": [],
-                "comment": None,
-                "data": None,
-                "data_source_format": "DELTA",
-                "expectations": [],
-                "grants": None,
-                "name": "brz_stock_prices",
-                "primary_key": None,
-                "schema_name": None,
-                "table_type": "MANAGED",
-                "timestamp_key": None,
-                "view_definition": None,
-                "warehouse_id": "08b717ce051a0261",
-            },
-            {
-                "builder": {
-                    "aggregation": None,
+                    "add_laktory_columns": True,
                     "as_dlt_view": False,
-                    "drop_columns": [],
                     "drop_duplicates": None,
                     "drop_source_columns": True,
                     "event_source": None,
-                    "filter": None,
-                    "joins": [],
-                    "joins_post_aggregation": [],
                     "layer": "SILVER",
                     "pipeline_name": "pl-stock-prices",
-                    "selects": None,
                     "table_source": {
+                        "drops": None,
+                        "filter": None,
                         "read_as_stream": True,
+                        "renames": None,
+                        "selects": None,
+                        "watermark": None,
                         "catalog_name": "dev",
                         "cdc": None,
-                        "selects": None,
                         "fmt": "DELTA",
-                        "filter": None,
                         "from_pipeline": True,
                         "name": "brz_stock_prices",
                         "path": None,
                         "schema_name": "markets",
-                        "watermark": None,
                     },
                     "template": "SILVER",
-                    "unions": [],
-                    "window_filter": None,
+                    "spark_chain": None,
                 },
-                "catalog_name": None,
+                "catalog_name": "dev1",
                 "columns": [
                     {
-                        "catalog_name": None,
+                        "catalog_name": "dev1",
                         "comment": None,
                         "name": "created_at",
                         "pii": None,
                         "raise_missing_arg_exception": True,
-                        "schema_name": None,
-                        "spark_func_args": [
-                            {
-                                "value": "data._created_at",
-                                "is_column": True,
-                                "to_lit": False,
-                                "to_expr": True,
-                            }
-                        ],
-                        "spark_func_kwargs": {},
-                        "spark_func_name": "coalesce",
-                        "sql_expression": None,
+                        "schema_name": "markets1",
                         "table_name": "slv_stock_prices",
                         "type": "timestamp",
                         "unit": None,
                     },
                     {
-                        "catalog_name": None,
+                        "catalog_name": "dev1",
                         "comment": None,
                         "name": "symbol",
                         "pii": None,
                         "raise_missing_arg_exception": True,
-                        "schema_name": None,
-                        "spark_func_args": [
-                            {
-                                "value": "data.symbol",
-                                "is_column": True,
-                                "to_lit": False,
-                                "to_expr": True,
-                            }
-                        ],
-                        "spark_func_kwargs": {},
-                        "spark_func_name": "coalesce",
-                        "sql_expression": None,
+                        "schema_name": "markets1",
                         "table_name": "slv_stock_prices",
                         "type": "string",
                         "unit": None,
                     },
                     {
-                        "catalog_name": None,
+                        "catalog_name": "dev1",
                         "comment": None,
                         "name": "open",
                         "pii": None,
                         "raise_missing_arg_exception": True,
-                        "schema_name": None,
-                        "spark_func_args": [
-                            {
-                                "value": "data.open",
-                                "is_column": True,
-                                "to_lit": False,
-                                "to_expr": True,
-                            }
-                        ],
-                        "spark_func_kwargs": {},
-                        "spark_func_name": "coalesce",
-                        "sql_expression": None,
+                        "schema_name": "markets1",
                         "table_name": "slv_stock_prices",
                         "type": "double",
                         "unit": None,
                     },
                     {
-                        "catalog_name": None,
+                        "catalog_name": "dev1",
                         "comment": None,
                         "name": "close",
                         "pii": None,
                         "raise_missing_arg_exception": True,
-                        "schema_name": None,
-                        "spark_func_args": [],
-                        "spark_func_kwargs": {},
-                        "spark_func_name": None,
-                        "sql_expression": "data.open",
+                        "schema_name": "markets1",
                         "table_name": "slv_stock_prices",
                         "type": "double",
                         "unit": None,
                     },
                 ],
                 "comment": None,
                 "data": [
@@ -203,39 +130,166 @@
                         "expression": "created_at > '2023-01-01'",
                         "action": "DROP",
                     },
                 ],
                 "grants": None,
                 "name": "slv_stock_prices",
                 "primary_key": None,
-                "schema_name": None,
+                "schema_name": "markets1",
                 "table_type": "MANAGED",
                 "timestamp_key": None,
                 "view_definition": None,
                 "warehouse_id": "08b717ce051a0261",
             },
+            {
+                "builder": {
+                    "add_laktory_columns": True,
+                    "as_dlt_view": False,
+                    "drop_duplicates": None,
+                    "drop_source_columns": False,
+                    "event_source": None,
+                    "layer": "SILVER",
+                    "pipeline_name": "pl-stock-prices",
+                    "table_source": {
+                        "drops": None,
+                        "filter": "created_at = '2023-09-01T00:00:00Z'",
+                        "read_as_stream": True,
+                        "renames": None,
+                        "selects": None,
+                        "watermark": None,
+                        "catalog_name": "dev",
+                        "cdc": None,
+                        "fmt": "DELTA",
+                        "from_pipeline": True,
+                        "name": "slv_stock_prices",
+                        "path": None,
+                        "schema_name": "markets",
+                    },
+                    "template": "SILVER",
+                    "spark_chain": {
+                        "nodes": [
+                            {
+                                "allow_missing_column_args": False,
+                                "column": None,
+                                "spark_func_args": [],
+                                "spark_func_kwargs": {
+                                    "other": {
+                                        "value": {
+                                            "drops": None,
+                                            "filter": None,
+                                            "read_as_stream": True,
+                                            "renames": {"symbol2": "symbol"},
+                                            "selects": None,
+                                            "watermark": None,
+                                            "catalog_name": "dev",
+                                            "cdc": None,
+                                            "fmt": "DELTA",
+                                            "from_pipeline": True,
+                                            "name": "slv_stockmeta",
+                                            "path": None,
+                                            "schema_name": "markets",
+                                        }
+                                    },
+                                    "on": {"value": ["symbol"]},
+                                },
+                                "spark_func_name": "smart_join",
+                                "sql_expression": None,
+                            },
+                            {
+                                "allow_missing_column_args": False,
+                                "column": {
+                                    "name": "symbol3",
+                                    "type": "string",
+                                    "unit": None,
+                                },
+                                "spark_func_args": [],
+                                "spark_func_kwargs": {},
+                                "spark_func_name": None,
+                                "sql_expression": "symbol",
+                            },
+                            {
+                                "allow_missing_column_args": False,
+                                "column": None,
+                                "spark_func_args": [{"value": "symbol"}],
+                                "spark_func_kwargs": {},
+                                "spark_func_name": "drop",
+                                "sql_expression": None,
+                            },
+                            {
+                                "allow_missing_column_args": False,
+                                "column": None,
+                                "spark_func_args": [],
+                                "spark_func_kwargs": {
+                                    "other": {
+                                        "value": {
+                                            "drops": None,
+                                            "filter": None,
+                                            "read_as_stream": True,
+                                            "renames": None,
+                                            "selects": None,
+                                            "watermark": None,
+                                            "catalog_name": "dev",
+                                            "cdc": None,
+                                            "fmt": "DELTA",
+                                            "from_pipeline": True,
+                                            "name": "slv_stock_names",
+                                            "path": None,
+                                            "schema_name": "markets",
+                                        }
+                                    },
+                                    "on": {"value": ["symbol3"]},
+                                },
+                                "spark_func_name": "smart_join",
+                                "sql_expression": None,
+                            },
+                        ]
+                    },
+                },
+                "catalog_name": "dev1",
+                "columns": [],
+                "comment": None,
+                "data": None,
+                "data_source_format": "DELTA",
+                "expectations": [],
+                "grants": None,
+                "name": "slv_join_stock_prices",
+                "primary_key": None,
+                "schema_name": "markets1",
+                "table_type": "MANAGED",
+                "timestamp_key": None,
+                "view_definition": None,
+                "warehouse_id": "08b717ce051a0261",
+            },
+        ],
+        "target": "markets1",
+        "udfs": [
+            {
+                "module_name": "stock_functions",
+                "function_name": "high",
+                "module_path": None,
+            }
         ],
-        "target": None,
-        "udfs": [{"module_name": "stock_functions", "function_name": "high"}],
     }
 
 
 def test_pipeline_pulumi():
     assert pl.resource_name == "pl-stock-prices"
     assert pl.options.model_dump(exclude_none=True) == {
         "depends_on": [],
         "delete_before_replace": True,
     }
     print(pl.pulumi_properties)
     assert pl.pulumi_properties == {
+        "catalog": "dev1",
         "channel": "PREVIEW",
         "clusters": [],
         "configuration": {},
         "name": "pl-stock-prices",
         "notifications": [],
+        "target": "markets1",
     }
 
     # Resources
     assert len(pl.core_resources) == 3
     r = pl.core_resources[-1]
     r.options.aliases = ["my-file"]
     assert pl.core_resources[-1].options.aliases == ["my-file"]
```

### Comparing `laktory-0.1.9/tests/test_schema.py` & `laktory-0.2.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_settings.py` & `laktory-0.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_spark_functions.py` & `laktory-0.2.0/tests/test_spark_functions.py`

 * *Files identical despite different names*

### Comparing `laktory-0.1.9/tests/test_sql_query.py` & `laktory-0.2.0/tests/test_sql_query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import os
 from laktory.models import SqlQuery
 
-root_dir = os.path.dirname(__file__)
-
 query = SqlQuery(
     name="google-prices",
     parent="/queries",
     query="SELECT * FROM dev.finance.slv_stock_prices",
     data_source_id="12345",
 )
```

### Comparing `laktory-0.1.9/tests/test_stack.py` & `laktory-0.2.0/tests/test_stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import copy
 import os
 
-from laktory._testing.stackvalidator import StackValidator
 from laktory import models
+from laktory._testing.stackvalidator import StackValidator
+from laktory._testing import Paths
 
-dirpath = os.path.dirname(__file__)
+paths = Paths(__file__)
 
-with open(os.path.join(dirpath, "stack.yaml"), "r") as fp:
+with open(os.path.join(paths.data, "stack.yaml"), "r") as fp:
     stack = models.Stack.model_validate_yaml(fp)
 
 stack.terraform.backend = {
     "azurerm": {
         "resource_group_name": "o3-rg-laktory-dev",
         "storage_account_name": "o3stglaktorydev",
         "container_name": "unit-testing",
@@ -458,15 +459,17 @@
 
 def test_terraform_stack():
     data_default = stack.to_terraform().model_dump()
     data_default["provider"]["databricks"]["token"] = "***"
     print(data_default)
     assert data_default == {
         "terraform": {
-            "required_providers": {"databricks": {"source": "databricks/databricks"}},
+            "required_providers": {
+                "databricks": {"source": "databricks/databricks", "version": ">=1.39"}
+            },
             "backend": {
                 "azurerm": {
                     "resource_group_name": "o3-rg-laktory-dev",
                     "storage_account_name": "o3stglaktorydev",
                     "container_name": "unit-testing",
                     "key": "terraform/dev.terraform.tfstate",
                 }
@@ -594,15 +597,15 @@
 
 
 def test_terraform_plan():
     tstack = stack.to_terraform(env="dev")
     tstack.terraform.backend = (
         None  # TODO: Add credentials to git actions to use azure backend
     )
-    tstack.init(flags=["-migrate-state"])
+    tstack.init(flags=["-migrate-state", "-upgrade"])
     tstack.plan()
 
 
 def test_all_resources():
     from tests.test_catalog import catalog
     from tests.test_directory import directory
     from tests.test_job import job
@@ -610,19 +613,20 @@
     from tests.test_metastore import metastore
     from tests.test_notebook import nb
     from tests.test_schema import schema
     from tests.test_sql_query import query
     from tests.test_user import user
     from tests.test_user import group
     from tests.test_workspacefile import workspace_file
+    from laktory._testing import Paths
 
-    root_dir = os.path.dirname(__file__)
+    paths = Paths(__file__)
 
-    nb.source = os.path.join(root_dir, nb.source)
-    workspace_file.source = os.path.join(root_dir, workspace_file.source)
+    nb.source = os.path.join(paths.root, nb.source)
+    workspace_file.source = os.path.join(paths.root, workspace_file.source)
 
     validator = StackValidator(
         resources={
             "catalogs": [catalog],
             "directories": [directory],
             "jobs": [job],
             "metastores": [metastore],
```

### Comparing `laktory-0.1.9/tests/test_workspacefile.py` & `laktory-0.2.0/tests/test_workspacefile.py`

 * *Files identical despite different names*

