# Comparing `tmp/snakemake-8.8.0.tar.gz` & `tmp/snakemake-8.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake-8.8.0.tar", last modified: Fri Mar 15 15:51:36 2024, max compression
+gzip compressed data, was "snakemake-8.9.0.tar", last modified: Tue Mar 19 09:58:45 2024, max compression
```

## Comparing `snakemake-8.8.0.tar` & `snakemake-8.9.0.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.246704 snakemake-8.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-15 15:51:27.000000 snakemake-8.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-15 15:51:27.000000 snakemake-8.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-15 15:51:36.246704 snakemake-8.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-15 15:51:27.000000 snakemake-8.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-15 15:51:27.000000 snakemake-8.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-15 15:51:36.246704 snakemake-8.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-15 15:51:27.000000 snakemake-8.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.246704 snakemake-8.8.0/snakemake/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-15 15:51:36.246704 snakemake-8.8.0/snakemake/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27788 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/caching/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/caching/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/caching/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    84943 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/common/
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/configfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tbdstring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/common/tests/testcases/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tests/testcases/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/common/tests/testcases/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tests/testcases/groups/Snakefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tests/testcases/groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/common/tests/testcases/simple/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tests/testcases/simple/Snakefile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/tests/testcases/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/common/workdir_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/cwl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   107615 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33310 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/deployment/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/deployment/containerize.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/deployment/env_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/deployment/singularity.py
--rw-r--r--   0 runner    (1001) docker     (127)    19118 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.230704 snakemake-8.8.0/snakemake/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/executors/dryrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/executors/google_lifesciences_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/executors/jobscript.sh
--rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/executors/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/executors/touch.py
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/gui.html
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57193 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/ioflags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/ioutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    56070 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.234704 snakemake-8.8.0/snakemake/linting/
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/linting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/linting/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/linting/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/linting/snakefiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    27171 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/output_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    37580 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/path_modifier.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22236 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.234704 snakemake-8.8.0/snakemake/remote/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/AzBlob.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/EGA.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/FTP.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/GS.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/HTTP.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/NCBI.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/S3.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/S3Mocked.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/SFTP.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/XRootD.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/dropbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/gfal.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/gridftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/iRODS.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/webdav.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/remote/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.234704 snakemake-8.8.0/snakemake/report/
--rw-r--r--   0 runner    (1001) docker     (127)    23372 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.238704 snakemake-8.8.0/snakemake/report/html_reporter/
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.238704 snakemake-8.8.0/snakemake/report/html_reporter/data/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/categories.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/configfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/rulegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/runtimes.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/data/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.238704 snakemake-8.8.0/snakemake/report/html_reporter/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.242704 snakemake-8.8.0/snakemake/report/html_reporter/template/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/abstract_menu.js
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/abstract_results.js
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/app.js
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/breadcrumbs.js
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/button.js
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/category.js
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/common.js
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/content.js
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/icon.js
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/list_heading.js
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/list_item.js
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/menu.js
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/navbar.js
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/report_info.js
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/result_info.js
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/result_view_button.js
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/rule_graph.js
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/rule_info.js
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/search_results.js
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/stats.js
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/components/subcategory.js
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/index.html.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/html_reporter/template/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report/rulegraph_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/report.css
--rw-r--r--   0 runner    (1001) docker     (127)    25467 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/ruleinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)    45830 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    29557 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.242704 snakemake-8.8.0/snakemake/script/
--rw-r--r--   0 runner    (1001) docker     (127)    49763 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/sourcecache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/spawn_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/target_jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.242704 snakemake-8.8.0/snakemake/template_rendering/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/template_rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/template_rendering/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/template_rendering/yte.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.242704 snakemake-8.8.0/snakemake/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.242704 snakemake-8.8.0/snakemake/unit_tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/unit_tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/unit_tests/templates/common.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/unit_tests/templates/ruletest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)    29148 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    76857 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-15 15:51:27.000000 snakemake-8.8.0/snakemake/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.246704 snakemake-8.8.0/snakemake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-15 15:51:36.000000 snakemake-8.8.0/snakemake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-15 15:51:36.000000 snakemake-8.8.0/snakemake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:51:36.000000 snakemake-8.8.0/snakemake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-15 15:51:36.000000 snakemake-8.8.0/snakemake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 15:51:35.000000 snakemake-8.8.0/snakemake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-15 15:51:36.000000 snakemake-8.8.0/snakemake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-15 15:51:36.000000 snakemake-8.8.0/snakemake.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 15:51:36.246704 snakemake-8.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_executor_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_expand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_persistence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/testapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    50227 2024-03-15 15:51:27.000000 snakemake-8.8.0/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    83780 2024-03-15 15:51:27.000000 snakemake-8.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.038907 snakemake-8.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-19 09:58:32.000000 snakemake-8.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-19 09:58:32.000000 snakemake-8.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-19 09:58:45.038907 snakemake-8.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-19 09:58:32.000000 snakemake-8.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-19 09:58:32.000000 snakemake-8.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-19 09:58:45.038907 snakemake-8.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-19 09:58:32.000000 snakemake-8.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.038907 snakemake-8.9.0/snakemake/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-19 09:58:45.038907 snakemake-8.9.0/snakemake/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27788 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.022907 snakemake-8.9.0/snakemake/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/caching/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6574 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/caching/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/caching/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84943 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.022907 snakemake-8.9.0/snakemake/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     9154 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/configfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tbdstring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.022907 snakemake-8.9.0/snakemake/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.022907 snakemake-8.9.0/snakemake/common/tests/testcases/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tests/testcases/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.022907 snakemake-8.9.0/snakemake/common/tests/testcases/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tests/testcases/groups/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tests/testcases/groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.022907 snakemake-8.9.0/snakemake/common/tests/testcases/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tests/testcases/simple/Snakefile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/tests/testcases/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/common/workdir_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/cwl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108124 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.026907 snakemake-8.9.0/snakemake/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33310 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/deployment/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/deployment/containerize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/deployment/env_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/deployment/singularity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19130 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.026907 snakemake-8.9.0/snakemake/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/executors/dryrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/executors/google_lifesciences_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/executors/jobscript.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    16604 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/executors/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/executors/touch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/gui.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57193 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/ioflags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12338 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/ioutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56232 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.026907 snakemake-8.9.0/snakemake/linting/
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/linting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/linting/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5917 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/linting/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/linting/snakefiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27171 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/output_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37580 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/path_modifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22236 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.030907 snakemake-8.9.0/snakemake/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/AzBlob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/EGA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/FTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/GS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/HTTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/NCBI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/S3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/S3Mocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/SFTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/XRootD.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/dropbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/gfal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/gridftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/iRODS.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/webdav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/remote/zenodo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.030907 snakemake-8.9.0/snakemake/report/
+-rw-r--r--   0 runner    (1001) docker     (127)    23372 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.030907 snakemake-8.9.0/snakemake/report/html_reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.030907 snakemake-8.9.0/snakemake/report/html_reporter/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/configfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/rulegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/runtimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/data/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.030907 snakemake-8.9.0/snakemake/report/html_reporter/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.034907 snakemake-8.9.0/snakemake/report/html_reporter/template/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/abstract_menu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/abstract_results.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/breadcrumbs.js
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/button.js
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/category.js
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/common.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/content.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/list_heading.js
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/list_item.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/menu.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/navbar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/report_info.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/result_info.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/result_view_button.js
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/rule_graph.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/rule_info.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/search_results.js
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/stats.js
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/components/subcategory.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/index.html.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/html_reporter/template/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report/rulegraph_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/report.css
+-rw-r--r--   0 runner    (1001) docker     (127)    25467 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/ruleinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45830 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29557 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.034907 snakemake-8.9.0/snakemake/script/
+-rw-r--r--   0 runner    (1001) docker     (127)    49763 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12019 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/sourcecache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/spawn_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/target_jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.034907 snakemake-8.9.0/snakemake/template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/template_rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/template_rendering/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/template_rendering/yte.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.034907 snakemake-8.9.0/snakemake/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.034907 snakemake-8.9.0/snakemake/unit_tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/unit_tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/unit_tests/templates/common.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/unit_tests/templates/ruletest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)    29148 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76857 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-03-19 09:58:32.000000 snakemake-8.9.0/snakemake/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.038907 snakemake-8.9.0/snakemake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-19 09:58:44.000000 snakemake-8.9.0/snakemake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-19 09:58:45.000000 snakemake-8.9.0/snakemake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:58:44.000000 snakemake-8.9.0/snakemake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-19 09:58:44.000000 snakemake-8.9.0/snakemake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 09:58:44.000000 snakemake-8.9.0/snakemake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-19 09:58:44.000000 snakemake-8.9.0/snakemake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 09:58:44.000000 snakemake-8.9.0/snakemake.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 09:58:45.038907 snakemake-8.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_executor_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16998 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/testapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50350 2024-03-19 09:58:32.000000 snakemake-8.9.0/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83780 2024-03-19 09:58:32.000000 snakemake-8.9.0/versioneer.py
```

### Comparing `snakemake-8.8.0/LICENSE.md` & `snakemake-8.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/PKG-INFO` & `snakemake-8.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake
-Version: 8.8.0
+Version: 8.9.0
 Summary: Workflow management system to create reproducible and scalable data analyses
 Author: Johannes Köster
 Author-email: johannes.koester@uni-due.de
 License: MIT
 Project-URL: Homepage, https://snakemake.github.io
 Project-URL: Documentation, https://snakemake.readthedocs.io
 Project-URL: Source, https://github.com/snakemake/snakemake
```

### Comparing `snakemake-8.8.0/README.md` & `snakemake-8.9.0/README.md`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/pyproject.toml` & `snakemake-8.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/setup.cfg` & `snakemake-8.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/api.py` & `snakemake-8.9.0/snakemake/api.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/benchmark.py` & `snakemake-8.9.0/snakemake/benchmark.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/caching/__init__.py` & `snakemake-8.9.0/snakemake/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/caching/hash.py` & `snakemake-8.9.0/snakemake/caching/hash.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/caching/local.py` & `snakemake-8.9.0/snakemake/caching/local.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/caching/storage.py` & `snakemake-8.9.0/snakemake/caching/storage.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/checkpoints.py` & `snakemake-8.9.0/snakemake/checkpoints.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/cli.py` & `snakemake-8.9.0/snakemake/cli.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/__init__.py` & `snakemake-8.9.0/snakemake/common/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/argparse.py` & `snakemake-8.9.0/snakemake/common/argparse.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/configfile.py` & `snakemake-8.9.0/snakemake/common/configfile.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/git.py` & `snakemake-8.9.0/snakemake/common/git.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/tbdstring.py` & `snakemake-8.9.0/snakemake/common/tbdstring.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/tests/__init__.py` & `snakemake-8.9.0/snakemake/common/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/tests/testcases/groups/Snakefile` & `snakemake-8.9.0/snakemake/common/tests/testcases/groups/Snakefile`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/tests/testcases/simple/Snakefile` & `snakemake-8.9.0/snakemake/common/tests/testcases/simple/Snakefile`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/common/workdir_handler.py` & `snakemake-8.9.0/snakemake/common/workdir_handler.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/cwl.py` & `snakemake-8.9.0/snakemake/cwl.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/dag.py` & `snakemake-8.9.0/snakemake/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1026,15 +1026,20 @@
                 await res.file.inventory()
 
             if not res.jobs:
                 # no producing job found
                 if self.workflow.is_main_process and not await res.file.exists():
                     # file not found, hence missing input
                     missing_input.add(res.file)
-                known_producers[res.file] = None
+                if not is_flagged(res.file, "before_update"):
+                    # record info that there is no known producer, but only
+                    # do that for files that are not flagged as before_update
+                    # otherwise, we would risk a conflict with corresponding files
+                    # that are flagged as 'update'.
+                    known_producers[res.file] = None
                 # file found, no problem
                 continue
 
             if res.known:
                 producer[res.file] = res.jobs[0]
             else:
                 try:
@@ -2014,40 +2019,41 @@
                 )
                 input_files = input_batch
 
         for file in input_files:
             if is_flagged(file, "before_update"):
                 # do not find a producer for this file, it shall be considered in its
                 # form before the update
-                continue
-            try:
-                yield PotentialDependency(file, known_producers[file], True)
-            except KeyError:
+                yield PotentialDependency(file, None, False)
+            else:
                 try:
-                    if file in job.dependencies:
-                        yield PotentialDependency(
-                            file,
-                            [
-                                self.new_job(
-                                    job.dependencies[file],
-                                    targetfile=file,
-                                    wildcards_dict=job.wildcards_dict,
-                                )
-                            ],
-                            False,
-                        )
-                    else:
-                        yield PotentialDependency(
-                            file,
-                            file2jobs(file, wildcards_dict=job.wildcards_dict),
-                            False,
-                        )
-                except MissingRuleException as ex:
-                    # no dependency found
-                    yield PotentialDependency(file, None, False)
+                    yield PotentialDependency(file, known_producers[file], True)
+                except KeyError:
+                    try:
+                        if file in job.dependencies:
+                            yield PotentialDependency(
+                                file,
+                                [
+                                    self.new_job(
+                                        job.dependencies[file],
+                                        targetfile=file,
+                                        wildcards_dict=job.wildcards_dict,
+                                    )
+                                ],
+                                False,
+                            )
+                        else:
+                            yield PotentialDependency(
+                                file,
+                                file2jobs(file, wildcards_dict=job.wildcards_dict),
+                                False,
+                            )
+                    except MissingRuleException as ex:
+                        # no dependency found
+                        yield PotentialDependency(file, None, False)
 
     def bfs(self, direction, *jobs, stop=lambda job: False):
         """Perform a breadth-first traversal of the DAG."""
         queue = deque(jobs)
         visited = set(queue)
         while queue:
             job = queue.popleft()
```

### Comparing `snakemake-8.8.0/snakemake/deployment/conda.py` & `snakemake-8.9.0/snakemake/deployment/conda.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/deployment/containerize.py` & `snakemake-8.9.0/snakemake/deployment/containerize.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/deployment/env_modules.py` & `snakemake-8.9.0/snakemake/deployment/env_modules.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/deployment/singularity.py` & `snakemake-8.9.0/snakemake/deployment/singularity.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/exceptions.py` & `snakemake-8.9.0/snakemake/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     elif isinstance(ex, ApiError):
         logger.error(f"Error: {ex}")
     elif isinstance(ex, CliException):
         logger.error(f"Error: {ex}")
     elif isinstance(ex, KeyboardInterrupt):
         logger.info("Cancelling snakemake on user request.")
     else:
-        logger.error(traceback.format_exeption(ex))
+        logger.error("\n".join(traceback.format_exception(ex)))
 
 
 def update_lineno(ex: SyntaxError, linemaps):
     if ex.filename and ex.lineno:
         linemap = linemaps[ex.filename]
         try:
             ex.lineno = linemap[ex.lineno]
```

### Comparing `snakemake-8.8.0/snakemake/executors/__init__.py` & `snakemake-8.9.0/snakemake/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/executors/dryrun.py` & `snakemake-8.9.0/snakemake/executors/dryrun.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/executors/google_lifesciences_helper.py` & `snakemake-8.9.0/snakemake/executors/google_lifesciences_helper.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/executors/local.py` & `snakemake-8.9.0/snakemake/executors/local.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/executors/touch.py` & `snakemake-8.9.0/snakemake/executors/touch.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/gui.html` & `snakemake-8.9.0/snakemake/gui.html`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/gui.py` & `snakemake-8.9.0/snakemake/gui.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/io.py` & `snakemake-8.9.0/snakemake/io.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/ioflags.py` & `snakemake-8.9.0/snakemake/ioflags.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/ioutils.py` & `snakemake-8.9.0/snakemake/ioutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from collections.abc import Mapping, Callable
 from functools import partial
+import inspect
+import os
 import re
 from typing import List, Optional, Union
 
+from snakemake.common import async_run
 import snakemake.io
 import snakemake.utils
 from snakemake.exceptions import LookupError
 from snakemake_interface_common.exceptions import WorkflowError
 
 
 class WildcardHandlerBase(ABC):
@@ -284,16 +287,40 @@
 
 
 # Alias for expand that provides a more intuitive name for the use case of
 # collecting files from previous jobs.
 collect = snakemake.io.expand
 
 
+def exists(path):
+    """Return True if the given file or directory exists.
+
+    This function considers any storage arguments given to Snakemake.
+    """
+    func_context = inspect.currentframe().f_back.f_locals
+    func_context_global = inspect.currentframe().f_back.f_globals
+
+    workflow = func_context.get("workflow") or func_context_global.get("workflow")
+
+    if workflow is None:
+        raise WorkflowError(
+            "The exists function can only be used within a Snakemake workflow "
+            "(the global variable 'workflow' has to be present)."
+        )
+
+    path = workflow.modifier.path_modifier.apply_default_storage(path)
+    if snakemake.io.is_flagged(path, "storage_object"):
+        return async_run(path.flags["storage_object"].managed_exists())
+    else:
+        return os.path.exists(path)
+
+
 def register_in_globals(_globals):
     _globals.update(
         {
             "lookup": lookup,
             "evaluate": evaluate,
             "branch": branch,
             "collect": collect,
+            "exists": exists,
         }
     )
```

### Comparing `snakemake-8.8.0/snakemake/jobs.py` & `snakemake-8.9.0/snakemake/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,19 +768,25 @@
             for f in self.log:
                 f.prepare()
             if self.benchmark:
                 self.benchmark.prepare()
 
         # wait for input files, respecting keep_storage_local
         wait_for_local = self.dag.workflow.storage_settings.keep_storage_local
-        await wait_for_files(
-            self.input,
-            wait_for_local=wait_for_local,
-            latency_wait=self.dag.workflow.execution_settings.latency_wait,
-        )
+        try:
+            await wait_for_files(
+                self.input,
+                wait_for_local=wait_for_local,
+                latency_wait=self.dag.workflow.execution_settings.latency_wait,
+            )
+        except IOError as ex:
+            raise WorkflowError(
+                ex,
+                rule=self.rule,
+            )
 
         if not self.is_shadow or self.is_norun:
             return
 
         # Create shadow directory structure
         self.shadow_dir = tempfile.mkdtemp(
             dir=self.rule.workflow.persistence.shadow_path
```

### Comparing `snakemake-8.8.0/snakemake/linting/__init__.py` & `snakemake-8.9.0/snakemake/linting/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/linting/links.py` & `snakemake-8.9.0/snakemake/linting/links.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/linting/rules.py` & `snakemake-8.9.0/snakemake/linting/rules.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/linting/snakefiles.py` & `snakemake-8.9.0/snakemake/linting/snakefiles.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/logging.py` & `snakemake-8.9.0/snakemake/logging.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/modules.py` & `snakemake-8.9.0/snakemake/modules.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/notebook.py` & `snakemake-8.9.0/snakemake/notebook.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/output_index.py` & `snakemake-8.9.0/snakemake/output_index.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/parser.py` & `snakemake-8.9.0/snakemake/parser.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/path_modifier.py` & `snakemake-8.9.0/snakemake/path_modifier.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/persistence.py` & `snakemake-8.9.0/snakemake/persistence.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/profiles.py` & `snakemake-8.9.0/snakemake/profiles.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/__init__.py` & `snakemake-8.9.0/snakemake/report/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/common.py` & `snakemake-8.9.0/snakemake/report/common.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/__init__.py` & `snakemake-8.9.0/snakemake/report/html_reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/common.py` & `snakemake-8.9.0/snakemake/report/html_reporter/common.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/configfiles.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/configfiles.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/packages.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/packages.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/results.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/results.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/rulegraph.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/rulegraph.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/rules.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/rules.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/runtimes.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/runtimes.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/data/timeline.py` & `snakemake-8.9.0/snakemake/report/html_reporter/data/timeline.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/abstract_menu.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/abstract_menu.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/abstract_results.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/abstract_results.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/app.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/app.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/breadcrumbs.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/breadcrumbs.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/category.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/category.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/content.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/content.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/icon.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/icon.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/menu.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/menu.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/navbar.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/navbar.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/report_info.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/report_info.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/result_info.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/result_info.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/result_view_button.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/result_view_button.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/rule_graph.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/rule_graph.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/rule_info.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/rule_info.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/components/search_results.js` & `snakemake-8.9.0/snakemake/report/html_reporter/template/components/search_results.js`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/index.html.jinja2` & `snakemake-8.9.0/snakemake/report/html_reporter/template/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/logo.svg` & `snakemake-8.9.0/snakemake/report/html_reporter/template/logo.svg`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/html_reporter/template/style.css` & `snakemake-8.9.0/snakemake/report/html_reporter/template/style.css`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report/rulegraph_spec.py` & `snakemake-8.9.0/snakemake/report/rulegraph_spec.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/report.css` & `snakemake-8.9.0/snakemake/report.css`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/resources.py` & `snakemake-8.9.0/snakemake/resources.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/ruleinfo.py` & `snakemake-8.9.0/snakemake/ruleinfo.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/rules.py` & `snakemake-8.9.0/snakemake/rules.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/scheduler.py` & `snakemake-8.9.0/snakemake/scheduler.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/script/__init__.py` & `snakemake-8.9.0/snakemake/script/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/settings.py` & `snakemake-8.9.0/snakemake/settings.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/shell.py` & `snakemake-8.9.0/snakemake/shell.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/sourcecache.py` & `snakemake-8.9.0/snakemake/sourcecache.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/spawn_jobs.py` & `snakemake-8.9.0/snakemake/spawn_jobs.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/storage.py` & `snakemake-8.9.0/snakemake/storage.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/target_jobs.py` & `snakemake-8.9.0/snakemake/target_jobs.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/template_rendering/__init__.py` & `snakemake-8.9.0/snakemake/template_rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/template_rendering/jinja2.py` & `snakemake-8.9.0/snakemake/template_rendering/jinja2.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/unit_tests/__init__.py` & `snakemake-8.9.0/snakemake/unit_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/unit_tests/templates/common.py.jinja2` & `snakemake-8.9.0/snakemake/unit_tests/templates/common.py.jinja2`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/unit_tests/templates/ruletest.py.jinja2` & `snakemake-8.9.0/snakemake/unit_tests/templates/ruletest.py.jinja2`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/utils.py` & `snakemake-8.9.0/snakemake/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/workflow.py` & `snakemake-8.9.0/snakemake/workflow.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake/wrapper.py` & `snakemake-8.9.0/snakemake/wrapper.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake.egg-info/PKG-INFO` & `snakemake-8.9.0/snakemake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake
-Version: 8.8.0
+Version: 8.9.0
 Summary: Workflow management system to create reproducible and scalable data analyses
 Author: Johannes Köster
 Author-email: johannes.koester@uni-due.de
 License: MIT
 Project-URL: Homepage, https://snakemake.github.io
 Project-URL: Documentation, https://snakemake.readthedocs.io
 Project-URL: Source, https://github.com/snakemake/snakemake
```

### Comparing `snakemake-8.8.0/snakemake.egg-info/SOURCES.txt` & `snakemake-8.9.0/snakemake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/snakemake.egg-info/requires.txt` & `snakemake-8.9.0/snakemake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_api.py` & `snakemake-8.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_executor_test_suite.py` & `snakemake-8.9.0/tests/test_executor_test_suite.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_expand.py` & `snakemake-8.9.0/tests/test_expand.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_io.py` & `snakemake-8.9.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_linting.py` & `snakemake-8.9.0/tests/test_linting.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_persistence.py` & `snakemake-8.9.0/tests/test_persistence.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_schema.py` & `snakemake-8.9.0/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/test_script.py` & `snakemake-8.9.0/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/testapi.py` & `snakemake-8.9.0/tests/testapi.py`

 * *Files identical despite different names*

### Comparing `snakemake-8.8.0/tests/tests.py` & `snakemake-8.9.0/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -2052,14 +2052,19 @@
 
 @skip_on_windows  # OS agnostic
 def test_summary():
     run(dpath("test01"), shellcmd="snakemake --summary", check_results=False)
 
 
 @skip_on_windows  # OS agnostic
+def test_exists():
+    run(dpath("test_exists"), check_results=False, executor="dryrun")
+
+
+@skip_on_windows  # OS agnostic
 def test_github_issue2732():
     run(dpath("test_github_issue2732"))
 
 
 def test_expand_list_of_functions():
     run(dpath("test_expand_list_of_functions"))
```

### Comparing `snakemake-8.8.0/versioneer.py` & `snakemake-8.9.0/versioneer.py`

 * *Files identical despite different names*

