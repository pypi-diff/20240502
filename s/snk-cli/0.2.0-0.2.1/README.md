# Comparing `tmp/snk_cli-0.2.0.tar.gz` & `tmp/snk_cli-0.2.1.tar.gz`

## Comparing `snk_cli-0.2.0.tar` & `snk_cli-0.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snk_cli-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk_cli-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 snk_cli-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/index.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/cli.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/config.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/dynamic_typer.md
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/options.md
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/subcommands.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/testing.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/utils.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/validate.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.0/docs/reference/workflow.md
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/__about__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/__init__.py
--rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/cli.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/conda.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/dynamic_typer.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/testing.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/utils.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/validate.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/workflow.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/config/__init__.py
--rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/config/config.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/config/utils.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/options/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/options/option.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/options/utils.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/config.py
--rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/env.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/profile.py
--rw-r--r--   0        0        0    18508 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/run.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 snk_cli-0.2.0/src/snk_cli/subcommands/script.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_conda_env.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_dynamic_typer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/cov.fasta
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/Snakefile
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/cli.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/config.yaml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/print_config/snk.yaml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/cli.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/config.yaml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/snk.yaml
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/resources/data.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/things/__about__.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/Snakefile
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/envs/python.yml
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/profiles/base/config.yaml
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/profiles/slurm/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/data/workflow/workflow/scripts/hello.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/__init__.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_dynamic_options.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_run.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_snk_config.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_subcommands.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_validate.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 snk_cli-0.2.0/tests/test_cli/test_workflow_cli.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snk_cli-0.2.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk_cli-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 snk_cli-0.2.0/README.md
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 snk_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 snk_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 snk_cli-0.2.1/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk_cli-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 snk_cli-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/index.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/cli.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/config.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/dynamic_typer.md
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/options.md
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/subcommands.md
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/testing.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/utils.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/validate.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 snk_cli-0.2.1/docs/reference/workflow.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/__about__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/__init__.py
+-rw-r--r--   0        0        0     8847 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/cli.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/conda.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/dynamic_typer.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/testing.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/utils.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/validate.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/workflow.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/config/__init__.py
+-rw-r--r--   0        0        0    10310 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/config/config.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/config/utils.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/options/__init__.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/options/option.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/options/utils.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/__init__.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/config.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/env.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/profile.py
+-rw-r--r--   0        0        0    18481 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/run.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 snk_cli-0.2.1/src/snk_cli/subcommands/script.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_conda_env.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_dynamic_typer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/cov.fasta
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/Snakefile
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/cli.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/config.yaml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/print_config/snk.yaml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/cli.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/config.yaml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/snk.yaml
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/resources/data.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/things/__about__.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/Snakefile
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/envs/python.yml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/profiles/base/config.yaml
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/profiles/slurm/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/data/workflow/workflow/scripts/hello.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/__init__.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_dynamic_options.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_run.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_snk_config.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_subcommands.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_validate.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 snk_cli-0.2.1/tests/test_cli/test_workflow_cli.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 snk_cli-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk_cli-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 snk_cli-0.2.1/README.md
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 snk_cli-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 snk_cli-0.2.1/PKG-INFO
```

### Comparing `snk_cli-0.2.0/mkdocs.yml` & `snk_cli-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/.github/workflows/publish.yml` & `snk_cli-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/.github/workflows/tests.yml` & `snk_cli-0.2.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/cli.py` & `snk_cli-0.2.1/src/snk_cli/cli.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/conda.py` & `snk_cli-0.2.1/src/snk_cli/conda.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/dynamic_typer.py` & `snk_cli-0.2.1/src/snk_cli/dynamic_typer.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/testing.py` & `snk_cli-0.2.1/src/snk_cli/testing.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/utils.py` & `snk_cli-0.2.1/src/snk_cli/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/validate.py` & `snk_cli-0.2.1/src/snk_cli/validate.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/workflow.py` & `snk_cli-0.2.1/src/snk_cli/workflow.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/config/config.py` & `snk_cli-0.2.1/src/snk_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/config/utils.py` & `snk_cli-0.2.1/src/snk_cli/config/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/options/utils.py` & `snk_cli-0.2.1/src/snk_cli/options/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/subcommands/config.py` & `snk_cli-0.2.1/src/snk_cli/subcommands/config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/subcommands/env.py` & `snk_cli-0.2.1/src/snk_cli/subcommands/env.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/subcommands/profile.py` & `snk_cli-0.2.1/src/snk_cli/subcommands/profile.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/src/snk_cli/subcommands/run.py` & `snk_cli-0.2.1/src/snk_cli/subcommands/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,15 @@
         Side Effects:
           Prints the snakemake help and exits.
 
         Examples:
           >>> RunApp._print_snakemake_help(True)
         """
         if value:
-            import snakemake
-
-            snakemake.main("-h")
+            execute_snakemake("-h")
 
     def run(
         self,
         ctx: typer.Context,
         configfile: Path = typer.Option(
             None,
             "--config",
```

### Comparing `snk_cli-0.2.0/src/snk_cli/subcommands/script.py` & `snk_cli-0.2.1/src/snk_cli/subcommands/script.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/test_dynamic_typer.py` & `snk_cli-0.2.1/tests/test_dynamic_typer.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/utils.py` & `snk_cli-0.2.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/artic_v4.1.bed` & `snk_cli-0.2.1/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/config.yaml` & `snk_cli-0.2.1/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/cov.fasta` & `snk_cli-0.2.1/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/workflow/snk.yaml` & `snk_cli-0.2.1/tests/data/workflow/snk.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/workflow/workflow/Snakefile` & `snk_cli-0.2.1/tests/data/workflow/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/workflow/workflow/envs/python.yml` & `snk_cli-0.2.1/tests/data/workflow/workflow/envs/python.yml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/data/workflow/workflow/profiles/slurm/config.yaml` & `snk_cli-0.2.1/tests/data/workflow/workflow/profiles/slurm/config.yaml`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/test_cli/test_dynamic_options.py` & `snk_cli-0.2.1/tests/test_cli/test_dynamic_options.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/test_cli/test_run.py` & `snk_cli-0.2.1/tests/test_cli/test_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,7 +35,16 @@
     assert "cli" in res.stdout
     res = runner.invoke(
         ["run", "-v", "--value", "cli", "--config", "tests/data/print_config/config.yaml",]
     )
     assert res.exit_code == 0, res.stderr
     assert "cli" in res.stdout, res.stderr
 
+def test_snakemake_help(local_runner: SnkCliRunner):
+    res = local_runner(["run", "-hs"])
+    assert res.exit_code == 0, res.stderr
+    assert "snakemake" in res.stdout
+
+def test_snakemake_version(local_runner: SnkCliRunner):
+    res = local_runner(["run", "--snake-v"])
+    assert res.exit_code == 0, res.stderr
+    assert res.stdout in ["7.32.4\n", "8.10.8\n"]
```

### Comparing `snk_cli-0.2.0/tests/test_cli/test_snk_config.py` & `snk_cli-0.2.1/tests/test_cli/test_snk_config.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/test_cli/test_subcommands.py` & `snk_cli-0.2.1/tests/test_cli/test_subcommands.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/test_cli/test_validate.py` & `snk_cli-0.2.1/tests/test_cli/test_validate.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/tests/test_cli/test_workflow_cli.py` & `snk_cli-0.2.1/tests/test_cli/test_workflow_cli.py`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/LICENSE.txt` & `snk_cli-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/README.md` & `snk_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `snk_cli-0.2.0/pyproject.toml` & `snk_cli-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -42,24 +42,19 @@
 [tool.hatch.version]
 path = "src/snk_cli/__about__.py"
 
 
 [[tool.hatch.envs.snakemake.matrix]]
 snakemake = ["7.32.4", "8.10.8"]
 
-[tool.hatch.snakemake.test]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
-  "snakemake=={matrix:snakemake}"]
-
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "snakemake=={matrix:snakemake:7.32.4}",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

### Comparing `snk_cli-0.2.0/PKG-INFO` & `snk_cli-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snk-cli
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: Documentation, https://github.com/unknown/snk-cli#readme
 Project-URL: Issues, https://github.com/unknown/snk-cli/issues
 Project-URL: Source, https://github.com/unknown/snk-cli
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

