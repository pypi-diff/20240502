# Comparing `tmp/hatch-1rc5.tar.gz` & `tmp/hatch-1rc6.tar.gz`

## Comparing `hatch-1rc5.tar` & `hatch-1rc6.tar`

### file list

```diff
@@ -1,225 +1,225 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hatch-1rc5/.flake8
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hatch-1rc5/.gitattributes
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatch-1rc5/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 hatch-1rc5/LICENSE.txt
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 hatch-1rc5/README.md
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 hatch-1rc5/hatch.toml
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 hatch-1rc5/mkdocs.yml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hatch-1rc5/mypy.ini
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 hatch-1rc5/pyproject.toml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 hatch-1rc5/docs/build.md
--rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 hatch-1rc5/docs/environment.md
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 hatch-1rc5/docs/index.md
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 hatch-1rc5/docs/install.md
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 hatch-1rc5/docs/intro.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hatch-1rc5/docs/next-steps.md
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 hatch-1rc5/docs/publish.md
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 hatch-1rc5/docs/version.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hatch-1rc5/docs/.scripts/49_global_refs.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hatch-1rc5/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hatch-1rc5/docs/.snippets/links.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch-1rc5/docs/.snippets/refs.txt
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 hatch-1rc5/docs/assets/css/custom.css
--rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 hatch-1rc5/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch-1rc5/docs/cli/about.md
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch-1rc5/docs/cli/reference.md
--rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 hatch-1rc5/docs/config/build.md
--rw-r--r--   0        0        0    10689 2020-02-02 00:00:00.000000 hatch-1rc5/docs/config/dependency.md
--rw-r--r--   0        0        0    18840 2020-02-02 00:00:00.000000 hatch-1rc5/docs/config/environment.md
--rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 hatch-1rc5/docs/config/hatch.md
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 hatch-1rc5/docs/config/metadata.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 hatch-1rc5/docs/config/project-templates.md
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hatch-1rc5/docs/meta/authors.md
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 hatch-1rc5/docs/meta/faq.md
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 hatch-1rc5/docs/meta/history.md
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/about.md
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/build-hook.md
--rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/builder.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/environment-collector.md
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/environment.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/metadata-hook.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/publisher.md
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/utilities.md
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/version-scheme.md
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 hatch-1rc5/docs/plugins/version-source.md
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/__init__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/py.typed
--rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/__init__.py
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/application.py
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/terminal.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/build/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/clean/__init__.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/config/__init__.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/dep/__init__.py
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/env/__init__.py
--rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/new/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/publish/__init__.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/run/__init__.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/shell/__init__.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/status/__init__.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/cli/version/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/config/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/config/constants.py
--rw-r--r--   0        0        0    24208 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/config/model.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/config/user.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/config/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/system.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/virtual.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/collectors/__init__.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/collectors/default.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/collectors/plugin/__init__.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/collectors/plugin/hooks.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/collectors/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/plugin/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/plugin/hooks.py
--rw-r--r--   0        0        0    27664 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/env/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/plugin/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/plugin/manager.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/plugin/specs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/project/__init__.py
--rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/project/config.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/project/core.py
--rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/project/env.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/publish/__init__.py
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/publish/pypi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/publish/plugin/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/publish/plugin/hooks.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/publish/plugin/interface.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/__init__.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/default.py
--rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/files_default.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/files_feature_ci.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/files_feature_cli.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/files_feature_tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/plugin/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/plugin/hooks.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/template/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/__init__.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/ci.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/fs.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/network.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/platform.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/shells.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/utils/structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/venv/__init__.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/venv/core.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/venv/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/version/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/version/scheme/__init__.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/version/scheme/standard.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/version/scheme/plugin/__init__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/version/scheme/plugin/hooks.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 hatch-1rc5/hatch/version/scheme/plugin/interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/__init__.py
--rw-r--r--   0        0        0     6875 2020-02-02 00:00:00.000000 hatch-1rc5/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/__init__.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/test_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/__init__.py
--rw-r--r--   0        0        0    41857 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/test_config.py
--rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/test_custom.py
--rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/test_sdist.py
--rw-r--r--   0        0        0    34960 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/test_wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/hooks/__init__.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/hooks/test_custom.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/plugin/__init__.py
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/builders/plugin/test_interface.py
--rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/downstream/integrate.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/downstream/requirements.txt
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/downstream/datadogpy/data.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/downstream/datadogpy/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/licenses/__init__.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/licenses/test_parse.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/licenses/test_supported.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/metadata/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/metadata/test_build.py
--rw-r--r--   0        0        0    43530 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/metadata/test_core.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/metadata/test_custom_hook.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/metadata/test_hatch.py
--rw-r--r--   0        0        0    49415 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/metadata/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/version/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/version/source/__init__.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hatch-1rc5/tests/backend/version/source/test_regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/test_root.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/build/__init__.py
--rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/build/test_build.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/clean/__init__.py
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/clean/test_clean.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/config/test_show.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/dep/__init__.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/dep/test_hash.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/env/__init__.py
--rw-r--r--   0        0        0    31401 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/env/test_create.py
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/env/test_prune.py
--rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/env/test_remove.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/env/test_show.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/new/__init__.py
--rw-r--r--   0        0        0    16172 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/new/test_new.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/publish/__init__.py
--rw-r--r--   0        0        0    15864 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/publish/test_publish.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/run/__init__.py
--rw-r--r--   0        0        0    25687 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/run/test_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/status/test_status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/version/__init__.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hatch-1rc5/tests/cli/version/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/config/__init__.py
--rw-r--r--   0        0        0    42132 2020-02-02 00:00:00.000000 hatch-1rc5/tests/config/test_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/dep/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 hatch-1rc5/tests/dep/test_core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/env/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/env/plugin/__init__.py
--rw-r--r--   0        0        0    31762 2020-02-02 00:00:00.000000 hatch-1rc5/tests/env/plugin/test_interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/__init__.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/__init__.py
--rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/licenses/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/__init__.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/basic.py
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/default.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/feature_ci.py
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/feature_cli.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/feature_src_layout.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/licenses_empty.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/licenses_multiple.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/projects_urls_empty.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/new/projects_urls_space_in_label.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/sdist/__init__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/sdist/standard_default.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/sdist/standard_default_build_script_artifacts.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/sdist/standard_default_support_legacy.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/sdist/standard_include.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/sdist/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_default_build_script.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_default_build_script_artifacts.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_default_build_script_artifacts_with_src_layout.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_default_license_multiple.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_default_license_single.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_default_python_constraint.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_editable_pth.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_editable_standard.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/standard_tests.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 hatch-1rc5/tests/helpers/templates/wheel/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/project/__init__.py
--rw-r--r--   0        0        0    90967 2020-02-02 00:00:00.000000 hatch-1rc5/tests/project/test_config.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 hatch-1rc5/tests/project/test_core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/utils/__init__.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 hatch-1rc5/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 hatch-1rc5/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 hatch-1rc5/tests/utils/test_structures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/venv/__init__.py
--rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 hatch-1rc5/tests/venv/test_core.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hatch-1rc5/tests/venv/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/version/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc5/tests/version/scheme/__init__.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 hatch-1rc5/tests/version/scheme/test_standard.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 hatch-1rc5/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hatch-1rc6/.flake8
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hatch-1rc6/.gitattributes
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 hatch-1rc6/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 hatch-1rc6/LICENSE.txt
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 hatch-1rc6/README.md
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 hatch-1rc6/hatch.toml
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 hatch-1rc6/mkdocs.yml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 hatch-1rc6/mypy.ini
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 hatch-1rc6/pyproject.toml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 hatch-1rc6/docs/build.md
+-rw-r--r--   0        0        0     5227 2020-02-02 00:00:00.000000 hatch-1rc6/docs/environment.md
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 hatch-1rc6/docs/index.md
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 hatch-1rc6/docs/install.md
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 hatch-1rc6/docs/intro.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 hatch-1rc6/docs/next-steps.md
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 hatch-1rc6/docs/publish.md
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 hatch-1rc6/docs/version.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 hatch-1rc6/docs/.scripts/49_global_refs.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hatch-1rc6/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 hatch-1rc6/docs/.snippets/links.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 hatch-1rc6/docs/.snippets/refs.txt
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 hatch-1rc6/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    12014 2020-02-02 00:00:00.000000 hatch-1rc6/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 hatch-1rc6/docs/cli/about.md
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 hatch-1rc6/docs/cli/reference.md
+-rw-r--r--   0        0        0    10042 2020-02-02 00:00:00.000000 hatch-1rc6/docs/config/build.md
+-rw-r--r--   0        0        0    10689 2020-02-02 00:00:00.000000 hatch-1rc6/docs/config/dependency.md
+-rw-r--r--   0        0        0    18840 2020-02-02 00:00:00.000000 hatch-1rc6/docs/config/environment.md
+-rw-r--r--   0        0        0     7843 2020-02-02 00:00:00.000000 hatch-1rc6/docs/config/hatch.md
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 hatch-1rc6/docs/config/metadata.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 hatch-1rc6/docs/config/project-templates.md
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hatch-1rc6/docs/meta/authors.md
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 hatch-1rc6/docs/meta/faq.md
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 hatch-1rc6/docs/meta/history.md
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/about.md
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/build-hook.md
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/builder.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/environment-collector.md
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/environment.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/metadata-hook.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/publisher.md
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/utilities.md
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/version-scheme.md
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 hatch-1rc6/docs/plugins/version-source.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/__init__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/py.typed
+-rw-r--r--   0        0        0     6396 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/__init__.py
+-rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/application.py
+-rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/terminal.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/build/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/clean/__init__.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/config/__init__.py
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/dep/__init__.py
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/env/__init__.py
+-rw-r--r--   0        0        0     4933 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/new/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/publish/__init__.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/run/__init__.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/shell/__init__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/status/__init__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/cli/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/config/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/config/constants.py
+-rw-r--r--   0        0        0    24208 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/config/model.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/config/user.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/config/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/system.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/virtual.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/collectors/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/collectors/default.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/collectors/plugin/__init__.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/collectors/plugin/hooks.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/collectors/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/plugin/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/plugin/hooks.py
+-rw-r--r--   0        0        0    27664 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/env/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/plugin/__init__.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/plugin/manager.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/plugin/specs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/project/__init__.py
+-rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/project/config.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/project/core.py
+-rw-r--r--   0        0        0    10869 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/project/env.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/publish/__init__.py
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/publish/pypi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/publish/plugin/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/publish/plugin/hooks.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/publish/plugin/interface.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/__init__.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/default.py
+-rw-r--r--   0        0        0     5663 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/files_default.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/files_feature_ci.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/files_feature_cli.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/files_feature_tests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/plugin/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/plugin/hooks.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/template/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/__init__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/ci.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/fs.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/network.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/platform.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/shells.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/utils/structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/venv/__init__.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/venv/core.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/venv/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/version/scheme/__init__.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/version/scheme/standard.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/version/scheme/plugin/__init__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/version/scheme/plugin/hooks.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 hatch-1rc6/hatch/version/scheme/plugin/interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/__init__.py
+-rw-r--r--   0        0        0     6989 2020-02-02 00:00:00.000000 hatch-1rc6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/__init__.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/test_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/__init__.py
+-rw-r--r--   0        0        0    47487 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/test_config.py
+-rw-r--r--   0        0        0     8788 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/test_custom.py
+-rw-r--r--   0        0        0    38953 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/test_sdist.py
+-rw-r--r--   0        0        0    34960 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/test_wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/hooks/__init__.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/hooks/test_custom.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/plugin/__init__.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/builders/plugin/test_interface.py
+-rw-r--r--   0        0        0     6498 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/downstream/integrate.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/downstream/requirements.txt
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/downstream/datadogpy/data.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/downstream/datadogpy/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/licenses/__init__.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/licenses/test_parse.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/licenses/test_supported.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/metadata/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/metadata/test_build.py
+-rw-r--r--   0        0        0    43530 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/metadata/test_core.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/metadata/test_custom_hook.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/metadata/test_hatch.py
+-rw-r--r--   0        0        0    49415 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/metadata/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/version/source/__init__.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hatch-1rc6/tests/backend/version/source/test_regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/test_root.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/build/__init__.py
+-rw-r--r--   0        0        0    32124 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/build/test_build.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/clean/__init__.py
+-rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/clean/test_clean.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     5681 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/dep/__init__.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/dep/test_hash.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/env/__init__.py
+-rw-r--r--   0        0        0    31401 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/env/test_create.py
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/env/test_prune.py
+-rw-r--r--   0        0        0     9118 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/env/test_remove.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/env/test_show.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/new/__init__.py
+-rw-r--r--   0        0        0    16172 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/new/test_new.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/publish/__init__.py
+-rw-r--r--   0        0        0    15864 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/publish/test_publish.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/run/__init__.py
+-rw-r--r--   0        0        0    25687 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/run/test_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/version/__init__.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 hatch-1rc6/tests/cli/version/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/config/__init__.py
+-rw-r--r--   0        0        0    42132 2020-02-02 00:00:00.000000 hatch-1rc6/tests/config/test_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/dep/__init__.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 hatch-1rc6/tests/dep/test_core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/env/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/env/plugin/__init__.py
+-rw-r--r--   0        0        0    31762 2020-02-02 00:00:00.000000 hatch-1rc6/tests/env/plugin/test_interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/__init__.py
+-rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/licenses/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/__init__.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/basic.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/default.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/feature_ci.py
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/feature_cli.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/feature_src_layout.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/licenses_empty.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/licenses_multiple.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/projects_urls_empty.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/new/projects_urls_space_in_label.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/sdist/__init__.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/sdist/standard_default.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/sdist/standard_default_build_script_artifacts.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/sdist/standard_default_support_legacy.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/sdist/standard_include.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/sdist/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/__init__.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_default_build_script.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_default_build_script_artifacts.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_default_build_script_artifacts_with_src_layout.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_default_license_multiple.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_default_license_single.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_default_python_constraint.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_editable_pth.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_editable_standard.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/standard_tests.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 hatch-1rc6/tests/helpers/templates/wheel/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/project/__init__.py
+-rw-r--r--   0        0        0    90967 2020-02-02 00:00:00.000000 hatch-1rc6/tests/project/test_config.py
+-rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 hatch-1rc6/tests/project/test_core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 hatch-1rc6/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 hatch-1rc6/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 hatch-1rc6/tests/utils/test_structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/venv/__init__.py
+-rw-r--r--   0        0        0     4862 2020-02-02 00:00:00.000000 hatch-1rc6/tests/venv/test_core.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hatch-1rc6/tests/venv/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/version/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch-1rc6/tests/version/scheme/__init__.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 hatch-1rc6/tests/version/scheme/test_standard.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 hatch-1rc6/PKG-INFO
```

### Comparing `hatch-1rc5/LICENSE.txt` & `hatch-1rc6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/README.md` & `hatch-1rc6/README.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch.toml` & `hatch-1rc6/hatch.toml`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/mkdocs.yml` & `hatch-1rc6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/pyproject.toml` & `hatch-1rc6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Build Tools",
 ]
 dependencies = [
   "atomicwrites~=1.4",
   "click~=8.0.3",
-  "hatchling>=0.5",
+  "hatchling>=0.6",
   "httpx~=0.21",
   "keyring~=23.4",
   "pexpect~=4.8.0",
   "platformdirs~=2.4",
   "pyperclip~=1.8",
   "rich~=10.16",
   "tomli-w~=1.0",
```

### Comparing `hatch-1rc5/docs/build.md` & `hatch-1rc6/docs/build.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/environment.md` & `hatch-1rc6/docs/environment.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/index.md` & `hatch-1rc6/docs/index.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/intro.md` & `hatch-1rc6/docs/intro.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/next-steps.md` & `hatch-1rc6/docs/next-steps.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/publish.md` & `hatch-1rc6/docs/publish.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/version.md` & `hatch-1rc6/docs/version.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/assets/css/custom.css` & `hatch-1rc6/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/assets/images/favicon.ico` & `hatch-1rc6/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/cli/about.md` & `hatch-1rc6/docs/cli/about.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/config/build.md` & `hatch-1rc6/docs/config/build.md`

 * *Files 10% similar despite different names*

```diff
@@ -323,7 +323,37 @@
     [build.hooks.hook3]
     [build.hooks.hook1]
 
     [build.targets.foo.hooks.hook2]
     ```
 
 When target `foo` is built, build hook `hook2` will be executed first, followed by `hook3`, and then finally `hook1`.
+
+### Conditional execution
+
+If you want to disable a build hook by default and control its use by [environment variables](#environment-variables), you can do so by setting the `enable-by-default` option to `false`:
+
+=== ":octicons-file-code-16: pyproject.toml"
+
+    ```toml
+    [tool.hatch.build.hooks.<HOOK_NAME>]
+    enable-by-default = false
+    ```
+
+=== ":octicons-file-code-16: hatch.toml"
+
+    ```toml
+    [build.hooks.<HOOK_NAME>]
+    enable-by-default = false
+    ```
+
+## Environment variables
+
+| Variable | Default | Description |
+| --- | --- | --- |
+| `HATCH_BUILD_CLEAN` | `false` | Whether or not existing artifacts should first be removed |
+| `HATCH_BUILD_CLEAN_HOOKS_AFTER` | `false` | Whether or not build hook artifacts should be removed after each build |
+| `HATCH_BUILD_HOOKS_ONLY` | `false` | Whether or not to only execute build hooks |
+| `HATCH_BUILD_NO_HOOKS` | `false` | Whether or not to disable all build hooks; this takes precedence over other options |
+| `HATCH_BUILD_HOOKS_ENABLE` | `false` | Whether or not to enable all build hooks |
+| `HATCH_BUILD_HOOK_ENABLE_<HOOK_NAME>` | `false` |  |
+| `HATCH_BUILD_LOCATION` | `dist` | The location with which to build the targets; only used by the [`build`](../cli/reference.md#hatch-build) command |
```

### Comparing `hatch-1rc5/docs/config/dependency.md` & `hatch-1rc6/docs/config/dependency.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/config/environment.md` & `hatch-1rc6/docs/config/environment.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/config/hatch.md` & `hatch-1rc6/docs/config/hatch.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/config/metadata.md` & `hatch-1rc6/docs/config/metadata.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/config/project-templates.md` & `hatch-1rc6/docs/config/project-templates.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/meta/authors.md` & `hatch-1rc6/docs/meta/authors.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/meta/faq.md` & `hatch-1rc6/docs/meta/faq.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/meta/history.md` & `hatch-1rc6/docs/meta/history.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## **Hatch**
 
 ### Unreleased
 
+### [1rc6](https://github.com/ofek/hatch/releases/tag/hatch-v1rc6) - 2022-01-06 ### {: #hatch-v1rc6 }
+
+***Added:***
+
+- Bump the minimum supported version of Hatchling
+
 ### [1rc5](https://github.com/ofek/hatch/releases/tag/hatch-v1rc5) - 2022-01-02 ### {: #hatch-v1rc5 }
 
 ***Fixed:***
 
 - Reduce default verbosity of config file creation for new users
 
 ### [1rc4](https://github.com/ofek/hatch/releases/tag/hatch-v1rc4) - 2022-01-01 ### {: #hatch-v1rc4 }
@@ -39,14 +45,24 @@
 
 -----
 
 ## **Hatchling**
 
 ### Unreleased
 
+### [0.6](https://github.com/ofek/hatch/releases/tag/hatchling-v0.6) - 2022-01-06 ### {: #hatchling-v0.6 }
+
+***Added:***
+
+- Add ability to conditionally execute build hooks
+
+***Fixed:***
+
+- Disregard hook dependencies when building without hooks
+
 ### [0.5](https://github.com/ofek/hatch/releases/tag/hatchling-v0.5) - 2022-01-01 ### {: #hatchling-v0.5 }
 
 ***Added:***
 
 - Add option to clean build hook artifacts after each build
 
 ***Fixed:***
```

### Comparing `hatch-1rc5/docs/plugins/about.md` & `hatch-1rc6/docs/plugins/about.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/build-hook.md` & `hatch-1rc6/docs/plugins/build-hook.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/builder.md` & `hatch-1rc6/docs/plugins/builder.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/environment-collector.md` & `hatch-1rc6/docs/plugins/environment-collector.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/environment.md` & `hatch-1rc6/docs/plugins/environment.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/metadata-hook.md` & `hatch-1rc6/docs/plugins/metadata-hook.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/publisher.md` & `hatch-1rc6/docs/plugins/publisher.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/utilities.md` & `hatch-1rc6/docs/plugins/utilities.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/version-scheme.md` & `hatch-1rc6/docs/plugins/version-scheme.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/docs/plugins/version-source.md` & `hatch-1rc6/docs/plugins/version-source.md`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/__init__.py` & `hatch-1rc6/hatch/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/application.py` & `hatch-1rc6/hatch/cli/application.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/terminal.py` & `hatch-1rc6/hatch/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/build/__init__.py` & `hatch-1rc6/hatch/cli/build/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,17 +43,19 @@
 )
 @click.option('--clean-only', is_flag=True, hidden=True)
 @click.pass_obj
 def build(app, location, targets, hooks_only, no_hooks, ext, clean, clean_hooks_after, clean_only):
     """Build a project."""
     import pickle
 
+    from hatchling.builders.constants import BuildEnvVars
     from hatchling.builders.plugin.interface import BuilderInterface
 
     from ...utils.fs import Path
+    from ...utils.structures import EnvVars
 
     if app.project.metadata.build.build_backend != 'hatchling.build':
         app.abort('Field `build-system.build-backend` must be set to `hatchling.build`')
 
     backend_requirements = []
     for requirement in app.project.metadata.build.requires_complex:
         if requirement.name != 'hatchling':
@@ -81,28 +83,33 @@
 
         builders = app.plugins.builder.collect(include_third_party=False)
         for target_name in sorted(builders):
             app.display_error(f'[tool.hatch.build.targets.{target_name}]')
 
         app.abort()
 
-    with app.project.location.as_cwd():
+    env_vars = {}
+    if no_hooks:
+        env_vars[BuildEnvVars.NO_HOOKS] = 'true'
+
+    with app.project.location.as_cwd(env_vars):
         environment = app.get_environment()
 
         for i, target in enumerate(targets):
             # Separate targets with a blank line
             if not clean_only and i != 0:
                 app.display_info()
 
             target_name, _, _ = target.partition(':')
             builder = BuilderInterface(str(app.project.location))
             builder.PLUGIN_NAME = target_name
 
             dependencies = list(backend_requirements)
-            dependencies.extend(builder.config.dependencies)
+            with environment.get_env_vars(), EnvVars(env_vars):
+                dependencies.extend(builder.config.dependencies)
 
             with app.status_waiting('Setting up build environment') as status:
                 with environment.build_environment(dependencies) as build_environment:
                     status.stop()
 
                     build_process = environment.get_build_process(
                         build_environment,
```

### Comparing `hatch-1rc5/hatch/cli/clean/__init__.py` & `hatch-1rc6/hatch/cli/clean/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/config/__init__.py` & `hatch-1rc6/hatch/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/dep/__init__.py` & `hatch-1rc6/hatch/cli/dep/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/env/__init__.py` & `hatch-1rc6/hatch/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/new/__init__.py` & `hatch-1rc6/hatch/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/publish/__init__.py` & `hatch-1rc6/hatch/cli/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/run/__init__.py` & `hatch-1rc6/hatch/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/shell/__init__.py` & `hatch-1rc6/hatch/cli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/status/__init__.py` & `hatch-1rc6/hatch/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/cli/version/__init__.py` & `hatch-1rc6/hatch/cli/version/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/config/constants.py` & `hatch-1rc6/hatch/config/constants.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/config/model.py` & `hatch-1rc6/hatch/config/model.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/config/user.py` & `hatch-1rc6/hatch/config/user.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/env/system.py` & `hatch-1rc6/hatch/env/system.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/env/virtual.py` & `hatch-1rc6/hatch/env/virtual.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/env/collectors/plugin/interface.py` & `hatch-1rc6/hatch/env/collectors/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/env/plugin/interface.py` & `hatch-1rc6/hatch/env/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/plugin/manager.py` & `hatch-1rc6/hatch/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/plugin/specs.py` & `hatch-1rc6/hatch/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/project/config.py` & `hatch-1rc6/hatch/project/config.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/project/core.py` & `hatch-1rc6/hatch/project/core.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/project/env.py` & `hatch-1rc6/hatch/project/env.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/publish/pypi.py` & `hatch-1rc6/hatch/publish/pypi.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/publish/plugin/interface.py` & `hatch-1rc6/hatch/publish/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/template/__init__.py` & `hatch-1rc6/hatch/template/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/template/default.py` & `hatch-1rc6/hatch/template/default.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/template/files_default.py` & `hatch-1rc6/hatch/template/files_default.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/template/files_feature_ci.py` & `hatch-1rc6/hatch/template/files_feature_ci.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/template/files_feature_cli.py` & `hatch-1rc6/hatch/template/files_feature_cli.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/template/plugin/interface.py` & `hatch-1rc6/hatch/template/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/utils/fs.py` & `hatch-1rc6/hatch/utils/fs.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/utils/platform.py` & `hatch-1rc6/hatch/utils/platform.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/utils/shells.py` & `hatch-1rc6/hatch/utils/shells.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/utils/structures.py` & `hatch-1rc6/hatch/utils/structures.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/venv/core.py` & `hatch-1rc6/hatch/venv/core.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/version/scheme/standard.py` & `hatch-1rc6/hatch/version/scheme/standard.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/hatch/version/scheme/plugin/interface.py` & `hatch-1rc6/hatch/version/scheme/plugin/interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/conftest.py` & `hatch-1rc6/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,17 @@
             line_queue.clear()
             original_args = sys.argv
             try:
                 sys.argv = command[3:]
                 mock = mocker.MagicMock()
 
                 try:
-                    hatchling()
+                    # The builder sets process-wide environment variables
+                    with EnvVars():
+                        hatchling()
                 except SystemExit as e:
                     mock.returncode = e.code
                 else:
                     mock.returncode = 0
 
                 mock.stdout = BytesIO(''.join(line_queue).encode('utf-8'))
                 return mock
```

### Comparing `hatch-1rc5/tests/backend/test_build.py` & `hatch-1rc6/tests/backend/test_build.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/builders/test_config.py` & `hatch-1rc6/tests/backend/builders/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 from os.path import join as pjoin
 
 import pathspec
 import pytest
 
+from hatch.utils.structures import EnvVars
+from hatchling.builders.constants import BuildEnvVars
 from hatchling.builders.plugin.interface import BuilderInterface
 
 
 class TestDirectory:
     def test_default(self, isolation):
         builder = BuilderInterface(str(isolation))
 
@@ -467,14 +469,84 @@
             },
         }
         builder = BuilderInterface(str(isolation), config=config)
         builder.PLUGIN_NAME = 'foo'
 
         assert builder.config.hook_config['foo']['baz'] == 'bar'
 
+    def test_env_var_no_hooks(self, isolation):
+        config = {'tool': {'hatch': {'build': {'hooks': {'foo': {'bar': 'baz'}}}}}}
+        builder = BuilderInterface(str(isolation), config=config)
+
+        with EnvVars({BuildEnvVars.NO_HOOKS: 'true'}):
+            assert builder.config.hook_config == {}
+
+    def test_enable_by_default(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'bar': 'baz', 'enable-by-default': False},
+                            'bar': {'foo': 'baz', 'enable-by-default': False},
+                            'baz': {'foo': 'bar'},
+                        }
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+
+        assert builder.config.hook_config == {'baz': {'foo': 'bar'}}
+
+    def test_env_var_all_override_enable_by_default(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'bar': 'baz', 'enable-by-default': False},
+                            'bar': {'foo': 'baz', 'enable-by-default': False},
+                            'baz': {'foo': 'bar'},
+                        }
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+
+        with EnvVars({BuildEnvVars.HOOKS_ENABLE: 'true'}):
+            assert builder.config.hook_config == {
+                'foo': {'bar': 'baz', 'enable-by-default': False},
+                'bar': {'foo': 'baz', 'enable-by-default': False},
+                'baz': {'foo': 'bar'},
+            }
+
+    def test_env_var_specific_override_enable_by_default(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'bar': 'baz', 'enable-by-default': False},
+                            'bar': {'foo': 'baz', 'enable-by-default': False},
+                            'baz': {'foo': 'bar'},
+                        }
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+
+        with EnvVars({f'{BuildEnvVars.HOOK_ENABLE_PREFIX}FOO': 'true'}):
+            assert builder.config.hook_config == {
+                'foo': {'bar': 'baz', 'enable-by-default': False},
+                'baz': {'foo': 'bar'},
+            }
+
 
 class TestDependencies:
     def test_default(self, isolation):
         builder = BuilderInterface(str(isolation))
 
         assert builder.config.dependencies == builder.config.dependencies == []
 
@@ -543,14 +615,93 @@
             }
         }
         builder = BuilderInterface(str(isolation), config=config)
         builder.PLUGIN_NAME = 'foo'
 
         assert builder.config.dependencies == ['baz', 'bar', 'test2']
 
+    def test_env_var_no_hooks(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'dependencies': ['foo']},
+                            'bar': {'dependencies': ['bar']},
+                            'baz': {'dependencies': ['baz']},
+                        },
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+        builder.PLUGIN_NAME = 'foo'
+
+        with EnvVars({BuildEnvVars.NO_HOOKS: 'true'}):
+            assert builder.config.dependencies == []
+
+    def test_hooks_enable_by_default(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'dependencies': ['foo'], 'enable-by-default': False},
+                            'bar': {'dependencies': ['bar'], 'enable-by-default': False},
+                            'baz': {'dependencies': ['baz']},
+                        },
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+        builder.PLUGIN_NAME = 'foo'
+
+        assert builder.config.dependencies == ['baz']
+
+    def test_hooks_env_var_all_override_enable_by_default(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'dependencies': ['foo'], 'enable-by-default': False},
+                            'bar': {'dependencies': ['bar'], 'enable-by-default': False},
+                            'baz': {'dependencies': ['baz']},
+                        },
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+        builder.PLUGIN_NAME = 'foo'
+
+        with EnvVars({BuildEnvVars.HOOKS_ENABLE: 'true'}):
+            assert builder.config.dependencies == ['foo', 'bar', 'baz']
+
+    def test_hooks_env_var_specific_override_enable_by_default(self, isolation):
+        config = {
+            'tool': {
+                'hatch': {
+                    'build': {
+                        'hooks': {
+                            'foo': {'dependencies': ['foo'], 'enable-by-default': False},
+                            'bar': {'dependencies': ['bar'], 'enable-by-default': False},
+                            'baz': {'dependencies': ['baz']},
+                        },
+                    }
+                }
+            }
+        }
+        builder = BuilderInterface(str(isolation), config=config)
+        builder.PLUGIN_NAME = 'foo'
+
+        with EnvVars({f'{BuildEnvVars.HOOK_ENABLE_PREFIX}FOO': 'true'}):
+            assert builder.config.dependencies == ['foo', 'baz']
+
 
 class TestPatternDefaults:
     def test_include(self, isolation):
         builder = BuilderInterface(str(isolation))
 
         assert builder.config.default_include_patterns() == []
```

### Comparing `hatch-1rc5/tests/backend/builders/test_custom.py` & `hatch-1rc6/tests/backend/builders/test_custom.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/builders/test_sdist.py` & `hatch-1rc6/tests/backend/builders/test_sdist.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/builders/test_wheel.py` & `hatch-1rc6/tests/backend/builders/test_wheel.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/builders/hooks/test_custom.py` & `hatch-1rc6/tests/backend/builders/hooks/test_custom.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/builders/plugin/test_interface.py` & `hatch-1rc6/tests/backend/builders/plugin/test_interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/downstream/integrate.py` & `hatch-1rc6/tests/backend/downstream/integrate.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/downstream/datadogpy/pyproject.toml` & `hatch-1rc6/tests/backend/downstream/datadogpy/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/licenses/test_parse.py` & `hatch-1rc6/tests/backend/licenses/test_parse.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/licenses/test_supported.py` & `hatch-1rc6/tests/backend/licenses/test_supported.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/metadata/test_build.py` & `hatch-1rc6/tests/backend/metadata/test_build.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/metadata/test_core.py` & `hatch-1rc6/tests/backend/metadata/test_core.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/metadata/test_custom_hook.py` & `hatch-1rc6/tests/backend/metadata/test_custom_hook.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/metadata/test_hatch.py` & `hatch-1rc6/tests/backend/metadata/test_hatch.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/metadata/test_utils.py` & `hatch-1rc6/tests/backend/metadata/test_utils.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/backend/version/source/test_regex.py` & `hatch-1rc6/tests/backend/version/source/test_regex.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/test_root.py` & `hatch-1rc6/tests/cli/test_root.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/build/test_build.py` & `hatch-1rc6/tests/cli/build/test_build.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/clean/test_clean.py` & `hatch-1rc6/tests/cli/clean/test_clean.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/config/test_find.py` & `hatch-1rc6/tests/cli/config/test_find.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/config/test_restore.py` & `hatch-1rc6/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/config/test_set.py` & `hatch-1rc6/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/config/test_show.py` & `hatch-1rc6/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/dep/test_hash.py` & `hatch-1rc6/tests/cli/dep/test_hash.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/env/test_create.py` & `hatch-1rc6/tests/cli/env/test_create.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/env/test_prune.py` & `hatch-1rc6/tests/cli/env/test_prune.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/env/test_remove.py` & `hatch-1rc6/tests/cli/env/test_remove.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/env/test_show.py` & `hatch-1rc6/tests/cli/env/test_show.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/new/test_new.py` & `hatch-1rc6/tests/cli/new/test_new.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/publish/test_publish.py` & `hatch-1rc6/tests/cli/publish/test_publish.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/run/test_run.py` & `hatch-1rc6/tests/cli/run/test_run.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/status/test_status.py` & `hatch-1rc6/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/cli/version/test_version.py` & `hatch-1rc6/tests/cli/version/test_version.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/config/test_model.py` & `hatch-1rc6/tests/config/test_model.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/dep/test_core.py` & `hatch-1rc6/tests/dep/test_core.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/env/plugin/test_interface.py` & `hatch-1rc6/tests/env/plugin/test_interface.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/helpers.py` & `hatch-1rc6/tests/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/licenses/__init__.py` & `hatch-1rc6/tests/helpers/templates/licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/basic.py` & `hatch-1rc6/tests/helpers/templates/new/basic.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/default.py` & `hatch-1rc6/tests/helpers/templates/new/default.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/feature_ci.py` & `hatch-1rc6/tests/helpers/templates/new/feature_ci.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/feature_cli.py` & `hatch-1rc6/tests/helpers/templates/new/feature_cli.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/feature_src_layout.py` & `hatch-1rc6/tests/helpers/templates/new/feature_src_layout.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/licenses_empty.py` & `hatch-1rc6/tests/helpers/templates/new/licenses_empty.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/licenses_multiple.py` & `hatch-1rc6/tests/helpers/templates/new/licenses_multiple.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/projects_urls_empty.py` & `hatch-1rc6/tests/helpers/templates/new/projects_urls_empty.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/new/projects_urls_space_in_label.py` & `hatch-1rc6/tests/helpers/templates/new/projects_urls_space_in_label.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/sdist/standard_default.py` & `hatch-1rc6/tests/helpers/templates/sdist/standard_default.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/sdist/standard_default_build_script_artifacts.py` & `hatch-1rc6/tests/helpers/templates/sdist/standard_default_build_script_artifacts.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/sdist/standard_default_support_legacy.py` & `hatch-1rc6/tests/helpers/templates/sdist/standard_default_support_legacy.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/sdist/standard_include.py` & `hatch-1rc6/tests/helpers/templates/sdist/standard_include.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_default_build_script.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_default_build_script.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_default_build_script_artifacts.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_default_build_script_artifacts.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_default_build_script_artifacts_with_src_layout.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_default_build_script_artifacts_with_src_layout.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_default_license_multiple.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_default_license_multiple.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_default_license_single.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_default_license_single.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_default_python_constraint.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_default_python_constraint.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_editable_pth.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_editable_pth.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_editable_standard.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_editable_standard.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/standard_tests.py` & `hatch-1rc6/tests/helpers/templates/wheel/standard_tests.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/helpers/templates/wheel/utils.py` & `hatch-1rc6/tests/helpers/templates/wheel/utils.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/project/test_config.py` & `hatch-1rc6/tests/project/test_config.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/project/test_core.py` & `hatch-1rc6/tests/project/test_core.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/utils/test_fs.py` & `hatch-1rc6/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/utils/test_platform.py` & `hatch-1rc6/tests/utils/test_platform.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/utils/test_structures.py` & `hatch-1rc6/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/venv/test_core.py` & `hatch-1rc6/tests/venv/test_core.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/venv/test_utils.py` & `hatch-1rc6/tests/venv/test_utils.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/tests/version/scheme/test_standard.py` & `hatch-1rc6/tests/version/scheme/test_standard.py`

 * *Files identical despite different names*

### Comparing `hatch-1rc5/PKG-INFO` & `hatch-1rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch
-Version: 1rc5
+Version: 1rc6
 Summary: Modern, extensible Python project management
 Project-URL: Documentation, https://ofek.dev/hatch/latest/
 Project-URL: Donate, https://github.com/sponsors/ofek
 Project-URL: History, https://ofek.dev/hatch/dev/meta/history/
 Project-URL: Issues, https://github.com/ofek/hatch/issues
 Project-URL: Source, https://github.com/ofek/hatch
 Author-email: Ofek Lev <oss@ofek.dev>
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.8
 Requires-Dist: atomicwrites~=1.4
 Requires-Dist: click~=8.0.3
-Requires-Dist: hatchling>=0.5
+Requires-Dist: hatchling>=0.6
 Requires-Dist: httpx~=0.21
 Requires-Dist: keyring~=23.4
 Requires-Dist: pexpect~=4.8.0
 Requires-Dist: platformdirs~=2.4
 Requires-Dist: pyperclip~=1.8
 Requires-Dist: rich~=10.16
 Requires-Dist: tomli-w~=1.0
```

