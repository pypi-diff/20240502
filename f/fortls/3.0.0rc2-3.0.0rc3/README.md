# Comparing `tmp/fortls-3.0.0rc2.tar.gz` & `tmp/fortls-3.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortls-3.0.0rc2.tar", last modified: Tue Jan  2 15:04:52 2024, max compression
+gzip compressed data, was "fortls-3.0.0rc3.tar", last modified: Thu May  2 20:28:30 2024, max compression
```

## Comparing `fortls-3.0.0rc2.tar` & `fortls-3.0.0rc3.tar`

### file list

```diff
@@ -1,252 +1,257 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.545975 fortls-3.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.497975 fortls-3.0.0rc2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.497975 fortls-3.0.0rc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.501975 fortls-3.0.0rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.github/workflows/update-intrinsics.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    40759 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-01-02 15:04:52.545975 fortls-3.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.501975 fortls-3.0.0rc2/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.501975 fortls-3.0.0rc2/assets/animations/
--rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/animations/intro-demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/f.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/logo2-animated.svg
--rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/logos.workspace.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.513975 fortls-3.0.0rc2/assets/lsp/
--rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/completion-ani.gif
--rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/completion-ani.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/completion.png
--rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/definition-goto.gif
--rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/definition-goto.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/definition-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/diagnostics1.png
--rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/doc-highlight.png
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/hover.png
--rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/hover2.png
--rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/references-peek.png
--rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/rename.gif
--rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/rename.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/rename2.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/rename2.mp4
--rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/sig-help.gif
--rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/sig-help.mp4
--rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/symbols-crop.png
--rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/symbols-doc.png
--rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/symbols-workspace.png
--rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/lsp/symbols.png
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/assets/symbol-class.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.513975 fortls-3.0.0rc2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/contact.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/editor_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/features.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/fortls.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.517975 fortls-3.0.0rc2/docs/html_extra/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/html_extra/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/html_extra/google3e426562ce42e98f.html
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/html_extra/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/options.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/docs/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.517975 fortls-3.0.0rc2/fortls/
--rw-r--r--   0 runner    (1001) docker     (127)    20802 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/fortls.schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/ftypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    17249 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/json_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/jsonrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    73218 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/langserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.517975 fortls-3.0.0rc2/fortls/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.525975 fortls-3.0.0rc2/fortls/parsers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/do.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/if_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/intrinsic.modules.json
--rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/intrinsic.procedures.json
--rw-r--r--   0 runner    (1001) docker     (127)   630426 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/intrinsic.procedures.markdown.json
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/keywords.json
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/method.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    84763 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/statements.json
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/subroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/use.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/parsers/internal/where.py
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/fortls/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.541975 fortls-3.0.0rc2/fortls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12341 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6889 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-02 15:04:52.000000 fortls-3.0.0rc2/fortls.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.525975 fortls-3.0.0rc2/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/licenses/fortran-language-server-license.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-01-02 15:04:52.545975 fortls-3.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.529975 fortls-3.0.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/setup_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_preproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_regex_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25784 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_hover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_server_signature_help.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.529975 fortls-3.0.0rc2/test/test_source/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/.fortls
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.529975 fortls-3.0.0rc2/test/test_source/completion/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/completion/test_vis_mod_completion.f90
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/completion/use_only_interface.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.533975 fortls-3.0.0rc2/test/test_source/diag/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/conf_long_lines.json
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_contains.f90
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_critical.f90
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_enum.f90
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_external.f90
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_forall.f90
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_function.f90
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_function_arg_list.f90
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_implicit_none.f90
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_lines.f90
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_scope_end_name_var.f90
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_scope_overreach.f90
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_semicolon.f90
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_use_ordering.f90
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_var_shadowing_keyword_arg.f90
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_variable.f90
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_visibility.f90
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/diag/test_where.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.533975 fortls-3.0.0rc2/test/test_source/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/docs/test_doxygen.f90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/docs/test_ford.f90
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/docs/test_module_and_type_doc.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.493975 fortls-3.0.0rc2/test/test_source/excldir/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.533975 fortls-3.0.0rc2/test/test_source/excldir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/excldir/sub1/tmp.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.533975 fortls-3.0.0rc2/test/test_source/excldir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/excldir/sub2/fake2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/f90_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/hover/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/associate_block.f90
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/associate_block_2.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/functions.f90
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/intent.f90
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/parameters.f90
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/pointers.f90
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/recursive.f90
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/spaced_keywords.f90
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/hover/types.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/imp/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/imp/import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/imp/submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/include/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/include/empty.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/parse/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/parse/line_continuations.f90
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/parse/submodule.f90
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/parse/test_incomplete_dims.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/parse/test_kinds_and_dims.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/pp/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/.fortls
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/.pp_conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/pp/include/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/include/petscerror.h
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/include/petscpc.h
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc.F90
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc_elif.F90
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc_elif_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc_if_elif_else.F90
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc_if_elif_skip.F90
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/pp/preproc_keywords.F90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.537975 fortls-3.0.0rc2/test/test_source/rename/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/rename/test_rename_imp_type_bound_proc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/rename/test_rename_intrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/rename/test_rename_nested.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.541975 fortls-3.0.0rc2/test/test_source/signature/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/signature/help.f90
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/signature/nested_sigs.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.541975 fortls-3.0.0rc2/test/test_source/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_abstract.f90
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_fixed.f
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_free.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_generic.f90
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_inc2.f90
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_inherit.f90
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_rename.F90
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_select.f90
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_submod.F90
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/subdir/test_vis.f90
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test.f90
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_block.f08
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_diagnostic_int.f90
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_import.f90
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_inc.f90
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_nonintrinsic.f90
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_prog.f08
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/test_submodule.f90
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:04:52.541975 fortls-3.0.0rc2/test/test_source/use/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/use/use.f90
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-02 15:04:34.000000 fortls-3.0.0rc2/test/test_source/wrong_syntax.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.955270 fortls-3.0.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.907270 fortls-3.0.0rc3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.907270 fortls-3.0.0rc3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.907270 fortls-3.0.0rc3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/workflows/docs_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.github/workflows/update-intrinsics.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    41274 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-02 20:28:30.955270 fortls-3.0.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.911270 fortls-3.0.0rc3/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.911270 fortls-3.0.0rc3/assets/animations/
+-rw-r--r--   0 runner    (1001) docker     (127)  1647490 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/animations/intro-demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/f.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11737 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/logo2-animated.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    78094 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/logos.workspace.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.923270 fortls-3.0.0rc3/assets/lsp/
+-rw-r--r--   0 runner    (1001) docker     (127)   791746 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/completion-ani.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   450880 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/completion-ani.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    36257 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/completion.png
+-rw-r--r--   0 runner    (1001) docker     (127)   597393 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/definition-goto.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   335329 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/definition-goto.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/definition-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49007 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/diagnostics1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43464 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/doc-highlight.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/hover.png
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/hover2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65080 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/references-peek.png
+-rw-r--r--   0 runner    (1001) docker     (127)   703611 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/rename.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   355841 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/rename.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   304764 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/rename2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   151579 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/rename2.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)   628798 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/sig-help.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   418094 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/sig-help.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)    50499 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/symbols-crop.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8288 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/symbols-doc.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25726 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/symbols-workspace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    54934 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/lsp/symbols.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/assets/symbol-class.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.927270 fortls-3.0.0rc3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7767 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/editor_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/fortls.parsers.internal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/fortls.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/fortls.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.927270 fortls-3.0.0rc3/docs/html_extra/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/html_extra/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/html_extra/google3e426562ce42e98f.html
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/html_extra/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/docs/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.927270 fortls-3.0.0rc3/fortls/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18046 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/fortls.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/ftypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/json_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/jsonrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74006 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/langserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.931270 fortls-3.0.0rc3/fortls/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.935270 fortls-3.0.0rc3/fortls/parsers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/do.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/if_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72890 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/intrinsic.modules.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44156 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/intrinsic.procedures.json
+-rw-r--r--   0 runner    (1001) docker     (127)   630306 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/intrinsic.procedures.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/keywords.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86130 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9597 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/statements.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/subroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6532 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/use.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/parsers/internal/where.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/fortls/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/fortls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 20:28:30.000000 fortls-3.0.0rc3/fortls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.935270 fortls-3.0.0rc3/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/licenses/fortran-language-server-license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-02 20:28:30.955270 fortls-3.0.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.939270 fortls-3.0.0rc3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/setup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_preproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_preproc_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_regex_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7451 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26297 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_hover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7861 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_server_signature_help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.943270 fortls-3.0.0rc3/test/test_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/.fortls
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.943270 fortls-3.0.0rc3/test/test_source/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/completion/test_vis_mod_completion.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/completion/use_only_interface.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.943270 fortls-3.0.0rc3/test/test_source/diag/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/conf_long_lines.json
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_contains.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_critical.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_enum.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_external.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_forall.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_function.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_function_arg_list.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_implicit_none.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_lines.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_scope_end_name_var.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_scope_overreach.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_semicolon.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_use_ordering.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_var_shadowing_keyword_arg.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_variable.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_visibility.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/diag/test_where.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/docs/test_doxygen.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/docs/test_ford.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/docs/test_module_and_type_doc.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.903270 fortls-3.0.0rc3/test/test_source/excldir/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/excldir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/excldir/sub1/tmp.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/excldir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/excldir/sub2/fake2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/f90_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/hover/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/associate_block.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/associate_block_2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/functions.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/intent.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/parameters.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/pointers.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/recursive.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/spaced_keywords.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/hover/types.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/imp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/imp/import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/imp/submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/include/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/include/empty.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.947270 fortls-3.0.0rc3/test/test_source/parse/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/parse/line_continuations.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/parse/submodule.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/parse/test_incomplete_dims.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/parse/test_kinds_and_dims.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/test/test_source/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/.fortls
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/.pp_conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/test/test_source/pp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/include/petscerror.h
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/include/petscpc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc_elif.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc_elif_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc_if_elif_else.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc_if_elif_skip.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/pp/preproc_keywords.F90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/test/test_source/rename/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/rename/test_rename_imp_type_bound_proc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/rename/test_rename_intrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/rename/test_rename_nested.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/test/test_source/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/signature/help.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/signature/nested_sigs.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/test/test_source/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_abstract.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_fixed.f
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_free.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_generic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_inc2.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_inherit.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_rename.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_select.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_submod.F90
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/subdir/test_vis.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_block.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_diagnostic_int.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_import.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_inc.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_nonintrinsic.f90
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_prog.f08
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/test_submodule.f90
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:28:30.951270 fortls-3.0.0rc3/test/test_source/use/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/use/use.f90
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 20:28:18.000000 fortls-3.0.0rc3/test/test_source/wrong_syntax.json
```

### Comparing `fortls-3.0.0rc2/.github/FUNDING.yml` & `fortls-3.0.0rc3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/.github/ISSUE_TEMPLATE/bug_report.md` & `fortls-3.0.0rc3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/.github/ISSUE_TEMPLATE/feature_request.md` & `fortls-3.0.0rc3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/.github/workflows/codeql-analysis.yml` & `fortls-3.0.0rc3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/.github/workflows/main.yml` & `fortls-3.0.0rc3/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -52,11 +52,13 @@
       - name: Coverage report
         run: |
           pip install .[dev]
           pytest --doctest-modules
         shell: bash
 
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
-          token: ${{ secrets.CODECOV_TOKEN }}
           fail_ci_if_error: true
+          verbose: true
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `fortls-3.0.0rc2/.github/workflows/python-publish.yml` & `fortls-3.0.0rc3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/.github/workflows/update-intrinsics.yml` & `fortls-3.0.0rc3/.github/workflows/update-intrinsics.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
       - name: Download M_intrinsics
         run: |
           git clone https://github.com/urbanjost/M_intrinsics
 
       - name: Update Markdown intrinsics
         run: |
-          python3 -m fortls.intrinsics
+          python3 -m fortls.parsers.internal.intrinsics
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@v5
+        uses: peter-evans/create-pull-request@v6
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           commit-message: "docs: update M_intrinsics"
           title: Update M_intrinsics
           body: |
             Auto-generated Pull Request to update M_intrinsics JSON definitions.
           branch: docs/update-intrinsics
```

### Comparing `fortls-3.0.0rc2/.pre-commit-config.yaml` & `fortls-3.0.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/CHANGELOG.md` & `fortls-3.0.0rc3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # CHANGELOG
 
 ## Unreleased
 
-## 2.14.0
+## 3.0.0
 
 ### Added
 
+- Added support for changing the default Python recursion depth
+  ([#312](https://github.com/fortran-lang/fortls/issues/312))
+- Added support for preprocessor macro expansions
+  ([#368](https://github.com/fortran-lang/fortls/pull/368))
+- Added support for leading white spaces in preprocessor directives
+  ([#297](https://github.com/fortran-lang/fortls/issues/297))
 - Added hover messages for Types and Modules
   ([#208](https://github.com/fortran-lang/fortls/issues/208))
 - Added support for Markdown intrinsics from the M_intrinsics repository
   ([#215](https://github.com/fortran-lang/fortls/issues/215))
 - Added and create a schema for fortls configuration files
   ([#204](https://github.com/fortran-lang/fortls/issues/204))
 - Added dependabot alers for PyPi
@@ -22,14 +28,17 @@
   provided in the option, without performing any type of modification.
   ([#300](https://github.com/fortran-lang/fortls/issues/300))
 - Changed the completion signature to include the full Markdown documentation
   for the completion item.
   ([#219](https://github.com/fortran-lang/fortls/issues/219))
 - Changed hover messages and signature help to use Markdown
   ([#45](https://github.com/fortran-lang/fortls/issues/45))
+- Changed automatic detection of fixed/free-form of files to ignore
+  preprocessor lines.
+  ([#302](https://github.com/fortran-lang/fortls/pull/302))
 
 ### Fixed
 
 - Fixed preprocessor bug with `if` and `elif` conditionals
   ([#322](https://github.com/fortran-lang/fortls/issues/322))
 - Fixed bug where type fields or methods were not detected if spaces were
   used around `%`
```

### Comparing `fortls-3.0.0rc2/CODE_OF_CONDUCT.md` & `fortls-3.0.0rc3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/CONTRIBUTING.md` & `fortls-3.0.0rc3/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ### Dependencies
 
 To build this project you will need [Python](https://www.python.org/) `>= 3.7` and [pip](https://www.python.org/) `>= 21.0`.
 To install all Python dependencies open a terminal go into the `fortls` cloned folder and run:
 
 ```sh
-pip install -e .[dev,docs]
+pip install -e ".[dev,docs]"
 ```
 
 ### Testing 🧪
 
 To verify that your cloning of the GitHub repository worked as expected open a terminal and run:
 
 ```sh
```

### Comparing `fortls-3.0.0rc2/LICENSE` & `fortls-3.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/PKG-INFO` & `fortls-3.0.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: fortls - Fortran Language Server
 Home-page: https://fortls.fortran-lang.org
 Author: Giannis Nikiteas
 Author-email: giannis.nikiteas@gmail.com
 License: MIT
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
@@ -38,29 +38,30 @@
 Provides-Extra: dev
 Requires-Dist: pytest>=7.2.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=3.0.2; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pydantic==1.10.13; extra == "dev"
+Requires-Dist: pydantic; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=4.0.0; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx_design; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-sitemap; extra == "docs"
 
 ![alt](https://raw.githubusercontent.com/fortran-lang/fortls/master/assets/logo.png)
 
 # fortls - Fortran Language Server
 
+[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat-square&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
 ![PyPI](https://img.shields.io/pypi/v/fortls?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fortls?style=flat-square)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fortls?style=flat-square&label=PyPi)](https://pepy.tech/project/fortls)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/fortls?label=Anaconda&style=flat-square)
 ![GitHub License](https://img.shields.io/github/license/fortran-lang/fortls?style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/main.yml?branch=master&label=CI&style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/docs.yml?branch=master&label=Docs&style=flat-square)
@@ -115,28 +116,14 @@
   - Generate type-bound procedures and implementation templates for
     deferred procedures
 
 ### Notes/Limitations
 
 - Signature help and hover does not handle elegantly overloaded functions i.e. interfaces
 
-## `fortls` vs `fortran-language-server`
-
-This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
-
-`fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
-the original `fortran-language-server` does not.
-
-For a complete and detailed list of the differences between the two Language Servers
-see the Documentation section: [Unique fortls features (not in fortran-language-server)](https://fortls.fortran-lang.org/fortls_changes.html)
-
-The name of executable for this project has been chosen to remain `fortls`
-to allow for integration with pre-existing plugins and workflows, but it could
-change in the future.
-
 ## Future plans
 
 `fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
 It does however still have fundamental limitations,
 namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
 
 We are excited to announce that we are working on creating a new Fortran Language Server
@@ -226,14 +213,28 @@
 | `textDocument/rename`            | Rename a symbol across the workspace                   |
 | `textDocument/didOpen`           | Document synchronisation upon opening                  |
 | `textDocument/didSave`           | Document synchronisation upon saving                   |
 | `textDocument/didClose`          | Document synchronisation upon closing                  |
 | `textDocument/didChange`         | Document synchronisation upon changes to the document  |
 | `textDocument/codeAction`        | **Experimental** Generate code                         |
 
+## `fortls` vs `fortran-language-server`
+
+This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
+
+`fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
+the original `fortran-language-server` does not.
+
+For a complete and detailed list of the differences between the two Language Servers
+see the Documentation section: [Unique fortls features (not in fortran-language-server)](https://fortls.fortran-lang.org/fortls_changes.html)
+
+The name of executable for this project has been chosen to remain `fortls`
+to allow for integration with pre-existing plugins and workflows, but it could
+change in the future.
+
 ## Acknowledgements
 
 This project would not have been possible without the original work of [@hansec](https://github.com/hansec/)
 in [`fortran-language-server`](https://github.com/hansec/fortran-language-server)
 
 <!-- ## Support
```

### Comparing `fortls-3.0.0rc2/README.md` & `fortls-3.0.0rc3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ![alt](https://raw.githubusercontent.com/fortran-lang/fortls/master/assets/logo.png)
 
 # fortls - Fortran Language Server
 
+[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat-square&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
 ![PyPI](https://img.shields.io/pypi/v/fortls?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fortls?style=flat-square)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fortls?style=flat-square&label=PyPi)](https://pepy.tech/project/fortls)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/fortls?label=Anaconda&style=flat-square)
 ![GitHub License](https://img.shields.io/github/license/fortran-lang/fortls?style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/main.yml?branch=master&label=CI&style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/docs.yml?branch=master&label=Docs&style=flat-square)
@@ -60,28 +61,14 @@
   - Generate type-bound procedures and implementation templates for
     deferred procedures
 
 ### Notes/Limitations
 
 - Signature help and hover does not handle elegantly overloaded functions i.e. interfaces
 
-## `fortls` vs `fortran-language-server`
-
-This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
-
-`fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
-the original `fortran-language-server` does not.
-
-For a complete and detailed list of the differences between the two Language Servers
-see the Documentation section: [Unique fortls features (not in fortran-language-server)](https://fortls.fortran-lang.org/fortls_changes.html)
-
-The name of executable for this project has been chosen to remain `fortls`
-to allow for integration with pre-existing plugins and workflows, but it could
-change in the future.
-
 ## Future plans
 
 `fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
 It does however still have fundamental limitations,
 namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
 
 We are excited to announce that we are working on creating a new Fortran Language Server
@@ -171,14 +158,28 @@
 | `textDocument/rename`            | Rename a symbol across the workspace                   |
 | `textDocument/didOpen`           | Document synchronisation upon opening                  |
 | `textDocument/didSave`           | Document synchronisation upon saving                   |
 | `textDocument/didClose`          | Document synchronisation upon closing                  |
 | `textDocument/didChange`         | Document synchronisation upon changes to the document  |
 | `textDocument/codeAction`        | **Experimental** Generate code                         |
 
+## `fortls` vs `fortran-language-server`
+
+This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
+
+`fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
+the original `fortran-language-server` does not.
+
+For a complete and detailed list of the differences between the two Language Servers
+see the Documentation section: [Unique fortls features (not in fortran-language-server)](https://fortls.fortran-lang.org/fortls_changes.html)
+
+The name of executable for this project has been chosen to remain `fortls`
+to allow for integration with pre-existing plugins and workflows, but it could
+change in the future.
+
 ## Acknowledgements
 
 This project would not have been possible without the original work of [@hansec](https://github.com/hansec/)
 in [`fortran-language-server`](https://github.com/hansec/fortran-language-server)
 
 <!-- ## Support
```

### Comparing `fortls-3.0.0rc2/SECURITY.md` & `fortls-3.0.0rc3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/LICENSE` & `fortls-3.0.0rc3/assets/LICENSE`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/README.md` & `fortls-3.0.0rc3/assets/README.md`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/animations/intro-demo.gif` & `fortls-3.0.0rc3/assets/animations/intro-demo.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/f.svg` & `fortls-3.0.0rc3/assets/f.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/icon.svg` & `fortls-3.0.0rc3/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/logo.png` & `fortls-3.0.0rc3/assets/logo.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/logo.svg` & `fortls-3.0.0rc3/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/logo2-animated.svg` & `fortls-3.0.0rc3/assets/logo2-animated.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/logos.workspace.svg` & `fortls-3.0.0rc3/assets/logos.workspace.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/completion-ani.gif` & `fortls-3.0.0rc3/assets/lsp/completion-ani.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/completion-ani.mp4` & `fortls-3.0.0rc3/assets/lsp/completion-ani.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/completion.png` & `fortls-3.0.0rc3/assets/lsp/completion.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/definition-goto.gif` & `fortls-3.0.0rc3/assets/lsp/definition-goto.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/definition-goto.mp4` & `fortls-3.0.0rc3/assets/lsp/definition-goto.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/definition-peek.png` & `fortls-3.0.0rc3/assets/lsp/definition-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/diagnostics1.png` & `fortls-3.0.0rc3/assets/lsp/diagnostics1.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/doc-highlight.png` & `fortls-3.0.0rc3/assets/lsp/doc-highlight.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/hover.png` & `fortls-3.0.0rc3/assets/lsp/hover.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/hover2.png` & `fortls-3.0.0rc3/assets/lsp/hover2.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/references-peek.png` & `fortls-3.0.0rc3/assets/lsp/references-peek.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/rename.gif` & `fortls-3.0.0rc3/assets/lsp/rename.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/rename.mp4` & `fortls-3.0.0rc3/assets/lsp/rename.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/rename2.gif` & `fortls-3.0.0rc3/assets/lsp/rename2.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/rename2.mp4` & `fortls-3.0.0rc3/assets/lsp/rename2.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/sig-help.gif` & `fortls-3.0.0rc3/assets/lsp/sig-help.gif`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/sig-help.mp4` & `fortls-3.0.0rc3/assets/lsp/sig-help.mp4`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/symbols-crop.png` & `fortls-3.0.0rc3/assets/lsp/symbols-crop.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/symbols-doc.png` & `fortls-3.0.0rc3/assets/lsp/symbols-doc.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/symbols-workspace.png` & `fortls-3.0.0rc3/assets/lsp/symbols-workspace.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/lsp/symbols.png` & `fortls-3.0.0rc3/assets/lsp/symbols.png`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/assets/symbol-class.svg` & `fortls-3.0.0rc3/assets/symbol-class.svg`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/Makefile` & `fortls-3.0.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/conf.py` & `fortls-3.0.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/contact.rst` & `fortls-3.0.0rc3/docs/contact.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/contributing.rst` & `fortls-3.0.0rc3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/editor_integration.rst` & `fortls-3.0.0rc3/docs/editor_integration.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/features.rst` & `fortls-3.0.0rc3/docs/features.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/fortls.rst` & `fortls-3.0.0rc3/docs/fortls.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 fortls package
 ==============
 
+Subpackages
+-----------
+
+.. toctree::
+   :maxdepth: 4
+
+   fortls.parsers
+
 Submodules
 ----------
 
 fortls.constants module
 -----------------------
 
 .. automodule:: fortls.constants
    :members:
    :undoc-members:
    :show-inheritance:
 
+fortls.debug module
+-------------------
+
+.. automodule:: fortls.debug
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 fortls.ftypes module
 --------------------
 
 .. automodule:: fortls.ftypes
    :members:
    :undoc-members:
    :show-inheritance:
@@ -32,22 +48,14 @@
 -----------------------
 
 .. automodule:: fortls.interface
    :members:
    :undoc-members:
    :show-inheritance:
 
-fortls.intrinsics module
-------------------------
-
-.. automodule:: fortls.intrinsics
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 fortls.json\_templates module
 -----------------------------
 
 .. automodule:: fortls.json_templates
    :members:
    :undoc-members:
    :show-inheritance:
@@ -64,34 +72,26 @@
 ------------------------
 
 .. automodule:: fortls.langserver
    :members:
    :undoc-members:
    :show-inheritance:
 
-fortls.objects module
----------------------
-
-.. automodule:: fortls.objects
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
-fortls.parse\_fortran module
-----------------------------
+fortls.regex\_patterns module
+-----------------------------
 
-.. automodule:: fortls.parse_fortran
+.. automodule:: fortls.regex_patterns
    :members:
    :undoc-members:
    :show-inheritance:
 
-fortls.regex\_patterns module
------------------------------
+fortls.schema module
+--------------------
 
-.. automodule:: fortls.regex_patterns
+.. automodule:: fortls.schema
    :members:
    :undoc-members:
    :show-inheritance:
 
 fortls.version module
 ---------------------
```

### Comparing `fortls-3.0.0rc2/docs/index.rst` & `fortls-3.0.0rc3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/make.bat` & `fortls-3.0.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/docs/options.rst` & `fortls-3.0.0rc3/docs/options.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 .. code-block:: json
 
    {
       "nthreads": 4,
       "notify_init": false,
       "incremental_sync": false,
+      "recursion_limit": 1000,
       "sort_keywords": false,
       "disable_autoupdate": false,
       "debug_log": false,
 
       "source_dirs": ["./**"],
       "incl_suffixes": [],
       "excl_suffixes": [],
```

### Comparing `fortls-3.0.0rc2/docs/quickstart.rst` & `fortls-3.0.0rc3/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/constants.py` & `fortls-3.0.0rc3/fortls/constants.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/fortls.schema.json` & `fortls-3.0.0rc3/fortls/fortls.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9956896551724138%*

 * *Differences: {"'properties'": "{'recursion_limit': OrderedDict([('default', 1000), ('description', 'Set the "*

 * *                 "maximum recursion depth for the parser (default: 1000)'), ('title', 'Recursion "*

 * *                 "Limit'), ('type', 'integer')])}"}*

```diff
@@ -145,14 +145,20 @@
         },
         "preserve_keyword_order": {
             "default": false,
             "description": "DEPRECATED, this is now the default. To sort use sort_keywords",
             "title": "Preserve Keyword Order",
             "type": "boolean"
         },
+        "recursion_limit": {
+            "default": 1000,
+            "description": "Set the maximum recursion depth for the parser (default: 1000)",
+            "title": "Recursion Limit",
+            "type": "integer"
+        },
         "sort_keywords": {
             "default": false,
             "description": "Display variable keywords information, function/subroutine definitions, etc. in a consistent (sorted) manner default: no sorting, display code as is)",
             "title": "Sort Keywords",
             "type": "boolean"
         },
         "source_dirs": {
```

### Comparing `fortls-3.0.0rc2/fortls/ftypes.py` & `fortls-3.0.0rc3/fortls/ftypes.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/helper_functions.py` & `fortls-3.0.0rc3/fortls/helper_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,16 +64,39 @@
 
     >>> detect_fixed_format(['C Fixed format'])
     True
 
     Lines wih ampersands are not fixed format
     >>> detect_fixed_format(['trailing line & ! comment'])
     False
+
+    But preprocessor lines will be ignored
+    >>> detect_fixed_format(
+    ...     ['#if defined(A) && !defined(B)', 'C Fixed format', '#endif'])
+    True
+
+    >>> detect_fixed_format(
+    ...     ['#if defined(A) && !defined(B)', ' free format', '#endif'])
+    False
+
+    And preprocessor line-continuation is taken into account
+    >>> detect_fixed_format(
+    ...     ['#if defined(A) \\\\ ', ' && !defined(B)', 'C Fixed format', '#endif'])
+    True
+
+    >>> detect_fixed_format(
+    ...     ['#if defined(A) \\\\', '&& \\\\', '!defined(B)', ' free format', '#endif'])
+    False
     """
+    pp_continue = False
     for line in file_lines:
+        # Ignore preprocessor lines
+        if line.startswith("#") or pp_continue:
+            pp_continue = line.rstrip().endswith("\\")
+            continue
         if FRegex.FREE_FORMAT_TEST.match(line):
             return False
         tmp_match = FRegex.VAR.match(line)
         if tmp_match and tmp_match.start(1) < 6:
             return False
         # Trailing ampersand indicates free or intersection format
         if not FRegex.FIXED_COMMENT.match(line):
```

### Comparing `fortls-3.0.0rc2/fortls/interface.py` & `fortls-3.0.0rc3/fortls/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,21 @@
     )
     parser.add_argument(
         "--incremental_sync",
         action="store_true",
         help="Use incremental document synchronization (beta)",
     )
     parser.add_argument(
+        "--recursion_limit",
+        type=int,
+        default=1000,
+        metavar="INTEGER",
+        help="Set the maximum recursion depth for the parser (default: %(default)s)",
+    )
+    parser.add_argument(
         "--sort_keywords",
         action="store_true",
         help=(
             "Display variable keywords information, function/subroutine definitions,"
             " etc. in a consistent (sorted) manner default: no sorting, display code"
             " as is)"
         ),
```

### Comparing `fortls-3.0.0rc2/fortls/json_templates.py` & `fortls-3.0.0rc3/fortls/json_templates.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/jsonrpc.py` & `fortls-3.0.0rc3/fortls/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/langserver.py` & `fortls-3.0.0rc3/fortls/langserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,27 +194,28 @@
         params: dict = request["params"]
         self.root_path = path_from_uri(
             params.get("rootUri") or params.get("rootPath") or ""
         )
         self.source_dirs.add(self.root_path)
 
         self._load_config_file()
+        update_recursion_limit(self.recursion_limit)
         self._resolve_globs_in_paths()
         self._config_logger(request)
         self._load_intrinsics()
         self._add_source_dirs()
         if self._update_version_pypi():
             self.post_message(
                 "Please restart the server for the new version to activate",
                 Severity.info,
             )
 
         # Initialize workspace
         self.workspace_init()
-        log.info(f"fortls - Fortran Language Server {__version__} Initialized")
+        log.info("fortls - Fortran Language Server %s Initialized", __version__)
         #
         server_capabilities = {
             "completionProvider": {
                 "resolveProvider": False,
                 "triggerCharacters": ["%"],
             },
             "definitionProvider": True,
@@ -747,19 +748,26 @@
             def_name = expand_name(curr_line, def_char)
         except (TypeError, AttributeError):
             return None
         if def_name == "":
             return None
         # Search in Preprocessor defined variables
         if def_name in def_file.pp_defs:
+            def_value = def_file.pp_defs.get(def_name)
+            def_arg_str = ""
+            if isinstance(def_value, tuple):
+                def_arg_str, def_value = def_value
+                def_arg_str = ", ".join([x.strip() for x in def_arg_str.split(",")])
+                def_arg_str = f"({def_arg_str})"
+
             var = Variable(
                 def_file.ast,
                 def_line + 1,
                 def_name,
-                f"#define {def_name} {def_file.pp_defs.get(def_name)}",
+                f"#define {def_name}{def_arg_str} {def_value}",
                 [],
             )
             return var
         curr_scope = def_file.ast.get_inner_scope(def_line + 1)
         # Traverse type tree if necessary
         if is_member:
             type_scope = climb_type_tree(var_stack, curr_scope, self.obj_tree)
@@ -1380,15 +1388,15 @@
                             file_obj.ast = FortranAST(file_obj)
                             self.workspace[filepath] = file_obj
                             return False, None
                         else:
                             return False, "File does not exist"  # Error during load
                 err_string, file_changed = file_obj.load_from_disk()
                 if err_string:
-                    log.error(f"{err_string} : {filepath}")
+                    log.error("%s : %s", err_string, filepath)
                     return False, err_string  # Error during file read
                 if not file_changed:
                     return False, None
             ast_new = file_obj.parse(
                 pp_defs=self.pp_defs, include_dirs=self.include_dirs
             )
             # Add the included read in pp_defs from to the ones specified in the
@@ -1582,14 +1590,15 @@
         # General options ------------------------------------------------------
         self.nthreads = config_dict.get("nthreads", self.nthreads)
         self.notify_init = config_dict.get("notify_init", self.notify_init)
         self.incremental_sync = config_dict.get(
             "incremental_sync", self.incremental_sync
         )
         self.sync_type: int = 2 if self.incremental_sync else 1
+        self.recursion_limit = config_dict.get("recursion_limit", self.recursion_limit)
         self.sort_keywords = config_dict.get("sort_keywords", self.sort_keywords)
         self.disable_autoupdate = config_dict.get(
             "disable_autoupdate", self.disable_autoupdate
         )
 
         # Autocomplete options -------------------------------------------------
         self.autocomplete_no_prefix = config_dict.get(
@@ -1815,12 +1824,28 @@
                     return True
         # No internet connection exceptions
         except (URLError, KeyError):
             self.post_message("Failed to update the fortls", Severity.warn)
         return False
 
 
+def update_recursion_limit(limit: int) -> None:
+    """Update the recursion limit of the Python interpreter
+
+    Parameters
+    ----------
+    limit : int
+        New recursion limit
+
+    Examples
+    --------
+    >>> update_recursion_limit(10000)
+    """
+    if limit != sys.getrecursionlimit():
+        sys.setrecursionlimit(limit)
+
+
 class JSONRPC2Error(Exception):
     def __init__(self, code, message, data=None):
         self.code = code
         self.message = message
         self.data = data
```

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/associate.py` & `fortls-3.0.0rc3/fortls/parsers/internal/associate.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/ast.py` & `fortls-3.0.0rc3/fortls/parsers/internal/ast.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/base.py` & `fortls-3.0.0rc3/fortls/parsers/internal/base.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/block.py` & `fortls-3.0.0rc3/fortls/parsers/internal/block.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/diagnostics.py` & `fortls-3.0.0rc3/fortls/parsers/internal/diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/function.py` & `fortls-3.0.0rc3/fortls/parsers/internal/function.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/imports.py` & `fortls-3.0.0rc3/fortls/parsers/internal/imports.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/interface.py` & `fortls-3.0.0rc3/fortls/parsers/internal/interface.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/intrinsic.modules.json` & `fortls-3.0.0rc3/fortls/parsers/internal/intrinsic.modules.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/intrinsic.procedures.json` & `fortls-3.0.0rc3/fortls/parsers/internal/intrinsic.procedures.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/intrinsic.procedures.markdown.json` & `fortls-3.0.0rc3/fortls/parsers/internal/intrinsic.procedures.markdown.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9825%*

 * *Differences: {"'ACOSH'": '"## acosh\\n\\n### **Name**\\n\\n**acosh** - \\\\[MATHEMATICS:TRIGONOMETRIC\\\\] '*

 * *            'Inverse hyperbolic cosine function\\n\\n### **Synopsis**\\n```fortran\\n    result = '*

 * *            'acosh(x)\\n```\\n```fortran\\n     elemental TYPE(kind=KIND) function '*

 * *            'acosh(x)\\n\\n      TYPE(kind=KIND),intent(in) :: x\\n```\\n### '*

 * *            '**Characteristics**\\n\\n - **TYPE** may be _real_ or _complex_\\n - **KIND** may be '*

 * *            'any kind supported by the associated ty […]*

```diff
@@ -1,12 +1,12 @@
 {
     "ABS": "## abs\n\n### **Name**\n\n**abs** - \\[NUMERIC\\] Absolute value\n\n### **Synopsis**\n```fortran\n    result = abs(a)\n```\n```fortran\n     elemental TYPE(kind=KIND) function abs(a)\n\n      TYPE(kind=KIND),intent(in) :: a\n```\n### **Characteristics**\n\n- **a** may be any _real_, _integer_, or _complex_ value.\n\n- If **a** is _complex_ the returned value will be a _real_ with the\n  same kind as **a**.\n\n  Otherwise the returned type and kind is the same as for **a**.\n\n### **Description**\n\n   **abs** computes the absolute value of numeric argument **a**.\n\n   In mathematics, the absolute value or modulus of a real number **x**,\n   denoted **|x|**, is the magnitude of **x** without regard to its sign.\n\n   The absolute value of a number may be thought of as its distance from\n   zero. So for a complex value the absolute value is a real number\n   with magnitude **sqrt(x%re\\*\\*2,x%im\\*\\*2)**, as if the real component\n   is the x value and the imaginary value is the y value for the point\n   \\<x,y\\>.\n\n### **Options**\n\n- **a**\n  : The value to compute the absolute value of.\n\n### **Result**\n\n   If **a** is of type _integer_ or _real_, the value of the result\n   is the absolute value **|a|** and of the same type and kind as the\n   input argument.\n\n   If **a** is _complex_ with value **(x, y)**, the result is a _real_\n   equal to a processor-dependent approximation to\n```fortran\n        sqrt(x**2 + y**2)\n```\n   computed without undue overflow or underflow (that means the\n   computation of the result can overflow the allowed magnitude of the\n   real value returned, and that very small values can produce underflows\n   if they are squared while calculating the returned value, for example).\n\n   That is, if you think of non-complex values as being complex values\n   on the x-axis and complex values as being x-y points <x%re,x%im>\n   the result of **abs** is the (positive) magnitude of the distance\n   of the value from the origin.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_abs\nimplicit none\ninteger,parameter :: dp=kind(0.0d0)\n\ninteger           :: i = -1\nreal              :: x = -1.0\ncomplex           :: z = (-3.0,-4.0)\ndoubleprecision   :: rr = -45.78_dp\n\ncharacter(len=*),parameter :: &\n   ! some formats\n   frmt  =  '(1x,a15,1x,\" In: \",g0,            T51,\" Out: \",g0)', &\n   frmtc = '(1x,a15,1x,\" In: (\",g0,\",\",g0,\")\",T51,\" Out: \",g0)',  &\n   g     = '(*(g0,1x))'\n\n  ! basic usage\n    ! any integer, real, or complex type\n    write(*, frmt)  'integer         ',  i, abs(i)\n    write(*, frmt)  'real            ',  x, abs(x)\n    write(*, frmt)  'doubleprecision ', rr, abs(rr)\n    write(*, frmtc) 'complex         ',  z, abs(z)\n\n  ! You can take the absolute value of any value whose positive value\n  ! is representable with the same type and kind.\n    write(*, *) 'abs range test : ', abs(huge(0)), abs(-huge(0))\n    write(*, *) 'abs range test : ', abs(huge(0.0)), abs(-huge(0.0))\n    write(*, *) 'abs range test : ', abs(tiny(0.0)), abs(-tiny(0.0))\n    ! A dusty corner is that abs(-huge(0)-1) of an integer would be\n    ! a representable negative value on most machines but result in a\n    ! positive value out of range.\n\n  ! elemental\n    write(*, g) ' abs is elemental:', abs([20,  0,  -1,  -3,  100])\n\n  ! COMPLEX input produces REAL output\n    write(*, g)' complex input produces real output', &\n    & abs(cmplx(30.0_dp,40.0_dp,kind=dp))\n    ! dusty corner: \"kind=dp\" is required or the value returned by\n    ! CMPLX() is a default real instead of double precision\n\n  ! the returned value for complex input can be thought of as the\n  ! distance from the origin <0,0>\n    write(*, g) ' distance of (', z, ') from zero is', abs( z )\n    write(*, g) ' so beware of overflow with complex values'\n    !write(*, g) abs(cmplx( huge(0.0), huge(0.0) ))\n    write(*, g) ' because the biggest default real is',huge(0.0)\n\nend program demo_abs\n```\nResults:\n```text\n    integer          In: -1                     Out: 1\n    real             In: -1.000000              Out: 1.000000\n    doubleprecision  In: -45.78000000000000     Out: 45.78000000000000\n    complex          In: (-3.000000,-4.000000)  Out: 5.000000\n    abs range test :   2147483647  2147483647\n    abs range test :   3.4028235E+38  3.4028235E+38\n    abs range test :   1.1754944E-38  1.1754944E-38\n    abs is elemental: 20 0 1 3 100\n    complex input produces real output 50.00000000000000\n    distance of ( -3.000000 -4.000000 ) from zero is 5.000000\n    so beware of overflow with complex values\n    Inf\n    because the biggest default real is .3402823E+39\n```\n### **Standard**\n\n   FORTRAN 77\n\n### **See Also**\n\n[**sign**(3)](#sign)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ACHAR": "## achar\n\n### **Name**\n\n**achar** - \\[CHARACTER:CONVERSION\\] Returns a character in a specified position in the ASCII collating sequence\n\n### **Synopsis**\n```fortran\n    result = achar(i [,kind])\n```\n```fortran\n     elemental character(len=1,kind=KIND) function achar(i,KIND)\n\n      integer(kind=**),intent(in) :: i\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- a kind designated as ** may be any supported kind for the type\n\n- The _character_ kind returned is the value of **kind** if present.\n  otherwise, a single default _character_ is returned.\n\n### **Description**\n\n  **achar** returns the character located at position **i** (commonly\n  called the _ADE_ or ASCII Decimal Equivalent) in the ASCII collating\n  sequence.\n\n  The **achar** function is often used for generating in-band escape\n  sequences to control terminal attributes, as it makes it easy to print\n  unprintable characters such as escape and tab. For example:\n```fortran\n   write(*,'(*(a))')achar(27),'[2J'\n```\n  will clear the screen on an ANSI-compatible terminal display,\n\n### **Note**\n\nThe ADEs (ASCII Decimal Equivalents) for ASCII are\n```text\n*-------*-------*-------*-------*-------*-------*-------*-------*\n| 00 nul| 01 soh| 02 stx| 03 etx| 04 eot| 05 enq| 06 ack| 07 bel|\n| 08 bs | 09 ht | 10 nl | 11 vt | 12 np | 13 cr | 14 so | 15 si |\n| 16 dle| 17 dc1| 18 dc2| 19 dc3| 20 dc4| 21 nak| 22 syn| 23 etb|\n| 24 can| 25 em | 26 sub| 27 esc| 28 fs | 29 gs | 30 rs | 31 us |\n| 32 sp | 33  ! | 34  \" | 35  # | 36  $ | 37  % | 38  & | 39  ' |\n| 40  ( | 41  ) | 42  * | 43  + | 44  , | 45  - | 46  . | 47  / |\n| 48  0 | 49  1 | 50  2 | 51  3 | 52  4 | 53  5 | 54  6 | 55  7 |\n| 56  8 | 57  9 | 58  : | 59  ; | 60  < | 61  = | 62  > | 63  ? |\n| 64  @ | 65  A | 66  B | 67  C | 68  D | 69  E | 70  F | 71  G |\n| 72  H | 73  I | 74  J | 75  K | 76  L | 77  M | 78  N | 79  O |\n| 80  P | 81  Q | 82  R | 83  S | 84  T | 85  U | 86  V | 87  W |\n| 88  X | 89  Y | 90  Z | 91  [ | 92  \\ | 93  ] | 94  ^ | 95  _ |\n| 96  ` | 97  a | 98  b | 99  c |100  d |101  e |102  f |103  g |\n|104  h |105  i |106  j |107  k |108  l |109  m |110  n |111  o |\n|112  p |113  q |114  r |115  s |116  t |117  u |118  v |119  w |\n|120  x |121  y |122  z |123  { |124  | |125  } |126  ~ |127 del|\n*-------*-------*-------*-------*-------*-------*-------*-------*\n```\n### **Options**\n\n- **i**\n  : the _integer_ value to convert to an ASCII character, in the range\n  0 to 127.\n  : **achar** shall have the value C for any character\n  C capable of representation as a default character.\n\n- **kind**\n  : a _integer_ initialization expression indicating the kind\n  parameter of the result.\n\n### **Result**\n  Assuming **i** has a value in the range 0 <= I <= 127, the result is the\n  character in position **i** of the ASCII collating sequence, provided\n  the processor is capable of representing that character in the character\n  kind of the result; otherwise, the result is processor dependent.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_achar\nuse,intrinsic::iso_fortran_env,only:int8,int16,int32,int64\nimplicit none\ninteger :: i\n   i=65\n   write(*,'(\"decimal     =\",i0)')i\n   write(*,'(\"character   =\",a1)')achar(i)\n   write(*,'(\"binary      =\",b0)')achar(i)\n   write(*,'(\"octal       =\",o0)')achar(i)\n   write(*,'(\"hexadecimal =\",z0)')achar(i)\n\n   write(*,'(8(i3,1x,a,1x),/)')(i,achar(i), i=32,126)\n\n   write(*,'(a)')upper('Mixed Case')\ncontains\n! a classic use of achar(3) is to convert the case of a string\n\npure elemental function upper(str) result (string)\n!\n!$@(#) upper(3f): function to return a trimmed uppercase-only string\n!\n! input string to convert to all uppercase\ncharacter(*), intent(in)      :: str\n! output string that contains no miniscule letters\ncharacter(len(str))           :: string\ninteger                       :: i, iend\ninteger,parameter             :: toupper = iachar('A')-iachar('a')\n   iend=len_trim(str)\n   ! initialize output string to trimmed input string\n   string = str(:iend)\n   ! process each letter in the string\n   do concurrent (i = 1:iend)\n       select case (str(i:i))\n       ! located miniscule letter\n       case ('a':'z')\n          ! change miniscule to majuscule letter\n          string(i:i) = achar(iachar(str(i:i))+toupper)\n       end select\n   enddo\nend function upper\nend program demo_achar\n```\nResults:\n```\n   decimal     =65\n   character   =A\n   binary      =1000001\n   octal       =101\n   hexadecimal =41\n    32    33 !  34 \"  35 #  36 $  37 %  38 &  39 '\n\n    40 (  41 )  42 *  43 +  44 ,  45 -  46 .  47 /\n\n    48 0  49 1  50 2  51 3  52 4  53 5  54 6  55 7\n\n    56 8  57 9  58 :  59 ;  60 <  61 =  62 >  63 ?\n\n    64 @  65 A  66 B  67 C  68 D  69 E  70 F  71 G\n\n    72 H  73 I  74 J  75 K  76 L  77 M  78 N  79 O\n\n    80 P  81 Q  82 R  83 S  84 T  85 U  86 V  87 W\n\n    88 X  89 Y  90 Z  91 [  92 \\  93 ]  94 ^  95 _\n\n    96 `  97 a  98 b  99 c 100 d 101 e 102 f 103 g\n\n   104 h 105 i 106 j 107 k 108 l 109 m 110 n 111 o\n\n   112 p 113 q 114 r 115 s 116 t 117 u 118 v 119 w\n\n   120 x 121 y 122 z 123 { 124 | 125 } 126 ~\n   MIXED CASE\n```\n### **Standard**\n\nFORTRAN 77. KIND argument added Fortran 2003\n\n### **See Also**\n\n[**char**(3)](#char),\n[**iachar**(3)](#iachar),\n[**ichar**(3)](#ichar)\n\n### **Resources**\n\n- [ANSI escape sequences](https://en.wikipedia.org/wiki/ANSI_escape_code)\n- [M_attr module](https://github.com/urbanjost/M_attr) for controlling ANSI-compatible terminals\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ACOS": "## acos\n\n### **Name**\n\n**acos** - \\[MATHEMATICS:TRIGONOMETRIC\\] Arccosine (inverse cosine) function\n\n### **Synopsis**\n```fortran\n    result = acos(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function acos(x)\n\n      TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **TYPE** may be _real_ or _complex_\n - **KIND** may be any kind supported by the associated type.\n - The returned value will be of the same type and kind as the argument.\n\n### **Description**\n\n**acos** computes the arccosine of **x** (inverse of **cos(x)**).\n\n### **Options**\n\n- **x**\n  : The value to compute the arctangent of.\n  : If the type is _real_, the value must satisfy |**x**| <= 1.\n\n### **Result**\n\nThe return value is of the same type and kind as **x**. The _real_ part of\nthe result is in radians and lies in the range **0 \\<= acos(x%re) \\<= PI** .\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_acos\nuse, intrinsic :: iso_fortran_env, only : real_kinds,real32,real64,real128\nimplicit none\ncharacter(len=*),parameter :: all='(*(g0,1x))'\nreal(kind=real64) :: x , d2r\n\n   ! basics\n    x = 0.866_real64\n    print all,'acos(',x,') is ', acos(x)\n\n   ! acos(-1) should be PI\n    print all,'for reference &\n    &PI ~= 3.14159265358979323846264338327950288419716939937510'\n    write(*,*) acos(-1.0_real64)\n    d2r=acos(-1.0_real64)/180.0_real64\n    print all,'90 degrees is ', d2r*90.0_real64, ' radians'\n   ! elemental\n    print all,'elemental',acos([-1.0,-0.5,0.0,0.50,1.0])\n   ! complex\n    print *,'complex',acos( (-1.0,  0.0) )\n    print *,'complex',acos( (-1.0, -1.0) )\n    print *,'complex',acos( ( 0.0, -0.0) )\n    print *,'complex',acos( ( 1.0,  0.0) )\n\nend program demo_acos\n```\nResults:\n```text\n acos( 0.86599999999999999 ) is  0.52364958093182890\n for reference PI ~= 3.14159265358979323846264338327950288419716939937510\n    3.1415926535897931\n 90 degrees is  1.5707963267948966  radians\n elemental 3.14159274 2.09439516 1.57079637 1.04719758 0.00000000\n  complex            (3.14159274,-0.00000000)\n  complex             (2.23703575,1.06127501)\n  complex             (1.57079637,0.00000000)\n  complex            (0.00000000,-0.00000000)\n```\n### **Standard**\n\nFORTRAN 77 ; for a _complex_ argument - Fortran 2008\n\n### **See Also**\nInverse function: [**cos**(3)](cos)\n\n### **Resources**\n- [wikipedia: inverse trigonometric functions](https://en.wikipedia.org/wiki/Inverse_trigonometric_functions)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
-    "ACOSH": "## acosh\n\n### **Name**\n\n**acosh** - \\[MATHEMATICS:TRIGONOMETRIC\\] Inverse hyperbolic cosine function\n\n### **Synopsis**\n```fortran\n    result = acosh(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function acosh(x)\n\n      TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **TYPE** may be _real_ or _complex_\n - **KIND** may be any kind supported by the associated type.\n - The returned value will be of the same type and kind as the argument.\n\n### **Description**\n\n**acosh** computes the inverse hyperbolic cosine of **x** in radians.\n\n### **Options**\n\n- **x**\n  : The value to compute the hyperbolic cosine of. A real value should \n  be \\>= 1 or the result with be a Nan.\n\n### **Result**\n\nThe result has a value equal to a processor-dependent approximation to\nthe inverse hyperbolic cosine function of X.\n\nIf **x** is _complex_, the imaginary part of the result is in radians\nand lies between\n```fortran\n 0 <= aimag(acosh(x)) <= PI\n```\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_acosh\nuse,intrinsic :: iso_fortran_env, only : dp=>real64,sp=>real32\nimplicit none\nreal(kind=dp), dimension(3) :: x = [ 1.0d0, 2.0d0, 3.0d0 ]\n   if( any(x.lt.1) )then\n      write (*,*) ' warning: values < 1 are present'\n   endif\n   write (*,*) acosh(x)\nend program demo_acosh\n```\nResults:\n```text\n 0.000000000000000E+000   1.31695789692482        1.76274717403909\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\nInverse function: [**cosh**(3)](#cosh)\n\n### **Resources**\n- [Wikipedia:hyperbolic functions](https://en.wikipedia.org/wiki/Hyperbolic_functions)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
+    "ACOSH": "## acosh\n\n### **Name**\n\n**acosh** - \\[MATHEMATICS:TRIGONOMETRIC\\] Inverse hyperbolic cosine function\n\n### **Synopsis**\n```fortran\n    result = acosh(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function acosh(x)\n\n      TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **TYPE** may be _real_ or _complex_\n - **KIND** may be any kind supported by the associated type.\n - The returned value will be of the same type and kind as the argument.\n\n### **Description**\n\n**acosh** computes the inverse hyperbolic cosine of **x** in radians.\n\n### **Options**\n\n- **x**\n  : The value to compute the hyperbolic cosine of. A real value should\n  be \\>= 1 or the result with be a Nan.\n\n### **Result**\n\nThe result has a value equal to a processor-dependent approximation to\nthe inverse hyperbolic cosine function of X.\n\nIf **x** is _complex_, the imaginary part of the result is in radians\nand lies between\n```fortran\n 0 <= aimag(acosh(x)) <= PI\n```\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_acosh\nuse,intrinsic :: iso_fortran_env, only : dp=>real64,sp=>real32\nimplicit none\nreal(kind=dp), dimension(3) :: x = [ 1.0d0, 2.0d0, 3.0d0 ]\n   if( any(x.lt.1) )then\n      write (*,*) ' warning: values < 1 are present'\n   endif\n   write (*,*) acosh(x)\nend program demo_acosh\n```\nResults:\n```text\n 0.000000000000000E+000   1.31695789692482        1.76274717403909\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\nInverse function: [**cosh**(3)](#cosh)\n\n### **Resources**\n- [Wikipedia:hyperbolic functions](https://en.wikipedia.org/wiki/Hyperbolic_functions)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ADJUSTL": "## adjustl\n\n### **Name**\n\n**adjustl** - \\[CHARACTER:WHITESPACE\\] Left-justified a string\n\n### **Synopsis**\n```fortran\n  result = adjustl(string)\n```\n```fortran\n   elemental character(len=len(string),kind=KIND) function adjustl(string)\n\n    character(len=*,kind=KIND),intent(in) :: string\n```\n### **Characteristics**\n - **string** is a _character_ variable of any supported kind\n - The return value is a _character_ variable of the same kind\n   and length as **string**\n\n### **Description**\n\n  **adjustl** will left-justify a string by removing leading\n  spaces. Spaces are inserted at the end of the string as needed.\n\n### **Options**\n\n- **string**\n  : the string to left-justify\n\n### **Result**\n\n  A copy of **string** where leading spaces are removed and the same\n  number of spaces are inserted on the end of **string**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_adjustl\nimplicit none\ncharacter(len=20) :: str = '   sample string'\ncharacter(len=:),allocatable :: astr\ninteger :: length\n\n   ! basic use\n    write(*,'(a,\"[\",a,\"]\")') 'original: ',str\n    str=adjustl(str)\n    write(*,'(a,\"[\",a,\"]\")') 'adjusted: ',str\n\n    ! a fixed-length string can be printed\n    ! trimmed using trim(3f) or len_trim(3f)\n    write(*,'(a,\"[\",a,\"]\")') 'trimmed:  ',trim(str)\n    length=len_trim(str)\n    write(*,'(a,\"[\",a,\"]\")') 'substring:',str(:length)\n\n    ! note an allocatable string stays the same length too\n    ! and is not trimmed by just an adjustl(3f) call.\n    astr='    allocatable string   '\n    write(*,'(a,\"[\",a,\"]\")') 'original:',astr\n    astr = adjustl(astr)\n    write(*,'(a,\"[\",a,\"]\")') 'adjusted:',astr\n    ! trim(3f) can be used to change the length\n    astr = trim(astr)\n    write(*,'(a,\"[\",a,\"]\")') 'trimmed: ',astr\n\nend program demo_adjustl\n```\nResults:\n```text\n   original: [   sample string    ]\n   adjusted: [sample string       ]\n   trimmed:  [sample string]\n   substring:[sample string]\n   original:[    allocatable string   ]\n   adjusted:[allocatable string       ]\n   trimmed: [allocatable string]\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**adjustr**(3)](#adjustr),\n[**trim**(3)](#trim)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ADJUSTR": "## adjustr\n\n### **Name**\n\n**adjustr** - \\[CHARACTER:WHITESPACE\\] Right-justify a string\n\n### **Synopsis**\n```fortran\n  result = adjustr(string)\n```\n```fortran\n   elemental character(len=len(string),kind=KIND) function adjustr(string)\n\n    character(len=*,kind=KIND),intent(in) :: string\n```\n### **Characteristics**\n\n- **string** is a _character_ variable\n- The return value is a _character_ variable of the same kind and\n  length as **string**\n\n### **Description**\n\n**adjustr** right-justifies a string by removing trailing spaces. Spaces\nare inserted at the start of the string as needed to retain the original\nlength.\n\n### **Options**\n\n- **string**\n  : the string to right-justify\n\n### **Result**\n\nTrailing spaces are removed and the same number of spaces are inserted\nat the start of **string**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_adjustr\nimplicit none\ncharacter(len=20) :: str\n   ! print a short number line\n   write(*,'(a)')repeat('1234567890',2)\n\n  ! basic usage\n   str = '  sample string '\n   write(*,'(a)') str\n   str = adjustr(str)\n   write(*,'(a)') str\n\n   !\n   ! elemental\n   !\n   write(*,'(a)')repeat('1234567890',5)\n   write(*,'(a)')adjustr([character(len=50) :: &\n   '  first           ', &\n   '     second       ', &\n   '         third    ' ])\n   write(*,'(a)')repeat('1234567890',5)\n\nend program demo_adjustr\n```\nResults:\n```text\n   12345678901234567890\n     sample string\n          sample string\n   12345678901234567890123456789012345678901234567890\n                                                first\n                                               second\n                                                third\n   12345678901234567890123456789012345678901234567890\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**adjustl**(3)](#adjustl),\n[**trim**(3)](#trim)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "AIMAG": "## aimag\n\n### **Name**\n\n**aimag** - \\[TYPE:NUMERIC\\] Imaginary part of complex number\n\n### **Synopsis**\n```fortran\n    result = aimag(z)\n```\n```fortran\n     elemental complex(kind=KIND) function aimag(z)\n\n      complex(kind=KIND),intent(in) :: z\n```\n### **Characteristics**\n\n- The type of the argument **z** shall be _complex_ and any supported\n  _complex_ kind\n\n- The return value is of type _real_ with the kind type parameter of\n  the argument.\n\n### **Description**\n\n  **aimag** yields the imaginary part of the complex argument **z**.\n\n  This is similar to the modern complex-part-designator **%IM** which also\n  designates the imaginary part of a value, accept a designator can appear\n  on the left-hand side of an assignment as well, as in **val%im=10.0**.\n\n### **Options**\n\n- **z**\n  : The _complex_ value to extract the imaginary component of.\n\n### **Result**\n\n  The return value is a _real_ value with the magnitude and sign of the\n  imaginary component of the argument **z**.\n\n  That is, If **z** has the value **(x,y)**, the result has the value\n  **y**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_aimag\nuse, intrinsic :: iso_fortran_env, only : real_kinds, &\n & real32, real64, real128\nimplicit none\ncharacter(len=*),parameter :: g='(*(1x,g0))'\ncomplex              :: z4\ncomplex(kind=real64) :: z8\n   ! basics\n    z4 = cmplx(1.e0, 2.e0)\n    print *, 'value=',z4\n    print g, 'imaginary part=',aimag(z4),'or', z4%im\n\n    ! other kinds other than the default may be supported\n    z8 = cmplx(3.e0_real64, 4.e0_real64,kind=real64)\n    print *, 'value=',z8\n    print g, 'imaginary part=',aimag(z8),'or', z8%im\n\n    ! an elemental function can be passed an array\n    print *\n    print *, [z4,z4/2.0,z4+z4,z4**3]\n    print *\n    print *, aimag([z4,z4/2.0,z4+z4,z4**3])\n\nend program demo_aimag\n```\nResults:\n```text\n value= (1.00000000,2.00000000)\n imaginary part= 2.00000000 or 2.00000000\n value= (3.0000000000000000,4.0000000000000000)\n imaginary part= 4.0000000000000000 or 4.0000000000000000\n\n (1.00000000,2.00000000) (0.500000000,1.00000000) (2.00000000,4.00000000)\n (-11.0000000,-2.00000000)\n\n   2.00000000       1.00000000       4.00000000      -2.00000000\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n- [**cmplx**(3)](#cmplx) - Complex conversion function\n- [**conjg**(3)](#conjg) - Complex conjugate function\n- [**real**(3)](#real) - Convert to real type\n\nFortran has strong support for _complex_ values, including many intrinsics\nthat take or produce _complex_ values in addition to algebraic and\nlogical expressions:\n\n[**abs**(3)](#abs),\n[**acosh**(3)](#acosh),\n[**acos**(3)](#acos),\n[**asinh**(3)](#asinh),\n[**asin**(3)](#asin),\n[**atan2**(3)](#atan2),\n[**atanh**(3)](#atanh),\n[**atan**(3)](#atan),\n[**cosh**(3)](#cosh),\n[**cos**(3)](#cos),\n[**co_sum**(3)](#co_sum),\n[**dble**(3)](#dble),\n[**dot_product**(3)](#dot_product),\n[**exp**(3)](#exp),\n[**int**(3)](#int),\n[**is_contiguous**(3)](#is_contiguous),\n[**kind**(3)](#kind),\n[**log**(3)](#log),\n[**matmul**(3)](#matmul),\n[**precision**(3)](#precision),\n[**product**(3)](#product),\n[**range**(3)](#range),\n[**rank**(3)](#rank),\n[**sinh**(3)](#sinh),\n[**sin**(3)](#sin),\n[**sqrt**(3)](#sqrt),\n[**storage_size**(3)](#storage_size),\n[**sum**(3)](#sum),\n[**tanh**(3)](#tanh),\n[**tan**(3)](#tan),\n[**unpack**(3)](#unpack),\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "AINT": "## aint\n\n### **Name**\n\n**aint** - \\[NUMERIC\\] Truncate toward zero to a whole number\n\n### **Synopsis**\n```fortran\n    result = aint(x [,kind])\n```\n```fortran\n     elemental real(kind=KIND) function iaint(x,KIND)\n\n      real(kind=**),intent(in)   :: x\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- a kind designated as ** may be any supported kind for the type\n- the result is a real of the default kind unless **kind** is specified.\n- **kind** is an _integer_ initialization expression indicating the\n  kind parameter of the result.\n\n### **Description**\n\n  **aint** truncates its argument toward zero to a whole number.\n\n### **Options**\n\n- **x**\n  : the _real_ value to truncate.\n\n- **kind**\n  : indicates the kind parameter of the result.\n\n### **Result**\n\n  The sign is the same as the sign of **x** unless the magnitude of **x**\n  is less than one, in which case zero is returned.\n\n  Otherwise **aint** returns the largest whole number that does not\n  exceed the magnitude of **x** with the same sign as the input.\n\n  That is, it truncates the value towards zero.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_aint\nuse, intrinsic :: iso_fortran_env, only : sp=>real32, dp=>real64\nimplicit none\nreal(kind=dp) :: x8\n   print *,'basics:'\n   print *,' just chops off the fractional part'\n   print *,  aint(-2.999), aint(-2.1111)\n   print *,' if |x| < 1 a positive zero is returned'\n   print *,  aint(-0.999), aint( 0.9999)\n   print *,' input may be of any real kind'\n   x8 = 4.3210_dp\n   print *, aint(-x8), aint(x8)\n   print *,'elemental:'\n   print *,aint([ &\n    &  -2.7,  -2.5, -2.2, -2.0, -1.5, -1.0, -0.5, &\n    &  0.0,   &\n    &  +0.5,  +1.0, +1.5, +2.0, +2.2, +2.5, +2.7  ])\nend program demo_aint\n```\nResults:\n```text\n basics:\n  just chops off the fractional part\n  -2.000000      -2.000000\n  if |x| < 1 a positive zero is returned\n  0.0000000E+00  0.0000000E+00\n  input may be of any real kind\n  -4.00000000000000        4.00000000000000\n elemental:\n  -2.000000      -2.000000      -2.000000      -2.000000      -1.000000\n  -1.000000      0.0000000E+00  0.0000000E+00  0.0000000E+00   1.000000\n   1.000000       2.000000       2.000000       2.000000       2.000000\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n[**anint**(3)](#anint),\n[**int**(3)](#int),\n[**nint**(3)](#nint),\n[**selected_int_kind**(3)](#selected_int_kind),\n[**ceiling**(3)](#ceiling),\n[**floor**(3)](#floor)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ALL": "## all\n\n### **Name**\n\n**all** - \\[ARRAY:REDUCTION\\] Determines if all the values are true\n\n### **Synopsis**\n```fortran\n   result = all(mask [,dim])\n```\n```fortran\n     function all(mask ,dim)\n\n      logical(kind=KIND),intent(in) :: mask(..)\n      integer,intent(in),optional   :: dim\n      logical(kind=KIND)            :: all(..)\n```\n### **Characteristics**\n\n - **mask** is a _logical_ array\n - **dim** is an _integer_\n - the result is a logical array if **dim** is supplied,\n   otherwise it is a logical scalar. It has the same characteristics\n   as **mask**\n\n### **Description**\n\n  **all** determines if all the values are true in **mask** in the\n  array along dimension **dim** if **dim** is specified; otherwise all\n  elements are tested together.\n\n  This testing type is called a logical conjunction of elements of\n  **mask** along dimension **dim**.\n\n  The mask is generally a _logical_ expression, allowing for comparing\n  arrays and many other common operations.\n\n### **Options**\n\n- **mask**\n  : the logical array to be tested for all elements being _.true_.\n\n- **dim**\n  : **dim** indicates the direction through the elements of **mask**\n  to group elements for testing.\n  : **dim** has a value that lies between one and the rank of **mask**.\n  : The corresponding actual argument shall not be an optional dummy\n  argument.\n  : If **dim** is not present all elements are tested and a single\n  scalar value is returned.\n\n### **Result**\n\n\n1.  If **dim** is not present **all(mask)** is _.true._ if all elements\n    of **mask** are _.true._. It also is _.true._ if **mask** has zero size;\n    otherwise, it is _.false._ .\n\n2.  If the rank of **mask** is one, then **all(mask, dim)** is equivalent\n    to **all(mask)**.\n\n3.  If the rank of **mask** is greater than one and **dim** is present then\n    **all(mask,dim)** returns an array with the rank (number of\n    dimensions)  of **mask** minus 1. The shape is determined from the\n    shape of **mask** where the **dim** dimension is elided. A value is\n    returned for each set of elements along the **dim** dimension.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_all\nimplicit none\nlogical,parameter :: T=.true., F=.false.\nlogical bool\n\n  ! basic usage\n   ! is everything true?\n   bool = all([ T,T,T ])\n   print *, 'are all values true?', bool\n   bool = all([ T,F,T ])\n   print *, 'are all values true now?', bool\n\n  ! compare matrices, even by a dimension\n   ARRAYS: block\n   integer :: a(2,3), b(2,3)\n    ! set everything to one except one value in b\n    a = 1\n    b = 1\n    b(2,2) = 2\n    ! now compare those two arrays\n    print *,'entire array :', all(a ==  b )\n    print *,'compare columns:', all(a ==  b, dim=1)\n    print *,'compare rows:', all(a ==  b, dim=2)\n  end block ARRAYS\n\nend program demo_all\n```\nResults:\n```text\n >  T\n >  F\n >  entire array : F\n >  compare columns: T F T\n >  compare rows: T F\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**any**(3)](#any)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ALLOCATED": "## allocated\n\n### **Name**\n\n**allocated** - \\[ARRAY:INQUIRY\\] Allocation status of an allocatable entity\n\n### **Synopsis**\n```fortran\n    result = allocated(array|scalar)\n```\n```fortran\n     logical function allocated(array,scalar)\n\n      type(TYPE(kind=**)),allocatable,optional :: array(..)\n      type(TYPE(kind=**)),allocatable,optional :: scalar\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **array** may be any allocatable array object of any type.\n - **scalar** may be any allocatable scalar of any type.\n - the result is a default logical scalar\n\n### **Description**\n\n  **allocated** checks the allocation status of both arrays\n  and scalars.\n\n At least one and only one of **array** or **scalar** must be specified.\n\n### **Options**\n\n- **entity**\n  : the _allocatable_ object to test.\n\n### **Result**\n\n  If the argument is allocated then the result is _.true._; otherwise,\n  it returns _.false._.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_allocated\nuse,intrinsic :: iso_fortran_env, only : dp=>real64,sp=>real32\nimplicit none\nreal(kind=sp), allocatable :: x(:)\ncharacter(len=256) :: message\ninteger :: istat\n  ! basics\n   if( allocated(x)) then\n       write(*,*)'do things if allocated'\n   else\n       write(*,*)'do things if not allocated'\n   endif\n\n   ! if already allocated, deallocate\n   if ( allocated(x) ) deallocate(x,STAT=istat, ERRMSG=message )\n   if(istat.ne.0)then\n      write(*,*)trim(message)\n      stop\n   endif\n\n   ! only if not allocated, allocate\n   if ( .not. allocated(x) ) allocate(x(20))\n\n  ! allocation and intent(out)\n   call intentout(x)\n   write(*,*)'note it is deallocated!',allocated(x)\n\n   contains\n\n   subroutine intentout(arr)\n   ! note that if arr has intent(out) and is allocatable,\n   ! arr is deallocated on entry\n   real(kind=sp),intent(out),allocatable :: arr(:)\n       write(*,*)'note it was allocated in calling program',allocated(arr)\n   end subroutine intentout\n\nend program demo_allocated\n```\nResults:\n```text\n >  do things if not allocated\n >  note it was allocated in calling program F\n >  note it is deallocated! F\n```\n### **Standard**\n\n  Fortran 95. allocatable scalar entities were added in Fortran 2003.\n\n### **See Also**\n\n[**move_alloc**(3)](#move_alloc)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "ANINT": "## anint\n\n### **Name**\n\n**anint** - \\[NUMERIC\\] Real nearest whole number\n\n### **Synopsis**\n```fortran\n    result = anint(a [,kind])\n```\n```fortran\n     elemental real(kind=KIND) function anint(x,KIND)\n\n      real(kind=**),intent(in)   :: x\n      integer,intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- **a** is type _real_ of any kind\n- **KIND** is a scalar integer constant expression.\n- the result is type _real_. The kind of the result is the same as **x**\n  unless specified by **kind**.\n\n### **Description**\n\n  **anint** rounds its argument to the nearest whole number.\n\n  Unlike **nint**(3) which returns an _integer_ the full range or real\n  values can be returned (_integer_ types typically have a smaller range\n  of values than _real_ types).\n\n### **Options**\n\n- **a**\n  : the value to round\n\n- **kind**\n  : specifies the kind of the result. The default is the kind of **a**.\n\n### **Result**\n\nThe return value is the real whole number nearest **a**.\n\nIf **a** is greater than zero, **anint(a)**(3) returns **aint(a + 0.5)**.\n\nIf **a** is less than or equal to zero then it returns **aint(a - 0.5)**,\nexcept **aint** specifies that for |**a**| < 1 the result is zero (0).\n\nIt is processor-dependent whether anint(a) returns negative zero when\n-0.5 < a <= -0.0.  Compiler switches are often available which enable\nor disable support of negative zero.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_anint\nuse, intrinsic :: iso_fortran_env, only : real32, real64, real128\nimplicit none\nreal,allocatable :: arr(:)\n\n  ! basics\n   print *, 'ANINT (2.783) has the value 3.0 =>', anint(2.783)\n   print *, 'ANINT (-2.783) has the value -3.0 =>', anint(-2.783)\n\n   print *, 'by default the kind of the output is the kind of the input'\n   print *, anint(1234567890.1234567890e0)\n   print *, anint(1234567890.1234567890d0)\n\n   print *, 'sometimes specifying the result kind is useful when passing'\n   print *, 'results as an argument, for example.'\n   print *, 'do you know why the results are different?'\n   print *, anint(1234567890.1234567890,kind=real64)\n   print *, anint(1234567890.1234567890d0,kind=real64)\n\n  ! elemental\n   print *, 'numbers on a cusp are always the most troublesome'\n   print *, anint([ -2.7, -2.5, -2.2, -2.0, -1.5, -1.0, -0.5, 0.0 ])\n\n   print *, 'negative zero is processor dependent'\n   arr=[ 0.0, 0.1, 0.5, 1.0, 1.5, 2.0, 2.2, 2.5, 2.7 ]\n   print *, anint(arr)\n   arr=[ -0.0, -0.1, -0.5, -1.0, -1.5, -2.0, -2.2, -2.5, -2.7 ]\n   print *, anint(arr)\n\nend program demo_anint\n```\nResults:\n```text\n >  ANINT (2.783) has the value 3.0 =>   3.000000\n >  ANINT (-2.783) has the value -3.0 =>  -3.000000\n >  by default the kind of the output is the kind of the input\n >   1.2345679E+09\n >    1234567890.00000\n >  sometimes specifying the result kind is useful when passing\n >  results as an argument, for example.\n >  do you know why the results are different?\n >    1234567936.00000\n >    1234567890.00000\n >  numbers on a cusp are always the most troublesome\n >   -3.000000      -3.000000      -2.000000      -2.000000      -2.000000\n >   -1.000000      -1.000000      0.0000000E+00\n >  negative zero is processor dependent\n >   0.0000000E+00  0.0000000E+00   1.000000       1.000000       2.000000\n >    2.000000       2.000000       3.000000       3.000000\n >   0.0000000E+00  0.0000000E+00  -1.000000      -1.000000      -2.000000\n >   -2.000000      -2.000000      -3.000000      -3.000000\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n[**aint**(3)](#aint),\n[**int**(3)](#int),\n[**nint**(3)](#nint),\n[**selected_int_kind**(3)](#selected_int_kind),\n[**ceiling**(3)](#ceiling),\n[**floor**(3)](#floor)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n\n",
@@ -80,15 +80,15 @@
     "EXECUTE_COMMAND_LINE": "## execute_command_line\n\n### **Name**\n\n**execute_command_line** - \\[SYSTEM:PROCESSES\\] Execute a shell command\n\n### **Synopsis**\n```fortran\n    call execute_command_line( &\n    & command [,wait] [,exitstat] [,cmdstat] [,cmdmsg] )\n```\n```fortran\n     subroutine execute_command_line(command,wait,exitstat,cmdstat,cmdmsg)\n\n      character(len=*),intent(in)             :: command\n      logical,intent(in),optional             :: wait\n      integer,intent(inout),optional          :: exitstat\n      integer,intent(inout),optional          :: cmdstat\n      character(len=*),intent(inout),optional :: cmdmsg\n```\n### **Characteristics**\n - **command** is a default _character_ scalar\n - **wait** is a default _logical_ scalar. If **wait** is present with the\n - **exitstat** is an _integer_ of the default kind.\n   It must be of a kind with at least a decimal exponent range of 9.\n - **cmdstat** is an _integer_ of default kind\n   The kind of the variable must support at least a decimal exponent range of four.\n\n - **cmdmsg** is a _character_ scalar of the default kind.\n\n### **Description**\n\n  For **execute_command_line** the **command** argument is passed\n  to the shell and executed. (The shell is generally **sh**(1) on Unix\n  systems, and cmd.exe on Windows.) If **wait** is present and has the\n  value _.false._, the execution of the command is asynchronous if the\n  system supports it; otherwise, the command is executed synchronously.\n\n  The three last arguments allow the user to get status information. After\n  synchronous execution, **exitstat** contains the integer exit code of\n  the command, as returned by **system**. **cmdstat** is set to zero if\n  the command line was executed (whatever its exit status was). **cmdmsg**\n  is assigned an error message if an error has occurred.\n\n  Note that the system call need not be thread-safe. It is the\n  responsibility of the user to ensure that the system is not called\n  concurrently if required.\n\n  When the command is executed synchronously, **execute_command_line**\n  returns after the command line has completed execution. Otherwise,\n  **execute_command_line** returns without waiting.\n\n  Because this intrinsic is making a system call, it is very system\n  dependent. Its behavior with respect to signaling is processor\n  dependent. In particular, on POSIX-compliant systems, the SIGINT and\n  SIGQUIT signals will be ignored, and the SIGCHLD will be blocked. As\n  such, if the parent process is terminated, the child process might\n  not be terminated alongside.\n\n  One of the most common causes of errors is that the program requested\n  is not in the search path. You should make sure that the program to be\n  executed is installed on your system and that it is in the system's\n  path when the program calls it. You can check if it is installed by\n  running it from the command prompt. If it runs successfully from the\n  command prompt, it means that it is installed, and so you should\n  next check that it is in the search path when the program executes\n  (usually this means checking the environment variable PATH).\n\n### **Options**\n\n- **command**\n  : the command line to be executed. The interpretation is\n  programming-environment dependent.\n\n- **wait**\n  : If **wait** is present with the\n  value _.false._, and the processor supports asynchronous execution of\n  the command, the command is executed asynchronously; otherwise it is\n  executed synchronously.\n\n  When the command is executed synchronously, **execute_command_line**\n  returns after the command line has completed execution. Otherwise,\n  **execute_command_line** returns without waiting.\n\n- **exitstat**\n  : If the command is executed synchronously, it is assigned the value\n  of the processor-dependent exit status. Otherwise, the value of\n  **exitstat** is unchanged.\n\n- **cmdstat**\n  : If an error condition occurs and **cmdstat** is not present, error\n  termination of execution of the image is initiated.\n\n  It is assigned the value **-1** if the processor does not support\n  command line execution, a processor-dependent positive value if an\n  error condition occurs, or the value **-2** if no error condition\n  occurs but **wait** is present with the value false and the processor\n  does not support asynchronous execution. Otherwise it is assigned\n  the value 0.\n\n- **cmdmsg**\n  : If an error condition occurs, it is assigned a processor-dependent\n  explanatory message. Otherwise, it is unchanged.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_exec\nimplicit none\n   integer :: i\n\n   call execute_command_line(\"external_prog.exe\", exitstat=i)\n   print *, \"Exit status of external_prog.exe was \", i\n\n   call execute_command_line(\"reindex_files.exe\", wait=.false.)\n   print *, \"Now reindexing files in the background\"\nend program demo_exec\n```\n### **Standard**\n\nFortran 2008\n\n### **See also**\n\n[**get_environment_variable**(3)](#get_environment_variable)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "EXP": "## exp\n\n### **Name**\n\n**exp** - \\[MATHEMATICS\\] Base-e exponential function\n\n### **Synopsis**\n```fortran\n    result = exp(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function exp(x)\n\n      TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** may be _real_ or _complex_ of any kind.\n - The return value has the same type and kind as **x**.\n\n### **Description**\n\n**exp** returns the value of _e_ (the base of natural logarithms)\nraised to the power of **x**.\n\n\"_e_\" is also known as _Euler's constant_.\n\nIf **x** is of type _complex_, its imaginary part is regarded as a value\nin radians such that if (see _Euler's formula_):\n```fortran\n    cx=(re,im)\n```\nthen\n```fortran\n    exp(cx) = exp(re) * cmplx(cos(im),sin(im),kind=kind(cx))\n```\nSince **exp** is the inverse function of **log**(3) the maximum valid magnitude\nof the _real_ component of **x** is **log(huge(x))**.\n\n### **Options**\n\n- **x**\n  : The type shall be _real_ or _complex_.\n\n### **Result**\n\nThe value of the result is **e\\*\\*x** where **e** is Euler's constant.\n\nIf **x** is of type complex, its imaginary part is\nregarded as a value in radians.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_exp\nimplicit none\nreal :: x, re, im\ncomplex :: cx\n\n   x = 1.0\n   write(*,*)\"Euler's constant is approximately\",exp(x)\n\n   !! complex values\n   ! given\n   re=3.0\n   im=4.0\n   cx=cmplx(re,im)\n\n   ! complex results from complex arguments are Related to Euler's formula\n   write(*,*)'given the complex value ',cx\n   write(*,*)'exp(x) is',exp(cx)\n   write(*,*)'is the same as',exp(re)*cmplx(cos(im),sin(im),kind=kind(cx))\n\n   ! exp(3) is the inverse function of log(3) so\n   ! the real component of the input must be less than or equal to\n   write(*,*)'maximum real component',log(huge(0.0))\n   ! or for double precision\n   write(*,*)'maximum doubleprecision component',log(huge(0.0d0))\n\n   ! but since the imaginary component is passed to the cos(3) and sin(3)\n   ! functions the imaginary component can be any real value\n\nend program demo_exp\n```\n\nResults:\n\n```text\n Euler's constant is approximately   2.718282\n given the complex value  (3.000000,4.000000)\n exp(x) is (-13.12878,-15.20078)\n is the same as (-13.12878,-15.20078)\n maximum real component   88.72284\n maximum doubleprecision component   709.782712893384\n```\n\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n- [**log**(3)](#log)\n\n### **Resources**\n\n- Wikipedia:[Exponential function](https://en.wikipedia.org/wiki/Exponential_function)\n\n- Wikipedia:[Euler's formula](https://en.wikipedia.org/wiki/Euler%27s_formula)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "EXPONENT": "## exponent\n\n### **Name**\n\n**exponent** - \\[MODEL_COMPONENTS\\] Exponent of floating-point number\n\n### **Synopsis**\n```fortran\n    result = exponent(x)\n```\n```fortran\n     elemental integer function exponent(x)\n\n      real(kind=**),intent(in) :: x\n```\n### **Characteristics**\n - **x**  shall be of type _real_ of any valid kind\n - the result is a default _integer_ type\n\n### **Description**\n\n  **exponent** returns the value of the exponent part of **x**, provided\n  the exponent is within the range of default _integers_.\n\n### **Options**\n\n- **x**\n  : the value to query the exponent of\n\n### **Result**\n\n  **exponent** returns the value of the exponent part of **x**\n\n  If **x** is zero the value returned is zero.\n\n  If **x** is an IEEE infinity or NaN, the result has the value HUGE(0).\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_exponent\nimplicit none\nreal :: x = 1.0\ninteger :: i\n   i = exponent(x)\n   print *, i\n   print *, exponent(0.0)\n   print *, exponent([10.0,100.0,1000.0,-10000.0])\n   ! beware of overflow, it may occur silently\n   !print *, 2**[10.0,100.0,1000.0,-10000.0]\n   print *, exponent(huge(0.0))\n   print *, exponent(tiny(0.0))\nend program demo_exponent\n```\nResults:\n```text\n >            4           7          10          14\n >          128\n >         -125\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions_\n",
     "EXTENDS_TYPE_OF": "## extends_type_of\n\n### **Name**\n\n**extends_type_of** - \\[STATE:INQUIRY\\] Determine if the dynamic type\nof **a** is an extension of the dynamic type of **mold**.\n\n### **Synopsis**\n```fortran\n    result = extends_type_of(a, mold)\n```\n```fortran\n     logical extends_type_of(a, mold)\n\n      type(TYPE(kind=KIND)),intent(in) :: a\n      type(TYPE(kind=KIND)),intent(in) :: mold\n```\n### **Characteristics**\n -**a** shall be an object or pointer to an extensible declared type,\n        or unlimited polymorphic. If it is a polymorphic pointer, it\n        shall not have an undefined association status.\n -**mole** shall be an object or pointer to an extensible declared type\n           or unlimited polymorphic. If it is a polymorphic pointer,\n           it shall not have an undefined association status.\n - the result is a scalar default logical type.\n\n### **Description**\n\n  **extends_type_of** is .true. if and only if the dynamic type of\n  **a** is or could be (for unlimited polymorphic) an extension of the\n  dynamic type of **mold**.\n\n#### NOTE1\n\n  The dynamic type of a disassociated pointer or unallocated allocatable\n  variable is its declared type.\n\n#### NOTE2\n\n  The test performed by **extends_type_of** is not the same as the\n  test performed by the type guard **class is**. The test performed by\n  **extends_type_of** does not consider kind type parameters.\n\n### **options**\n- **a**\n    : be an object of extensible declared type or unlimited\n    polymorphic. If it is a polymorphic pointer, it shall not have an\n    undefined association status.\n\n- **mold**\n    : be an object of extensible declared type or unlimited\n    polymorphic. If it is a polymorphic pointer, it shall not have an\n    undefined association status.\n\n### **Result**\n\n  If **mold** is unlimited polymorphic and is either a disassociated\n  pointer or unallocated allocatable variable, the result is true.\n\n  Otherwise if **a** is unlimited polymorphic and is either a\n  disassociated pointer or unallocated allocatable variable, the result\n  is false.\n\n  Otherwise the result is true if and only if the dynamic type of **a**\n\n  if the dynamic type of A or MOLD is extensible, the result is true if\n  and only if the dynamic type of A is an extension type of the dynamic\n  type of MOLD; otherwise the result is processor dependent.\n\n\n### **Examples**\n\nSample program:\n```fortran\n  ! program demo_extends_type_of\n  module M_demo_extends_type_of\n  implicit none\n  private\n\n  type nothing\n  end type nothing\n\n  type, extends(nothing) :: dot\n    real :: x=0\n    real :: y=0\n  end type dot\n\n  type, extends(dot) :: point\n    real :: z=0\n  end type point\n\n  type something_else\n  end type something_else\n\n  public :: nothing\n  public :: dot\n  public :: point\n  public :: something_else\n\n  end module M_demo_extends_type_of\n\n  program demo_extends_type_of\n  use M_demo_extends_type_of, only : nothing, dot, point, something_else\n  implicit none\n  type(nothing) :: grandpa\n  type(dot) :: dad\n  type(point) :: me\n  type(something_else) :: alien\n\n   write(*,*)'these should all be true'\n   write(*,*)extends_type_of(me,grandpa),'I am descended from Grandpa'\n   write(*,*)extends_type_of(dad,grandpa),'Dad is descended from Grandpa'\n   write(*,*)extends_type_of(me,dad),'Dad is my ancestor'\n\n   write(*,*)'is an object an extension of itself?'\n   write(*,*)extends_type_of(grandpa,grandpa) ,'self-propagating!'\n   write(*,*)extends_type_of(dad,dad) ,'clone!'\n\n   write(*,*)' you did not father your grandfather'\n   write(*,*)extends_type_of(grandpa,dad),'no paradox here'\n\n   write(*,*)extends_type_of(dad,me),'no paradox here'\n   write(*,*)extends_type_of(grandpa,me),'no relation whatsoever'\n   write(*,*)extends_type_of(grandpa,alien),'no relation'\n   write(*,*)extends_type_of(me,alien),'not what everyone thinks'\n\n   call pointers()\n   contains\n\n   subroutine pointers()\n   ! Given the declarations and assignments\n   type t1\n   real c\n   end type\n   type, extends(t1) :: t2\n   end type\n   class(t1), pointer :: p, q\n      allocate (p)\n      allocate (t2 :: q)\n      ! the result of EXTENDS_TYPE_OF (P, Q) will be false, and the result\n      ! of EXTENDS_TYPE_OF (Q, P) will be true.\n      write(*,*)'(P,Q)',extends_type_of(p,q),\"mind your P's and Q's\"\n      write(*,*)'(Q,P)',extends_type_of(q,p)\n   end subroutine pointers\n\n  end program demo_extends_type_of\n```\nResults:\n```text\n    these should all be true\n    T I am descended from Grandpa\n    T Dad is descended from Grandpa\n    T Dad is my ancestor\n    is an object an extension of itself?\n    T self-propagating!\n    T clone!\n     you did not father your grandfather\n    F no paradox here\n    F no paradox here\n    F no relation whatsoever\n    F no relation\n    F not what everyone thinks\n    (P,Q) F mind your P's and Q's\n    (Q,P) T\n```\n### **Standard**\n\n   Fortran 2003\n\n### **See Also**\n\n[**same_type_as**(3)](#same_type_as)\n\n  _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "FINDLOC": "## findloc\n\n### **Name**\n\n**findloc** - \\[ARRAY:LOCATION\\] Location of first element of ARRAY\nidentified by MASK along dimension DIM matching a target value\n\n### **Synopsis**\n\n```fortran\n    result = findloc (array, value, dim [,mask] [,kind] [,back]) |\n             findloc (array, value [,mask] [,kind] [,back])\n```\n```fortran\n     function findloc (array, value, dim, mask, kind, back)\n\n      type(TYPE(kind=KIND)),intent(in)     :: array(..)\n      type(TYPE(kind=KIND)),intent(in)     :: value\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n      integer(kind=**),intent(in),optional :: kind\n      logical(kind=**),intent(in),optional :: back\n```\n### **Characteristics**\n\n- **array** is an array of any intrinsic type.\n- **value** shall be scalar but in type conformance with **array**,\n  as specified for the operator == or the operator .EQV..\n- **dim** an _integer_ corresponding to a dimension of **array**.\n  The corresponding actual argument shall not be an optional dummy\n  argument.\n- **mask** is logical and shall be conformable with **array**.\n- **kind** a scalar integer initialization expression (ie. a constant)\n- **back** a logical scalar.\n- the result is _integer_ of default kind or kind **kind** if the\n  **kind** argument is present. If **dim** does not appear, the result\n  is an array of rank one and of size equal to the rank of **array**;\n  otherwise, the result is an array of the same rank and shape as\n  **array** reduced by the dimension **dim**.\n\n**NOTE**: a kind designated as ** may be any supported kind for the type\n\n### **Description**\n\n**findloc** returns the location of the first element of **array**\nidentified by **mask** along dimension **dim** having a value equal\nto **value**.\n\nIf both **array** and **value** are of type logical, the comparison is\nperformed with the **.eqv.** operator; otherwise, the comparison is\nperformed with the == operator. If the value of the comparison is\n_.true._, that element of **array** matches **value**.\n\nIf only one element matches **value**, that element's subscripts are\nreturned. Otherwise, if more than one element matches **value** and\n**back** is absent or present with the value _.false._, the element whose\nsubscripts are returned is the first such element, taken in array\nelement order. If **back** is present with the value _.true._, the element\nwhose subscripts are returned is the last such element, taken in array\nelement order.\n\n### **Options**\n\n- **array**\n  : shall be an array of intrinsic type.\n\n- **value**\n  : shall be scalar and in type conformance with **array**.\n\n- **dim**\n  : shall be an integer scalar with a value in the range 1 <= **DIM** <=\n  n, where n is the rank of **array**. The corresponding actual argument\n  shall not be an optional dummy argument.\n\n- **mask**\n  : (optional) shall be of type logical and shall be conformable with\n  **array**.\n\n- **kind**\n  : (optional) shall be a scalar integer initialization expression.\n\n- **back**\n  : (optional) shall be a logical scalar.\n\n### **Result**\n\n**kind** is present, the kind type\nparameter is that specified by the value of **kind**; otherwise the kind\ntype parameter is that of default integer type. If **dim** does not appear,\nthe result is an array of rank one and of size equal to the rank of\n**array**; otherwise, the result is of rank n - 1 and shape\n```\n   [d1, d2, . . ., dDIM-1, dDIM+1, . . ., dn ]\n```\nwhere\n```\n   [d1, d2, . . ., dn ]\n```\nis the shape of **array**.\n\n### **Result**\n\n- **Case (i):**\n  The result of **findloc (array, value)** is a rank-one array whose\n  element values are the values of the subscripts of an element of\n  **array** whose value matches **value**. If there is such a value, the\n  ith subscript returned lies in the range 1 to ei, where ei is the\n  extent of the ith dimension of **array**. If no elements match **value**\n  or **array** has size zero, all elements of the result are zero.\n\n- **Case (ii):**\n  the result of **findloc (array, value, mask = mask)** is a\n  rank-one array whose element values are the values of the subscripts\n  of an element of **array**, corresponding to a true element of **mask**,\n  whose value matches **value**. If there is such a value, the ith\n  subscript returned lies in the range 1 to ei, where ei is the\n  extent of the ith dimension of **array**. If no elements match\n  **value**, **array** has size zero, or every element of **mask** has the\n  value false, all elements of the result are zero.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_findloc\nlogical,parameter :: T=.true., F=.false.\ninteger,allocatable :: ibox(:,:)\nlogical,allocatable :: mask(:,:)\n  ! basics\n   ! the first element matching the value is returned AS AN ARRAY\n   call printi('== 6',findloc ([2, 6, 4, 6], value = 6))\n   call printi('== 6',findloc ([2, 6, 4, 6], value = 6,back=.true.))\n   ! the first element matching the value is returned AS A SCALAR\n   call printi('== 6',findloc ([2, 6, 4, 6], value = 6,dim=1))\n   call printi('== 6',findloc ([2, 6, 4, 6], value = 6,back=.true.,dim=1))\n\n   ibox=reshape([ 0,-5,  7, 7, &\n                  3, 4, -1, 2, &\n                  1, 5,  6, 7] ,shape=[3,4],order=[2,1])\n\n   mask=reshape([ T, T, F, T, &\n                  T, T, F, T, &\n                  T, T, F, T] ,shape=[3,4],order=[2,1])\n\n   call printi('array is', ibox )\n   call printl('mask  is', mask )\n   print *, 'so for == 7 and back=.false.'\n   call printi('so for == 7 the address of the element is', &\n           & findloc (ibox, 7, mask = mask) )\n   print *, 'so for == 7 and back=.true.'\n   call printi('so for == 7 the address of the element is', &\n           & findloc (ibox, 7, mask = mask, back=.true.) )\n\n   print *,'This is independent of declared lower bounds for the array'\n\n   print *, ' using dim=N'\n   ibox=reshape([ 1,  2, -9,  &\n                  2,  2,  6 ] ,shape=[2,3],order=[2,1])\n\n   call printi('array is', ibox )\n   ! has the value [2, 1, 0] and\n   call printi('',findloc (ibox, value = 2, dim = 1) )\n   ! has the value [2, 1].\n   call printi('',findloc (ibox, value = 2, dim = 2) )\ncontains\n! GENERIC ROUTINES TO PRINT MATRICES\nsubroutine printl(title,a)\nimplicit none\n!@(#) print small 2d logical scalar, vector, matrix in row-column format\ncharacter(len=*),intent(in)  :: title\nlogical,intent(in)           :: a(..)\n\ncharacter(len=*),parameter   :: row='(\" > [ \",*(l1:,\",\"))'\ncharacter(len=*),parameter   :: all='(\" \",*(g0,1x))'\nlogical,allocatable          :: b(:,:)\ninteger                      :: i\n   write(*,all,advance='no')trim(title)\n   ! copy everything to a matrix to keep code simple\n   select rank(a)\n   rank (0); write(*,'(a)')' (a scalar)'; b=reshape([a],[1,1])\n   rank (1); write(*,'(a)')' (a vector)'; b=reshape(a,[size(a),1])\n   rank (2); write(*,'(a)')' (a matrix)'; b=a\n   rank default; stop '*printl* unexpected rank'\n   end select\n   do i=1,size(b,dim=1)\n      write(*,fmt=row,advance='no')b(i,:)\n      write(*,'(\" ]\")')\n   enddo\n   write(*,all) '>shape=',shape(a),',rank=',rank(a),',size=',size(a)\n   write(*,*)\nend subroutine printl\n\nsubroutine printi(title,a)\nimplicit none\n!@(#) print small 2d integer scalar, vector, matrix in row-column format\ncharacter(len=*),intent(in)  :: title\ninteger,intent(in)           :: a(..)\ncharacter(len=*),parameter   :: all='(\" \",*(g0,1x))'\ncharacter(len=20)            :: row\ninteger,allocatable          :: b(:,:)\ninteger                      :: i\n   write(*,all,advance='no')trim(title)\n   ! copy everything to a matrix to keep code simple\n   select rank(a)\n   rank (0); write(*,'(a)')' (a scalar)'; b=reshape([a],[1,1])\n   rank (1); write(*,'(a)')' (a vector)'; b=reshape(a,[size(a),1])\n   rank (2); write(*,'(a)')' (a matrix)'; b=a\n   rank default; stop '*printi* unexpected rank'\n   end select\n   ! find how many characters to use for integers\n   write(row,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(b))))))+2\n   ! use this format to write a row\n   row='(\" > [\",*(i'//trim(row)//':,\",\"))'\n   do i=1,size(b,dim=1)\n      write(*,fmt=row,advance='no')b(i,:)\n      write(*,'(\" ]\")')\n   enddo\n   write(*,all) '>shape=',shape(a),',rank=',rank(a),',size=',size(a)\n   write(*,*)\nend subroutine printi\nend program demo_findloc\n```\nResults:\n```text\n >  == 6  (a vector)\n >  > [  2 ]\n >  >shape= 1 ,rank= 1 ,size= 1\n >\n >  == 6  (a vector)\n >  > [  4 ]\n >  >shape= 1 ,rank= 1 ,size= 1\n >\n >  == 6  (a scalar)\n >  > [  2 ]\n >  >shape= ,rank= 0 ,size= 1\n >\n >  == 6  (a scalar)\n >  > [  4 ]\n >  >shape= ,rank= 0 ,size= 1\n >\n >  array is  (a matrix)\n >  > [  0, -5,  7,  7 ]\n >  > [  3,  4, -1,  2 ]\n >  > [  1,  5,  6,  7 ]\n >  >shape= 3 4 ,rank= 2 ,size= 12\n >\n >  mask  is  (a matrix)\n >  > [ T,T,F,T ]\n >  > [ T,T,F,T ]\n >  > [ T,T,F,T ]\n >  >shape= 3 4 ,rank= 2 ,size= 12\n >\n >  so for == 7 and back=.false.\n >  so for == 7 the address of the element is  (a vector)\n >  > [  1 ]\n >  > [  4 ]\n >  >shape= 2 ,rank= 1 ,size= 2\n >\n >  so for == 7 and back=.true.\n >  so for == 7 the address of the element is  (a vector)\n >  > [  3 ]\n >  > [  4 ]\n >  >shape= 2 ,rank= 1 ,size= 2\n >\n >  This is independent of declared lower bounds for the array\n >   using dim=N\n >  array is  (a matrix)\n >  > [  1,  2, -9 ]\n >  > [  2,  2,  6 ]\n >  >shape= 2 3 ,rank= 2 ,size= 6\n >\n >    (a vector)\n >  > [  2 ]\n >  > [  1 ]\n >  > [  0 ]\n >  >shape= 3 ,rank= 1 ,size= 3\n >\n >    (a vector)\n >  > [  2 ]\n >  > [  1 ]\n >  >shape= 2 ,rank= 1 ,size= 2\n >\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n - [**maxloc**(3)](#maxloc) - Location of the maximum value within an array\n - [**minloc**(3)](#minloc) - Location of the minimum value within an array\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "FLOOR": "## floor\n\n### **Name**\n\n**floor** - \\[NUMERIC\\] Function to return largest integral value\nnot greater than argument\n\n### **Synopsis**\n```fortran\n    result = floor(a [,kind])\n```\n```fortran\n     elemental integer(kind=KIND) function floor( a ,kind )\n\n      real(kind=**),intent(in) :: a\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- a kind designated as ** may be any supported kind for the type\n- **a** is a _real_ of any kind\n- _KIND_ is any valid value for type _integer_.\n- the result is an _integer_ of the specified or default kind\n\n### **Description**\n\n**floor** returns the greatest integer less than or equal to **a**.\n\nIn other words, it picks the whole number at or to the left of the value on\nthe number line.\n\nThis means care has to be taken that the magnitude of the _real_ value **a**\ndoes not exceed the range of the output value, as the range of values supported\nby _real_ values is typically larger than the range for _integers_.\n\n### **Options**\n\n- **a**\n  : The value to operate on. Valid values are restricted by the size of\n  the returned _integer_ kind to the range **-huge(int(a,kind=KIND))-1**\n  to **huge(int(a),kind=KIND)**.\n\n- **kind**\n  : A scalar _integer_ constant initialization expression\n  indicating the kind parameter of the result.\n\n### **Result**\n\nThe return value is of type _integer(kind)_ if **kind** is present and of\ndefault-kind _integer_ otherwise.\n\nThe result is undefined if it cannot be represented in the specified\ninteger type.\n\nIf in range for the kind of the result the result is the whole number\nat or to the left of the input value on the number line.\n\nIf **a** is positive the result is the value with the fractional part\nremoved.\n\nIf **a** is negative, it is the whole number at or to the left of the\ninput value.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_floor\nimplicit none\nreal :: x = 63.29\nreal :: y = -63.59\n    print *, x, floor(x)\n    print *, y, floor(y)\n   ! elemental\n   print *,floor([ &\n   &  -2.7,  -2.5, -2.2, -2.0, -1.5, -1.0, -0.5, &\n   &  0.0,   &\n   &  +0.5,  +1.0, +1.5, +2.0, +2.2, +2.5, +2.7  ])\n\n   ! note even a small deviation from the whole number changes the result\n   print *,      [2.0,2.0-epsilon(0.0),2.0-2*epsilon(0.0)]\n   print *,floor([2.0,2.0-epsilon(0.0),2.0-2*epsilon(0.0)])\n\n   ! A=Nan, Infinity or  <huge(0_KIND)-1 < A > huge(0_KIND) is undefined\nend program demo_floor\n```\nResults:\n```text\n >     63.29000             63\n >    -63.59000            -64\n >            -3         -3         -3         -2         -2         -1\n >            -1          0          0          1          1          2\n >             2          2          2\n >     2.000000      2.000000      2.000000\n >             2          1          1\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**ceiling**(3)](#ceiling),\n[**nint**(3)](#nint),\n[**aint**(3)](#aint),\n[**anint**(3)](#anint),\n[**int**(3)](#int),\n[**selected_int_kind**(3)](#selected_int_kind)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n<!--\nreal function floor(fval0)\n!@(#) return largest integer not greater than x as a real\n   fval=fval0\n   if(fval.ne.float(int(fval))) then\n      if(fval.gt.0.0) fval = int(fval)\n      if(fval.lt.0.0) fval = int(fval)-1\n   endif\n   floor=fval\nend function floor\n-->\n",
     "FRACTION": "## fraction\n\n### **Name**\n\n**fraction** - \\[MODEL_COMPONENTS\\] Fractional part of the model representation\n\n### **Synopsis**\n```fortran\n    result = fraction(x)\n```\n```fortran\n     elemental real(kind=KIND) function fraction(x)\n\n      real(kind=KIND),intent(in) :: fraction\n```\n### **Characteristics**\n\n  - **x** is of type _real_\n  - The result has the same characteristics as the argument.\n\n### **Description**\n\n  **fraction** returns the fractional part of the model representation\n  of **x**.\n\n### **Options**\n\n- **x**\n  : The value to interrogate\n\n### **Result**\n\nThe fractional part of the model representation of **x** is returned;\nit is **x \\* radix(x)\\*\\*(-exponent(x))**.\n\nIf **x** has the value zero, the result is zero.\n\nIf **x** is an IEEE NaN, the result is that NaN.\n\nIf **x** is an IEEE infinity, the result is an IEEE NaN.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_fraction\nimplicit none\nreal :: x\n   x = 178.1387e-4\n   print *, fraction(x), x * radix(x)**(-exponent(x))\nend program demo_fraction\n```\nResults:\n```text\n     0.5700439      0.5700439\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions_\n",
-    "GAMMA": "## gamma\n\n### **Name**\n\n**gamma** - \\[MATHEMATICS\\] Gamma function, which yields factorials for positive whole numbers\n\n### **Synopsis**\n```fortran\n    result = gamma(x)\n```\n```fortran\n     elemental real(kind=KIND) function gamma( x)\n\n      type(real,kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** is a _real_ value\n - returns a _real_ value with the kind as **x**.\n\n### **Description**\n\n  **gamma(x)** computes Gamma of **x**. For positive whole number values of **n** the\n  Gamma function can be used to calculate factorials, as **(n-1)! == gamma(real(n))**.\n  That is\n```text\nn! == gamma(real(n+1))\n```\n$$\n\\\\__Gamma__(x) = \\\\int\\_0\\*\\*\\\\infty\nt\\*\\*{x-1}{\\\\mathrm{e}}\\*\\*{__-t__}\\\\,{\\\\mathrm{d}}t\n$$\n\n### **Options**\n\n- **x**\n  : Shall be of type _real_ and neither zero nor a negative integer.\n\n### **Result**\n\n  The return value is of type _real_ of the same kind as _x_. The result\n  has a value equal to a processor-dependent approximation to the gamma\n  function of **x**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_gamma\nuse, intrinsic :: iso_fortran_env, only : wp=>real64, int64\nimplicit none\nreal :: x, xa(4)\ninteger :: i, j\n\n   ! basic usage\n   x = gamma(1.0)\n   write(*,*)'gamma(1.0)=',x\n\n   ! elemental\n   xa=gamma([1.0,2.0,3.0,4.0])\n   write(*,*)xa\n   write(*,*)\n\n\n   ! gamma() is related to the factorial function\n   do i = 1, 171\n      ! check value is not too big for default integer type\n      if (factorial(i)  <=  huge(0)) then\n         write(*,*) i, nint(factorial(i)), 'integer'\n      elseif (factorial(i)  <=  huge(0_int64)) then\n         write(*,*) i, nint(factorial(i),kind=int64),'integer(kind=int64)'\n      else\n         write(*,*) i, factorial(i) , 'user factorial function'\n         write(*,*) i, product([(real(j, kind=wp), j=1, i)]), 'product'\n         write(*,*) i, gamma(real(i + 1, kind=wp)), 'gamma directly'\n      endif\n   enddo\n\n\ncontains\nfunction factorial(i) result(f)\n!  GAMMA(X) computes Gamma of X. For positive whole number values of N the\n!  Gamma function can be used to calculate factorials, as (N-1)! ==\n!  GAMMA(REAL(N)). That is\n!\n!      n! == gamma(real(n+1))\n!\ninteger, intent(in) :: i\nreal(kind=wp) :: f\n   if (i  <=  0) then\n      write(*,'(*(g0))') '<ERROR> gamma(3) function value ', i, ' <= 0'\n      stop '<STOP> bad value in gamma function'\n   endif\n   f = anint(gamma(real(i + 1,kind=wp)))\nend function factorial\n\nend program demo_gamma\n```\nResults:\n```text\n >  gamma(1.0)=   1.00000000    \n >    1.00000000       1.00000000       2.00000000       6.00000000    \n > \n >            1           1 integer\n >            2           2 integer\n >            3           6 integer\n >            4          24 integer\n >            5         120 integer\n >            6         720 integer\n >            7        5040 integer\n >            8       40320 integer\n >            9      362880 integer\n >           10     3628800 integer\n >           11    39916800 integer\n >           12   479001600 integer\n >           13           6227020800 integer(kind=int64)\n >           14          87178291200 integer(kind=int64)\n >           15        1307674368000 integer(kind=int64)\n >           16       20922789888000 integer(kind=int64)\n >           17      355687428096000 integer(kind=int64)\n >           18     6402373705728001 integer(kind=int64)\n >           19   121645100408832000 integer(kind=int64)\n >           20  2432902008176640000 integer(kind=int64)\n >           21   5.1090942171709440E+019 user factorial function\n >           21   5.1090942171709440E+019 product\n >           21   5.1090942171709440E+019 gamma directly\n >            :\n >            :\n >            :\n >          170   7.2574156153079990E+306 user factorial function\n >          170   7.2574156153079940E+306 product\n >          170   7.2574156153079990E+306 gamma directly\n >          171                  Infinity user factorial function\n >          171                  Infinity product\n >          171                  Infinity gamma directly\n```\n\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\nLogarithm of the Gamma function: [**log_gamma**(3)](#log_gamma)\n\n### **Resources**\n\n[Wikipedia: Gamma_function](https://en.wikipedia.org/wiki/Gamma_function)\n\n _fortran-lang intrinsic descriptions_\n",
+    "GAMMA": "## gamma\n\n### **Name**\n\n**gamma** - \\[MATHEMATICS\\] Gamma function, which yields factorials for positive whole numbers\n\n### **Synopsis**\n```fortran\n    result = gamma(x)\n```\n```fortran\n     elemental real(kind=**) function gamma( x)\n\n      type(real,kind=**),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** is a _real_ value of any available KIND\n - returns a _real_ value with the same kind as **x**.\n\n### **Description**\n\n  **gamma(x)** computes Gamma of **x**. For positive whole number values of **n** the\n  Gamma function can be used to calculate factorials, as **(n-1)! == gamma(real(n))**.\n  That is\n```text\nn! == gamma(real(n+1))\n```\n$$\n\\\\__Gamma__(x) = \\\\int\\_0\\*\\*\\\\infty\nt\\*\\*{x-1}{\\\\mathrm{e}}\\*\\*{__-t__}\\\\,{\\\\mathrm{d}}t\n$$\n\n### **Options**\n\n- **x**\n  : Shall be of type _real_ and neither zero nor a negative integer.\n\n### **Result**\n\n  The return value is of type _real_ of the same kind as _x_. The result\n  has a value equal to a processor-dependent approximation to the gamma\n  function of **x**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_gamma\nuse, intrinsic :: iso_fortran_env, only : wp=>real64, int64\nimplicit none\nreal :: x, xa(4)\ninteger :: i, j\n\n   ! basic usage\n   x = gamma(1.0)\n   write(*,*)'gamma(1.0)=',x\n\n   ! elemental\n   xa=gamma([1.0,2.0,3.0,4.0])\n   write(*,*)xa\n   write(*,*)\n\n\n   ! gamma() is related to the factorial function\n   do i = 1, 171\n      ! check value is not too big for default integer type\n      if (factorial(i)  <=  huge(0)) then\n         write(*,*) i, nint(factorial(i)), 'integer'\n      elseif (factorial(i)  <=  huge(0_int64)) then\n         write(*,*) i, nint(factorial(i),kind=int64),'integer(kind=int64)'\n      else\n         write(*,*) i, factorial(i) , 'user factorial function'\n         write(*,*) i, product([(real(j, kind=wp), j=1, i)]), 'product'\n         write(*,*) i, gamma(real(i + 1, kind=wp)), 'gamma directly'\n      endif\n   enddo\n\n\ncontains\nfunction factorial(i) result(f)\n!  GAMMA(X) computes Gamma of X. For positive whole number values of N the\n!  Gamma function can be used to calculate factorials, as (N-1)! ==\n!  GAMMA(REAL(N)). That is\n!\n!      n! == gamma(real(n+1))\n!\ninteger, intent(in) :: i\nreal(kind=wp) :: f\n   if (i  <=  0) then\n      write(*,'(*(g0))') '<ERROR> gamma(3) function value ', i, ' <= 0'\n      stop '<STOP> bad value in gamma function'\n   endif\n   f = anint(gamma(real(i + 1,kind=wp)))\nend function factorial\n\nend program demo_gamma\n```\nResults:\n```text\n >  gamma(1.0)=   1.00000000\n >    1.00000000       1.00000000       2.00000000       6.00000000\n >\n >            1           1 integer\n >            2           2 integer\n >            3           6 integer\n >            4          24 integer\n >            5         120 integer\n >            6         720 integer\n >            7        5040 integer\n >            8       40320 integer\n >            9      362880 integer\n >           10     3628800 integer\n >           11    39916800 integer\n >           12   479001600 integer\n >           13           6227020800 integer(kind=int64)\n >           14          87178291200 integer(kind=int64)\n >           15        1307674368000 integer(kind=int64)\n >           16       20922789888000 integer(kind=int64)\n >           17      355687428096000 integer(kind=int64)\n >           18     6402373705728001 integer(kind=int64)\n >           19   121645100408832000 integer(kind=int64)\n >           20  2432902008176640000 integer(kind=int64)\n >           21   5.1090942171709440E+019 user factorial function\n >           21   5.1090942171709440E+019 product\n >           21   5.1090942171709440E+019 gamma directly\n >            :\n >            :\n >            :\n >          170   7.2574156153079990E+306 user factorial function\n >          170   7.2574156153079940E+306 product\n >          170   7.2574156153079990E+306 gamma directly\n >          171                  Infinity user factorial function\n >          171                  Infinity product\n >          171                  Infinity gamma directly\n```\n\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\nLogarithm of the Gamma function: [**log_gamma**(3)](#log_gamma)\n\n### **Resources**\n\n[Wikipedia: Gamma_function](https://en.wikipedia.org/wiki/Gamma_function)\n\n _fortran-lang intrinsic descriptions_\n",
     "GET_COMMAND": "## get_command\n\n### **Name**\n\n**get_command** - \\[SYSTEM:COMMAND LINE\\] Get the entire command line invocation\n\n### **Synopsis**\n```fortran\n    call get_command([command] [,length] [,status] [,errmsg])\n```\n```fortran\n     subroutine get_command( command ,length ,status, errmsg )\n\n      character(len=*),intent(out),optional   :: command\n      integer(kind=**),intent(out),optional   :: length\n      integer(kind=**),intent(out),optional   :: status\n      character(len=*),intent(inout),optional :: errmsg\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n   meeting the conditions described herein.\n - **command** and **errmsg** are scalar _character_ variables of default kind.\n - **length** and **status** are scalar _integer_ with a decimal exponent\n   range of at least four.\n\n### **Description**\n\n**get_command** retrieves the entire command line that was used to\ninvoke the program.\n\nNote that what is typed on the command line is often processed by\na shell. The shell typically processes special characters and white\nspace before passing it to the program. The processing can typically be\nturned off by turning off globbing or quoting the command line arguments\nand/or changing the default field separators, but this should rarely\nbe necessary.\n\n### **Result**\n\n- **command**\n  : If **command** is present, the entire command line that was used\n  to invoke the program is stored into it. If the command cannot be\n  determined, **command** is assigned all blanks.\n\n- **length**\n  : If **length** is present, it is assigned the length of the command line.\n  It is system-dependent as to whether trailing blanks will be counted.\n  : If the command length cannot be determined, a length of 0 is assigned.\n\n- **status**\n  : If **status** is present, it is assigned 0 upon success of the\n  command, **-1** if **command** is too short to store the command line,\n  or a positive value in case of an error.\n\n- **errmsg**\n  : It is assigned a processor-dependent explanatory message if the\n  command retrieval fails. Otherwise, it is unchanged.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_get_command\nimplicit none\ninteger                      :: command_line_length\ncharacter(len=:),allocatable :: command_line\n   ! get command line length\n   call get_command(length=command_line_length)\n   ! allocate string big enough to hold command line\n   allocate(character(len=command_line_length) :: command_line)\n   ! get command line as a string\n   call get_command(command=command_line)\n   ! trim leading spaces just in case\n   command_line=adjustl(command_line)\n   write(*,'(\"OUTPUT:\",a)')command_line\nend program demo_get_command\n```\nResults:\n```bash\n     # note that shell expansion removes some of the whitespace\n     # without quotes\n     ./test_get_command  arguments    on command   line to   echo\n\n     OUTPUT:./test_get_command arguments on command line to echo\n\n     # using the bash shell with single quotes\n     ./test_get_command  'arguments  *><`~[]!{}?\"\\'| '\n\n     OUTPUT:./test_get_command arguments  *><`~[]!{}?\"'|\n```\n### **Standard**\n\nFortran 2003\n\n### **See Also**\n\n[**get_command_argument**(3)](#get_command_argument),\n[**command_argument_count**(3)](#command_argument_count)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n#\n",
     "GET_COMMAND_ARGUMENT": "## get_command_argument\n\n### **Name**\n\n**get_command_argument** - \\[SYSTEM:COMMAND LINE\\] Get command line arguments\n\n### **Synopsis**\n```fortran\n  call get_command_argument(number [,value] [,length] &\n  & [,status] [,errmsg])\n```\n```fortran\n   subroutine get_command_argument( number, value, length, &\n   & status ,errmsg)\n\n    integer(kind=**),intent(in)             :: number\n    character(len=*),intent(out),optional   :: value\n    integer(kind=**),intent(out),optional   :: length\n    integer(kind=**),intent(out),optional   :: status\n    character(len=*),intent(inout),optional :: errmsg\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n   meeting the conditions described herein.\n - **number**, **length**, and **status** are scalar _integer_\n   with a decimal exponent range of at least four.\n - **value** and **errmsg** are scalar _character_ variables of default\n   kind.\n\n### **Description**\n\n**get_command_argument** retrieves or queries the n-th argument that\nwas passed on the command line to the current program execution.\n\nThere is not anything specifically stated about what an argument is but\nin practice the arguments are strings split on whitespace unless the\narguments are quoted. IFS values (Internal Field Separators) used by\ncommon shells are typically ignored and unquoted whitespace is almost\nalways the separator.\n\nShells have often expanded command arguments and spell characters before\npassing them to the program, so the strings read are often not exactly\nwhat the user typed on the command line.\n\n### **Options**\n\n- **number**\n  : is a non-negative number indicating which argument of the current\n  program command line is to be retrieved or queried.\n  : If **number = 0**, the argument pointed to is set to the name of the\n  program (on systems that support this feature).\n  : if the processor does not have such a concept as a command name the\n  value of command argument 0 is processor dependent.\n  : For values from 1 to the number of arguments passed to the program a\n  value is returned in an order determined by the processor. Conventionally\n  they are returned consecutively as they appear on the command line from\n  left to right.\n\n### **Result**\n\n- **value**\n  : The **value** argument holds the command line argument.\n  If **value** can not hold the argument, it is truncated to fit the\n  length of **value**.\n  : If there are less than **number** arguments specified at the command\n  line or if the argument specified does not exist for other reasons,\n  **value** will be filled with blanks.\n\n- **length**\n  : The **length** argument contains the length of the n-th command\n  line argument. The length of **value** has no effect on this value,\n  It is the length required to hold all the significant characters of\n  the argument regardless of how much storage is provided by **value**.\n\n- **status**\n  : If the argument retrieval fails, **status** is a positive number;\n  if **value** contains a truncated command line argument, **status**\n  is **-1**; and otherwise the **status** is zero.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_get_command_argument\nimplicit none\ncharacter(len=255)           :: progname\ninteger                      :: count, i, argument_length, istat\ncharacter(len=:),allocatable :: arg\n\n ! command name assuming it is less than 255 characters in length\n  call get_command_argument (0, progname, status=istat)\n  if (istat == 0) then\n     print *, \"The program's name is \" // trim (progname)\n  else\n     print *, \"Could not get the program's name \" // trim (progname)\n  endif\n\n ! get number of arguments\n  count = command_argument_count()\n  write(*,*)'The number of arguments is ',count\n\n  !\n  ! allocate string array big enough to hold command line\n  ! argument strings and related information\n  !\n  do i=1,count\n     call get_command_argument(number=i,length=argument_length)\n     if(allocated(arg))deallocate(arg)\n     allocate(character(len=argument_length) :: arg)\n     call get_command_argument(i, arg,status=istat)\n     ! show the results\n     write (*,'(i3.3,1x,i0.5,1x,i0.5,1x,\"[\",a,\"]\")') &\n     & i,istat,argument_length,arg\n  enddo\n\nend program demo_get_command_argument\n```\nResults:\n```text\n./demo_get_command_argument a  test 'of getting  arguments ' \" leading\"\n```\n```text\n The program's name is ./demo_get_command_argument\n The number of arguments is            4\n001 00000 00001 [a]\n002 00000 00004 [test]\n003 00000 00022 [of getting  arguments ]\n004 00000 00008 [ leading]\n```\n### **Standard**\n\nFortran 2003\n\n### **See Also**\n\n[**get_command**(3)](#get_command),\n[**command_argument_count**(3)](#command_argument_count)\n\n_fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n#\n",
     "GET_ENVIRONMENT_VARIABLE": "## get_environment_variable\n\n### **Name**\n\n**get_environment_variable** - \\[SYSTEM:ENVIRONMENT\\] Get value of an environment variable\n\n### **Synopsis**\n```fortran\n    call get_environment_variable(name [,value] [,length] &\n    & [,status] [,trim_name] [,errmsg] )\n```\n```fortran\n     subroutine character(len=*) get_environment_variable( &\n     & name, value, length, status, trim_name, errmsg )\n\n      character(len=*),intent(in) :: name\n      character(len=*),intent(out),optional   :: value\n      integer(kind=**),intent(out),optional   :: length\n      integer(kind=**),intent(out),optional   :: status\n      logical,intent(out),optional            :: trim_name\n      character(len=*),intent(inout),optional :: errmsg\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n   meeting the conditions described herein.\n - **name**, **value**, and **errmsg**  are a scalar _character_ of\n   default kind.\n - **length** and **status** are _integer_ scalars with a decimal exponent\n   range of at least four.\n - **trim_name** is a scalar of type _logical_ and of default kind.\n\n### **Description**\n\n**get_environment_variable** gets the **value** of the environment\nvariable **name**.\n\nNote that **get_environment_variable** need not be thread-safe. It\nis the responsibility of the user to ensure that the environment is not\nbeing updated concurrently.\n\nIf running in parallel be aware\nIt is processor dependent whether an environment variable that exists\non an image also exists on another image, and if it does exist on both\nimages whether the values are the same or different.\n\n### **Options**\n\n- **name**\n  : The name of the environment variable to query.\n  The interpretation of case is processor dependent.\n\n### **Result**\n\n- **value**\n  : The value of the environment variable being queried. If **value**\n  is not large enough to hold the data, it is truncated. If the variable\n  **name** is not set or has no value, or the processor does not support\n  environment variables **value** will be filled with blanks.\n\n- **length**\n  : Argument **length** contains the length needed for storing the\n  environment variable **name**. It is zero if the environment variable\n  is not set.\n\n- **status**\n  : **status** is **-1** if **value** is present but too short for the\n  environment variable; it is **1** if the environment variable does\n  not exist and **2** if the processor does not support environment\n  variables; in all other cases **status** is zero.\n\n- **trim_name**\n  : If **trim_name** is present with the value _.false._, the trailing\n  blanks in **name** are significant; otherwise they are not part of\n  the environment variable name.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_getenv\nimplicit none\ncharacter(len=:),allocatable :: homedir\ncharacter(len=:),allocatable :: var\n\n     var='HOME'\n     homedir=get_env(var)\n     write (*,'(a,\"=\"\"\",a,\"\"\"\")')var,homedir\n\ncontains\n\nfunction get_env(name,default) result(value)\n! a function that makes calling get_environment_variable(3) simple\nimplicit none\ncharacter(len=*),intent(in)          :: name\ncharacter(len=*),intent(in),optional :: default\ncharacter(len=:),allocatable         :: value\ninteger                              :: howbig\ninteger                              :: stat\ninteger                              :: length\n   length=0\n   value=''\n   if(name.ne.'')then\n      call get_environment_variable( name, &\n      & length=howbig,status=stat,trim_name=.true.)\n      select case (stat)\n      case (1)\n       print *, name, \" is not defined in the environment. Strange...\"\n       value=''\n      case (2)\n       print *, &\n       \"This processor does not support environment variables. Boooh!\"\n       value=''\n      case default\n       ! make string of sufficient size to hold value\n       if(allocated(value))deallocate(value)\n       allocate(character(len=max(howbig,1)) :: value)\n       ! get value\n       call get_environment_variable( &\n       & name,value,status=stat,trim_name=.true.)\n       if(stat.ne.0)value=''\n      end select\n   endif\n   if(value.eq.''.and.present(default))value=default\nend function get_env\n\nend program demo_getenv\n```\nTypical Results:\n```text\n   HOME=\"/home/urbanjs\"\n```\n### **Standard**\n\nFortran 2003\n\n### **See also**\n\n[**get_command_argument**(3)](#get_command_argument),\n[**get_command**(3)](#get_command)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n#\n",
     "HUGE": "## huge\n\n### **Name**\n\n**huge** - \\[NUMERIC MODEL\\] Largest number of a type and kind\n\n### **Synopsis**\n```fortran\n    result = huge(x)\n```\n```fortran\n     TYPE(kind=KIND) function huge(x)\n\n      TYPE(kind=KIND),intent(in) :: x(..)\n```\n### **Characteristics**\n\n - **x** may be any _real_ or _integer_ scalar or array and any kind.\n - The result will be a scalar of the same type and kind as the input **x**\n\n### **Description**\n\n  **huge** returns the largest number that is not an overflow\n  for the kind and type of **x**.\n\n### **Options**\n\n- **x**\n  : **x** is an arbitrary value which is used merely to determine what\n  _kind_ and _type_ of scalar is being queried. It need not be defined,\n  as only its characteristics are used.\n\n### **Result**\n\n  The result is the largest value supported by the specified type\n  and kind.\n\n  Note the result is as the same kind as the input to ensure the returned\n  value does not overflow. Any assignment of the result to a variable\n  should take this into consideration.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_huge\nimplicit none\ncharacter(len=*),parameter :: f='(i2,1x,2(i11,1x),f14.0:,1x,l1,1x,a)'\ninteger :: i,j,k,biggest\nreal :: v, w\ndoubleprecision :: tally\n   ! basic\n   print *, huge(0), huge(0.0), huge(0.0d0)\n   print *, tiny(0.0), tiny(0.0d0)\n\n   tally=0.0d0\n   ! note subtracting one because counter is the end value+1 on exit\n   do i=0,huge(0)-1\n      tally=tally+i\n   enddo\n   write(*,*)'tally=',tally\n\n   ! advanced\n   biggest=huge(0)\n   ! be careful of overflow when using integers in computation\n   do i=1,14\n      j=6**i   ! Danger, Danger\n      w=6**i   ! Danger, Danger\n      v=6.0**i\n      k=v      ! Danger, Danger\n\n      if(v.gt.biggest)then\n         write(*,f) i, j, k, v, v.eq.w, 'wrong j and k and w'\n      else\n         write(*,f) i, j, k, v, v.eq.w\n      endif\n\n   enddo\nend program demo_huge\n```\nResults:\n```\n  2147483647  3.4028235E+38  1.797693134862316E+308\n  1.1754944E-38  2.225073858507201E-308\n\n    1      6           6             6. T\n    2      36          36            36. T\n    3      216         216           216. T\n    4      1296        1296          1296. T\n    5      7776        7776          7776. T\n    6      46656       46656         46656. T\n    7      279936      279936        279936. T\n    8      1679616     1679616       1679616. T\n    9      10077696    10077696      10077696. T\n    10     60466176    60466176      60466176. T\n    11     362797056   362797056     362797056. T\n    12    -2118184960 -2147483648    2176782336. F wrong for j and k and w\n    13     175792128  -2147483648   13060694016. F wrong for j and k and w\n    14     1054752768 -2147483648   78364164096. F wrong for j and k and w\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "HYPOT": "## hypot\n\n### **Name**\n\n**hypot** - \\[MATHEMATICS\\] Returns the Euclidean distance - the distance between a point and the origin.\n\n### **Synopsis**\n```fortran\n    result = hypot(x, y)\n```\n```fortran\n     elemental real(kind=KIND) function hypot(x,y)\n\n      real(kind=KIND),intent(in) :: x\n      real(kind=KIND),intent(in) :: y\n```\n### **Characteristics**\n\n - **x,y** and the result shall all be _real_ and of the same **kind**.\n\n### **Description**\n\n**hypot** is referred to as the Euclidean distance function. It is\nequal to\n```fortran\nsqrt(x**2+y**2)\n```\nwithout undue underflow or overflow.\n\nIn mathematics, the _Euclidean distance_ between two points in Euclidean\nspace is the length of a line segment between two points.\n\n**hypot(x,y)** returns the distance between the point **<x,y>** and\nthe origin.\n\n### **Options**\n\n- **x**\n: The type shall be _real_.\n\n- **y**\n  : The type and kind type parameter shall be the same as **x**.\n\n### **Result**\n\nThe return value has the same type and kind type parameter as **x**.\n\nThe result is the positive magnitude of the distance of the point\n**<x,y>** from the origin **<0.0,0.0>** .\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_hypot\nuse, intrinsic :: iso_fortran_env, only : &\n & real_kinds, real32, real64, real128\nimplicit none\nreal(kind=real32) :: x, y\nreal(kind=real32),allocatable :: xs(:), ys(:)\ninteger :: i\ncharacter(len=*),parameter :: f='(a,/,SP,*(3x,g0,1x,g0:,/))'\n\n   x = 1.e0_real32\n   y = 0.5e0_real32\n\n   write(*,*)\n   write(*,'(*(g0))')'point <',x,',',y,'> is ',hypot(x,y)\n   write(*,'(*(g0))')'units away from the origin'\n   write(*,*)\n\n   ! elemental\n   xs=[  x,  x**2,  x*10.0,  x*15.0, -x**2  ]\n   ys=[  y,  y**2, -y*20.0,  y**2,   -y**2  ]\n\n   write(*,f)\"the points\",(xs(i),ys(i),i=1,size(xs))\n   write(*,f)\"have distances from the origin of \",hypot(xs,ys)\n   write(*,f)\"the closest is\",minval(hypot(xs,ys))\n\nend program demo_hypot\n```\n\nResults:\n\n```text\n   point <1.00000000,0.500000000> is 1.11803401\n   units away from the origin\n\n   the points\n      +1.00000000 +0.500000000\n      +1.00000000 +0.250000000\n      +10.0000000 -10.0000000\n      +15.0000000 +0.250000000\n      -1.00000000 -0.250000000\n   have distances from the origin of\n      +1.11803401 +1.03077638\n      +14.1421356 +15.0020828\n      +1.03077638\n   the closest is\n      +1.03077638\n```\n### **Standard**\n\nFortran 2008\n\n### **See also**\n\n[****(3)](#)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "IACHAR": "## iachar\n\n### **Name**\n\n**iachar** - \\[CHARACTER:CONVERSION\\] Return integer ASCII code of a character\n\n### **Synopsis**\n```fortran\n    result = iachar(c [,kind])\n```\n```fortran\n     elemental integer(kind=KIND) function iachar(c,kind)\n\n      character(len=1),intent(in) :: c\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n - **c** is a single character\n - The return value is of type _integer_ and of kind **KIND**. If **KIND**\n   is absent, the return value is of default integer kind.\n\n NOTE:\n : a kind designated as ** may be any supported kind for the type\n\n### **Description**\n\n  **iachar** returns the code for the ASCII character in the first\n  character position of C.\n\n### **Options**\n\n- **c**\n  : A character to determine the ASCII code of.\n  : A common extension is to allow strings but all but the first character\n  is then ignored.\n\n- **kind**\n  : A constant initialization expression indicating the kind\n  parameter of the result.\n\n### **Result**\n\n  the result is the position of the character **c** in the ASCII\n  collating sequence. It is nonnegative and less than or equal to 127.\n\n  By ASCII, it is meant that **c** is in the collating sequence defined\n  by the codes specified in ISO/IEC 646:1991 (International Reference\n  Version).\n\n  The value of the result is processor dependent if **c** is not in the\n  ASCII collating sequence.\n\n  The results are consistent with the **lge**(3), **lgt**(3), **lle**(3),\n  and **llt**(3) comparison functions. For example, if **lle(C, D)**\n  is true, **iachar(C) <= iachar (D)** is true where **C** and **D**\n  are any two characters representable by the processor.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_iachar\nimplicit none\n   ! basic usage\n    ! just does a string one character long\n    write(*,*)iachar('A')\n    ! elemental: can do an array of letters\n    write(*,*)iachar(['A','Z','a','z'])\n\n   ! convert all characters to lowercase\n    write(*,'(a)')lower('abcdefg ABCDEFG')\ncontains\n!\npure elemental function lower(str) result (string)\n! Changes a string to lowercase\ncharacter(*), intent(In)     :: str\ncharacter(len(str))          :: string\ninteger                      :: i\n   string = str\n   ! step thru each letter in the string in specified range\n   do i = 1, len(str)\n      select case (str(i:i))\n      case ('A':'Z') ! change letter to miniscule\n         string(i:i) = char(iachar(str(i:i))+32)\n      case default\n      end select\n   end do\nend function lower\n!\nend program demo_iachar\n```\nResults:\n```text\n   65\n   65          90          97         122\n   abcdefg abcdefg\n```\n### **Standard**\n\n  Fortran 95 , with KIND argument - Fortran 2003\n\n### **See Also**\n\n[**achar**(3)](#achar),\n[**char**(3)](#char),\n[**ichar**(3)](#ichar)\n\n  See [**ichar**(3)](#ichar) in particular for a discussion of converting\n  between numerical values and formatted string representations.\n\n  Functions that perform operations on character strings, return lengths\n  of arguments, and search for certain arguments:\n\n- **Elemental:**\n  [**adjustl**(3)](#adjustl), [**adjustr**(3)](#adjustr), [**index**(3)](#index),\n  [**scan**(3)](#scan), [**verify**(3)](#verify)\n\n- **Nonelemental:**\n  [**len_trim**(3)](#len_trim),\n  [**len**(3)](#len),\n  [**repeat**(3)](#repeat), [**trim**(3)](#trim)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "IALL": "## iall\n\n### **Name**\n\n**iall** - \\[BIT:LOGICAL\\] Bitwise and of array elements\n\n### **Synopsis**\n```fortran\n    result = iall(array [,mask]) | iall(array ,dim [,mask])\n```\n```fortran\n     integer(kind=KIND) function iall(array,dim,mask)\n\n      integer(kind=KIND),intent(in)        :: array(*)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(*)\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **array** must be an _integer_ array\n - **mask** is a _logical_ array that conforms to **array** of any\n   _logical_ kind.\n - **dim** may be of any _integer_ kind.\n - The result will by of the same type and kind as **array**.\n\n### **Description**\n\n  **iall** reduces with a bitwise _and_ the elements of **array** along\n  dimension **dim** if the corresponding element in **mask** is _.true._.\n\n### **Options**\n\n- **array**\n  : Shall be an array of type _integer_\n\n- **dim**\n  : (Optional) shall be a scalar of type _integer_ with a value in the\n  range from **1 to n**, where **n** equals the rank of **array**.\n\n- **mask**\n  : (Optional) shall be of type _logical_ and either be a scalar or an\n  array of the same shape as **array**.\n\n### **Result**\n\n  The result is of the same type as **array**.\n\n  If **dim** is absent, a scalar with the bitwise _all_ of all elements in\n  **array** is returned. Otherwise, an array of rank **n-1**, where **n**\n  equals the rank of **array**, and a shape similar to that of **array**\n  with dimension **dim** dropped is returned.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_iall\nuse, intrinsic :: iso_fortran_env, only : integer_kinds, &\n & int8, int16, int32, int64\nimplicit none\ninteger(kind=int8) :: a(2)\n\n   a(1) = int(b'00100100')\n   a(2) = int(b'01101010')\n\n   print '(b8.8)', iall(a)\n\nend program demo_iall\n```\nResults:\n```text\n > 00100000\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**iany**(3)](#iany),\n[**iparity**(3)](#iparity),\n[**iand**(3)](#iand)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
@@ -126,15 +126,15 @@
     "MASKL": "## maskl\n\n### **Name**\n\n**maskl** - \\[BIT:SET\\] Generates a left justified mask\n\n### **Synopsis**\n```fortran\n    result = maskl( i [,kind] )\n```\n```fortran\n     elemental integer(kind=KIND) function maskl(i,KIND)\n\n      integer(kind=**),intent(in) :: i\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- a kind designated as ** may be any supported kind for the type\n- **i** is an integer\n- **kind** Shall be a scalar constant expression of type _integer_\n  whose value is a supported _integer_ kind.\n- The result is an _integer_ of the same _kind_ as **i** unless **kind** is\n  present, which is then used to specify the kind of the result.\n\n### **Description**\n\n  **maskl** has its leftmost **i** bits set to **1**, and the remaining\n  bits set to **0**.\n\n### **Options**\n\n- **i**\n  : the number of left-most bits to set in the _integer_ result. It\n  must be from 0 to the number of bits for the kind of the result.\n  The default kind of the result is the same as **i** unless the result\n  size is specified by **kind**. That is, these Fortran statements must\n  be _.true._ :\n```fortran\n   i >= 0 .and. i < bitsize(i) ! if KIND is not specified\n   i >= 0 .and. i < bitsize(0_KIND) ! if KIND is specified\n```\n- **kind**\n  : designates the kind of the _integer_ result.\n\n### **Result**\n\n  The leftmost **i** bits of the output _integer_ are set to 1 and the\n  other bits are set to 0.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_maskl\nimplicit none\ninteger :: i\n  ! basics\n   i=3\n   write(*,'(i0,1x,b0)') i, maskl(i)\n\n  ! elemental\n   write(*,'(*(i11,1x,b0.32,1x,/))') maskl([(i,i,i=0,bit_size(0),4)])\nend program demo_maskl\n```\nResults:\n```text\n > 3 11100000000000000000000000000000\n >           0 00000000000000000000000000000000\n >  -268435456 11110000000000000000000000000000\n >   -16777216 11111111000000000000000000000000\n >    -1048576 11111111111100000000000000000000\n >      -65536 11111111111111110000000000000000\n >       -4096 11111111111111111111000000000000\n >        -256 11111111111111111111111100000000\n >         -16 11111111111111111111111111110000\n >          -1 11111111111111111111111111111111\n\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**maskr**(3)](#maskr)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MASKR": "## maskr\n\n### **Name**\n\n**maskr** - \\[BIT:SET\\] Generates a right-justified mask\n\n### **Synopsis**\n```fortran\n    result = maskr( i [,kind] )\n```\n```fortran\n     elemental integer(kind=KIND) function maskr(i,KIND)\n\n      integer(kind=**),intent(in) :: i\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- a kind designated as ** may be any supported kind for the type\n- **i** is an integer\n- **kind** Shall be a scalar constant expression of type _integer_\n  whose value is a supported _integer_ kind.\n- The result is an _integer_ of the same _kind_ as **i** unless **kind** is\n  present, which is then used to specify the kind of the result.\n\n### **Description**\n\n  **maskr** generates an _integer_ with its rightmost **i**\n  bits set to 1, and the remaining bits set to 0.\n\n### **Options**\n\n- **i**\n  : the number of right-most bits to set in the _integer_ result. It\n  must be from 0 to the number of bits for the kind of the result.\n  The default kind of the result is the same as **i** unless the result\n  size is specified by **kind**. That is, these Fortran statements must\n  be _.true._ :\n```fortran\n   i >= 0 .and. i < bitsize(i) ! if KIND is not specified\n   i >= 0 .and. i < bitsize(0_KIND) ! if KIND is specified\n```\n- **kind**\n  : designates the kind of the _integer_ result.\n\n### **Result**\n\n  The rightmost **i** bits of the output _integer_ are set to 1 and the\n  other bits are set to 0.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_maskr\nimplicit none\ninteger :: i\n\n  ! basics\n   print *,'basics'\n   write(*,'(i0,t5,b32.32)') 1, maskr(1)\n   write(*,'(i0,t5,b32.32)') 5,  maskr(5)\n   write(*,'(i0,t5,b32.32)') 11, maskr(11)\n   print *,\"should be equivalent on two's-complement processors\"\n   write(*,'(i0,t5,b32.32)') 1,  shiftr(-1,bit_size(0)-1)\n   write(*,'(i0,t5,b32.32)') 5,  shiftr(-1,bit_size(0)-5)\n   write(*,'(i0,t5,b32.32)') 11, shiftr(-1,bit_size(0)-11)\n\n  ! elemental\n   print *,'elemental '\n   print *,'(array argument accepted like called with each element)'\n   write(*,'(*(i11,1x,b0.32,1x,/))') maskr([(i,i,i=0,bit_size(0),4)])\n\nend program demo_maskr\n```\nResults:\n```text\n >   basics\n >  1   00000000000000000000000000000001\n >  5   00000000000000000000000000011111\n >  11  00000000000000000000011111111111\n >   should be equivalent on two's-complement processors\n >  1   00000000000000000000000000000001\n >  5   00000000000000000000000000011111\n >  11  00000000000000000000011111111111\n >   elemental\n >   (array argument accepted like called with each element)\n >            0 00000000000000000000000000000000\n >           15 00000000000000000000000000001111\n >          255 00000000000000000000000011111111\n >         4095 00000000000000000000111111111111\n >        65535 00000000000000001111111111111111\n >      1048575 00000000000011111111111111111111\n >     16777215 00000000111111111111111111111111\n >    268435455 00001111111111111111111111111111\n >           -1 11111111111111111111111111111111\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**maskl**(3)](#maskl)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MATMUL": "## matmul\n\n### **Name**\n\n**matmul** - \\[TRANSFORMATIONAL\\] Numeric or logical matrix\nmultiplication\n\n### **Synopsis**\n```fortran\n    result = matmul(matrix_a,matrix_b)\n```\n```fortran\n     function matmul(matrix_a, matrix_b)\n\n      type(TYPE1(kind=**))      :: matrix_a(..)\n      type(TYPE2(kind=**))      :: matrix_b(..)\n      type(TYPE(kind=PROMOTED)) :: matmul(..)\n```\n### **Characteristics**\n\n - **matrix_a** is a numeric (_integer_, _real_, or _complex_ ) or\n   _logical_ array of rank one two.\n - **matrix_b** is a numeric (_integer_, _real_, or _complex_ ) or\n   _logical_ array of rank one two.\n - At least one argument must be rank two.\n - the size of the first dimension of **matrix_b** must equal the size\n   of the last dimension of **matrix_a**.\n - the type of the result is the same as if an element of each argument\n   had been multiplied as a RHS expression (that is, if the arguments\n   are not of the same type the result follows the same rules of promotion\n   as a simple scalar multiplication of the two types would produce)\n - If one argument is _logical_, both must be _logical_. For logicals\n   the resulting type is as if the _.and._ operator has been used on\n   elements from the arrays.\n - The shape of the result depends on the shapes of the arguments\n   as described below.\n\n### **Description**\n\n **matmul** performs a matrix multiplication on numeric or logical\n arguments.\n\n### **Options**\n\n- **matrix_a**\n  : A numeric or logical array with a rank of one or two.\n\n- **matrix_b**\n  : A numeric or logical array with a rank of one or two. The last\n  dimension of **matrix_a** and the first dimension of **matrix_b**\n  must be equal.\n\n  Note that **matrix_a** and **matrix_b** may be different numeric\n  types.\n\n### **Result**\n\n####  **Numeric Arguments**\n\n  If **matrix_a** and **matrix_b** are numeric the result is an\n  array containing the conventional matrix product of **matrix_a**\n  and **matrix_b**.\n\n  First, for the numeric expression **C=matmul(A,B)**\n\n   - Any vector **A(n)** is treated as a row vector **A(1,n)**.\n   - Any vector **B(n)** is treated as a column vector **B(n,1)**.\n\n#####  **Shape and Rank**\n\n  The shape of the result can then be determined as the number of rows\n  of the first matrix and the number of columns of the second; but if\n  any argument is of rank one (a vector) the result is also rank one.\n  Conversely when both arguments are of rank two, the result has a rank\n  of two. That is ...\n\n   + If **matrix_a** has shape [n,m] and **matrix_b** has shape [m,k],\n     the result has shape [n,k].\n   + If **matrix_a** has shape [m] and **matrix_b** has shape [m,k],\n     the result has shape [k].\n   + If **matrix_a** has shape [n,m] and **matrix_b** has shape [m],\n     the result has shape [n].\n\n#####  **Values**\n\n  Then element **C(i,j)** of the product is obtained by multiplying\n  term-by-term the entries of the ith row of **A** and the jth column\n  of **B**, and summing these products. In other words, **C(i,j)**\n  is the dot product of the ith row of **A** and the jth column of **B**.\n\n#### **Logical Arguments**\n\n#####  **Values**\n\n  If **matrix_a** and **matrix_b** are of type logical, the array elements\n  of the result are instead:\n```fortran\n  Value_of_Element (i,j) = &\n  ANY( (row_i_of_MATRIX_A) .AND. (column_j_of_MATRIX_B) )\n```\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_matmul\nimplicit none\ninteger :: a(2,3), b(3,2), c(2), d(3), e(2,2), f(3), g(2), v1(4),v2(4)\n   a = reshape([1, 2, 3, 4, 5, 6], [2, 3])\n   b = reshape([10, 20, 30, 40, 50, 60], [3, 2])\n   c = [1, 2]\n   d = [1, 2, 3]\n   e = matmul(a, b)\n   f = matmul(c,a)\n   g = matmul(a,d)\n\n   call print_matrix_int('A is ',a)\n   call print_matrix_int('B is ',b)\n   call print_vector_int('C is ',c)\n   call print_vector_int('D is ',d)\n   call print_matrix_int('E is matmul(A,B)',e)\n   call print_vector_int('F is matmul(C,A)',f)\n   call print_vector_int('G is matmul(A,D)',g)\n\n   ! look at argument shapes when one is a vector\n   write(*,'(\" > shape\")')\n   ! at least one argument must be of rank two\n   ! so for two vectors at least one must be reshaped\n   v1=[11,22,33,44]\n   v2=[10,20,30,40]\n\n   ! these return a vector C(1:1)\n   ! treat A(1:n) as A(1:1,1:n)\n   call print_vector_int('Cd is a vector (not a scalar)',&\n   & matmul(reshape(v1,[1,size(v1)]),v2))\n   ! or treat B(1:m) as B(1:m,1:1)\n   call print_vector_int('cD is a vector too',&\n   & matmul(v1,reshape(v2,[size(v2),1])))\n\n   ! or treat A(1:n) as A(1:1,1:n) and B(1:m) as B(1:m,1:1)\n   ! but note this returns a matrix C(1:1,1:1) not a vector!\n   call print_matrix_int('CD is a matrix',matmul(&\n   & reshape(v1,[1,size(v1)]), &\n   & reshape(v2,[size(v2),1])))\n\ncontains\n\n! CONVENIENCE ROUTINES TO PRINT IN ROW-COLUMN ORDER\nsubroutine print_vector_int(title,arr)\ncharacter(len=*),intent(in)  :: title\ninteger,intent(in)           :: arr(:)\n   call print_matrix_int(title,reshape(arr,[1,shape(arr)]))\nend subroutine print_vector_int\n\nsubroutine print_matrix_int(title,arr)\n!@(#) print small 2d integer arrays in row-column format\ncharacter(len=*),parameter :: all='(\" > \",*(g0,1x))' ! a handy format\ncharacter(len=*),intent(in)  :: title\ninteger,intent(in)           :: arr(:,:)\ninteger                      :: i\ncharacter(len=:),allocatable :: biggest\n\n   print all\n   print all, trim(title)\n   biggest='           '  ! make buffer to write integer into\n   ! find how many characters to use for integers\n   write(biggest,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(arr))))))+2\n   ! use this format to write a row\n   biggest='(\" > [\",*(i'//trim(biggest)//':,\",\"))'\n   ! print one row of array at a time\n   do i=1,size(arr,dim=1)\n      write(*,fmt=biggest,advance='no')arr(i,:)\n      write(*,'(\" ]\")')\n   enddo\n\nend subroutine print_matrix_int\n\nend program demo_matmul\n```\nResults:\n```text\n    >\n    > A is\n    > [  1,  3,  5 ]\n    > [  2,  4,  6 ]\n    >\n    > B is\n    > [  10,  40 ]\n    > [  20,  50 ]\n    > [  30,  60 ]\n    >\n    > C is\n    > [  1,  2 ]\n    >\n    > D is\n    > [  1,  2,  3 ]\n    >\n    > E is matmul(A,B)\n    > [  220,  490 ]\n    > [  280,  640 ]\n    >\n    > F is matmul(C,A)\n    > [   5,  11,  17 ]\n    >\n    > G is matmul(A,D)\n    > [  22,  28 ]\n    > shape\n    >\n    > Cd is a vector (not a scalar)\n    > [  3300 ]\n    >\n    > cD is a vector too\n    > [  3300 ]\n    >\n    > CD is a matrix\n    > [  3300 ]\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**product**(3)](#product),\n[**transpose**(3)](#transpose)\n\n### **Resources**\n\n- [Matrix multiplication : Wikipedia](https://en.wikipedia.org/wiki/Matrix_multiplication)\n- The Winograd variant of Strassen's matrix-matrix multiply algorithm may\n  be of interest for optimizing multiplication of very large matrices. See\n```text\n    \"GEMMW: A portable level 3 BLAS Winograd variant of Strassen's\n    matrix-matrix multiply algorithm\",\n\n    Douglas, C. C., Heroux, M., Slishman, G., and Smith, R. M.,\n    Journal of Computational Physics,\n    Vol. 110, No. 1, January 1994, pages 1-10.\n\n  The numerical instabilities of Strassen's method for matrix\n  multiplication requires special processing.\n```\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MAX": "## max\n\n### **Name**\n\n**max** - \\[NUMERIC\\] Maximum value of an argument list\n\n### **Synopsis**\n```fortran\n    result = max(a1, a2, a3, ...)\n```\n```fortran\n     elemental TYPE(kind=KIND) function max(a1, a2, a3, ... )\n\n      TYPE(kind=KIND,intent(in),optional :: a1\n      TYPE(kind=KIND,intent(in),optional :: a2\n      TYPE(kind=KIND,intent(in),optional :: a3\n                :\n                :\n                :\n```\n### **Characteristics**\n\n - **a3, a3, a4, ...** must be of the same type and kind as **a1**\n - the arguments may (all) be _integer_, _real_ or _character_\n - there must be at least two arguments\n - the length of a character result is the length of the longest argument\n - the type and kind of the result is the same as those of the arguments\n\n### **Description**\n\n  **max** returns the argument with the largest (most positive) value.\n\n  For arguments of character type, the result is as if the arguments had\n  been successively compared with the intrinsic operational operators,\n  taking into account the collating sequence of the _character_ kind.\n\n  If the selected _character_ argument is shorter than the longest\n  argument, the result is as all values were extended with blanks on\n  the right to the length of the longest argument.\n\n  It is unusual for a Fortran intrinsic to take an arbitrary number of\n  options, and in addition **max** is elemental, meaning any number\n  of arguments may be arrays as long as they are of the same shape.\n  The examples have an extended description clarifying the resulting\n  behavior for those not familiar with calling a \"scalar\" function\n  elementally with arrays.\n\n  See maxval(3) for simply getting the max value of an array.\n\n### **Options**\n\n- **a1**\n  : The first argument determines the type and kind of the returned\n  value, and of any remaining arguments as well as being a member of\n  the set of values to find the maximum (most positive) value of.\n\n- **a2,a3,...**\n  : the remaining arguments of which to find the maximum value(s) of.\n  : There must be at least two arguments to **max(3)**.\n\n### **Result**\n\n  The return value corresponds to an array of the same shape of any\n  array argument, or a scalar if all arguments are scalar.\n\n  The returned value when any argument is an array will be an array of\n  the same shape where each element is the maximum value occurring at\n  that location, treating all the scalar values as arrays of that same\n  shape with all elements set to the scalar value.\n\n### **Examples**\n\nSample program\n```fortran\nprogram demo_max\nimplicit none\nreal :: arr1(4)= [10.0,11.0,30.0,-100.0]\nreal :: arr2(5)= [20.0,21.0,32.0,-200.0,2200.0]\ninteger :: box(3,4)= reshape([-6,-5,-4,-3,-2,-1,1,2,3,4,5,6],shape(box))\n\n  ! basic usage\n   ! this is simple enough when all arguments are scalar\n\n   ! the most positive value is returned, not the one with the\n   ! largest magnitude\n   write(*,*)'scalars:',max(10.0,11.0,30.0,-100.0)\n   write(*,*)'scalars:',max(-22222.0,-0.0001)\n\n   ! strings do not need to be of the same length\n   write(*,*)'characters:',max('the','words','order')\n\n   ! leading spaces are significant; everyone is padded on the right\n   ! to the length of the longest argument\n   write(*,*)'characters:',max('c','bb','a')\n   write(*,*)'characters:',max(' c','b','a')\n\n  ! elemental\n   ! there must be at least two arguments, so even if A1 is an array\n   ! max(A1) is not valid. See MAXVAL(3) and/or MAXLOC(3) instead.\n\n   ! strings in a single array do need to be of the same length\n   ! but the different objects can still be of different lengths.\n   write(*,\"(*('\"\"',a,'\"\"':,1x))\")MAX(['A','Z'],['BB','Y '])\n   ! note the result is now an array with the max of every element\n   ! position, as can be illustrated numerically as well:\n   write(*,'(a,*(i3,1x))')'box=   ',box\n   write(*,'(a,*(i3,1x))')'box**2=',sign(1,box)*box**2\n   write(*,'(a,*(i3,1x))')'max    ',max(box,sign(1,box)*box**2)\n\n   ! Remember if any argument is an array by the definition of an\n   ! elemental function all the array arguments must be the same shape.\n\n   ! to find the single largest value of arrays you could use something\n   ! like MAXVAL([arr1, arr2]) or probably better (no large temp array),\n   ! max(maxval(arr1),maxval(arr2)) instead\n\n   ! so this returns an array of the same shape as any input array\n   ! where each result is the maximum that occurs at that position.\n   write(*,*)max(arr1,arr2(1:4))\n   ! this returns an array just like arr1 except all values less than\n   ! zero are set to zero:\n   write(*,*)max(box,0)\n   ! When mixing arrays and scalars you can think of the scalars\n   ! as being a copy of one of the arrays with all values set to\n   ! the scalar value.\n\nend program demo_max\n```\nResults:\n```text\n    scalars:   30.00000\n    scalars: -9.9999997E-05\n    characters:words\n    characters:c\n    characters:b\n   \"BB\" \"Z \"\n   box=    -6  -5  -4  -3  -2  -1   1   2   3   4   5   6\n   box**2=-36 -25 -16  -9  -4  -1   1   4   9  16  25  36\n   max     -6  -5  -4  -3  -2  -1   1   4   9  16  25  36\n   20.00000  21.00000  32.00000  -100.0000\n   0  0  0  0  0  0\n   1  2  3  4  5  6\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n[**maxloc**(3)](#maxloc),\n[**minloc**(3)](#minloc),\n[**maxval**(3)](#maxval),\n[**minval**(3)](#minval),\n[**min**(3)](#min)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MAXEXPONENT": "## maxexponent\n\n### **Name**\n\n**maxexponent** - \\[NUMERIC MODEL\\] Maximum exponent of a real kind\n\n### **Synopsis**\n```fortran\n    result = maxexponent(x)\n```\n```fortran\n     elemental integer function maxexponent(x)\n\n      real(kind=**),intent(in)   :: x\n```\n### **Characteristics**\n\n - **x**  is a _real_ scalar or array of any _real_ kind\n - the result is a default _integer_ scalar\n\n### **Description**\n\n  **maxexponent** returns the maximum exponent in the model of the\n  type of **x**.\n\n### **Options**\n\n- **x**\n  : A value used to select the kind of _real_ to return a value for.\n\n### **Result**\n\n  The value returned is the maximum exponent for the kind of the value\n  queried\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_maxexponent\nuse, intrinsic :: iso_fortran_env, only : real32,real64,real128\nimplicit none\ncharacter(len=*),parameter :: g='(*(g0,1x))'\n   print  g,  minexponent(0.0_real32),   maxexponent(0.0_real32)\n   print  g,  minexponent(0.0_real64),   maxexponent(0.0_real64)\n   print  g,  minexponent(0.0_real128),  maxexponent(0.0_real128)\nend program demo_maxexponent\n```\nResults:\n```text\n   -125 128\n   -1021 1024\n   -16381 16384\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MAXLOC": "## maxloc\n\n### **Name**\n\n**maxloc** - \\[ARRAY:LOCATION\\] Location of the maximum value within an array\n\n### **Synopsis**\n```fortran\n    result = maxloc(array [,mask]) | maxloc(array [,dim] [,mask])\n```\n```fortran\n     NUMERIC function maxloc(array, dim, mask)\n\n      NUMERIC,intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n```\n### **Characteristics**\n\n  - a kind designated as ** may be any supported kind for the type\n  - **NUMERIC** designates any intrinsic numeric type and kind.\n\n### **Description**\n\n**maxloc** determines the location of the element in the array with\nthe maximum value, or, if the **dim** argument is supplied, determines\nthe locations of the maximum element along each row of the array in the\n**dim** direction.\n\nIf **mask** is present, only the elements for which **mask**\nis _.true._ are considered. If more than one element in the array has\nthe maximum value, the location returned is that of the first such element\nin array element order.\n\nIf the array has zero size, or all of the elements\nof **mask** are .false., then the result is an array of zeroes. Similarly,\nif **dim** is supplied and all of the elements of **mask** along a given\nrow are zero, the result value for that row is zero.\n\n### **Options**\n\n- **array**\n  : Shall be an array of type _integer_, _real_, or _character_.\n\n- **dim**\n  : (Optional) Shall be a scalar of type _integer_, with a value between\n  one and the rank of **array**, inclusive. It may not be an optional\n  dummy argument.\n\n- **mask**\n  : Shall be an array of type _logical_, and conformable with **array**.\n\n### **Result**\n\nIf **dim** is absent, the result is a rank-one array with a length equal\nto the rank of **array**. If **dim** is present, the result is an array\nwith a rank one less than the rank of **array**, and a size corresponding\nto the size of **array** with the **dim** dimension removed. If **dim**\nis present and **array** has a rank of one, the result is a scalar. In\nall cases, the result is of default _integer_ type.\n\nThe value returned is reference to the offset from the beginning of the\narray, not necessarily the subscript value if the array subscripts do\nnot start with one.\n\n### **Examples**\n\nsample program\n\n```fortran\nprogram demo_maxloc\nimplicit none\ninteger      :: ii\ninteger,save :: i(-3:3)=[(abs(abs(ii)-50),ii=-3,3)]\ninteger,save :: ints(3,5)= reshape([&\n   1,  2,  3,  4,  5, &\n   10, 20, 30, 40, 50, &\n   11, 22, 33, 44, 55  &\n],shape(ints),order=[2,1])\n\n    write(*,*) maxloc(ints)\n    write(*,*) maxloc(ints,dim=1)\n    write(*,*) maxloc(ints,dim=2)\n    ! when array bounds do not start with one remember MAXLOC(3) returns\n    ! the offset relative to the lower bound-1 of the location of the\n    ! maximum value, not the subscript of the maximum value. When the\n    ! lower bound of the array is one, these values are the same. In\n    ! other words, MAXLOC(3) returns the subscript of the value assuming\n    ! the first subscript of the array is one no matter what the lower\n    ! bound of the subscript actually is.\n    write(*,'(g0,1x,g0)') (ii,i(ii),ii=lbound(i,dim=1),ubound(i,dim=1))\n    write(*,*)maxloc(i)\n\nend program demo_maxloc\n```\n\nResults:\n\n```text\n >     3       5\n >     3       3       3       3       3\n >     5       5       5\n >  -3 47\n >  -2 48\n >  -1 49\n >  0 50\n >  1 49\n >  2 48\n >  3 47\n```\n\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n - [**findloc**(3)](#findloc) - Location of first element of ARRAY\n   identified by MASK along dimension DIM matching a target\n - [**minloc**(3)](#minloc) - Location of the minimum value within an array\n - [**maxval**(3)](#maxval)\n - [**minval**(3)](#minval)\n - [**max**(3)](#max)\n\n _fortran-lang intrinsic descriptions_\n",
     "MAXVAL": "## maxval\n\n### **Name**\n\n**maxval** - \\[ARRAY:REDUCTION\\] Determines the maximum value in an array or row\n\n### **Synopsis**\n```fortran\n    result = maxval(array [,mask]) | maxval(array [,dim] [,mask])\n```\n```fortran\n     NUMERIC function maxval(array ,dim, mask)\n\n      NUMERIC,intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **NUMERIC** designates any numeric type and kind.\n\n### **Description**\n\n  **maxval** determines the maximum value of the elements in an\n  array value, or, if the **dim** argument is supplied, determines the\n  maximum value along each row of the array in the **dim** direction. If\n  **mask** is present, only the elements for which **mask** is _.true._\n  are considered. If the array has zero size, or all of the elements of\n  **mask** are _.false._, then the result is the most negative number\n  of the type and kind of **array** if **array** is numeric, or a string\n  of nulls if **array** is of character type.\n\n### **Options**\n\n- **array**\n  : Shall be an array of type _integer_, _real_, or _character_.\n\n- **dim**\n  : (Optional) Shall be a scalar of type _integer_, with a value between\n  one and the rank of **array**, inclusive. It may not be an optional\n  dummy argument.\n\n- **mask**\n  : (Optional) Shall be an array of type _logical_, and conformable with\n  **array**.\n\n### **Result**\n\nIf **dim** is absent, or if **array** has a rank of one, the result is a scalar.\nIf **dim** is present, the result is an array with a rank one less than the\nrank of **array**, and a size corresponding to the size of **array** with the\n**dim** dimension removed. In all cases, the result is of the same type and\nkind as **array**.\n\n### **Examples**\n\nsample program:\n\n```fortran\nprogram demo_maxval\nimplicit none\ninteger,save :: ints(3,5)= reshape([&\n   1,  2,  3,  4,  5, &\n  10, 20, 30, 40, 50, &\n  11, 22, 33, 44, 55  &\n],shape(ints),order=[2,1])\n\n   write(*,*) maxval(ints)\n   write(*,*) maxval(ints,dim=1)\n   write(*,*) maxval(ints,dim=2)\n   ! find biggest number less than 30 with mask\n   write(*,*) maxval(ints,mask=ints.lt.30)\nend program demo_maxval\n```\nResults:\n```\n >  55\n >  11     22     33     44     55\n >   5     50     55\n >  22\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**maxloc**(3)](#maxloc),\n[**minloc**(3)](#minloc),\n[**minval**(3)](#minval),\n[**max**(3)](#max),\n[**min**(3)](#min)\n\n _fortran-lang intrinsic descriptions_\n",
-    "MERGE": "## merge\n\n### **Name**\n\n**merge** - \\[ARRAY:CONSTRUCTION\\] Merge variables\n\n### **Synopsis**\n```fortran\n    result = merge(tsource, fsource, mask)\n```\n```fortran\n     elemental type(TYPE(kind=KIND)) function merge(tsource,fsource,mask)\n\n      type(TYPE(kind=KIND)),intent(in) :: tsource\n      type(TYPE(kind=KIND)),intent(in) :: fsource\n      logical(kind=**),intent(in)   :: mask\n      mask** : Shall be of type logical.\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **tsource** May be of any type, including user-defined.\n - **fsource** Shall be of the same type and type parameters as **tsource**.\n - **mask** shall be of type logical.\n - The result will by of the same type and type parameters as **tsource**.\n\n\n### **Description**\n\nThe elemental function **merge** selects values from two arrays or\nscalars according to a logical mask. The result is equal to an element\nof **tsource** where the corresponding element of **mask** is _.true._, or an\nelement of **fsource** when it is _.false._ .\n\nMulti-dimensional arrays are supported.\n\nNote that argument expressions to **merge** are not required to be\nshort-circuited so (as an example) if the array **x** contains zero values\nin the statement below the standard does not prevent floating point\ndivide by zero being generated; as **1.0/x** may be evaluated for all values\nof **x** before the mask is used to select which value to retain:\n\n```fortran\n      y = merge( 1.0/x, 0.0, x /= 0.0 )\n```\n\nNote the compiler is also free to short-circuit or to generate an\ninfinity so this may work in many programming environments but is not\nrecommended.\n\nFor cases like this one may instead use masked assignment via the **where**\nconstruct:\n\n```fortran\n      where(x .ne. 0.0)\n         y = 1.0/x\n      elsewhere\n         y = 0.0\n      endwhere\n```\n\ninstead of the more obscure\n\n```fortran\n      merge(1.0/merge(x,1.0,x /= 0.0), 0.0, x /= 0.0)\n```\n### **Options**\n\n- **tsource**\n  : May be of any type, including user-defined.\n\n- **fsource**\n  : Shall be of the same type and type parameters as **tsource**.\n\n- **mask**\n  : Shall be of type _logical_.\n\nNote that (currently) _character_ values must be of the same length.\n\n### **Result**\n  The result is built from an element of **tsource** if **mask** is\n  _.true._ and from **fsource** otherwise.\n\n  Because **tsource** and **fsource** are required to have the same type\n  and type parameters (for both the declared and dynamic types), the\n  result is polymorphic if and only if both **tsource** and **fsource**\n  are polymorphic.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_merge\nimplicit none\ninteger :: tvals(2,3), fvals(2,3), answer(2,3)\nlogical :: mask(2,3)\ninteger :: i\ninteger :: k\nlogical :: chooseleft\n\n   ! Works with scalars\n   k=5\n   write(*,*)merge (1.0, 0.0, k > 0)\n   k=-2\n   write(*,*)merge (1.0, 0.0, k > 0)\n\n   ! set up some simple arrays that all conform to the\n   ! same shape\n   tvals(1,:)=[  10, -60,  50 ]\n   tvals(2,:)=[ -20,  40, -60 ]\n\n   fvals(1,:)=[ 0, 3, 2 ]\n   fvals(2,:)=[ 7, 4, 8 ]\n\n   mask(1,:)=[ .true.,  .false., .true. ]\n   mask(2,:)=[ .false., .false., .true. ]\n\n   ! lets use the mask of specific values\n   write(*,*)'mask of logicals'\n   answer=merge( tvals, fvals, mask )\n   call printme()\n\n   ! more typically the mask is an expression\n   write(*, *)'highest values'\n   answer=merge( tvals, fvals, tvals > fvals )\n   call printme()\n\n   write(*, *)'lowest values'\n   answer=merge( tvals, fvals, tvals < fvals )\n   call printme()\n\n   write(*, *)'zero out negative values'\n   answer=merge( 0, tvals, tvals < 0)\n   call printme()\n\n   write(*, *)'binary choice'\n   chooseleft=.false.\n   write(*, '(3i4)')merge([1,2,3],[10,20,30],chooseleft)\n   chooseleft=.true.\n   write(*, '(3i4)')merge([1,2,3],[10,20,30],chooseleft)\n\ncontains\n\nsubroutine printme()\n      write(*, '(3i4)')(answer(i, :), i=1, size(answer, dim=1))\nend subroutine printme\n\nend program demo_merge\n```\nResults:\n```text\n >    1.00000000    \n >    0.00000000    \n >  mask of logicals\n >   10   3  50\n >    7   4 -60\n >  highest values\n >   10   3  50\n >    7  40   8\n >  lowest values\n >    0 -60   2\n >  -20   4 -60\n >  zero out negative values\n >   10   0  50\n >    0  40   0\n >  binary choice\n >   10  20  30\n >    1   2   3\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n- [**pack**(3)](#pack) packs an array into an array of rank one\n- [**spread**(3)](#spread) is used to add a dimension and replicate data\n- [**unpack**(3)](#unpack) scatters the elements of a vector\n- [**transpose**(3)](#transpose) - Transpose an array of rank two\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
+    "MERGE": "## merge\n\n### **Name**\n\n**merge** - \\[ARRAY:CONSTRUCTION\\] Merge variables\n\n### **Synopsis**\n```fortran\n    result = merge(tsource, fsource, mask)\n```\n```fortran\n     elemental type(TYPE(kind=KIND)) function merge(tsource,fsource,mask)\n\n      type(TYPE(kind=KIND)),intent(in) :: tsource\n      type(TYPE(kind=KIND)),intent(in) :: fsource\n      logical(kind=**),intent(in)   :: mask\n      mask** : Shall be of type logical.\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **tsource** May be of any type, including user-defined.\n - **fsource** Shall be of the same type and type parameters as **tsource**.\n - **mask** shall be of type logical.\n - The result will by of the same type and type parameters as **tsource**.\n\n\n### **Description**\n\nThe elemental function **merge** selects values from two arrays or\nscalars according to a logical mask. The result is equal to an element\nof **tsource** where the corresponding element of **mask** is _.true._, or an\nelement of **fsource** when it is _.false._ .\n\nMulti-dimensional arrays are supported.\n\nNote that argument expressions to **merge** are not required to be\nshort-circuited so (as an example) if the array **x** contains zero values\nin the statement below the standard does not prevent floating point\ndivide by zero being generated; as **1.0/x** may be evaluated for all values\nof **x** before the mask is used to select which value to retain:\n\n```fortran\n      y = merge( 1.0/x, 0.0, x /= 0.0 )\n```\n\nNote the compiler is also free to short-circuit or to generate an\ninfinity so this may work in many programming environments but is not\nrecommended.\n\nFor cases like this one may instead use masked assignment via the **where**\nconstruct:\n\n```fortran\n      where(x .ne. 0.0)\n         y = 1.0/x\n      elsewhere\n         y = 0.0\n      endwhere\n```\n\ninstead of the more obscure\n\n```fortran\n      merge(1.0/merge(x,1.0,x /= 0.0), 0.0, x /= 0.0)\n```\n### **Options**\n\n- **tsource**\n  : May be of any type, including user-defined.\n\n- **fsource**\n  : Shall be of the same type and type parameters as **tsource**.\n\n- **mask**\n  : Shall be of type _logical_.\n\nNote that (currently) _character_ values must be of the same length.\n\n### **Result**\n  The result is built from an element of **tsource** if **mask** is\n  _.true._ and from **fsource** otherwise.\n\n  Because **tsource** and **fsource** are required to have the same type\n  and type parameters (for both the declared and dynamic types), the\n  result is polymorphic if and only if both **tsource** and **fsource**\n  are polymorphic.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_merge\nimplicit none\ninteger :: tvals(2,3), fvals(2,3), answer(2,3)\nlogical :: mask(2,3)\ninteger :: i\ninteger :: k\nlogical :: chooseleft\n\n   ! Works with scalars\n   k=5\n   write(*,*)merge (1.0, 0.0, k > 0)\n   k=-2\n   write(*,*)merge (1.0, 0.0, k > 0)\n\n   ! set up some simple arrays that all conform to the\n   ! same shape\n   tvals(1,:)=[  10, -60,  50 ]\n   tvals(2,:)=[ -20,  40, -60 ]\n\n   fvals(1,:)=[ 0, 3, 2 ]\n   fvals(2,:)=[ 7, 4, 8 ]\n\n   mask(1,:)=[ .true.,  .false., .true. ]\n   mask(2,:)=[ .false., .false., .true. ]\n\n   ! lets use the mask of specific values\n   write(*,*)'mask of logicals'\n   answer=merge( tvals, fvals, mask )\n   call printme()\n\n   ! more typically the mask is an expression\n   write(*, *)'highest values'\n   answer=merge( tvals, fvals, tvals > fvals )\n   call printme()\n\n   write(*, *)'lowest values'\n   answer=merge( tvals, fvals, tvals < fvals )\n   call printme()\n\n   write(*, *)'zero out negative values'\n   answer=merge( 0, tvals, tvals < 0)\n   call printme()\n\n   write(*, *)'binary choice'\n   chooseleft=.false.\n   write(*, '(3i4)')merge([1,2,3],[10,20,30],chooseleft)\n   chooseleft=.true.\n   write(*, '(3i4)')merge([1,2,3],[10,20,30],chooseleft)\n\ncontains\n\nsubroutine printme()\n      write(*, '(3i4)')(answer(i, :), i=1, size(answer, dim=1))\nend subroutine printme\n\nend program demo_merge\n```\nResults:\n```text\n >    1.00000000\n >    0.00000000\n >  mask of logicals\n >   10   3  50\n >    7   4 -60\n >  highest values\n >   10   3  50\n >    7  40   8\n >  lowest values\n >    0 -60   2\n >  -20   4 -60\n >  zero out negative values\n >   10   0  50\n >    0  40   0\n >  binary choice\n >   10  20  30\n >    1   2   3\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n- [**pack**(3)](#pack) packs an array into an array of rank one\n- [**spread**(3)](#spread) is used to add a dimension and replicate data\n- [**unpack**(3)](#unpack) scatters the elements of a vector\n- [**transpose**(3)](#transpose) - Transpose an array of rank two\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MERGE_BITS": "## merge_bits\n\n### **Name**\n\n**merge_bits** - \\[BIT:COPY\\] Merge bits using a mask\n\n### **Synopsis**\n```fortran\n    result = merge_bits(i, j, mask)\n```\n```fortran\n     elemental integer(kind=KIND) function merge_bits(i,j,mask)\n\n      integer(kind=KIND), intent(in) :: i, j, mask\n```\n### **Characteristics**\n\n - the result and all input values have the same _integer_ type and\n   KIND with the exception that the mask and either **i** or **j** may be\n   a BOZ constant.\n\n### **Description**\n\nA common graphics operation in Ternary Raster Operations is to combine\nbits from two different sources, generally referred to as bit-blending.\n**merge_bits** performs a masked bit-blend of **i** and **j** using\nthe bits of the **mask** value to determine which of the input values\nto copy bits from.\n\nSpecifically, The k-th bit of the result is equal to the k-th bit of\n**i** if the k-th bit of **mask** is **1**; it is equal to the k-th bit\nof **j** otherwise (so all three input values must have the same number\nof bits).\n\nThe resulting value is the same as would result from\n```fortran\n    ior (iand (i, mask),iand (j, not (mask)))\n```\nAn exception to all values being of the same _integer_ type is that **i**\nor **j** and/or the mask may be a BOZ constant (A BOZ constant means it is\neither a Binary, Octal, or Hexadecimal literal constant). The BOZ values\nare converted to the _integer_ type of the non-BOZ value(s) as if called\nby the intrinsic function **int()** with the kind of the non-BOZ value(s),\nso the BOZ values must be in the range of the type of the result.\n\n### **Options**\n\n- **i**\n  : value to select bits from when the associated bit in the mask is **1**.\n\n- **j**\n  : value to select bits from when the associated bit in the mask is **0**.\n\n- **mask**\n  : a value whose bits are used as a mask to select bits from **i** and **j**\n\n### **Result**\n\nThe bits blended from **i** and **j** using the mask **mask**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_merge_bits\nuse,intrinsic :: iso_fortran_env,  only : int8, int16, int32, int64\nimplicit none\ninteger(kind=int16) :: if_one,if_zero,msk\ncharacter(len=*),parameter :: fmt='(*(g0, 1X))'\n\n   ! basic usage\n   print *,'MERGE_BITS( 5,10,41) should be 3.=>',merge_bits(5,10,41)\n   print *,'MERGE_BITS(13,18,22) should be 4.=>',merge_bits(13,18,22)\n\n   ! use some values in base2 illustratively:\n   if_one =int(b'1010101010101010',kind=int16)\n   if_zero=int(b'0101010101010101',kind=int16)\n\n   msk=int(b'0101010101010101',kind=int16)\n   print '(\"should get all zero bits =>\",b16.16)', &\n   & merge_bits(if_one,if_zero,msk)\n\n   msk=int(b'1010101010101010',kind=int16)\n   print '(\"should get all ones bits =>\",b16.16)', &\n   & merge_bits(if_one,if_zero,msk)\n\n   ! using BOZ values\n   print fmt, &\n   & merge_bits(32767_int16,    o'12345',         32767_int16), &\n   & merge_bits(o'12345', 32767_int16, b'0000000000010101'), &\n   & merge_bits(32767_int16,    o'12345',             z'1234')\n\n   ! a do-it-yourself equivalent for comparison and validation\n   print fmt, &\n   & ior(iand(32767_int16, 32767_int16),                   &\n   &   iand(o'12345', not(32767_int16))),                  &\n\n   & ior(iand(o'12345', int(o'12345', kind=int16)),        &\n   &   iand(32767_int16, not(int(o'12345', kind=int16)))), &\n\n   & ior(iand(32767_int16, z'1234'),                       &\n   &   iand(o'12345', not(int( z'1234', kind=int16))))\n\nend program demo_merge_bits\n```\nResults:\n```text\n    MERGE_BITS( 5,10,41) should be 3.=>           3\n    MERGE_BITS(13,18,22) should be 4.=>           4\n   should get all zero bits =>0000000000000000\n   should get all ones bits =>1111111111111111\n   32767 32751 5877\n   32767 32767 5877\n```\n### **Standard**\n\nFortran 2008\n\n### **See also**\n\n[****(3)](#)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MIN": "## min\n\n### **Name**\n\n**min** - \\[NUMERIC\\] Minimum value of an argument list\n\n### **Synopsis**\n```fortran\n    result = min(a1, a2, a3, ... )\n```\n```fortran\n     elemental TYPE(kind=KIND) function min(a1, a2, a3, ... )\n\n      TYPE(kind=KIND,intent(in)   :: a1\n      TYPE(kind=KIND,intent(in)   :: a2\n      TYPE(kind=KIND,intent(in)   :: a3\n                :\n                :\n                :\n```\n### **Characteristics**\n\n- **TYPE** may be _integer_, _real_ or _character_.\n\n### **Description**\n\n**min** returns the argument with the smallest (most negative) value.\n\nSee **max**(3) for an extended example of the behavior of **min** as\nand **max**(3).\n\n### **Options**\n\n- **a1**\n  : the first element of the set of values to determine the minimum of.\n\n- **a2, a3, ...**\n  : An expression of the same type and kind as **a1** completing the\n  set of values to find the minimum of.\n\n### **Result**\n\nThe return value corresponds to the minimum value among the arguments,\nand has the same type and kind as the first argument.\n\n### **Examples**\n\nSample program\n```fortran\nprogram demo_min\nimplicit none\n    write(*,*)min(10.0,11.0,30.0,-100.0)\nend program demo_min\n```\nResults:\n```\n      -100.0000000\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n[**maxloc**(3)](#maxloc),\n[**minloc**(3)](#minloc),\n[**minval**(3)](#minval),\n[**max**(3)](#max),\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MINEXPONENT": "## minexponent\n\n### **Name**\n\n**minexponent** - \\[NUMERIC MODEL\\] Minimum exponent of a real kind\n\n### **Synopsis**\n```fortran\n    result = minexponent(x)\n```\n```fortran\n     elemental integer function minexponent(x)\n\n      real(kind=**),intent(in) :: x\n```\n### **Characteristics**\n\n - **x**  is a _real_ scalar or array of any _real_ kind\n - the result is a default _integer_ scalar\n\n### **Description**\n\n  **minexponent** returns the minimum exponent in the model of the\n  type of **x**.\n\n### **Options**\n\n- **x**\n  : A value used to select the kind of _real_ to return a value for.\n\n### **Result**\n\n  The value returned is the maximum exponent for the kind of the value\n  queried\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_minexponent\nuse, intrinsic :: iso_fortran_env, only : &\n &real_kinds, real32, real64, real128\nimplicit none\nreal(kind=real32) :: x\nreal(kind=real64) :: y\n    print *, minexponent(x), maxexponent(x)\n    print *, minexponent(y), maxexponent(y)\nend program demo_minexponent\n```\nExpected Results:\n```\n        -125         128\n       -1021        1024\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MINLOC": "## minloc\n\n### **Name**\n\n**minloc** - \\[ARRAY:LOCATION\\] Location of the minimum value within an array\n\n### **Synopsis**\n```fortran\n    result = minloc(array [,mask]) | minloc(array [,dim] [,mask])\n```\n```fortran\n     NUMERIC function minloc(array, dim, mask)\n\n      NUMERIC,intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n```\n### **Characteristics**\n\n  - a kind designated as ** may be any supported kind for the type\n  - **NUMERIC** is any numeric type and kind.\n\n### **Description**\n\n  **minloc** determines the location of the element in the array with\n  the minimum value, or, if the **dim** argument is supplied, determines\n  the locations of the minimum element along each row of the array in\n  the **dim** direction.\n\n  If **mask** is present, only the elements for which **mask** is _true._\n  are considered.\n\n  If more than one element in the array has the minimum value, the\n  location returned is that of the first such element in array element\n  order.\n\n  If the array has zero size, or all of the elements of **mask** are\n  _.false._, then the result is an array of zeroes. Similarly, if **dim**\n  is supplied and all of the elements of **mask** along a given row are\n  zero, the result value for that row is zero.\n\n### **Options**\n\n- **array**\n  : Shall be an array of type _integer_, _real_, or _character_.\n\n- **dim**\n  : (Optional) Shall be a scalar of type _integer_, with a value between\n  one and the rank of **array**, inclusive. It may not be an optional\n  dummy argument.\n\n- **mask**\n  : Shall be an array of type _logical_, and conformable with **array**.\n\n### **Result**\n\nIf **dim** is absent, the result is a rank-one array with a length equal\nto the rank of **array**. If **dim** is present, the result is an array\nwith a rank one less than the rank of **array**, and a size corresponding\nto the size of **array** with the **dim** dimension removed. If **dim**\nis present and **array** has a rank of one, the result is a scalar. In\nall cases, the result is of default _integer_ type.\n\n### **Examples**\n\nsample program:\n\n```fortran\nprogram demo_minloc\nimplicit none\ninteger,save :: ints(3,5)= reshape([&\n   4, 10,  1,  7, 13, &\n   9, 15,  6, 12,  3, &\n  14,  5, 11,  2,  8  &\n],shape(ints),order=[2,1])\n   write(*,*) minloc(ints)\n   write(*,*) minloc(ints,dim=1)\n   write(*,*) minloc(ints,dim=2)\n   ! where in each column is the smallest number .gt. 10 ?\n   write(*,*) minloc(ints,dim=2,mask=ints.gt.10)\n   ! a one-dimensional array with dim=1 explicitly listed returns a scalar\n   write(*,*) minloc(pack(ints,.true.),dim=1) ! scalar\nend program demo_minloc\n```\nResults:\n```text\n >        1       3\n >        1       3       1       3       2\n >        3       5       4\n >        5       4       3\n >        7\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n - [**findloc**(3)](#findloc) - Location of first element of ARRAY\n   identified by MASK along dimension DIM matching a target\n - [**maxloc**(3)](#maxloc) - Location of the maximum value within an array\n - [**minloc**](#minloc) - Location of the minimum value within an array\n - [**min**(3)](#min)\n - [**minval**(3)](#minval)\n - [**maxval**(3)](#maxval)\n - [**max**(3)](#max)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MINVAL": "## minval\n\n### **Name**\n\n**minval** - \\[ARRAY:REDUCTION\\] Minimum value of an array\n\n### **Synopsis**\n```fortran\n    result = minval(array, [mask]) | minval(array [,dim] [,mask])\n```\n```fortran\n     NUMERIC function minval(array, dim, mask)\n\n      NUMERIC,intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **NUMERIC** is any numeric type and kind.\n\n### **Description**\n\n  **minval** determines the minimum value of the elements in an array\n  value, or, if the **dim** argument is supplied, determines the minimum\n  value along each row of the array in the **dim** direction.\n\n  If **mask** is present, only the elements for which **mask** is\n  _.true._ are considered.\n\n  If the array has zero size, or all of the elements of **mask**\n  are _.false._, then the result is **huge(array)** if **array** is\n  numeric, or a string of **char(len=255)** characters if **array**\n  is of character type.\n\n### **Options**\n\n- **array**\n  : Shall be an array of type _integer_, _real_, or _character_.\n\n- **dim**\n  : (Optional) Shall be a scalar of type _integer_, with a value between\n  one and the rank of ARRAY, inclusive. It may not be an optional\n  dummy argument.\n\n- **mask**\n  : Shall be an array of type _logical_, and conformable with **array**.\n\n### **Result**\n\nIf **dim** is absent, or if **array** has a rank of one, the result is a scalar.\n\nIf **dim** is present, the result is an array with a rank one less than the\nrank of **array**, and a size corresponding to the size of **array** with the\n**dim** dimension removed. In all cases, the result is of the same type and\nkind as **array**.\n\n### **Examples**\n\nsample program:\n```fortran\nprogram demo_minval\nimplicit none\ninteger :: i\ncharacter(len=*),parameter :: g='(3x,*(g0,1x))'\n\ninteger,save :: ints(3,5)= reshape([&\n       1,  -2,   3,   4,   5,  &\n      10,  20, -30,  40,  50,  &\n      11,  22,  33, -44,  55  &\n],shape(ints),order=[2,1])\n\ninteger,save :: box(3,5,2)\n\n   box(:,:,1)=ints\n   box(:,:,2)=-ints\n\n   write(*,*)'Given the array'\n   write(*,'(1x,*(g4.4,1x))') &\n   & (ints(i,:),new_line('a'),i=1,size(ints,dim=1))\n\n   write(*,*)'What is the smallest element in the array?'\n   write(*,g) minval(ints),'at <',minloc(ints),'>'\n\n   write(*,*)'What is the smallest element in each column?'\n   write(*,g) minval(ints,dim=1)\n\n   write(*,*)'What is the smallest element in each row?'\n   write(*,g) minval(ints,dim=2)\n\n   ! notice the shape of the output has less columns\n   ! than the input in this case\n   write(*,*)'What is the smallest element in each column,'\n   write(*,*)'considering only those elements that are'\n   write(*,*)'greater than zero?'\n   write(*,g) minval(ints, dim=1, mask = ints > 0)\n\n   write(*,*)&\n   & 'if everything is false a zero-sized array is NOT returned'\n   write(*,*) minval(ints, dim=1, mask = .false.)\n   write(*,*)'even for a zero-sized input'\n   write(*,g) minval([integer ::], dim=1, mask = .false.)\n\n   write(*,*)'a scalar answer for everything false is huge()'\n   write(*,g) minval(ints, mask = .false.)\n   write(*,g) minval([integer ::], mask = .false.)\n\n   write(*,*)'some calls with three dimensions'\n   write(*,g) minval(box, mask = .true. )\n   write(*,g) minval(box, dim=1, mask = .true. )\n\n   write(*,g) minval(box, dim=2, mask = .true. )\n   write(*,g) 'shape of answer is ', &\n   & shape(minval(box, dim=2, mask = .true. ))\n\nend program demo_minval\n```\nResults:\n```text\n > Given the array\n >    1   -2    3    4    5\n >   10   20  -30   40   50\n >   11   22   33  -44   55\n >\n > What is the smallest element in the array?\n >   -44 at < 3 4 >\n > What is the smallest element in each column?\n >   1 -2 -30 -44 5\n > What is the smallest element in each row?\n >   -2 -30 -44\n > What is the smallest element in each column,\n > considering only those elements that are\n > greater than zero?\n >   1 20 3 4 5\n > if everything is false a zero-sized array is NOT returned\n >  2147483647  2147483647  2147483647  2147483647  2147483647\n > even for a zero-sized input\n >   2147483647\n > a scalar answer for everything false is huge()\n >   2147483647\n >   2147483647\n > some calls with three dimensions\n >   -55\n >   1 -2 -30 -44 5 -11 -22 -33 -40 -55\n >   -2 -30 -44 -5 -50 -55\n >   shape of answer is  3 2\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**min**(3)](#min),\n[**minloc**(3)](#minloc)\n[**maxloc**(3)](#maxloc),\n[**maxval**(3)](#maxval),\n[**min**(3)](#min)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MOD": "## mod\n\n### **Name**\n\n**mod** - \\[NUMERIC\\] Remainder function\n\n### **Synopsis**\n```fortran\n    result = mod(a, p)\n```\n```fortran\n     elemental type(TYPE(kind=KIND)) function mod(a,p)\n\n      type(TYPE(kind=KIND)),intent(in) :: a\n      type(TYPE(kind=KIND)),intent(in) :: p\n```\n### **Characteristics**\n\n  - The result and arguments are all of the same type and kind.\n  - The type  may be any kind of _real_ or _integer_.\n\n### **Description**\n\n**mod** computes the remainder of the division of **a** by **p**.\n\n  In mathematics, the remainder is the amount \"left over\" after\n  performing some computation. In arithmetic, the remainder is the\n  integer \"left over\" after dividing one integer by another to produce\n  an integer quotient (integer division). In algebra of polynomials, the\n  remainder is the polynomial \"left over\" after dividing one polynomial\n  by another. The modulo operation is the operation that produces such\n  a remainder when given a dividend and divisor.\n\n  - (remainder). (2022, October 10). In Wikipedia.\n     https://en.wikipedia.org/wiki/Remainder\n\n### **Options**\n\n- **a**\n  : The dividend\n\n- **p**\n  : the divisor (not equal to zero).\n\n### **Result**\n\n  The return value is the result of **a - (int(a/p) \\* p)**.\n\n  As can be seen by the formula the sign of **p** is canceled out.\n  Therefore the returned value always has the sign of **a**.\n\n  Of course, the magnitude of the result will be less than the magnitude\n  of **p**, as the result has been reduced by all multiples of **p**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_mod\nimplicit none\n\n   ! basics\n    print *, mod( -17,  3 ), modulo( -17,  3 )\n    print *, mod(  17, -3 ), modulo(  17, -3 )\n    print *, mod(  17,  3 ), modulo(  17,  3 )\n    print *, mod( -17, -3 ), modulo( -17, -3 )\n\n    print *, mod(-17.5, 5.2), modulo(-17.5, 5.2)\n    print *, mod( 17.5,-5.2), modulo( 17.5,-5.2)\n    print *, mod( 17.5, 5.2), modulo( 17.5, 5.2)\n    print *, mod(-17.5,-5.2), modulo(-17.5,-5.2)\n\n  ! with a divisor of 1 the fractional part is returned\n    print *, mod(-17.5, 1.0), modulo(-17.5, 1.0)\n    print *, mod( 17.5,-1.0), modulo( 17.5,-1.0)\n    print *, mod( 17.5, 1.0), modulo( 17.5, 1.0)\n    print *, mod(-17.5,-1.0), modulo(-17.5,-1.0)\n\nend program demo_mod\n```\nResults:\n```text\n             -2           1\n              2          -1\n              2           2\n             -2          -2\n     -1.900001       3.299999\n      1.900001      -3.299999\n      1.900001       1.900001\n     -1.900001      -1.900001\n    -0.5000000      0.5000000\n     0.5000000     -0.5000000\n     0.5000000      0.5000000\n    -0.5000000     -0.5000000\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n - [**modulo**(3)](#modulo) - Modulo function\n - [**aint**(3)](#aint) - truncate toward zero to a whole _real_ number\n - [**int**(3)](#int) - truncate toward zero to a whole _integer_ number\n - [**anint**(3)](#anint) -  _real_ nearest whole number\n - [**nint**(3)](#nint) - _integer_ nearest whole number\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "MODULO": "## modulo\n\n### **Name**\n\n**modulo** - \\[NUMERIC\\] Modulo function\n\n### **Synopsis**\n```fortran\n    result = modulo(a, p)\n```\n```fortran\n     elemental TYPE(kind=KIND) function modulo(a,p)\n\n      TYPE(kind=KIND),intent(in) :: a\n      TYPE(kind=KIND),intent(in) :: p\n```\n### **Characteristics**\n\n  - **a** may be any kind of _real_ or _integer_.\n  - **p** is the same type and kind as **a**\n  - The result and arguments are all of the same type and kind.\n\n### **Description**\n\n**modulo** computes the **a** modulo **p**.\n\n### **Options**\n\n- **a**\n  : the value to take the **modulo** of\n\n- **p**\n  : The value to reduce **a** by till the remainder is <= **p**.\n    It shall not be zero.\n\n### **Result**\n\nThe type and kind of the result are those of the arguments.\n\n- If **a** and **p** are of type _integer_: **modulo(a,p)** has the value of\n  **a - floor (real(a) / real(p)) \\* p**.\n\n- If **a** and **p** are of type _real_: **modulo(a,p)** has the value of\n  **a - floor (a / p) \\* p**.\n\nThe returned value has the same sign as **p** and a magnitude less than the\nmagnitude of **p**.\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_modulo\nimplicit none\n     print *, modulo(17,3)        ! yields 2\n     print *, modulo(17.5,5.5)    ! yields 1.0\n\n     print *, modulo(-17,3)       ! yields 1\n     print *, modulo(-17.5,5.5)   ! yields 4.5\n\n     print *, modulo(17,-3)       ! yields -1\n     print *, modulo(17.5,-5.5)   ! yields -4.5\nend program demo_modulo\n```\nResults:\n```text\n >            2\n >    1.000000\n >            1\n >    4.500000\n >           -1\n >   -4.500000\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**mod**(3)](#mod)\n\n _fortran-lang intrinsic descriptions_\n",
@@ -152,41 +152,41 @@
     "PARITY": "## parity\n\n### **Name**\n\n**parity** - \\[ARRAY:REDUCTION\\] Array reduction by .NEQV. operation\n\n### **Synopsis**\n```fortran\n    result = parity( mask [,dim] )\n```\n```fortran\n     logical(kind=KIND) function parity(mask, dim)\n\n      type(logical(kind=KIND)),intent(in)        :: mask(..)\n      type(integer(kind=**)),intent(in),optional :: dim\n```\n### **Characteristics**\n\n  - **mask** is a _logical_ array\n  - **dim** is an integer scalar\n  - the result is of type _logical_ with the same kind type parameter as **mask**.\n    It is a scalar if **dim** does not appear; otherwise it is the rank and shape\n    of **mask** with the dimension specified by **dim** removed.\n  - a kind designated as ** may be any supported kind for the type\n\n### **Description**\n\n**parity** calculates the parity array (i.e. the reduction using .neqv.) of\n**mask** along dimension **dim** if **dim** is present and not 1. Otherwise, it\nreturns the parity of the entire **mask** array as a scalar.\n\n### **Options**\n\n  - **mask**\n    : Shall be an array of type _logical_.\n\n  - **dim**\n    : (Optional) shall be a scalar of type _integer_ with a value in the\n    range from _1 to n_, where _n_ equals the rank of **mask**.\n\n### **Result**\n\n  The result is of the same type as **mask**.\n\n  If **dim** is absent, a scalar with the parity of all elements in **mask**\n  is returned: _.true._ if an odd number of elements are _.true._\n  and _.false._ otherwise.\n\n  If MASK has rank one, PARITY (MASK, DIM) is equal to PARITY (MASK). Otherwise, the\n  result is an array of parity values with dimension **dim** dropped.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_parity\nimplicit none\nlogical, parameter :: T=.true., F=.false.\nlogical :: x(3,4)\n  ! basics\n   print *, parity([T,F])\n   print *, parity([T,F,F])\n   print *, parity([T,F,F,T])\n   print *, parity([T,F,F,T,T])\n   x(1,:)=[T,T,T,T]\n   x(2,:)=[T,T,T,T]\n   x(3,:)=[T,T,T,T]\n   print *, parity(x)\n   print *, parity(x,dim=1)\n   print *, parity(x,dim=2)\nend program demo_parity\n```\nResults:\n```text\n >  T\n >  T\n >  F\n >  T\n >  F\n >  T T T T\n >  F F F\n```\n### **Standard**\n\nFortran 2008\n\n### **See also**\n\n - [**all**(3)](#all) - Determines if all the values are true\n - [**any**(3)](#any) - Determines if any of the values in the logical array are _.true._\n - [**count**(3)](#count) - Count true values in an array\n - [**sum**(3)](#sum) - Sum the elements of an array\n - [**maxval**(3)](#maxval) - Determines the maximum value in an array or row\n - [**minval**(3)](#minval) - Minimum value of an array\n - [**product**(3)](#product) - Product of array elements\n - [**reduce**(3)](#reduce) - General array reduction\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "POPCNT": "## popcnt\n\n### **Name**\n\n**popcnt** - \\[BIT:COUNT\\] Number of bits set\n\n### **Synopsis**\n```fortran\n    result = popcnt(i)\n```\n```fortran\n     elemental integer function popcnt(i)\n\n      integer(kind=KIND), intent(in) :: i\n```\n### **Characteristics**\n\n- **i** may be an _integer_ of any kind.\n- The return value is an _integer_ of the default integer kind.\n\n### **Description**\n\n  **popcnt** returns the number of bits set to one in the binary\n  representation of an _integer_.\n\n### **Options**\n\n- **i**\n  : value to count set bits in\n\n### **Result**\n\nThe number of bits set to one in **i**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_popcnt\nuse, intrinsic :: iso_fortran_env, only : integer_kinds, &\n   & int8, int16, int32, int64\nimplicit none\ncharacter(len=*),parameter :: pretty='(b64,1x,i0)'\n  ! basic usage\n   print pretty, 127,     popcnt(127)\n   print pretty, int(b\"01010\"), popcnt(int(b\"01010\"))\n\n  ! any kind of an integer can be used\n   print pretty, huge(0_int8),  popcnt(huge(0_int8))\n   print pretty, huge(0_int16), popcnt(huge(0_int16))\n   print pretty, huge(0_int32), popcnt(huge(0_int32))\n   print pretty, huge(0_int64), popcnt(huge(0_int64))\nend program demo_popcnt\n```\nResults:\n\nNote that on most machines the first bit is the sign bit, and a zero is\nused for positive values; but that this is system-dependent. These are\ntypical values, where the huge(3f) function has set all but the first\nbit to 1.\n```text\n >                                                         1111111 7\n >                                                            1010 2\n >                                                         1111111 7\n >                                                 111111111111111 15\n >                                 1111111111111111111111111111111 31\n > 111111111111111111111111111111111111111111111111111111111111111 63\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\nThere are many procedures that operator or query values at the bit level:\n\n[**poppar**(3)](#poppar),\n[**leadz**(3)](#leadz),\n[**trailz**(3)](#trailz)\n[**atomic_and**(3)](#atomic_and),\n[**atomic_fetch_and**(3)](#atomic_fetch_and),\n[**atomic_fetch_or**(3)](#atomic_fetch_or),\n[**atomic_fetch_xor**(3)](#atomic_fetch_xor),\n[**atomic_or**(3)](#atomic_or),\n[**atomic_xor**(3)](#atomic_xor),\n[**bge**(3)](#bge),\n[**bgt**(3)](#bgt),\n[**bit_size**(3)](#bit_size),\n[**ble**(3)](#ble),\n[**blt**(3)](#blt),\n[**btest**(3)](#btest),\n[**dshiftl**(3)](#dshiftl),\n[**dshiftr**(3)](#dshiftr),\n[**iall**(3)](#iall),\n[**iand**(3)](#iand),\n[**iany**(3)](#iany),\n[**ibclr**(3)](#ibclr),\n[**ibits**(3)](#ibits),\n[**ibset**(3)](#ibset),\n[**ieor**(3)](#ieor),\n[**ior**(3)](#ior),\n[**iparity**(3)](#iparity),\n[**ishftc**(3)](#ishftc),\n[**ishft**(3)](#ishft),\n[**maskl**(3)](#maskl),\n[**maskr**(3)](#maskr),\n[**merge_bits**(3)](#merge_bits),\n[**mvbits**(3)](#mvbits),\n[**not**(3)](#not),\n[**shifta**(3)](#shifta),\n[**shiftl**(3)](#shiftl),\n[**shiftr**(3)](#shiftr),\n[**storage_size**(3)](#storage_size)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "POPPAR": "## poppar\n\n### **Name**\n\n**poppar** - \\[BIT:COUNT\\] Parity of the number of bits set\n\n### **Synopsis**\n```fortran\n    result = poppar(i)\n```\n```fortran\n     elemental integer function poppar(i)\n\n      integer(kind=KIND), intent(in) :: i\n```\n### **Characteristics**\n\n- **i** is an _integer_ of any kind\n- the return value is a default kind _integer_\n\n### **Description**\n\n  **poppar** returns the parity of an integer's binary representation\n  (i.e., the parity of the number of bits set).\n\n  The parity is expressed as\n\n  + **0** (zero) if **i** has an even number of bits set to **1**.\n  + **1** (one) if the number of bits set to one **1** is odd,\n\n### **Options**\n\n- **i**\n  : The value to query for its bit parity\n\n### **Result**\n\n  The return value is equal to **0** if **i** has an even number of bits\n  set and **1** if an odd number of bits are set.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_poppar\nuse, intrinsic :: iso_fortran_env, only : integer_kinds, &\n   & int8, int16, int32, int64\nimplicit none\ncharacter(len=*),parameter :: pretty='(b64,1x,i0)'\n   ! basic usage\n   print pretty, 127,     poppar(127)\n   print pretty, 128,     poppar(128)\n   print pretty, int(b\"01010\"), poppar(int(b\"01010\"))\n\n   ! any kind of an integer can be used\n   print pretty, huge(0_int8),  poppar(huge(0_int8))\n   print pretty, huge(0_int16), poppar(huge(0_int16))\n   print pretty, huge(0_int32), poppar(huge(0_int32))\n   print pretty, huge(0_int64), poppar(huge(0_int64))\nend program demo_poppar\n```\nResults:\n```text\n >                                                          1111111 1\n >                                                         10000000 1\n >                                                             1010 0\n >                                  1111111111111111111111111111111 1\n >                                                          1111111 1\n >                                                  111111111111111 1\n >                                  1111111111111111111111111111111 1\n >  111111111111111111111111111111111111111111111111111111111111111 1\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\nThere are many procedures that operator or query values at the bit level:\n\n[**popcnt**(3)](#popcnt),\n[**leadz**(3)](#leadz),\n[**trailz**(3)](#trailz)\n[**atomic_and**(3)](#atomic_and),\n[**atomic_fetch_and**(3)](#atomic_fetch_and),\n[**atomic_fetch_or**(3)](#atomic_fetch_or),\n[**atomic_fetch_xor**(3)](#atomic_fetch_xor),\n[**atomic_or**(3)](#atomic_or),\n[**atomic_xor**(3)](#atomic_xor),\n[**bge**(3)](#bge),\n[**bgt**(3)](#bgt),\n[**bit_size**(3)](#bit_size),\n[**ble**(3)](#ble),\n[**blt**(3)](#blt),\n[**btest**(3)](#btest),\n[**dshiftl**(3)](#dshiftl),\n[**dshiftr**(3)](#dshiftr),\n[**iall**(3)](#iall),\n[**iand**(3)](#iand),\n[**iany**(3)](#iany),\n[**ibclr**(3)](#ibclr),\n[**ibits**(3)](#ibits),\n[**ibset**(3)](#ibset),\n[**ieor**(3)](#ieor),\n[**ior**(3)](#ior),\n[**iparity**(3)](#iparity),\n[**ishftc**(3)](#ishftc),\n[**ishft**(3)](#ishft),\n[**maskl**(3)](#maskl),\n[**maskr**(3)](#maskr),\n[**merge_bits**(3)](#merge_bits),\n[**mvbits**(3)](#mvbits),\n[**not**(3)](#not),\n[**shifta**(3)](#shifta),\n[**shiftl**(3)](#shiftl),\n[**shiftr**(3)](#shiftr),\n[**storage_size**(3)](#storage_size)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "PRECISION": "## precision\n\n### **Name**\n\n**precision** - \\[NUMERIC MODEL\\] Decimal precision of a real kind\n\n### **Synopsis**\n```fortran\n    result = precision(x)\n```\n```fortran\n     integer function precision(x)\n\n      TYPE(kind=**),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** shall be of type _real_ or _complex_. It may be a scalar or an array.\n - the result is a default _integer_ scalar.\n\n### **Description**\n\n  **precision** returns the decimal precision in the model of the type\n  of **x**.\n\n### **Options**\n\n- **x**\n  : the type and kind of the argument are used to determine which number\n  model to query.  The value of the argument is not unused; it may even\n  be undefined.\n\n### **Result**\n\n   The precision of values of the type and kind of **x**\n<!--\n   Result Value. The result has the value INT ((p - 1) * LOG10 (b)) + k, where b and p are as defined in 16.4\n   for the model representing real numbers with the same value for the kind type parameter as X, and where k is 1\n   if b is an integral power of 10 and 0 otherwise.\n-->\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_precision\nuse,intrinsic :: iso_fortran_env, only : dp=>real64,sp=>real32\nimplicit none\nreal(kind=sp)    :: x(2)\ncomplex(kind=dp) :: y\n\n   print *, precision(x), range(x)\n   print *, precision(y), range(y)\n\nend program demo_precision\n```\nResults:\n```text\n  >           6          37\n  >          15         307\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "PRESENT": "## present\n\n### **Name**\n\n**present** - [STATE:INQUIRY\\] Determine whether an optional dummy argument\nis specified\n\n### **Synopsis**\n```fortran\n    result = present(a)\n```\n```fortran\n     logical function present (a)\n\n      type(TYPE(kind=KIND)) :: a(..)\n```\n### **Characteristics**\n\n- **a** May be of any type and may be a pointer, scalar or array value,\n  or a dummy procedure.\n\n### **Description**\n\n  **present** can be used in a procedure to determine if an optional\n  dummy argument was present on the current call to the procedure.\n\n  **a** shall be the name of an optional dummy argument that is accessible\n  in the subprogram in which the **present** function reference\n  appears. There are no other requirements on **a**.\n\n  Note when an argument is not present when the current procedure is\n  invoked, you may only pass it as an optional argument to another\n  procedure or pass it as an argument to **present**.\n\n### **Options**\n\n- **a**\n  : the name of an optional dummy argument accessible within the current\n  subroutine or function.\n\n### **Result**\n\n  Returns _.true._ if the optional argument **a** is present (was passed\n  on the call to the procedure) , or _.false._ otherwise.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_present\nimplicit none\ninteger :: answer\n   ! argument to func() is not present\n   answer=func()\n   write(*,*) answer\n   ! argument to func() is present\n   answer=func(1492)\n   write(*,*) answer\ncontains\n!\ninteger function func(x)\n! the optional characteristic on this definition allows this variable\n! to not be specified on a call; and also allows it to subsequently\n! be passed to PRESENT(3):\ninteger, intent(in), optional :: x\ninteger :: x_local\n   !\n   ! basic\n   if(present(x))then\n     ! if present, you can use x like any other variable.\n     x_local=x\n   else\n     ! if not, you cannot define or reference x except to\n     ! pass it as an optional parameter to another procedure\n     ! or in a call to present(3f)\n     x_local=0\n   endif\n   !\n   func=x_local**2\n   !\n   ! passing the argument on to other procedures\n   ! so something like this is a bad idea because x is used\n   ! as the first argument to merge(3f) when it might not be\n   ! present\n   ! xlocal=merge(x,0,present(x)) ! NO!!\n   !\n   ! We can pass it to another procedure if another\n   ! procedure declares the argument as optional as well,\n   ! or we have tested that X is present\n   call tattle('optional argument x',x)\n   if(present(x))call not_optional(x)\nend function\n!\nsubroutine tattle(label,arg)\ncharacter(len=*),intent(in) :: label\ninteger,intent(in),optional :: arg\n   if(present(arg))then\n      write(*,*)label,' is present'\n   else\n      write(*,*)label,' is not present'\n   endif\nend subroutine tattle\n!\nsubroutine not_optional(arg)\ninteger,intent(in) :: arg\n   write(*,*)'already tested X is defined',arg\nend subroutine not_optional\n!\nend program demo_present\n```\nResults:\n```text\n    optional argument x is not present\n              0\n    optional argument x is present\n    already tested X is defined 1492\n        2226064\n```\n### **Standard**\n\nFortran 95\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "PRODUCT": "## product\n\n### **Name**\n\n**product** - \\[ARRAY:REDUCTION\\] Product of array elements\n\n### **Synopsis**\n```fortran\n    result = product(array [,dim] [,mask])\n```\n```fortran\n     NUMERIC function product(array, dim, mask)\n\n      NUMERIC,intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n```\n### **Characteristics**\n\n  - a kind designated as ** may be any supported kind for the type\n  - **NUMERIC** is any numeric type and kind.\n\n### **Description**\n\n**product** multiplies together all the selected elements of **array**,\nor along dimension **dim** if the corresponding element in **mask**\nis _.true._.\n\nIf **dim** is absent, a scalar with the product of all elements in **array** is\nreturned. (Note a zero-sized **array** returns **1**).\n\nWhen **dim** is present, If the masked array has a dimension of one\n(ie. is a vector) the result is a scalar. Otherwise, an array of rank\n**n-1**, where **n** equals the rank of **array**, and a shape similar\nto that of **array** with dimension **dim** dropped is returned.\n\n### **Options**\n\n- **array**\n  : Shall be an array of type _integer_, _real_ or _complex_.\n\n- **dim**\n  : shall be a scalar of type _integer_ with a value in the\n  range from **1 to n**, where **n** equals the rank of **array**.\n\n- **mask**\n  : shall be of type _logical_ and either be a scalar or an\n  array of the same shape as **array**.\n\n### **Result**\n\nThe result is of the same type as **array**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_product\nimplicit none\ncharacter(len=*),parameter :: all='(*(g0,1x))' ! a handy format\ncharacter(len=1),parameter :: nl=new_line('a')\n\nNO_DIM: block\n!    If DIM is not specified, the result is the product of all the\n!    selected array elements.\ninteger :: i,n, p1, p2\ninteger,allocatable :: array(:)\n   ! all elements are selected by default\n   do n=1,10\n      print all, 'factorial of ',n,' is ', product([(real(i),i=1,n)])\n   enddo\n\n   ! using a mask\n   array=[10,12,13,15,20,25,30]\n   p1=product(array, mask=mod(array, 2)==1) ! only odd elements\n   p2=product(array, mask=mod(array, 2)/=1) ! only even elements\n   print all, nl,'product of all elements',product(array) ! all elements\n   print all, ' odd * even =',nl,p1,'*',p2,'=',p1*p2\n\n   ! NOTE: If ARRAY is a zero-sized array, the result is equal to one\n   print all\n   print all, 'zero-sized array=>',product([integer :: ])\n   ! NOTE: If nothing in the mask is true, this also results in a null\n   !       array\n   print all, 'all elements have a false mask=>', &\n            & product(array,mask=.false.)\n\nendblock NO_DIM\n\nWITH_DIM: block\ninteger :: rect(2,3)\ninteger :: box(2,3,4)\n\n!  lets fill a few arrays\n   rect = reshape([ &\n     1, 2, 3,       &\n     4, 5, 6        &\n   ],shape(rect),order=[2,1])\n   call print_matrix_int('rect',rect)\n\n!  Find the product of each column in RECT.\n   print all, 'product of columns=',product(rect, dim = 1)\n\n! Find the product of each row in RECT.\n   print all, 'product of rows=',product(rect, dim = 2)\n\n! now lets try a box\n   box(:,:,1)=rect\n   box(:,:,2)=rect*(+10)\n   box(:,:,3)=rect*(-10)\n   box(:,:,4)=rect*2\n   ! lets look at the values\n   call print_matrix_int('box 1',box(:,:,1))\n   call print_matrix_int('box 2',box(:,:,2))\n   call print_matrix_int('box 3',box(:,:,3))\n   call print_matrix_int('box 4',box(:,:,4))\n\n   ! remember without dim= even a box produces a scalar\n   print all, 'no dim gives a scalar',product(real(box))\n\n   ! only one plane has negative values, so note all the \"1\" values\n   ! for vectors with no elements\n   call print_matrix_int('negative values', &\n   & product(box,mask=box < 0,dim=1))\n\n!   If DIM is specified and ARRAY has rank greater than one, the\n!   result is a new array in which dimension DIM has been eliminated.\n\n   ! pick a dimension to multiply though\n   call print_matrix_int('dim=1',product(box,dim=1))\n\n   call print_matrix_int('dim=2',product(box,dim=2))\n\n   call print_matrix_int('dim=3',product(box,dim=3))\n\nendblock WITH_DIM\n\ncontains\n\nsubroutine print_matrix_int(title,arr)\nimplicit none\n\n!@(#) print small 2d integer arrays in row-column format\n\ncharacter(len=*),intent(in)  :: title\ninteger,intent(in)           :: arr(:,:)\ninteger                      :: i\ncharacter(len=:),allocatable :: biggest\n\n   print all\n   print all, trim(title),':(',shape(arr),')'  ! print title\n   biggest='           '  ! make buffer to write integer into\n   ! find how many characters to use for integers\n   write(biggest,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(arr))))))+2\n   ! use this format to write a row\n   biggest='(\" > [\",*(i'//trim(biggest)//':,\",\"))'\n   ! print one row of array at a time\n   do i=1,size(arr,dim=1)\n      write(*,fmt=biggest,advance='no')arr(i,:)\n      write(*,'(\" ]\")')\n   enddo\n\nend subroutine print_matrix_int\n\nend program demo_product\n```\n\nResults:\n\n```text\nfactorial of  1  is  1.000000\nfactorial of  2  is  2.000000\nfactorial of  3  is  6.000000\nfactorial of  4  is  24.00000\nfactorial of  5  is  120.0000\nfactorial of  6  is  720.0000\nfactorial of  7  is  5040.000\nfactorial of  8  is  40320.00\nfactorial of  9  is  362880.0\nfactorial of  10  is  3628800.\n\n product of all elements 351000000\n odd * even =\n 4875 * 72000 = 351000000\n\nzero-sized array=> 1\nall elements have a false mask=> 1\n\nrect :( 2 3 )\n > [  1,  2,  3 ]\n > [  4,  5,  6 ]\nproduct of columns= 4 10 18\nproduct of rows= 6 120\n\nbox 1 :( 2 3 )\n > [  1,  2,  3 ]\n > [  4,  5,  6 ]\n\nbox 2 :( 2 3 )\n > [  10,  20,  30 ]\n > [  40,  50,  60 ]\n\nbox 3 :( 2 3 )\n > [ -10, -20, -30 ]\n > [ -40, -50, -60 ]\n\nbox 4 :( 2 3 )\n > [   2,   4,   6 ]\n > [   8,  10,  12 ]\nno dim gives a scalar .1719927E+26\n\nnegative values :( 3 4 )\n > [     1,     1,   400,     1 ]\n > [     1,     1,  1000,     1 ]\n > [     1,     1,  1800,     1 ]\n\ndim=1 :( 3 4 )\n > [     4,   400,   400,    16 ]\n > [    10,  1000,  1000,    40 ]\n > [    18,  1800,  1800,    72 ]\n\ndim=2 :( 2 4 )\n > [       6,    6000,   -6000,      48 ]\n > [     120,  120000, -120000,     960 ]\n\ndim=3 :( 2 3 )\n > [    -200,   -3200,  -16200 ]\n > [  -51200, -125000, -259200 ]\n```\n\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**sum**(3)](#sum), note that an element by element multiplication is done\ndirectly using the star character.\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "RADIX": "## radix\n\n### **Name**\n\n**radix** - \\[NUMERIC MODEL\\] Base of a numeric model\n\n### **Synopsis**\n```fortran\n   result = radix(x)\n```\n```fortran\n    integer function radix(x)\n\n     TYPE(kind=**),intent(in) :: x(..)\n```\n### **Characteristics**\n\n   - **x** may be scalar or an array of any _real_ or _integer_ type.\n   - the result is a default integer scalar.\n\n### **Description**\n\n  **radix** returns the base of the internal model representing the\n  numeric entity **x**.\n\n  In a positional numeral system, the radix or base is the number of\n  unique digits, including the digit zero, used to represent numbers.\n\n  This function helps to represent the internal computing model\n  generically, but will be 2 (representing a binary machine) for any\n  common platform for all the numeric types.\n\n### **Options**\n\n- **x**\n  : used to identify the type of number to query.\n\n### **Result**\n\n  The returned value indicates what base is internally used to represent\n  the type of numeric value **x** represents.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_radix\nimplicit none\n   print *, \"The radix for the default integer kind is\", radix(0)\n   print *, \"The radix for the default real kind is\", radix(0.0)\n   print *, \"The radix for the doubleprecision real kind is\", radix(0.0d0)\nend program demo_radix\n```\nResults:\n```text\n >  The radix for the default integer kind is           2\n >  The radix for the default real kind is           2\n >  The radix for the doubleprecision real kind is           2\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
-    "RANDOM_INIT": "## random_init\n\n### **Name**\n\n**random_init** - \\[MATHEMATICS:RANDOM\\] Initializes the state of\nthe pseudorandom number generator\n\n### **Synopsis**\n```fortran\n    call random_init(repeatable, image_distinct)\n\n     logical,intent(in) :: repeatable\n     logical,intent(in) :: image_distinct\n```\n### **Characteristics**\n\n- **harvest** and **image_distinct** are logical scalars\n\n### Description\n\nInitializes the state of the pseudorandom number generator used by \n**random_number**.\n\n### **Options**\n\n**repeatable**\n: If it is **.true.**, the seed is set to a processor-dependent\nvalue that is the same each time **random_init** is called from the\nsame image. The term \"same image\" means a single instance of program\nexecution. The sequence of random numbers is different for repeated\nexecution of the program. \n\nIf it is **.false.**, the seed is set to a processor-dependent value.\n\n**image_distinct**\n: If is `.true.`, the seed is set to a processor-dependent value that\nis distinct from the seed set by a call to **random_init**in another\nimage. If it is **.false.**, the seed is set value that does depend\nwhich image called **random_init**.\n\n\n### **Examples**\n\nSample program:\n\n```fortran\n    program demo_random_init\n    implicit none\n    real x(3), y(3)\n       call random_init(.true., .true.)\n       call random_number(x)\n       call random_init(.true., .true.)\n       call random_number(y)\n       ! x and y should be the same sequence\n       if ( any(x /= y) ) stop \"x(:) and y(:) are not all equal\"\n    end program demo_random_init\n```\n## **Standard**\n\nFortran 2018\n```\n## **See also**\n\n[random_number](#random_number),\n[random_seed](random_seed)\n\n _fortran-lang intrinsic descriptions\n",
+    "RANDOM_INIT": "## random_init\n\n### **Name**\n\n**random_init** - \\[MATHEMATICS:RANDOM\\] Initializes the state of\nthe pseudorandom number generator\n\n### **Synopsis**\n```fortran\n    call random_init(repeatable, image_distinct)\n\n     logical,intent(in) :: repeatable\n     logical,intent(in) :: image_distinct\n```\n### **Characteristics**\n\n- **harvest** and **image_distinct** are logical scalars\n\n### Description\n\nInitializes the state of the pseudorandom number generator used by\n**random_number**.\n\n### **Options**\n\n**repeatable**\n: If it is **.true.**, the seed is set to a processor-dependent\nvalue that is the same each time **random_init** is called from the\nsame image. The term \"same image\" means a single instance of program\nexecution. The sequence of random numbers is different for repeated\nexecution of the program.\n\nIf it is **.false.**, the seed is set to a processor-dependent value.\n\n**image_distinct**\n: If is `.true.`, the seed is set to a processor-dependent value that\nis distinct from the seed set by a call to **random_init**in another\nimage. If it is **.false.**, the seed is set value that does depend\nwhich image called **random_init**.\n\n\n### **Examples**\n\nSample program:\n\n```fortran\n    program demo_random_init\n    implicit none\n    real x(3), y(3)\n       call random_init(.true., .true.)\n       call random_number(x)\n       call random_init(.true., .true.)\n       call random_number(y)\n       ! x and y should be the same sequence\n       if ( any(x /= y) ) stop \"x(:) and y(:) are not all equal\"\n    end program demo_random_init\n```\n## **Standard**\n\nFortran 2018\n\n## **See also**\n\n[random_number](#random_number),\n[random_seed](random_seed)\n\n _fortran-lang intrinsic descriptions\n",
     "RANDOM_NUMBER": "## random_number\n\n### **Name**\n\n**random_number** - \\[MATHEMATICS:RANDOM\\] Pseudo-random number\n\n### **Synopsis**\n```fortran\n    call random_number(harvest)\n```\n```fortran\n     subroutine random_number(harvest)\n\n      real,intent(out) :: harvest(..)\n```\n### **Characteristics**\n\n- **harvest** and the result are default _real_ variables\n\n### **Description**\n\n**random_number** returns a single pseudorandom number or an array of\npseudorandom numbers from the uniform distribution over the range\n0 \\<= x \\< 1.\n\n### **Options**\n\n- **harvest**\n  : Shall be a scalar or an array of type _real_.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_random_number\nuse, intrinsic :: iso_fortran_env, only : dp=>real64\nimplicit none\ninteger, allocatable :: seed(:)\ninteger              :: n\ninteger              :: first,last\ninteger              :: i\ninteger              :: rand_int\ninteger,allocatable  :: count(:)\nreal(kind=dp)        :: rand_val\n   call random_seed(size = n)\n   allocate(seed(n))\n   call random_seed(get=seed)\n   first=1\n   last=10\n   allocate(count(last-first+1))\n   ! To have a discrete uniform distribution on the integers\n   ! [first, first+1, ..., last-1, last] carve the continuous\n   ! distribution up into last+1-first equal sized chunks,\n   ! mapping each chunk to an integer.\n   !\n   ! One way is:\n   !   call random_number(rand_val)\n   ! choose one from last-first+1 integers\n   !   rand_int = first + FLOOR((last+1-first)*rand_val)\n      count=0\n      ! generate a lot of random integers from 1 to 10 and count them.\n      ! with a large number of values you should get about the same\n      ! number of each value\n      do i=1,100000000\n         call random_number(rand_val)\n         rand_int=first+floor((last+1-first)*rand_val)\n         if(rand_int.ge.first.and.rand_int.le.last)then\n            count(rand_int)=count(rand_int)+1\n         else\n            write(*,*)rand_int,' is out of range'\n         endif\n      enddo\n      write(*,'(i0,1x,i0)')(i,count(i),i=1,size(count))\nend program demo_random_number\n```\nResults:\n```\n   1 10003588\n   2 10000104\n   3 10000169\n   4 9997996\n   5 9995349\n   6 10001304\n   7 10001909\n   8 9999133\n   9 10000252\n   10 10000196\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**random_seed**(3)](#random_seed)\n\n _fortran-lang intrinsic descriptions_\n",
-    "RANDOM_SEED": "## random_seed\n\n### **Name**\n\n**random_seed** - \\[MATHEMATICS:RANDOM\\] Initialize a pseudo-random number sequence\n\n### **Synopsis**\n```fortran\n    call random_seed( [size] [,put] [,get] )\n```\n```fortran\n     subroutine random_seed( size, put, get )\n\n      integer,intent(out),optional :: size\n      integer,intent(in),optional :: put(*)\n      integer,intent(out),optional :: get(*)\n```\n### **Characteristics**\n - **size** a scalar default _integer_\n - **put** a rank-one default _integer_ array\n - **get** a rank-one default _integer_ array\n - the result\n\n### **Description**\n\n**random_seed** restarts or queries the state of the pseudorandom\nnumber generator used by random_number.\n\nIf random_seed is called without arguments, it is seeded with random\ndata retrieved from the operating system.\n\n### **Options**\n\n- **size**\n  : specifies the minimum size of the arrays used with the **put**\n  and **get** arguments.\n\n- **put**\n  : the size of the array must be larger than or equal to the number\n  returned by the **size** argument.\n\n- **get**\n  : It is **intent(out)** and the size of the array must be larger than\n  or equal to the number returned by the **size** argument.\n\n### **Examples**\n\nSample program:\n\n```fortran\n    program demo_random_seed\n    implicit none\n    integer, allocatable :: seed(:)\n    integer :: n\n    \n       call random_seed(size = n)\n       allocate(seed(n))\n       call random_seed(get=seed)\n       write (*, *) seed\n    \n    end program demo_random_seed\n```\nResults:\n```text\n     -674862499 -1750483360  -183136071  -317862567   682500039\n     349459   344020729 -1725483289\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**random_number**(3)](#random_number)\n\n _fortran-lang intrinsic descriptions_\n",
+    "RANDOM_SEED": "## random_seed\n\n### **Name**\n\n**random_seed** - \\[MATHEMATICS:RANDOM\\] Initialize a pseudo-random number sequence\n\n### **Synopsis**\n```fortran\n    call random_seed( [size] [,put] [,get] )\n```\n```fortran\n     subroutine random_seed( size, put, get )\n\n      integer,intent(out),optional :: size\n      integer,intent(in),optional :: put(*)\n      integer,intent(out),optional :: get(*)\n```\n### **Characteristics**\n - **size** a scalar default _integer_\n - **put** a rank-one default _integer_ array\n - **get** a rank-one default _integer_ array\n - the result\n\n### **Description**\n\n**random_seed** restarts or queries the state of the pseudorandom\nnumber generator used by random_number.\n\nIf random_seed is called without arguments, it is seeded with random\ndata retrieved from the operating system.\n\n### **Options**\n\n- **size**\n  : specifies the minimum size of the arrays used with the **put**\n  and **get** arguments.\n\n- **put**\n  : the size of the array must be larger than or equal to the number\n  returned by the **size** argument.\n\n- **get**\n  : It is **intent(out)** and the size of the array must be larger than\n  or equal to the number returned by the **size** argument.\n\n### **Examples**\n\nSample program:\n\n```fortran\n    program demo_random_seed\n    implicit none\n    integer, allocatable :: seed(:)\n    integer :: n\n\n       call random_seed(size = n)\n       allocate(seed(n))\n       call random_seed(get=seed)\n       write (*, *) seed\n\n    end program demo_random_seed\n```\nResults:\n```text\n     -674862499 -1750483360  -183136071  -317862567   682500039\n     349459   344020729 -1725483289\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**random_number**(3)](#random_number)\n\n _fortran-lang intrinsic descriptions_\n",
     "RANGE": "## range\n\n### **Name**\n\n**range** - \\[NUMERIC MODEL\\] Decimal exponent range of a numeric kind\n\n### **Synopsis**\n```fortran\n    result = range(x)\n```\n```fortran\n      integer function range (x)\n\n       TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** may be of type _integer_, _real_, or _complex_. It may be a scalar or an array.\n - **KIND** is any kind supported by the type of **x**\n - the result is a default _integer_ scalar\n\n### **Description**\n\n  **range** returns the decimal exponent range in the model of the\n  type of **x**.\n\n  Since **x** is only used to determine the type and kind being\n  interrogated, the value need not be defined.\n\n### **Options**\n\n- **x**\n  : the value whose type and kind are used for the query\n\n### **Result**\n\n  Case (i)\n  : For an integer argument, the result has the value\n```fortran\n    int (log10 (huge(x)))\n```\n  Case (ii)\n  : For a real argument, the result has the value\n```fortran\n     int(min (log10 (huge(x)), -log10(tiny(x) )))\n  ```\n  Case (iii)\n  : For a complex argument, the result has the value\n```fortran\n    range(real(x))\n```\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_range\nuse,intrinsic :: iso_fortran_env, only : dp=>real64,sp=>real32\nimplicit none\nreal(kind=sp)    :: x(2)\ncomplex(kind=dp) :: y\n   print *, precision(x), range(x)\n   print *, precision(y), range(y)\nend program demo_range\n```\nResults:\n```text\n >            6          37\n >           15         307\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "RANK": "## rank\n\n### **Name**\n\n**rank** - \\[ARRAY:INQUIRY\\] Rank of a data object\n\n### **Synopsis**\n```fortran\n    result = rank(a)\n```\n```fortran\n     integer function rank(a)\n\n      type(TYPE(kind=**)),intent(in) :: a(..)\n```\n### **Characteristics**\n\n -  **a** can be of any type **TYPE** and rank.\n - a kind designated as ** may be any supported kind for the type\n\n### **Description**\n\n  **rank** returns the rank of a scalar or array data object.\n\n  The rank of an array is the number of dimensions it has (zero for a scalar).\n\n### **Options**\n\n- **a** is the data object to query the dimensionality of. The rank returned\n  may be from 0 to 16.\n\n  The argument **a** may be any data object type, including an assumed-rank\n  array.\n\n### **Result**\n\n  For arrays, their rank is returned; for scalars zero is returned.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_rank\nimplicit none\n\n! a bunch of data objects to query\ninteger           :: a\nreal, allocatable :: b(:,:)\nreal, pointer     :: c(:)\ncomplex           :: d\n\n! make up a type\ntype mytype\n   integer :: int\n   real :: float\n   character :: char\nend type mytype\ntype(mytype) :: any_thing(1,2,3,4,5)\n\n  ! basics\n   print *, 'rank of scalar a=',rank(a)\n   ! you can query this array even though it is not allocated\n   print *, 'rank of matrix b=',rank(b)\n   print *, 'rank of vector pointer c=',rank(c)\n   print *, 'rank of complex scalar d=',rank(d)\n\n  ! you can query any type, not just intrinsics\n   print *, 'rank of any arbitrary type=',rank(any_thing)\n\n  ! an assumed-rank object may be queried\n   call query_int(10)\n   call query_int([20,30])\n   call query_int( reshape([40,50,60,70],[2,2]) )\n\n  ! you can even query an unlimited polymorphic entity\n   call query_anything(10.0)\n   call query_anything([.true.,.false.])\n   call query_anything( reshape([40.0,50.0,60.0,70.0],[2,2]) )\n\ncontains\n\nsubroutine query_int(data_object)\n! It is hard to do much with something dimensioned\n! name(..) if not calling C except inside of a\n! SELECT_RANK construct but one thing you can\n! do is call the inquiry functions ...\ninteger,intent(in) :: data_object(..)\ncharacter(len=*),parameter :: all='(*(g0,1x))'\n\n   if(rank(data_object).eq.0)then\n      print all,&\n      & 'passed a scalar to an assumed rank,  &\n      & rank=',rank(data_object)\n   else\n      print all,&\n      & 'passed an array to an assumed rank,  &\n      & rank=',rank(data_object)\n   endif\n\nend subroutine query_int\n\nsubroutine query_anything(data_object)\nclass(*),intent(in) ::data_object(..)\ncharacter(len=*),parameter :: all='(*(g0,1x))'\n  if(rank(data_object).eq.0)then\n    print all,&\n    &'passed a scalar to an unlimited polymorphic rank=', &\n    & rank(data_object)\n  else\n    print all,&\n    & 'passed an array to an unlimited polymorphic, rank=', &\n    & rank(data_object)\n  endif\nend subroutine query_anything\n\nend program demo_rank\n```\nResults:\n```text\n    rank of scalar a=           0\n    rank of matrix b=           2\n    rank of vector pointer c=           1\n    rank of complex scalar d=           0\n    rank of any arbitrary type=           5\n   passed a scalar to an assumed rank,   rank= 0\n   passed an array to an assumed rank,   rank= 1\n   passed an array to an assumed rank,   rank= 2\n   passed a scalar to an unlimited polymorphic rank= 0\n   passed an array to an unlimited polymorphic, rank= 1\n   passed an array to an unlimited polymorphic, rank= 2\n```\n### **Standard**\n\n### **See also**\n\n#### Array inquiry:\n\n- [**size**(3)](#size) -  Determine the size of an array\n- [**rank**](#rank) -  Rank of a data object\n- [**shape**(3)](#shape) -  Determine the shape of an array\n- [**ubound**(3)](#ubound) -  Upper dimension bounds of an array\n- [**lbound**(3)](#lbound) -  Lower dimension bounds of an array\n\n#### State Inquiry:\n\n- [**allocated**(3)](#allocated) -  Status of an allocatable entity\n- [**is_contiguous**(3)](#is_contiguous) -  Test if object is contiguous\n\n#### Kind Inquiry:\n\n- [**kind**(3)](#kind) - Kind of an entity\n\n#### Bit Inquiry:\n\n- [**storage_size**(3)](#storage_size) - Storage size in bits\n- [**bit_size**(3)](#bit_size) -  Bit size inquiry function\n- [**btest**(3)](#btest) - Tests a bit of an _integer_ value.\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n#\n",
     "REAL": "## real\n\n### **Name**\n\n**real** - \\[TYPE:NUMERIC\\] Convert to real type\n\n### **Synopsis**\n```fortran\n  result = real(x [,kind])\n```\n```fortran\n   elemental real(kind=KIND) function real(x,KIND)\n\n    TYPE(kind=**),intent(in) :: x\n    integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n - the type of **x** may be _integer_, _real_, or _complex_; or a BOZ-literal-constant.\n - **kind** is a _integer_ initialization expression (a constant expression)\n   + If **kind** is present it defines the kind of the _real_ result\n   + if **kind** is not present\n     - when **x** is _complex_ the result is a _real_ of the same kind as **x**.\n     - when **x** is _real_ or _integer_ the result is a _real_ of default kind\n - a kind designated as ** may be any supported kind for the type\n\n### **Description**\n\n**real** converts its argument **x** to a _real_ type.\n\nThe real part of a complex value is returned. For complex values this\nis similar to the modern complex-part-designator **%RE** which also\ndesignates the real part of a _complex_ value.\n\n```fortran\n      z=(3.0,4.0)     ! if z is a complex value\n      print *, z%re == real(z) ! these expressions are equivalent\n```\n### **Options**\n\n- **x**\n  : An _integer_, _real_, or _complex_ value to convert to _real_.\n\n- **kind**\n  : When present the value of **kind** defines the kind of the result.\n\n### **Result**\n\n1.  **real(x)** converts **x** to a default _real_ type if **x** is an _integer_\n    or _real_ variable.\n\n2.  **real(x)** converts a _complex_ value to a _real_ type with the\n    magnitude of the real component of the input with kind type\n    parameter the same as **x**.\n\n3.  **real(x, kind)** is converted to a _real_ type with kind type\n    parameter **kind** if **x** is a _complex_, _integer_, or _real_ variable.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_real\nuse,intrinsic :: iso_fortran_env, only : dp=>real64\nimplicit none\ncomplex              :: zr = (1.0, 2.0)\ndoubleprecision      :: xd=huge(3.0d0)\ncomplex(kind=dp) :: zd=cmplx(4.0e0_dp,5.0e0_dp,kind=dp)\n\n   print *, real(zr), aimag(zr)\n   print *, dble(zd), aimag(zd)\n\n   write(*,*)xd,real(xd,kind=kind(0.0d0)),dble(xd)\nend program demo_real\n```\nResults:\n```\n 1.00000000       2.00000000\n 4.0000000000000000       5.0000000000000000\n 1.7976931348623157E+308  1.7976931348623157E+308  1.7976931348623157E+308\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n- [**aimag**(3)](#aimag) - Imaginary part of complex number\n- [**cmplx**(3)](#cmplx) - Complex conversion function\n- [**conjg**(3)](#conjg) - Complex conjugate function\n\nFortran has strong support for _complex_ values, including many intrinsics\nthat take or produce _complex_ values in addition to algebraic and\nlogical expressions:\n\n[**abs**(3)](#abs),\n[**acosh**(3)](#acosh),\n[**acos**(3)](#acos),\n[**asinh**(3)](#asinh),\n[**asin**(3)](#asin),\n[**atan2**(3)](#atan2),\n[**atanh**(3)](#atanh),\n[**atan**(3)](#atan),\n[**cosh**(3)](#cosh),\n[**cos**(3)](#cos),\n[**co_sum**(3)](#co_sum),\n[**dble**(3)](#dble),\n[**dot_product**(3)](#dot_product),\n[**exp**(3)](#exp),\n[**int**(3)](#int),\n[**is_contiguous**(3)](#is_contiguous),\n[**kind**(3)](#kind),\n[**log**(3)](#log),\n[**matmul**(3)](#matmul),\n[**precision**(3)](#precision),\n[**product**(3)](#product),\n[**range**(3)](#range),\n[**rank**(3)](#rank),\n[**sinh**(3)](#sinh),\n[**sin**(3)](#sin),\n[**sqrt**(3)](#sqrt),\n[**storage_size**(3)](#storage_size),\n[**sum**(3)](#sum),\n[**tanh**(3)](#tanh),\n[**tan**(3)](#tan),\n[**unpack**(3)](#unpack),\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "REDUCE": "## reduce\n\n### **Name**\n\n**reduce** - \\[TRANSFORMATIONAL\\] General reduction of an array\n\n### **Synopsis**\n\nThere are two forms to this function:\n```fortran\n   result = reduce(array, operation [,mask]  [,identity]  [,ordered] )\n```\nor\n```fortran\n   result = reduce (array, operation, dim  &\n   & [,mask] [,identity] [,ordered] )\n```\n```fortran\n    type(TYPE(kind=KIND)) function reduce &\n    & (array, operation, dim, mask, identity, ordered )\n\n     type(TYPE(kind=KIND)),intent(in) :: array\n     pure function                  :: operation\n     integer,intent(in),optional    :: dim\n     logical,optional               :: mask\n     type(TYPE),intent(in),optional :: identity\n     logical,intent(in),optional    :: ordered\n```\n### **Characteristics**\n\n - **array** is an array of any type\n - **operation** is a pure function with exactly two arguments\n   + each argument is scalar, non-allocatable, a nonpointer,\n     nonpolymorphic and nonoptional with the same type and kind as array.\n   + if one argument has the asynchronous, target, or value attribute so\n     shall the other.\n - **dim** is an _integer_ scalar\n - **mask** is a logical conformable with **array**\n - **identity** is a scalar with the same type and type parameters as **array**\n - **ordered** is a logical scalar\n - the result is of the same type and type parameters as **array**.\n\n### **Description**\n\n   **reduce** reduces a list of conditionally selected values from\n   an array to a single value by iteratively applying a binary function.\n\n   Common in functional programming, a **reduce** function applies a\n   binary operator (a pure function with two arguments) to all elements\n   cumulatively.\n\n   **reduce** is a \"higher-order\" function; ie. it is a function that\n   receives other functions as arguments.\n\n   The **reduce** function receives a binary operator (a function with\n   two arguments, just like the basic arithmetic operators). It is first\n   applied to two unused values in the list to generate an accumulator\n   value which is subsequently used as the first argument to the function\n   as the function is recursively applied to all the remaining selected\n   values in the input array.\n\n### **Options**\n\n- **array**\n  : An array of any type and allowed rank to select values from.\n\n- **operation**\n  : shall be a pure function with exactly two arguments;\n  each argument shall be a scalar, nonallocatable,\n  nonpointer, nonpolymorphic, nonoptional dummy data object\n  with the same type and type parameters as **array**. If\n  one argument has the ASYNCHRONOUS, TARGET, or VALUE\n  attribute, the other shall have that attribute. Its result\n  shall be a nonpolymorphic scalar and have the same type\n  and type parameters as **array**. **operation** should\n  implement a mathematically associative operation. It\n  need not be commutative.\n\n  NOTE\n\n  If **operation** is not computationally associative, REDUCE\n  without ORDERED=.TRUE. with the same argument values\n  might not always produce the same result, as the processor\n  can apply the associative law to the evaluation.\n\n  Many operations that mathematically are associative are\n  not when applied to floating-point numbers. The order\n  you sum values in may affect the result, for example.\n\n- **dim**\n  : An integer scalar with a value in the range\n  1<= **dim** <= n, where n is the rank of **array**.\n\n- **mask**\n  : (optional) shall be of type logical and shall be\n  conformable with **array**.\n\n  When present only those elements of **array** are passed\n  to **operation** for which the corresponding elements\n  of **mask** are true, as if **array* was filtered with\n  **pack(3)**.\n\n- **identity**\n  : shall be scalar with the same type and type parameters as **array**.\n  If the initial sequence is empty, the result has the value **identify**\n  if **identify** is present, and otherwise, error termination is\n  initiated.\n\n- **ordered**\n  : shall be a logical scalar. If **ordered** is present with the value\n  _.true._, the calls to the **operator** function begins with the first\n  two elements of **array** and the process continues in row-column\n  order until the sequence has only one element which is the value of the\n  reduction. Otherwise, the compiler is free to assume that the operation\n  is commutative and may evaluate the reduction in the most optimal way.\n\n### **Result**\n\nThe result is of the same type and type parameters as **array**. It is\nscalar if **dim** does not appear.\n\nIf **dim** is present, it indicates the one dimension along which to\nperform the reduction, and the resultant array has a rank reduced by\none relative to the input array.\n\n### **Examples**\n\n   The following examples all use the function MY\\_MULT, which returns\n   the product of its two real arguments.\n```fortran\n   program demo_reduce\n   implicit none\n   character(len=*),parameter :: f='(\"[\",*(g0,\",\",1x),\"]\")'\n   integer,allocatable :: arr(:), b(:,:)\n\n   ! Basic usage:\n      ! the product of the elements of an array\n      arr=[1, 2, 3, 4 ]\n      write(*,*) arr\n      write(*,*) 'product=', reduce(arr, my_mult)\n      write(*,*) 'sum=', reduce(arr, my_sum)\n\n   ! Examples of masking:\n      ! the product of only the positive elements of an array\n      arr=[1, -1, 2, -2, 3, -3 ]\n      write(*,*)'positive value product=',reduce(arr, my_mult, mask=arr>0)\n   ! sum values ignoring negative values\n      write(*,*)'sum positive values=',reduce(arr, my_sum, mask=arr>0)\n\n   ! a single-valued array returns the single value as the\n   ! calls to the operator stop when only one element remains\n      arr=[ 1234 ]\n      write(*,*)'single value sum',reduce(arr, my_sum )\n      write(*,*)'single value product',reduce(arr, my_mult )\n\n   ! Example of operations along a dimension:\n   !  If B is the array   1 3 5\n   !                      2 4 6\n      b=reshape([1,2,3,4,5,6],[2,3])\n      write(*,f) REDUCE(B, MY_MULT),'should be [720]'\n      write(*,f) REDUCE(B, MY_MULT, DIM=1),'should be [2,12,30]'\n      write(*,f) REDUCE(B, MY_MULT, DIM=2),'should be [15, 48]'\n\n   contains\n\n   pure function my_mult(a,b) result(c)\n   integer,intent(in) :: a, b\n   integer            :: c\n      c=a*b\n   end function my_mult\n\n   pure function my_sum(a,b) result(c)\n   integer,intent(in) :: a, b\n   integer            :: c\n      c=a+b\n   end function my_sum\n\n   end program demo_reduce\n```\nResults:\n```text\n     >  1 2 3 4\n     >  product= 24\n     >  sum=     10\n     >  positive value sum= 6\n     >  sum positive values= 6\n     >  single value sum     1234\n     >  single value product 1234\n     > [720, should be [720],\n     > [2, 12, 30, should be [2,12,30],\n     > [15, 48, should be [15, 48],\n```\n### **Standard**\n\n   Fortran 2018\n\n### **See Also**\n- [co_reduce(3)](#co_reduce)\n\n### **Resources**\n\n- [associative:wikipedia](https://en.wikipedia.org/wiki/Associative_property)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "REPEAT": "## repeat\n\n### **Name**\n\n**repeat** - \\[CHARACTER\\] Repeated string concatenation\n\n### **Synopsis**\n```fortran\n    result = repeat(string, ncopies)\n```\n```fortran\n     character(len=len(string)*ncopies) function repeat(string, ncopies)\n\n      character(len=*),intent(in)   :: string\n      integer(kind=**),intent(in)   :: ncopies\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **string** is a scalar _character_ type.\n - **ncopies** is a scalar integer.\n - the result is a new scalar of type _character_ of the same kind as\n   **string**\n\n### **Description**\n\n  **repeat** concatenates copies of a string.\n\n### **Options**\n\n- **string**\n  : The input string to repeat\n\n- **ncopies**\n  : Number of copies to make of **string**, greater than or equal to zero (0).\n\n### **Result**\n\n  A new string built up from **ncopies** copies of **string**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_repeat\nimplicit none\n    write(*,'(a)') repeat(\"^v\", 35)         ! line break\n    write(*,'(a)') repeat(\"_\", 70)          ! line break\n    write(*,'(a)') repeat(\"1234567890\", 7)  ! number line\n    write(*,'(a)') repeat(\"         |\", 7)  !\nend program demo_repeat\n```\nResults:\n```text\n > ^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v^v\n > ______________________________________________________________________\n > 1234567890123456789012345678901234567890123456789012345678901234567890\n >          |         |         |         |         |         |         |\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\nFunctions that perform operations on character strings:\n\n- **Elemental:**\n  [**adjustl**(3)](#adjustl),\n  [**adjustr**(3)](#adjustr),\n  [**index**(3)](#index),\n  [**scan**(3)](#scan),\n  [**verify**(3)](#verify)\n\n- **Non-elemental:**\n  [**len_trim**(3)](#len_trim),\n  [**len**(3)](#len),\n  [**repeat**](#repeat),\n  [**trim**(3)](#trim)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n#\n",
     "RESHAPE": "\n\n## reshape\n\n### **Name**\n\n**reshape** - \\[ARRAY:RESHAPE\\] Function to reshape an array\n\n### **Synopsis**\n```fortran\n    result = reshape( source, shape [,pad] [,order] )\n```\n```fortran\n     type(TYPE(kind=KIND)) function reshape\n\n      type(TYPE(kind=KIND)),intent(in)          :: source(..)\n      integer(kind=**),intent(in)               :: shape(:)\n      type(TYPE(kind=KIND)),intent(in),optional :: pad(..)\n      integer(kind=**),intent(in),optional      :: order(:)\n```\n### **Characteristics**\n\n - **source** is an array of any type\n - **shape** defines a Fortran shape and therefore an _integer_ vector\n   (of rank one) of constant size of up to 16 non-negative values.\n - **pad** is the same type as **source**\n - **order** is the same shape as **shape**\n - The result is an array of shape **shape** with the same type as **source**.\n - a kind designated as ** may be any supported kind for the type\n\n### **Description**\n\n**reshape** constructs an array of arbitrary shape **shape** using the elements\nfrom **source** and possibly **pad** to fill it.\n\nIf necessary, the new array may be padded with elements from **pad**\nor permuted as defined by **order**.\n\nAmong many other uses, **reshape** can be used to reorder a Fortran array\nto match C array ordering before the array is passed from Fortran to a\nC procedure.\n\n### **Options**\n\n- **source**\n  : an array containing the elements to be copied to the result.\n  there must be enough elements in the source to fill the new shape\n  if **pad** is omitted or has size zero. Expressed in Fortran ...\n```fortran\n   if(.not.present(pad))then\n      if(size(source) < product(shape))then\n        stop 'not enough elements in the old array to fill the new one'\n      endif\n   endif\n```\n- **shape**\n  : This is the shape of the new array being generated.\n    Being by definition a shape; all elements are either positive integers\n    or zero, the size but be 1 or greater, it may have up to 16 elements\n    but must be of constant fixed size and rank one.\n\n- **pad**\n  : used to fill in extra values if the result array is larger than **source**.\n    It will be used repeatedly after all the elements of **source** have been\n    placed in the result until the result has all elements assigned.\n  : If it is absent or is a zero-sized array, you can only make\n    **source** into another array of the same size as **source** or smaller.\n\n- **order**\n  : used to insert elements in the result in an order other\n    than the normal Fortran array element order, in which the first dimension\n    varies fastest.\n  : By definition of ranks the values have to be a permutation of the numbers\n    from 1 to n, where n is the rank of **shape**.\n  : the elements of **source** and pad are placed into the result in order;\n    changing the left-most rank most rapidly by default. To change the order by\n    which the elements are placed in the result use **order**.\n\n### **Result**\n\nThe result is an array of shape **shape** with the same type and type\nparameters as **source**. It is first filled with the values of elements\nof **source**, with the remainder filled with repeated copies of **pad**\nuntil all elements are filled. The new array may be smaller than\n**source**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_reshape\nimplicit none\n! notice the use of \"shape(box)\" on the RHS\ninteger :: box(3,4)=reshape([1,2,3,4,5,6,7,8,9,10,11,12],shape(box))\ninteger,allocatable :: v(:,:)\ninteger :: rc(2)\n   ! basics0\n    ! what is the current shape of the array?\n    call printi('shape of box is ',box)\n    ! change the shape\n    call printi('reshaped ',reshape(box,[2,6]))\n    call printi('reshaped ',reshape(box,[4,3]))\n\n   ! fill in row column order using order\n    v=reshape([1,2,3,4,10,20,30,40,100,200,300,400],[1,12])\n    call printi('here is some data to shape',v)\n    call printi('normally fills columns first ',reshape([v],[3,4]))\n    call printi('fill rows first', reshape([v],[3,4],order=[2,1]))\n\n    ! if we take the data and put in back in filling\n    ! rows first instead of columns, and flipping the\n    ! height and width of the box we not only fill in\n    ! a vector using row-column order we actually\n    ! transpose it.\n    rc(2:1:-1)=shape(box)\n    ! copy the data in changing column number fastest\n    v=reshape(box,rc,order=[2,1])\n    call printi('reshaped and reordered',v)\n    ! of course we could have just done a transpose\n    call printi('transposed',transpose(box))\n\n   ! making the result bigger than source using pad\n    v=reshape(box,rc*2,pad=[-1,-2,-3],order=[2,1])\n    call printi('bigger and padded and reordered',v)\ncontains\n\nsubroutine printi(title,arr)\nimplicit none\n\n!@(#) print small 2d integer arrays in row-column format\n\ncharacter(len=*),parameter :: all='(*(g0,1x))' ! a handy format\ncharacter(len=*),intent(in)  :: title\ninteger,intent(in)           :: arr(:,:)\ninteger                      :: i\ncharacter(len=:),allocatable :: biggest\n\n   print all\n   print all, trim(title),':(',shape(arr),')'  ! print title\n   biggest='           '  ! make buffer to write integer into\n   ! find how many characters to use for integers\n   write(biggest,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(arr))))))+2\n   ! use this format to write a row\n   biggest='(\" > [\",*(i'//trim(biggest)//':,\",\"))'\n   ! print one row of array at a time\n   do i=1,size(arr,dim=1)\n      write(*,fmt=biggest,advance='no')arr(i,:)\n      write(*,'(\" ]\")')\n   enddo\n\nend subroutine printi\n\nend program demo_reshape\n```\nResults:\n```text\n   shape of box is :( 3 4 )\n    > [   1,   4,   7,  10 ]\n    > [   2,   5,   8,  11 ]\n    > [   3,   6,   9,  12 ]\n\n   reshaped :( 2 6 )\n    > [   1,   3,   5,   7,   9,  11 ]\n    > [   2,   4,   6,   8,  10,  12 ]\n\n   reshaped :( 4 3 )\n    > [   1,   5,   9 ]\n    > [   2,   6,  10 ]\n    > [   3,   7,  11 ]\n    > [   4,   8,  12 ]\n\n   here is some data to shape :( 1 12 )\n    > [   1,   2,   3,   4,  10,  20,  30,  40, 100, 200, 300, 400 ]\n\n   normally fills columns first :( 3 4 )\n    > [    1,    4,   30,  200 ]\n    > [    2,   10,   40,  300 ]\n    > [    3,   20,  100,  400 ]\n\n   fill rows first :( 3 4 )\n    > [    1,    2,    3,    4 ]\n    > [   10,   20,   30,   40 ]\n    > [  100,  200,  300,  400 ]\n\n   reshaped and reordered :( 4 3 )\n    > [   1,   2,   3 ]\n    > [   4,   5,   6 ]\n    > [   7,   8,   9 ]\n    > [  10,  11,  12 ]\n\n   transposed :( 4 3 )\n    > [   1,   2,   3 ]\n    > [   4,   5,   6 ]\n    > [   7,   8,   9 ]\n    > [  10,  11,  12 ]\n\n   bigger and padded and reordered :( 8 6 )\n    > [   1,   2,   3,   4,   5,   6 ]\n    > [   7,   8,   9,  10,  11,  12 ]\n    > [  -1,  -2,  -3,  -1,  -2,  -3 ]\n    > [  -1,  -2,  -3,  -1,  -2,  -3 ]\n    > [  -1,  -2,  -3,  -1,  -2,  -3 ]\n    > [  -1,  -2,  -3,  -1,  -2,  -3 ]\n    > [  -1,  -2,  -3,  -1,  -2,  -3 ]\n    > [  -1,  -2,  -3,  -1,  -2,  -3 ]\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**shape**(3)](#shape),\n[**pack**(3)](#pack),\n[**transpose**(3)](#transpose)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n\n",
     "RRSPACING": "## rrspacing\n\n### **Name**\n\n**rrspacing** - \\[MODEL_COMPONENTS\\] Reciprocal of the relative spacing of a numeric type\n\n### **Synopsis**\n```fortran\n    result = rrspacing(x)\n```\n```fortran\n     elemental real(kind=KIND) function rrspacing(x)\n\n      real(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** is type _real_ an any kind\n - The return value is of the same type and kind as **x**.\n\n### **Description**\n\n**rrspacing** returns the reciprocal of the relative spacing of model\nnumbers near **x**.\n\n<!--\n 5 Result Value. The result has the value |Y* b-e|*bp = ABS (FRACTION (Y)) * RADIX (X) / EPSILON (X),\n    where b, e, and p are as defined in 16.4 for Y, the value nearest to X in the model for real values whose kind type\n    parameter is that of X; if there are two such values, the value of greater absolute value is taken. If X is an IEEE\n    infinity, the result is an IEEE NaN. If X is an IEEE NaN, the result is that NaN.\n 6 Example. RRSPACING (-3.0) has the value 0:75x224 for reals whose model is as in 16.4, NOTE 1.\n-->\n\n### **Options**\n\n- **x**\n  : Shall be of type _real_.\n\n### **Result**\n\n  The return value is of the same type and kind as **x**. The value returned\n  is equal to **abs(fraction(x)) \\* float(radix(x))\\*\\*digits(x)**.\n\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions_\n",
     "SAME_TYPE_AS": "## same_type_as\n\n### **Name**\n\n**same_type_as** - \\[STATE:INQUIRY\\] Query dynamic types for equality\n\n### **Synopsis**\n```fortran\n    result = same_type_as(a, b)\n```\n```fortran\n     logical same_type_as(a, b)\n\n      type(TYPE(kind=KIND)),intent(in) :: a\n      type(TYPE(kind=KIND)),intent(in) :: b\n```\n### **Characteristics**\n\n- **a** shall be an object of extensible declared type or unlimited\n  polymorphic. If it is a polymorphic pointer, it shall not have\n  an undefined association status.\n\n- **b** shall be an object of extensible declared type or unlimited\n  polymorphic. If it is a polymorphic pointer, it shall not have\n  an undefined association status.\n\n### **Description**\n\n**same_type_as** queries the dynamic types of objects for equality.\n\n### **Options**\n\n- **a**\n  : object to compare to **b** for equality of type\n\n- **b**\n  : object to be compared to for equality of type\n\n### **Result**\n\n  If the dynamic type of **a** or **b** is extensible, the result is true\n  if and only if the dynamic type of **a** is the same as the dynamic\n  type of **b**. If neither **a** nor **b** has extensible dynamic type,\n  the result is processor dependent.\n\n    NOTE1\n\n  The dynamic type of a disassociated pointer or unallocated allocatable\n  variable is its declared type. An unlimited polymorphic entity has no\n  declared type.\n\n    NOTE2\n\n  The test performed by SAME_TYPE_AS is not the same as the test performed\n  by the type guard TYPE IS. The test performed by SAME_TYPE_AS does\n  not consider kind type parameters.\n\nSample program:\n```fortran\n  ! program demo_same_type_as\n  module M_ether\n  implicit none\n  private\n\n  type   :: dot\n    real :: x=0\n    real :: y=0\n  end type dot\n\n  type, extends(dot) :: point\n    real :: z=0\n  end type point\n\n  type something_else\n  end type something_else\n\n  public :: dot\n  public :: point\n  public :: something_else\n\n  end module M_ether\n\n  program demo_same_type_as\n  use M_ether, only : dot, point, something_else\n  implicit none\n  type(dot) :: dad, mom\n  type(point) :: me\n  type(something_else) :: alien\n\n   write(*,*)same_type_as(me,dad),'I am descended from Dad, but equal?'\n   write(*,*)same_type_as(me,me) ,'I am what I am'\n   write(*,*)same_type_as(dad,mom) ,'what a pair!'\n\n   write(*,*)same_type_as(dad,me),'no paradox here'\n   write(*,*)same_type_as(dad,alien),'no relation'\n\n   call pointers()\n   contains\n   subroutine pointers()\n   ! Given the declarations and assignments\n   type t1\n      real c\n   end type\n   type, extends(t1) :: t2\n   end type\n   class(t1), pointer :: p, q, r\n      allocate (p, q)\n      allocate (t2 :: r)\n      ! the result of SAME_TYPE_AS (P, Q) will be true, and the result\n      ! of SAME_TYPE_AS (P, R) will be false.\n      write(*,*)'(P,Q)',same_type_as(p,q),\"mind your P's and Q's\"\n      write(*,*)'(P,R)',same_type_as(p,r)\n   end subroutine pointers\n\n  end program demo_same_type_as\n```\nResults:\n```text\n    F I am descended from Dad, but equal?\n    T I am what I am\n    T what a pair!\n    F no paradox here\n    F no relation\n    (P,Q) T mind your P's and Q's\n    (P,R) F\n```\n### **Standard**\n\nFortran 2003\n\n### **See Also**\n\n[**extends_type_of**(3)](#extends_type_of)\n\n _fortran-lang intrinsic descriptions_\n",
-    "SCALE": "## scale\n\n### **Name**\n\n**scale** - \\[MODEL_COMPONENTS\\] Scale a real value by a whole power of the radix\n\n### **Synopsis**\n```fortran\n    result = scale(x, i)\n```\n```fortran\n     elemental real(kind=KIND) function scale(x, i)\n\n      real(kind=KIND),intent(in)   :: x\n      integer(kind=**),intent(in)  :: i\n```\n### **Characteristics**\n\n   - **x** is type _real_ of any kind\n   - **i** is type an _integer_ of any kind\n   - the result is _real_ of the same kind as **x**\n\n### **Description**\n\n   **scale** returns x \\* **radix(x)\\*\\*i**.\n\n   It is almost certain the radix(base) of the platform is two, therefore\n   **scale** is generally the same as **x*2\\*\\*i**\n\n### **Options**\n\n- **x**\n  : the value to multiply by **radix(x)\\*\\*i**. Its type and kind is used\n  to determine the radix for values with its characteristics and determines\n  the characteristics of the result, so care must be taken the returned\n  value is within the range of the characteristics of **x**.\n\n- **i**\n  : The power to raise the radix of the machine to\n\n### **Result**\n\nThe return value is **x \\* radix(x)\\*\\*i**, assuming that value can be\nrepresented by a value of the type and kind of **x**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_scale\nimplicit none\nreal :: x \ncomplex :: c\ninteger :: i\n   x = 1.0\n   print *, (scale(x,i),i=1,5)\n   x = 3.0\n   print *, (scale(x,i),i=1,5)\n   print *, (scale(log(1.0),i),i=1,5)\n   ! on modern machines radix(x) is almost certainly 2\n   x = 178.1387e-4\n   i = 5\n   print *, x, i, scale(x, i), x*radix(x)**i\n   ! x*radix(x)**i is the same except roundoff errors are not restricted\n   i = 2\n   print *, x, i, scale(x, i), x*radix(x)**i\n   ! relatively easy to do complex values as well\n   c=(3.0,4.0)\n   print *, c, i, scale_complex(c, i)!, c*radix(c)**i\ncontains\n   function scale_complex(x, n)\n   ! example supporting complex value for default kinds\n      complex, intent(in) :: x\n      integer, intent(in) :: n\n      complex :: scale_complex\n      scale_complex = cmplx(scale(x%re, n), scale(x%im, n), kind=kind(x%im))\n   end function scale_complex\nend program demo_scale\n```\nResults:\n```text\n > 2.00000000 4.00000000  8.00000000     16.0000000 32.0000000    \n > 6.00000000 12.0000000 24.0000000      48.0000000 96.0000000    \n > 0.00000000 0.00000000  0.00000000     0.00000000 0.00000000    \n > 1.78138707E-02    5   0.570043862      0.570043862    \n > 1.78138707E-02    2   7.12554827E-02   7.12554827E-02\n > (3.00000000,4.00000000) 2 (12.0000000,16.0000000)\n\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
+    "SCALE": "## scale\n\n### **Name**\n\n**scale** - \\[MODEL_COMPONENTS\\] Scale a real value by a whole power of the radix\n\n### **Synopsis**\n```fortran\n    result = scale(x, i)\n```\n```fortran\n     elemental real(kind=KIND) function scale(x, i)\n\n      real(kind=KIND),intent(in)   :: x\n      integer(kind=**),intent(in)  :: i\n```\n### **Characteristics**\n\n   - **x** is type _real_ of any kind\n   - **i** is type an _integer_ of any kind\n   - the result is _real_ of the same kind as **x**\n\n### **Description**\n\n   **scale** returns x \\* **radix(x)\\*\\*i**.\n\n   It is almost certain the radix(base) of the platform is two, therefore\n   **scale** is generally the same as **x*2\\*\\*i**\n\n### **Options**\n\n- **x**\n  : the value to multiply by **radix(x)\\*\\*i**. Its type and kind is used\n  to determine the radix for values with its characteristics and determines\n  the characteristics of the result, so care must be taken the returned\n  value is within the range of the characteristics of **x**.\n\n- **i**\n  : The power to raise the radix of the machine to\n\n### **Result**\n\nThe return value is **x \\* radix(x)\\*\\*i**, assuming that value can be\nrepresented by a value of the type and kind of **x**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_scale\nimplicit none\nreal :: x\ncomplex :: c\ninteger :: i\n   x = 1.0\n   print *, (scale(x,i),i=1,5)\n   x = 3.0\n   print *, (scale(x,i),i=1,5)\n   print *, (scale(log(1.0),i),i=1,5)\n   ! on modern machines radix(x) is almost certainly 2\n   x = 178.1387e-4\n   i = 5\n   print *, x, i, scale(x, i), x*radix(x)**i\n   ! x*radix(x)**i is the same except roundoff errors are not restricted\n   i = 2\n   print *, x, i, scale(x, i), x*radix(x)**i\n   ! relatively easy to do complex values as well\n   c=(3.0,4.0)\n   print *, c, i, scale_complex(c, i)!, c*radix(c)**i\ncontains\nfunction scale_complex(x, n)\n! example supporting complex value for default kinds\ncomplex, intent(in) :: x\ninteger, intent(in) :: n\ncomplex :: scale_complex\n   scale_complex=cmplx(scale(x%re, n), scale(x%im, n), kind=kind(x%im))\nend function scale_complex\nend program demo_scale\n```\nResults:\n```text\n > 2.00000000 4.00000000  8.00000000     16.0000000 32.0000000\n > 6.00000000 12.0000000 24.0000000      48.0000000 96.0000000\n > 0.00000000 0.00000000  0.00000000     0.00000000 0.00000000\n > 1.78138707E-02    5   0.570043862      0.570043862\n > 1.78138707E-02    2   7.12554827E-02   7.12554827E-02\n > (3.00000000,4.00000000) 2 (12.0000000,16.0000000)\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**set_exponent**(3)](#set_exponent),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SCAN": "## scan\n\n### **Name**\n\n**scan** - \\[CHARACTER:SEARCH\\] Scan a string for the presence of a set of characters\n\n### **Synopsis**\n```fortran\n    result = scan( string, set, [,back] [,kind] )\n```\n```fortran\n     elemental integer(kind=KIND) function scan(string,set,back,kind)\n\n      character(len=*,kind=**),intent(in) :: string\n      character(len=*,kind=**),intent(in) :: set\n      logical,intent(in),optional :: back\n      integer,intent(in),optional :: kind\n```\n### **Characteristics**\n\n - **string** is a _character_ string of any kind\n - **set** must be a _character_ string with the same kind as **string**\n - **back** is a _logical_\n - **kind** is a scalar _integer_ constant expression\n - the result is an _integer_ with the kind specified by **kind**. If\n   **kind** is not present the result is a default _integer_.\n\n### **Description**\n\n  **scan** scans a **string** for any of the characters in a **set**\n  of characters.\n\n  If **back** is either absent or equals _.false._, this function\n  returns the position of the leftmost character of **STRING** that is\n  in **set**. If **back** equals _.true._, the rightmost position is\n  returned. If no character of **set** is found in **string**, the result\n  is zero.\n\n### **Options**\n\n- **string**\n  : the string to be scanned\n\n- **set**\n  : the set of characters which will be matched\n\n- **back**\n  : if _.true._ the position of the rightmost character matched is\n  returned, instead of the leftmost.\n\n- **kind**\n  : the kind of the returned value is the same as **kind** if\n  present. Otherwise a default _integer_ kind is returned.\n\n### **Result**\n\n  If **back** is absent or is present with the value false and if\n  **string** contains at least one character that is in **set**, the value\n  of the result is the position of the leftmost character of **string**\n  that is in **set**.\n\n  If **back** is present with the value true and if **string** contains at\n  least one character that is in **set**, the value of the result is the\n  position of the rightmost character of **string** that is in **set**.\n\n  The value of the result is zero if no character of STRING is in SET\n  or if the length of STRING or SET is zero.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_scan\nimplicit none\n   write(*,*) scan(\"fortran\", \"ao\")          ! 2, found 'o'\n   write(*,*) scan(\"fortran\", \"ao\", .true.)  ! 6, found 'a'\n   write(*,*) scan(\"fortran\", \"c++\")         ! 0, found none\nend program demo_scan\n```\nResults:\n```text\n >            2\n >            6\n >            0\n```\n### **Standard**\n\nFortran 95 , with KIND argument - Fortran 2003\n\n### **See Also**\n\nFunctions that perform operations on character strings, return lengths\nof arguments, and search for certain arguments:\n\n- **Elemental:**\n  [**adjustl**(3)](#adjustl), [**adjustr**(3)](#adjustr), [**index**(3)](#index),\n  [**verify**(3)](#verify)\n\n- **Nonelemental:**\n  [**len\\_trim**(3)](#len_trim),\n  [**len**(3)](#len),\n  [**repeat**(3)](#repeat), [**trim**(3)](#trim)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SELECTED_CHAR_KIND": "## selected_char_kind\n\n### **Name**\n\n**selected_char_kind** - \\[KIND\\] Select character kind such as \"Unicode\"\n\n### **Synopsis**\n```fortran\n    result = selected_char_kind(name)\n```\n```fortran\n     integer function selected_char_kind(name)\n\n      character(len=*),intent(in) :: name\n```\n### **Characteristics**\n\n - **name** is a default _character_ scalar\n - the result is a default _integer_ scalar\n\n### **Description**\n\n  **selected_char_kind** returns a kind parameter value for the\n  character set named **name**.\n\n  If a name is not supported, -1 is returned. Otherwise the result is a\n  value equal to that kind type parameter value.\n\n  The list of supported names is processor-dependent except for \"DEFAULT\".\n\n + If **name** has the value \"DEFAULT\", then the result has a value equal to\n   that of the kind type parameter of default character. This name is\n   always supported.\n\n + If **name** has the value \"ASCII\", then the result has a value equal\n   to that of the kind type parameter of ASCII character.\n\n + If **name** has the value \"ISO_10646\", then the result has a value equal\n   to that of the kind type parameter of the ISO 10646 character kind\n   (corresponding to UCS-4 as specified in ISO/IEC 10646).\n\n + If **name** is a processor-defined name of some other character kind\n   supported by the processor, then the result has a value equal to that\n   kind type parameter value.\n  Pre-defined names include \"ASCII\" and \"ISO_10646\".\n\n  The NAME is interpreted without respect to case or trailing blanks.\n\n### **Options**\n\n- **name**\n  : A name to query the processor-dependent kind value of, and/or to determine\n  if supported. **name**, interpreted without respect to case or\n  trailing blanks.\n\n  Currently, supported character sets include \"ASCII\" and \"DEFAULT\" and\n  \"ISO_10646\" (Universal Character Set, UCS-4) which is commonly known as\n  \"Unicode\". Supported names other than \"DEFAULT\" are processor dependent.\n\n### **Result**\n\n\n### **Examples**\n\nSample program:\n\n```fortran\nLinux\nprogram demo_selected_char_kind\nuse iso_fortran_env\nimplicit none\n\nintrinsic date_and_time,selected_char_kind\n\n! set some aliases for common character kinds\n! as the numbers can vary from platform to platform\n\ninteger, parameter :: default = selected_char_kind (\"default\")\ninteger, parameter :: ascii =   selected_char_kind (\"ascii\")\ninteger, parameter :: ucs4  =   selected_char_kind ('ISO_10646')\ninteger, parameter :: utf8  =   selected_char_kind ('utf-8')\n\n! assuming ASCII and UCS4 are supported (ie. not equal to -1)\n! define some string variables\ncharacter(len=26, kind=ascii ) :: alphabet\ncharacter(len=30, kind=ucs4  ) :: hello_world\ncharacter(len=30, kind=ucs4  ) :: string\n\n   write(*,*)'ASCII     ',&\n    & merge('Supported    ','Not Supported',ascii /= -1)\n   write(*,*)'ISO_10646 ',&\n    & merge('Supported    ','Not Supported',ucs4 /= -1)\n   write(*,*)'UTF-8     ',&\n    & merge('Supported    ','Not Supported',utf8 /= -1)\n\n   if(default.eq.ascii)then\n       write(*,*)'ASCII is the default on this processor'\n   endif\n\n  ! for constants the kind precedes the value, somewhat like a\n  ! BOZ constant\n   alphabet = ascii_\"abcdefghijklmnopqrstuvwxyz\"\n   write (*,*) alphabet\n\n   hello_world = ucs4_'Hello World and Ni Hao -- ' &\n                 // char (int (z'4F60'), ucs4)     &\n                 // char (int (z'597D'), ucs4)\n\n  ! an encoding option is required on OPEN for non-default I/O\n   if(ucs4 /= -1 )then\n      open (output_unit, encoding='UTF-8')\n      write (*,*) trim (hello_world)\n   else\n      write (*,*) 'cannot use utf-8'\n   endif\n\n   call create_date_string(string)\n   write (*,*) trim (string)\n\ncontains\n\n! The following produces a Japanese date stamp.\nsubroutine create_date_string(string)\nintrinsic date_and_time,selected_char_kind\ninteger,parameter :: ucs4 = selected_char_kind(\"ISO_10646\")\ncharacter(len=1,kind=ucs4),parameter :: &\n       nen =   char(int( z'5e74' ),ucs4), & ! year\n       gatsu = char(int( z'6708' ),ucs4), & ! month\n       nichi = char(int( z'65e5' ),ucs4)    ! day\ncharacter(len= *, kind= ucs4) string\ninteger values(8)\n   call date_and_time(values=values)\n   write(string,101) values(1),nen,values(2),gatsu,values(3),nichi\n 101 format(*(i0,a))\nend subroutine create_date_string\n\nend program demo_selected_char_kind\n```\nResults:\n\nThe results are very processor-dependent\n```text\n >  ASCII     Supported\n >  ISO_10646 Supported\n >  UTF-8     Not Supported\n >  ASCII is the default on this processor\n >  abcdefghijklmnopqrstuvwxyz\n >  Hello World and Ni Hao -- \u4f60\u597d\n >  2022\u5e7410\u670815\u65e5\n```\n### **Standard**\n\nFortran 2003\n\n### **See also**\n\n[**selected_int_kind**(3)](#selected_int_kind),\n[**selected_real_kind**(3)](#selected_real_kind)\n\n[**achar**(3)](#achar),\n[**char**(3)](#char),\n[**ichar**(3)](#ichar),\n[**iachar**(3)](#iachar)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SELECTED_INT_KIND": "## selected_int_kind\n\n### **Name**\n\n**selected_int_kind** - \\[KIND\\] Choose integer kind\n\n### **Synopsis**\n```fortran\n    result = selected_int_kind(r)\n```\n```fortran\n    integer function selected_int_kind(r)\n\n     integer(kind=KIND),intent(in) :: r\n```\n### **Characteristics**\n\n - **r** is an _integer_ scalar.\n - the result is an default integer scalar.\n\n### **Description**\n\n  **selected_int_kind** return the kind value of the smallest\n  integer type that can represent all values ranging from **-10\\*\\*r**\n  (exclusive) to **10\\*\\*r** (exclusive). If there is no integer kind\n  that accommodates this range, selected_int_kind returns **-1**.\n\n### **Options**\n\n- **r**\n  : The value specifies the required range of powers of ten that need\n    supported by the kind type being returned.\n\n### **Result**\n\n  The result has a value equal to the value of the kind type parameter\n  of an integer type that represents all values in the requested range.\n\n  if no such kind type parameter is available on the processor, the\n  result is -1.\n\n  If more than one kind type parameter meets the criterion, the value\n  returned is the one with the smallest decimal exponent range, unless\n  there are several such values, in which case the smallest of these\n  kind values is returned.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_selected_int_kind\nimplicit none\ninteger,parameter :: k5 = selected_int_kind(5)\ninteger,parameter :: k15 = selected_int_kind(15)\ninteger(kind=k5) :: i5\ninteger(kind=k15) :: i15\n\n    print *, huge(i5), huge(i15)\n\n    ! the following inequalities are always true\n    print *, huge(i5) >= 10_k5**5-1\n    print *, huge(i15) >= 10_k15**15-1\nend program demo_selected_int_kind\n```\nResults:\n```text\n  >   2147483647  9223372036854775807\n  >  T\n  >  T\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**aint**(3)](#aint),\n[**anint**(3)](#anint),\n[**int**(3)](#int),\n[**nint**(3)](#nint),\n[**ceiling**(3)](#ceiling),\n[**floor**(3)](#floor)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SELECTED_REAL_KIND": "## selected_real_kind\n\n### **Name**\n\n**selected_real_kind** - \\[KIND\\] Choose real kind\n\n### **Synopsis**\n```fortran\n    result = selected_real_kind([p] [,r] [,radix] )\n```\n```fortran\n    integer function selected_int_kind(r)\n\n     real(kind=KIND),intent(in),optional :: p\n     real(kind=KIND),intent(in),optional :: r\n     real(kind=KIND),intent(in),optional :: radix\n```\n### **Characteristics**\n\n - **p** is an _integer_ scalar\n - **r** is an _integer_ scalar\n - **radix** is an _integer_ scalar\n - the result is an default _integer_ scalar\n\n### **Description**\n\n   **selected_real_kind** return the kind value of a _real_ data type with\n   decimal precision of at least **p** digits, exponent range of at least\n   **r**, and with a radix of **radix**. That is, if such a kind exists\n\n    + it has the decimal precision as returned by **precision**(3) of at\n      least **p** digits.\n    + a decimal exponent range, as returned by the function **range**(3)\n      of at least **r**\n    + a radix, as returned by the function **radix**(3) , of **radix**,\n\n   If the requested kind does not exist, -1 is returned.\n\n   At least one argument shall be present.\n\n### **Options**\n\n- **p**\n  : the requested precision\n\n- **r**\n  : the requested range\n\n- **radix**\n  : the desired radix\n\n  Before **Fortran 2008**, at least one of the arguments **r** or **p** shall\n  be present; since **Fortran 2008**, they are assumed to be zero if\n  absent.\n\n### **Result**\n\n  selected_real_kind returns the value of the kind type parameter of\n  a real data type with decimal precision of at least **p** digits,\n  a decimal exponent range of at least R, and with the requested\n  **radix**.\n\n  If **p** or **r** is absent, the result value is the same as if it\n  were present with the value zero.\n\n\n  If the **radix** parameter is absent, there is no requirement on\n  the radix of the selected kind and real kinds with any radix can be\n  returned.\n\n  If more than one real data type meet the criteria, the kind\n  of the data type with the smallest decimal precision is returned. If\n  no real data type matches the criteria, the result is\n\n  - **-1**\n  : if the processor does not support a real data type with a\n    precision greater than or equal to **p**, but the **r** and **radix**\n    requirements can be fulfilled\n\n  - **-2**\n  : if the processor does not support a real type with an\n    exponent range greater than or equal to **r**, but **p** and **radix** are\n    fulfillable\n\n  - **-3**\n  : if **radix** but not **p** and **r** requirements are fulfillable\n\n  - **-4**\n  : if **radix** and either **p** or **r** requirements are fulfillable\n\n  - **-5**\n  : if there is no real type with the given **radix**\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_selected_real_kind\nimplicit none\ninteger,parameter :: p6 = selected_real_kind(6)\ninteger,parameter :: p10r100 = selected_real_kind(10,100)\ninteger,parameter :: r400 = selected_real_kind(r=400)\nreal(kind=p6) :: x\nreal(kind=p10r100) :: y\nreal(kind=r400) :: z\n\n   print *, precision(x), range(x)\n   print *, precision(y), range(y)\n   print *, precision(z), range(z)\nend program demo_selected_real_kind\n```\nResults:\n```text\n  >            6          37\n  >           15         307\n  >           18        4931\n```\n### **Standard**\n\nFortran 95 ; with RADIX - Fortran 2008\n\n### **See Also**\n\n[**precision**(3)](#precision),\n[**range**(3)](#range),\n[**radix**(3)](#radix)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SET_EXPONENT": "## set_exponent\n\n### **Name**\n\n**set_exponent** - \\[MODEL_COMPONENTS\\] real value with specified exponent\n\n### **Synopsis**\n```fortran\n    result = set_exponent(x, i)\n```\n```fortran\n     elemental real(kind=KIND) function set_exponent(x,i)\n\n      real(kind=KIND),intent(in) :: x\n      integer(kind=**),intent(in) :: i\n```\n### **Characteristics**\n\n - **x** is type _real_\n - **i** is type _integer_\n - a kind designated as ** may be any supported kind for the type\n\n - The return value is of the same type and kind as **x**.\n\n### **Description**\n\n  **set_exponent** returns the real number whose fractional part is\n  that of **x** and whose exponent part is **i**.\n\n### **Options**\n\n- **x**\n  : Shall be of type _real_.\n\n- **i**\n  : Shall be of type _integer_.\n\n### **Result**\n\n  The return value is of the same type and kind as **x**. The real number\n  whose fractional part is that of **x** and whose exponent part\n  if **i** is returned; it is **fraction(x) \\* radix(x)\\*\\*i**.\n\n  If **x** has the value zero, the result has the same value as **x**.\n\n  If **x** is an IEEE infinity, the result is an IEEE NaN.\n\n  If **x** is an IEEE NaN, the result is the same NaN.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_setexp\nimplicit none\nreal :: x = 178.1387e-4\ninteger :: i = 17\n   print *, set_exponent(x, i), fraction(x) * radix(x)**i\nend program demo_setexp\n```\nResults:\n```text\n      74716.7891       74716.7891\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**spacing**(3)](#spacing),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions_\n",
     "SHAPE": "## shape\n\n### **Name**\n\n**shape** - \\[ARRAY:INQUIRY\\] Determine the shape of an array or scalar\n\n### **Synopsis**\n```fortran\n  result = shape( source [,kind] )\n```\n```fortran\n   integer(kind=KIND) function shape( source, KIND )\n\n    type(TYPE(kind=**)),intent(in)       :: source(..)\n    integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n  - a kind designated as ** may be any supported kind for the type\n\n  - **source** is an array or scalar of any type. If **source** is a pointer\n    it must be associated and allocatable arrays must be allocated. It shall\n    not be an assumed-size array.\n\n  - **KIND** is a constant _integer_ initialization expression.\n\n  - the result is an _integer_ array of rank one with size equal to the\n    rank of **source** of the kind specified by **KIND** if **KIND**\n    is present, otherwise it has the default integer kind.\n\n### **Description**\n\n  **shape** queries the shape of an array.\n\n### **Options**\n\n- **source**\n  : an array or scalar of any type. If **source** is a pointer it\n  must be associated and allocatable arrays must be allocated.\n\n- **kind**\n  : indicates the kind parameter of the result.\n\n### **Result**\n\n  An _integer_ array of rank one with as many elements as **source**\n  has dimensions.\n\n  The elements of the resulting array correspond to the extent of\n  **source** along the respective dimensions.\n\n  If **source** is a scalar, the result is an empty array (a rank-one\n  array of size zero).\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_shape\nimplicit none\ncharacter(len=*),parameter :: all='(*(g0,1x))'\ninteger, dimension(-1:1, -1:2) :: a\n   print all, 'shape of array=',shape(a)\n   print all, 'shape of constant=',shape(42)\n   print all, 'size of shape of constant=',size(shape(42))\n   print all, 'ubound of array=',ubound(a)\n   print all, 'lbound of array=',lbound(a)\nend program demo_shape\n```\nResults:\n```text\n   shape of array= 3 4\n   shape of constant=\n   size of shape of constant= 0\n   ubound of array= 1 2\n   lbound of array= -1 -1\n```\n### **Standard**\n\nFortran 95 ; with KIND argument Fortran 2003\n\n### **See Also**\n\n#### Array inquiry:\n\n- [**size**(3)](#size) -  Determine the size of an array\n- [**rank**(3)](#rank) -  Rank of a data object\n- [**ubound**(3)](#ubound) -  Upper dimension bounds of an array\n- [**lbound**(3)](#lbound) -  Lower dimension bounds of an array\n\n#### State Inquiry:\n\n- [**allocated**(3)](#allocated) -  Status of an allocatable entity\n- [**is_contiguous**(3)](#is_contiguous) -  Test if object is contiguous\n\n#### Kind Inquiry:\n\n- [**kind**(3)](#kind) - Kind of an entity\n\n#### Bit Inquiry:\n\n- [**storage_size**(3)](#storage_size) - Storage size in bits\n- [**bit_size**(3)](#bit_size) -  Bit size inquiry function\n- [**btest**(3)](#btest) - Tests a bit of an _integer_ value.\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SHIFTA": "## shifta\n\n### **Name**\n\n**shifta** - \\[BIT:SHIFT\\] Right shift with fill\n\n### **Synopsis**\n```fortran\n    result = shifta(i, shift )\n```\n```fortran\n     elemental integer(kind=KIND) function shifta(i, shift)\n\n      integer(kind=KIND),intent(in) :: i\n      integer(kind=**),intent(in) :: shift\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **i** is an _integer_ of any kind\n - **shift** is an _integer_ of any kind\n - the result will automatically be of the same type, kind and rank as **i**.\n\n### **Description**\n\n  **shifta** returns a value corresponding to **i** with all of the\n  bits shifted right by **shift** places and the vacated bits on the\n  left filled with the value of the original left-most bit.\n\n### **Options**\n\n- **i**\n  : The initial value to shift and fill\n\n- **shift**\n  : how many bits to shift right.\n    It shall be nonnegative and less than or equal to **bit_size(i)**.\n    or the value is undefined. If **shift** is zero the result is **i**.\n\n### **Result**\n\n  The result has the value obtained by shifting the bits of **i** to\n  the right **shift**  bits and replicating the leftmost bit of **i**\n  in the left **shift** bits (Note the leftmost bit in \"two's complement\"\n  representation is the sign bit).\n\n  Bits shifted out from the right end are lost.\n\n  If **shift** is zero the result is **i**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_shifta\nuse,intrinsic :: iso_fortran_env, only : int8, int16, int32, int64\nimplicit none\ninteger(kind=int32) :: ival\ninteger             :: shift\ninteger(kind=int32) :: oval\ninteger(kind=int32),allocatable :: ivals(:)\ninteger             :: i\ninteger(kind=int8)  :: arr(2,2)=reshape([2,4,8,16],[2,2])\n\n  ! basic usage\n  write(*,*)shifta(100,3)\n\n  ! loop through some interesting values\n   shift=5\n\n   ivals=[ -1, -0, +0, +1, &\n   & int(b\"01010101010101010101010101010101\"), &\n   & int(b\"10101010101010101010101010101010\"), &\n   & int(b\"00000000000000000000000000011111\") ]\n\n   ! does your platform distinguish between +0 and -0?\n   ! note the original leftmost bit is used to fill in the vacated bits\n\n   write(*,'(/,\"SHIFT =  \",i0)') shift\n   do i=1,size(ivals)\n      ival=ivals(i)\n      write(*,'(  \"I =      \",b32.32,\" == \",i0)') ival,ival\n      oval=shifta(ival,shift)\n      write(*,'(  \"RESULT = \",b32.32,\" == \",i0)') oval,oval\n   enddo\n   ! elemental\n   write(*,*)\"characteristics of the result are the same as input\"\n   write(*,'(*(g0,1x))') &\n     & \"kind=\",kind(shifta(arr,3)), \"shape=\",shape(shifta(arr,3)), &\n     & \"size=\",size(shifta(arr,3)) !, \"rank=\",rank(shifta(arr,3))\n\nend program demo_shifta\n```\nResults:\n\n```text\n >           12\n >\n > SHIFT =  5\n > I =      11111111111111111111111111111111 == -1\n > RESULT = 11111111111111111111111111111111 == -1\n > I =      00000000000000000000000000000000 == 0\n > RESULT = 00000000000000000000000000000000 == 0\n > I =      00000000000000000000000000000000 == 0\n > RESULT = 00000000000000000000000000000000 == 0\n > I =      00000000000000000000000000000001 == 1\n > RESULT = 00000000000000000000000000000000 == 0\n > I =      01010101010101010101010101010101 == 1431655765\n > RESULT = 00000010101010101010101010101010 == 44739242\n > I =      10101010101010101010101010101010 == -1431655766\n > RESULT = 11111101010101010101010101010101 == -44739243\n > I =      00000000000000000000000000011111 == 31\n > RESULT = 00000000000000000000000000000000 == 0\n >  characteristics of the result are the same as input\n > kind= 1 shape= 2 2 size= 4\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**shiftl**(3)](#shiftl),\n[**shiftr**(3)](#shiftr),\n[**ishft**(3)](#ishft),\n[**ishftc**(3)](#ishftc)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SHIFTL": "## shiftl\n\n### **Name**\n\n**shiftl** - \\[BIT:SHIFT\\] Shift bits left\n\n### **Synopsis**\n```fortran\n    result = shiftl( i, shift )\n```\n```fortran\n     elemental integer(kind=KIND) function shiftl(i, shift)\n\n      integer(kind=KIND),intent(in) :: i\n      integer(kind=**),intent(in) :: shift\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **i** is an _integer_ of any kind\n - **shift** is an _integer_ of any kind\n - the result will automatically be of the same type, kind and rank as **i**.\n\n### **Description**\n\n  **shiftl** returns a value corresponding to **i** with all of the\n  bits shifted left by **shift** places.\n\n  Bits shifted out from the left end are lost, and bits shifted in from\n  the right end are set to **0**.\n\n  If the absolute value of **shift** is greater than **bit_size(i)**,\n  the value is undefined.\n\n  For example, for a 16-bit integer left-shifted five ...\n```text\n    >  |a|b|c|d|e|f|g|h|i|j|k|l|m|n|o|p| <- original 16-bit example\n    >  |f|g|h|i|j|k|l|m|n|o|p|           <- left-shifted five\n    >  |f|g|h|i|j|k|l|m|n|o|p|0|0|0|0|0| <- right-padded with zeros\n```\nNote the value of the result is the same as **ishft (i, shift)**.\n\n### **Options**\n\n- **i**\n  : The initial value to shift and fill in with zeros\n\n- **shift**\n  : how many bits to shift left.\n    It shall be nonnegative and less than or equal to **bit_size(i)**.\n\n### **Result**\n\nThe return value is of type _integer_ and of the same kind as **i**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_shiftl\nuse,intrinsic :: iso_fortran_env, only : int8, int16, int32, int64\nimplicit none\ninteger             :: shift\ninteger(kind=int32) :: oval\ninteger(kind=int32) :: ival\ninteger(kind=int32),allocatable :: ivals(:)\ninteger             :: i\n\n  print *, ' basic usage'\n  ival=100\n  write(*,*)ival, shiftl(ival,3)\n\n ! elemental (input values may be conformant arrays)\n  print *, ' elemental'\n\n ! loop through some ivalues\n   shift=9\n   ivals=[ &\n   & int(b\"01010101010101010101010101010101\"), &\n   & int(b\"10101010101010101010101010101010\"), &\n   & int(b\"11111111111111111111111111111111\") ]\n\n   write(*,'(/,\"SHIFT =  \",i0)') shift\n   do i=1,size(ivals)\n      ! print initial value as binary and decimal\n      write(*,'(  \"I =      \",b32.32,\" == \",i0)') ivals(i),ivals(i)\n      ! print shifted value as binary and decimal\n      oval=shiftl(ivals(i),shift)\n      write(*,'(  \"RESULT = \",b32.32,\" == \",i0)') oval,oval\n   enddo\n\n  ! more about elemental\n   ELEM : block\n   integer(kind=int8)  :: arr(2,2)=reshape([2,4,8,16],[2,2])\n   write(*,*)\"characteristics of the result are the same as input\"\n   write(*,'(*(g0,1x))') &\n     & \"kind=\",kind(shiftl(arr,3)), \"shape=\",shape(shiftl(arr,3)), &\n     & \"size=\",size(shiftl(arr,3)) !, \"rank=\",rank(shiftl(arr,3))\n   endblock ELEM\n\nend program demo_shiftl\n```\nResults:\n```text\n >    basic usage\n >           100         800\n >    elemental\n >\n >  SHIFT =  9\n >  I =      01010101010101010101010101010101 == 1431655765\n >  RESULT = 10101010101010101010101000000000 == -1431655936\n >  I =      10101010101010101010101010101010 == -1431655766\n >  RESULT = 01010101010101010101010000000000 == 1431655424\n >  I =      11111111111111111111111111111111 == -1\n >  RESULT = 11111111111111111111111000000000 == -512\n >   characteristics of the result are the same as input\n >  kind= 1 shape= 2 2 size= 4\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**shifta**(3)](#shifta),\n[**shiftr**(3)](#shiftr),\n[**ishft**(3)](#ishft),\n[**ishftc**(3)](#ishftc)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SHIFTR": "## shiftr\n\n### **Name**\n\n**shiftr** - \\[BIT:SHIFT\\] Shift bits right\n\n### **Synopsis**\n```fortran\n    result = shiftr( i, shift )\n```\n```fortran\n     elemental integer(kind=KIND) function shiftr(i, shift)\n\n      integer(kind=KIND),intent(in) :: i\n      integer(kind=**),intent(in) :: shift\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **i** is an _integer_ of any kind\n - **shift** is an _integer_ of any kind\n - the result will automatically be of the same type, kind and rank as **i**.\n\n### **Description**\n\n  **shiftr** returns a value corresponding to **i** with all of the\n  bits shifted right by **shift** places.\n\n  If the absolute value of **shift** is greater than **bit_size(i)**,\n  the value is undefined.\n\n  Bits shifted out from the right end are lost, and bits shifted in from\n  the left end are set to 0.\n\n  For example, for a 16-bit integer right-shifted five ...\n```text\n    >  |a|b|c|d|e|f|g|h|i|j|k|l|m|n|o|p| <- original 16-bit example\n    >            |a|b|c|d|e|f|g|h|i|j|k| <- right-shifted five\n    >  |0|0|0|0|0|f|g|h|i|j|k|l|m|n|o|p| <- left-padded with zeros\n```\n  Note the value of the result is the same as **ishft (i, -shift)**.\n\n### **Options**\n\n- **i**\n  : The value to shift\n\n- **shift**\n  : How many bits to shift right.\n    It shall be nonnegative and less than or equal to **bit_size(i)**.\n\n### **Result**\n\n  The remaining bits shifted right **shift** positions.\n  Vacated positions on the left are filled with zeros.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_shiftr\nuse,intrinsic :: iso_fortran_env, only : int8, int16, int32, int64\nimplicit none\ninteger             :: shift\ninteger(kind=int32) :: oval\ninteger(kind=int32) :: ival\ninteger(kind=int32),allocatable :: ivals(:)\ninteger             :: i\n\n  print *,' basic usage'\n  ival=100\n  write(*,*)ival, shiftr(100,3)\n\n  ! elemental (input values may be conformant arrays)\n  print *,' elemental'\n   shift=9\n   ivals=[ &\n   & int(b\"01010101010101010101010101010101\"), &\n   & int(b\"10101010101010101010101010101010\"), &\n   & int(b\"11111111111111111111111111111111\") ]\n\n   write(*,'(/,\"SHIFT =  \",i0)') shift\n   do i=1,size(ivals)\n      ! print initial value as binary and decimal\n      write(*,'(  \"I =      \",b32.32,\" == \",i0)') ivals(i),ivals(i)\n      ! print shifted value as binary and decimal\n      oval=shiftr(ivals(i),shift)\n      write(*,'(  \"RESULT = \",b32.32,\" == \",i0,/)') oval,oval\n   enddo\n\n   ! more on elemental\n   ELEM : block\n   integer(kind=int8)  :: arr(2,2)=reshape([2,4,8,16],[2,2])\n   write(*,*)\"characteristics of the result are the same as input\"\n   write(*,'(*(g0,1x))') &\n     & \"kind=\",kind(shiftr(arr,3)), \"shape=\",shape(shiftr(arr,3)), &\n     & \"size=\",size(shiftr(arr,3)) !, \"rank=\",rank(shiftr(arr,3))\n   endblock ELEM\n\nend program demo_shiftr\n```\nResults:\n```text\n  >    basic usage\n  >           100          12\n  >    elemental\n  >\n  >  SHIFT =  9\n  >  I =      01010101010101010101010101010101 == 1431655765\n  >  RESULT = 00000000001010101010101010101010 == 2796202\n  >\n  >  I =      10101010101010101010101010101010 == -1431655766\n  >  RESULT = 00000000010101010101010101010101 == 5592405\n  >\n  >  I =      11111111111111111111111111111111 == -1\n  >  RESULT = 00000000011111111111111111111111 == 8388607\n  >\n  >   characteristics of the result are the same as input\n  >  kind= 1 shape= 2 2 size= 4\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**shifta**(3)](#shifta),\n[**shiftl**(3)](#shiftl),\n[**ishft**(3)](#ishft),\n[**ishftc**(3)](#ishftc)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SIGN": "## sign\n\n### **Name**\n\n**sign** - \\[NUMERIC\\] Sign copying function\n\n### **Synopsis**\n```fortran\n    result = sign(a, b)\n```\n```fortran\n     elemental type(TYPE(kind=KIND))function sign(a, b)\n\n      type(TYPE(kind=KIND)),intent(in) :: a, b\n```\n### **Characteristics**\n\n - **a** shall be of type integer or real.\n - **b** shall be of the same type as **a**.\n - the characteristics of the result are the same as **a**.\n\n### **Description**\n\n  **sign** returns a value with the magnitude of _a_ but with the\n  sign of _b_.\n\n  For processors that distinguish between positive and negative zeros\n  _sign()_ may be used to distinguish between _real_ values 0.0 and\n  -0.0. SIGN (1.0, -0.0) will return  -1.0 when a negative zero is\n  distinguishable.\n\n### **Options**\n\n  - **a**\n    : The value whose magnitude will be returned.\n\n  - **b**\n    : The value whose sign will be returned.\n\n### **Result**\n\n  a value with the magnitude of **a** with the sign of **b**. That is,\n\n  - If _b \\>= 0_ then the result is _abs(a)_\n  - else if _b < 0_ it is -_abs(a)_.\n  - if _b_ is _real_ and the processor distinguishes between _-0.0_\n    and _0.0_ then the\n    result is _-abs(a)_\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_sign\nimplicit none\n  ! basics\n   print *,  sign( -12,  1 )\n   print *,  sign( -12,  0 )\n   print *,  sign( -12, -1 )\n   print *,  sign(  12,  1 )\n   print *,  sign(  12,  0 )\n   print *,  sign(  12, -1 )\n\n   if(sign(1.0,-0.0)== -1.0)then\n      print *, 'this processor distinguishes +0 from -0'\n   else\n      print *, 'this processor does not distinguish +0 from -0'\n   endif\n\n   print *,  'elemental', sign( -12.0, [1.0, 0.0, -1.0] )\n\nend program demo_sign\n```\nResults:\n```text\n             12\n             12\n            -12\n             12\n             12\n            -12\n    this processor does not distinguish +0 from -0\n    elemental   12.00000       12.00000      -12.00000\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See also**\n\n[**abs**(3)](#abs)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SIN": "## sin\n\n### **Name**\n\n**sin** - \\[MATHEMATICS:TRIGONOMETRIC\\] Sine function\n\n### **Synopsis**\n```fortran\n    result = sin(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function sin(x)\n\n      TYPE(kind=KIND) :: x\n```\n### **Characteristics**\n\n  - **x** may be any _real_ or _complex_ type\n  - **KIND** may be any kind supported by the associated type of **x**.\n  - The returned value will be of the same type and kind as the argument\n    **x**.\n\n### **Description**\n\n  **sin** computes the sine of an angle given the size of the angle\n  in radians.\n\n  The sine of an angle in a right-angled triangle is the ratio of the\n  length of the side opposite the given angle divided by the length of\n  the hypotenuse.\n\n### **Options**\n\n- **x**\n  : The angle in radians to compute the sine of.\n\n### **Result**\n\n- **result**\n  The return value contains the processor-dependent approximation of\n  the sine of **x**\n\n  If X is of type _real_, it is regarded as a value in radians.\n\n  If X is of type _complex_, its real part is regarded as a value\n  in radians.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram sample_sin\nimplicit none\nreal :: x = 0.0\n   x = sin(x)\n   write(*,*)'X=',x\nend program sample_sin\n```\nResults:\n```text\n >  X=  0.0000000E+00\n```\n### Extended Example\n\n#### Haversine Formula\n\n  From the article on \"Haversine formula\" in Wikipedia:\n```text\n    The haversine formula is an equation important in navigation,\n    giving great-circle distances between two points on a sphere from\n    their longitudes and latitudes.\n```\n  So to show the great-circle distance between the Nashville International\n  Airport (BNA) in TN, USA, and the Los Angeles International Airport\n  (LAX) in CA, USA you would start with their latitude and longitude,\n  commonly given as\n```text\n  BNA: N 36 degrees 7.2',   W 86 degrees 40.2'\n  LAX: N 33 degrees 56.4',  W 118 degrees 24.0'\n```\n  which converted to floating-point values in degrees is:\n```text\n       Latitude Longitude\n\n     - BNA\n       36.12, -86.67\n\n     - LAX\n       33.94, -118.40\n```\n  And then use the haversine formula to roughly calculate the distance\n  along the surface of the Earth between the locations:\n\nSample program:\n```fortran\nprogram demo_sin\nimplicit none\nreal :: d\n    d = haversine(36.12,-86.67, 33.94,-118.40) ! BNA to LAX\n    print '(A,F9.4,A)', 'distance: ',d,' km'\ncontains\nfunction haversine(latA,lonA,latB,lonB) result (dist)\n!\n! calculate great circle distance in kilometers\n! given latitude and longitude in degrees\n!\nreal,intent(in) :: latA,lonA,latB,lonB\nreal :: a,c,dist,delta_lat,delta_lon,lat1,lat2\nreal,parameter :: radius = 6371 ! mean earth radius in kilometers,\n! recommended by the International Union of Geodesy and Geophysics\n\n! generate constant pi/180\nreal, parameter :: deg_to_rad = atan(1.0)/45.0\n   delta_lat = deg_to_rad*(latB-latA)\n   delta_lon = deg_to_rad*(lonB-lonA)\n   lat1 = deg_to_rad*(latA)\n   lat2 = deg_to_rad*(latB)\n   a = (sin(delta_lat/2))**2 + &\n          & cos(lat1)*cos(lat2)*(sin(delta_lon/2))**2\n   c = 2*asin(sqrt(a))\n   dist = radius*c\nend function haversine\nend program demo_sin\n```\nResults:\n```text\n > distance: 2886.4446 km\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See Also**\n\n[**asin**(3)](#asin),\n[**cos**(3)](#cos),\n[**tan**(3)](#tan),\n[**acosh**(3)](#acosh),\n[**acos**(3)](#acos),\n[**asinh**(3)](#asinh),\n[**atan2**(3)](#atan2),\n[**atanh**(3)](#atanh),\n[**acosh**(3)](#acosh),\n[**asinh**(3)](#asinh),\n[**atanh**(3)](#atanh)\n\n### **Resources**\n\n- [Wikipedia:sine and cosine](https://en.wikipedia.org/wiki/Sine_and_cosine)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SINH": "## sinh\n\n### **Name**\n\n**sinh** - \\[MATHEMATICS:TRIGONOMETRIC\\] Hyperbolic sine function\n\n### **Synopsis**\n```fortran\n    result = sinh(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function sinh(x)\n\n      TYPE(kind=KIND) :: x\n```\n### **Characteristics**\n\n - **TYPE** may be _real_ or _complex_\n - **KIND** may be any kind supported by the associated type.\n - The returned value will be of the same type and kind as the argument.\n\n### **Description**\n\n  **sinh** computes the hyperbolic sine of **x**.\n\n  The hyperbolic sine of x is defined mathematically as:\n```fortran\n     sinh(x) = (exp(x) - exp(-x)) / 2.0\n```\n\n### **Options**\n\n- **x**\n  : The value to calculate the hyperbolic sine of\n\n### **Result**\n\n  The result has a value equal to a processor-dependent approximation\n  to sinh(X). If X is of type complex its imaginary part is regarded\n  as a value in radians.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_sinh\nuse, intrinsic :: iso_fortran_env, only : &\n& real_kinds, real32, real64, real128\nimplicit none\nreal(kind=real64) :: x = - 1.0_real64\nreal(kind=real64) :: nan, inf\ncharacter(len=20) :: line\n\n  ! basics\n   print *, sinh(x)\n   print *, (exp(x)-exp(-x))/2.0\n\n  ! sinh(3) is elemental and can handle an array\n   print *, sinh([x,2.0*x,x/3.0])\n\n   ! a NaN input returns NaN\n   line='NAN'\n   read(line,*) nan\n   print *, sinh(nan)\n\n   ! a Inf input returns Inf\n   line='Infinity'\n   read(line,*) inf\n   print *, sinh(inf)\n\n   ! an overflow returns Inf\n   x=huge(0.0d0)\n   print *, sinh(x)\n\nend program demo_sinh\n```\nResults:\n```text\n  -1.1752011936438014\n  -1.1752011936438014\n  -1.1752011936438014       -3.6268604078470190      -0.33954055725615012\n                       NaN\n                  Infinity\n                  Infinity\n```\n### **Standard**\n\nFortran 95 , for a complex argument Fortran 2008\n\n### **See Also**\n\n[**asinh**(3)](#asinh)\n\n### **Resources**\n\n- [Wikipedia:hyperbolic functions](https://en.wikipedia.org/wiki/Hyperbolic_functions)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SIZE": "## size\n\n### **Name**\n\n**size** - \\[ARRAY:INQUIRY\\] Determine the size of an array or extent of one dimension\n\n### **Synopsis**\n```fortran\n    result = size(array [,dim] [,kind])\n```\n```fortran\n     integer(kind=KIND) function size(array,dim,kind)\n\n      type(TYPE(kind=KIND)),intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      integer(kind=**),intent(in),optional :: KIND\n```\n### **Characteristics**\n\n- **array** is an assumed-rank array or array of any type and associated\n  kind.\n\n  If **array** is a pointer it must be associated and allocatable arrays\n  must be allocated.\n- **dim** is an integer scalar\n- **kind** is a scalar integer constant expression.\n- the result is an integer scalar of kind **KIND**. If **KIND** is absent\n  a _integer_ of default kind is returned.\n- a kind designated as ** may be any supported kind for the type\n\n\n### **Description**\n\n  **size(3)** returns the total number of elements in an array, or\n  if **dim** is specified returns the number of elements along that\n  dimension.\n\n  **size** determines the extent of **array** along a specified\n  dimension **dim**, or the total number of elements in **array** if\n  **dim** is absent.\n\n### **Options**\n\n- **array**\n  : the array to measure the number of elements of.\n  If **array* is an assumed-size array, **dim** shall be present with a value less\n  than the rank of **array**.\n\n- **dim**\n  : a value shall be\n  in the range from 1 to n, where n equals the rank of **array**.\n\n  If not present the total number of elements of the entire array\n  are returned.\n\n- **kind**\n  : An _integer_ initialization expression indicating the kind\n  parameter of the result.\n\n  If absent the kind type parameter of the returned value is that of\n  default integer type.\n\n  The **kind** must allow for the magnitude returned by **size** or\n  results are undefined.\n\n  If **kind** is absent, the return value is of default _integer_ kind.\n\n### **Result**\n\n  If **dim** is not present **array** is assumed-rank, the result has a\n  value equal to **PRODUCT(SHAPE(ARRAY,KIND))**. Otherwise, the result\n  has a value equal to the total number of elements of **array**.\n\n  If **dim** is present the number of elements along that dimension\n  are returned, except that if ARRAY is assumed-rank and associated\n  with an assumed-size array and DIM is present with a value equal to\n  the rank of **array**, the value is -1.\n\n  NOTE1\n\n  If **array** is assumed-rank and has rank zero, **dim** cannot be\n  present since it cannot satisfy the requirement\n\n   1 <= DIM <= 0.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_size\nimplicit none\ninteger :: arr(0:2,-5:5)\n   write(*,*)'SIZE of simple two-dimensional array'\n   write(*,*)'SIZE(arr)       :total count of elements:',size(arr)\n   write(*,*)'SIZE(arr,DIM=1) :number of rows         :',size(arr,dim=1)\n   write(*,*)'SIZE(arr,DIM=2) :number of columns      :',size(arr,dim=2)\n\n   ! pass the same array to a procedure that passes the value two\n   ! different ways\n   call interfaced(arr,arr)\ncontains\n\nsubroutine interfaced(arr1,arr2)\n! notice the difference in the array specification\n! for arr1 and arr2.\ninteger,intent(in) :: arr1(:,:)\ninteger,intent(in) :: arr2(2,*)\n   !\n   write(*,*)'interfaced assumed-shape array'\n   write(*,*)'SIZE(arr1)        :',size(arr1)\n   write(*,*)'SIZE(arr1,DIM=1)  :',size(arr1,dim=1)\n   write(*,*)'SIZE(arr1,DIM=2)  :',size(arr1,dim=2)\n\n!  write(*,*)'SIZE(arr2)        :',size(arr2)\n   write(*,*)'SIZE(arr2,DIM=1)  :',size(arr2,dim=1)\n!\n! CANNOT DETERMINE SIZE OF ASSUMED SIZE ARRAY LAST DIMENSION\n!  write(*,*)'SIZE(arr2,DIM=2)  :',size(arr2,dim=2)\n\nend subroutine interfaced\n\nend program demo_size\n```\nResults:\n```text\n    SIZE of simple two-dimensional array\n    SIZE(arr)       :total count of elements:          33\n    SIZE(arr,DIM=1) :number of rows         :           3\n    SIZE(arr,DIM=2) :number of columns      :          11\n    interfaced assumed-shape array\n    SIZE(arr1)        :          33\n    SIZE(arr1,DIM=1)  :           3\n    SIZE(arr1,DIM=2)  :          11\n    SIZE(arr2,DIM=1)  :           2\n```\n### **Standard**\n\nFortran 95 , with **kind** argument - Fortran 2003\n\n### **See Also**\n\n#### Array inquiry:\n\n- [**size**](#size) -  Determine the size of an array\n- [**rank**(3)](#rank) -  Rank of a data object\n- [**shape**(3)](#shape) -  Determine the shape of an array\n- [**ubound**(3)](#ubound) -  Upper dimension bounds of an array\n- [**lbound**(3)](#lbound) -  Lower dimension bounds of an array\n\n#### State Inquiry:\n\n- [**allocated**(3)](#allocated) -  Status of an allocatable entity\n- [**is_contiguous**(3)](#is_contiguous) -  Test if object is contiguous\n\n#### Kind Inquiry:\n\n- [**kind**(3)](#kind) - Kind of an entity\n\n#### Bit Inquiry:\n\n- [**storage_size**(3)](#storage_size) - Storage size in bits\n- [**bit_size**(3)](#bit_size) -  Bit size inquiry function\n- [**btest**(3)](#btest) - Tests a bit of an _integer_ value.\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SPACING": "## spacing\n\n### **Name**\n\n**spacing** - \\[MODEL_COMPONENTS\\] Smallest distance between two numbers of a given type\n\n### **Synopsis**\n```fortran\n    result = spacing(x)\n```\n```fortran\n     elemental real(kind=KIND) function spacing(x)\n\n      real(kind=KIND), intent(in) :: x\n```\n### **Characteristics**\n\n  - **x** is type real of any valid kind\n  - The result is of the same type as the input argument **x**.\n\n### **Description**\n\n  **spacing** determines the distance between the argument **x**\n  and the nearest adjacent number of the same type.\n\n### **Options**\n\n- **x**\n  : Shall be of type _real_.\n\n### **Result**\n\n   If **x** does not have the value zero and is not an IEEE infinity or NaN, the result has the value\n   nearest to **x** for values of the same type and kind assuming the value is representable.\n\n   Otherwise, the value is the same as **tiny(x)**.\n     + zero produces **tiny(x)**\n     + IEEE Infinity produces an IEEE Nan\n     + if an IEEE NaN, that NaN is returned\n\n   If there are two extended model values equally near to **x**, the\n   value of greater absolute value is taken.\n<!--\n       b**(e-p), where b, e, and p are as defined in 16.4\n-->\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_spacing\nimplicit none\ninteger, parameter :: sgl = selected_real_kind(p=6, r=37)\ninteger, parameter :: dbl = selected_real_kind(p=13, r=200)\n\n   write(*,*) spacing(1.0_sgl)\n   write(*,*) nearest(1.0_sgl,+1.0),nearest(1.0_sgl,+1.0)-1.0\n\n   write(*,*) spacing(1.0_dbl)\nend program demo_spacing\n```\nResults:\n\nTypical values ...\n\n```text\n     1.1920929E-07\n      1.000000      1.1920929E-07\n     0.9999999     -5.9604645E-08\n     2.220446049250313E-016\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**digits**(3)](#digits),\n[**epsilon**(3)](#epsilon),\n[**exponent**(3)](#exponent),\n[**fraction**(3)](#fraction),\n[**huge**(3)](#huge),\n[**maxexponent**(3)](#maxexponent),\n[**minexponent**(3)](#minexponent),\n[**nearest**(3)](#nearest),\n[**precision**(3)](#precision),\n[**radix**(3)](#radix),\n[**range**(3)](#range),\n[**rrspacing**(3)](#rrspacing),\n[**scale**(3)](#scale),\n[**set_exponent**(3)](#set_exponent),\n[**tiny**(3)](#tiny)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
-    "SPREAD": "## spread\n\n### **Name**\n\n**spread** - \\[ARRAY:CONSTRUCTION\\] Add a dimension and replicate data\n\n### **Synopsis**\n```fortran\n    result = spread(source, dim, ncopies)\n```\n```fortran\n     TYPE(kind=KIND) function spread(source, dim, ncopies)\n\n      TYPE(kind=KIND)             :: source(..)\n      integer(kind=**),intent(in) :: dim\n      integer(kind=**),intent(in) :: ncopies\n```\n### **Characteristics**\n\n- **source** is a scalar or array of any type and a rank less than fifteen.\n- **dim** is an _integer_ scalar\n- **ncopies** is an integer scalar\n\n### **Description**\n\n**spread** replicates a **source** array along a specified dimension\n**dim**. The copy is repeated **ncopies** times.\n\nSo to add additional rows to a matrix **dim=1** would be used, but to\nadd additional rows **dim=2** would be used, for example.\n\nIf **source** is scalar, the size of the resulting vector is **ncopies**\nand each element of the result has a value equal to **source**.\n\n### **Options**\n\n- **source**\n  : the input data to duplicate\n\n- **dim**\n  : The additional dimension value in the range from\n  **1** to **n+1**, where **n** equals the rank of **source**.\n\n- **ncopies**\n  : the number of copies of the original data to generate\n\n### **Result**\n\nThe result is an array of the same type as **source** and has rank **n+1**\nwhere **n** equals the rank of **source**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_spread\nimplicit none\n\ninteger a1(4,3), a2(3,4), v(4), s\n\n   write(*,'(a)' ) &\n   'TEST SPREAD(3)                                      ', &\n   '  SPREAD(3) is a FORTRAN90 function which replicates', &\n   '  an array by adding a dimension.                   ', &\n   ' '\n\n   s = 99\n   call printi('suppose we have a scalar S',s)\n\n   write(*,*) 'to add a new dimension (1) of extent 4 call'\n   call printi('spread( s, dim=1, ncopies=4 )',spread ( s, 1, 4 ))\n\n   v = [ 1, 2, 3, 4 ]\n   call printi(' first we will set V to',v)\n\n   write(*,'(a)')' and then do \"spread ( v, dim=2, ncopies=3 )\"'\n   a1 = spread ( v, dim=2, ncopies=3 )\n   call printi('uses v as a column and makes 3 columns',a1)\n\n   a2 = spread ( v, 1, 3 )\n   call printi(' spread(v,1,3) uses v as a row and makes 3 rows',a2)\n\ncontains\n! CONVENIENCE ROUTINE; NOT DIRECTLY CONNECTED TO SPREAD(3)\nsubroutine printi(title,a)\nuse, intrinsic :: iso_fortran_env, only : stderr=>ERROR_UNIT,&\n & stdin=>INPUT_UNIT, stdout=>OUTPUT_UNIT\nimplicit none\n\n!@(#) print small 2d integer scalar, vector, matrix in row-column format\n\ncharacter(len=*),parameter   :: all='(\" \",*(g0,1x))'\ncharacter(len=*),intent(in)  :: title\ncharacter(len=20)            :: row\ninteger,intent(in)           :: a(..)\ninteger                      :: i\n\n   write(*,all,advance='no')trim(title)\n   ! select rank of input\n   select rank(a)\n   rank (0); write(*,'(a)')' (a scalar)'\n      write(*,'(\" > [ \",i0,\" ]\")')a\n   rank (1); write(*,'(a)')' (a vector)'\n      ! find how many characters to use for integers\n      write(row,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(a))))))+2\n      ! use this format to write a row\n      row='(\" > [\",*(i'//trim(row)//':,\",\"))'\n      do i=1,size(a)\n         write(*,fmt=row,advance='no')a(i)\n         write(*,'(\" ]\")')\n      enddo\n   rank (2); write(*,'(a)')' (a matrix) '\n      ! find how many characters to use for integers\n      write(row,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(a))))))+2\n      ! use this format to write a row\n      row='(\" > [\",*(i'//trim(row)//':,\",\"))'\n      do i=1,size(a,dim=1)\n         write(*,fmt=row,advance='no')a(i,:)\n         write(*,'(\" ]\")')\n      enddo\n   rank default\n      write(stderr,*)'*printi* did not expect rank=', rank(a), &\n       & 'shape=', shape(a),'size=',size(a)\n      stop '*printi* unexpected rank'\n   end select\n   write(*,all) '>shape=',shape(a),',rank=',rank(a),',size=',size(a)\n   write(*,*)\n\nend subroutine printi\n\nend program demo_spread\n```\nResults:\n```text\n > TEST SPREAD(3)                                      \n >   SPREAD(3) is a FORTRAN90 function which replicates\n >   an array by adding a dimension.                   \n >  \n >  suppose we have a scalar S  (a scalar)\n >  > [ 99 ]\n >  >shape= ,rank= 0 ,size= 1\n > \n >  to add a new dimension (1) of extent 4 call\n >  spread( s, dim=1, ncopies=4 )  (a vector)\n >  > [  99 ]\n >  > [  99 ]\n >  > [  99 ]\n >  > [   0 ]\n >  >shape= 4 ,rank= 1 ,size= 4\n > \n >   first we will set V to  (a vector)\n >  > [  1 ]\n >  > [  2 ]\n >  > [  3 ]\n >  > [  4 ]\n >  >shape= 4 ,rank= 1 ,size= 4\n > \n >  and then do \"spread ( v, dim=2, ncopies=3 )\"\n >  uses v as a column and makes 3 columns  (a matrix) \n >  > [  1,  1,  1 ]\n >  > [  2,  2,  2 ]\n >  > [  3,  3,  3 ]\n >  > [  4,  4,  4 ]\n >  >shape= 4 3 ,rank= 2 ,size= 12\n > \n >   spread(v,1,3) uses v as a row and makes 3 rows  (a matrix) \n >  > [  1,  2,  3,  4 ]\n >  > [  1,  2,  3,  4 ]\n >  > [  1,  2,  3,  4 ]\n >  >shape= 3 4 ,rank= 2 ,size= 12\n > \n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**merge**(3)](#merge),\n[**pack**(3)](#pack),\n[**unpack**(3)](#unpack)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n<!--\nwhen adding dimension 3,4,5, ... why is 15 not allowed if 16 is allowed?\n\nneed an illustration of what happens with higher dimension array\n-->\n",
+    "SPREAD": "## spread\n\n### **Name**\n\n**spread** - \\[ARRAY:CONSTRUCTION\\] Add a dimension and replicate data\n\n### **Synopsis**\n```fortran\n    result = spread(source, dim, ncopies)\n```\n```fortran\n     TYPE(kind=KIND) function spread(source, dim, ncopies)\n\n      TYPE(kind=KIND)             :: source(..)\n      integer(kind=**),intent(in) :: dim\n      integer(kind=**),intent(in) :: ncopies\n```\n### **Characteristics**\n\n- **source** is a scalar or array of any type and a rank less than fifteen.\n- **dim** is an _integer_ scalar\n- **ncopies** is an integer scalar\n\n### **Description**\n\n**spread** replicates a **source** array along a specified dimension\n**dim**. The copy is repeated **ncopies** times.\n\nSo to add additional rows to a matrix **dim=1** would be used, but to\nadd additional rows **dim=2** would be used, for example.\n\nIf **source** is scalar, the size of the resulting vector is **ncopies**\nand each element of the result has a value equal to **source**.\n\n### **Options**\n\n- **source**\n  : the input data to duplicate\n\n- **dim**\n  : The additional dimension value in the range from\n  **1** to **n+1**, where **n** equals the rank of **source**.\n\n- **ncopies**\n  : the number of copies of the original data to generate\n\n### **Result**\n\nThe result is an array of the same type as **source** and has rank **n+1**\nwhere **n** equals the rank of **source**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_spread\nimplicit none\n\ninteger a1(4,3), a2(3,4), v(4), s\n\n   write(*,'(a)' ) &\n   'TEST SPREAD(3)                                      ', &\n   '  SPREAD(3) is a FORTRAN90 function which replicates', &\n   '  an array by adding a dimension.                   ', &\n   ' '\n\n   s = 99\n   call printi('suppose we have a scalar S',s)\n\n   write(*,*) 'to add a new dimension (1) of extent 4 call'\n   call printi('spread( s, dim=1, ncopies=4 )',spread ( s, 1, 4 ))\n\n   v = [ 1, 2, 3, 4 ]\n   call printi(' first we will set V to',v)\n\n   write(*,'(a)')' and then do \"spread ( v, dim=2, ncopies=3 )\"'\n   a1 = spread ( v, dim=2, ncopies=3 )\n   call printi('uses v as a column and makes 3 columns',a1)\n\n   a2 = spread ( v, 1, 3 )\n   call printi(' spread(v,1,3) uses v as a row and makes 3 rows',a2)\n\ncontains\n! CONVENIENCE ROUTINE; NOT DIRECTLY CONNECTED TO SPREAD(3)\nsubroutine printi(title,a)\nuse, intrinsic :: iso_fortran_env, only : stderr=>ERROR_UNIT,&\n & stdin=>INPUT_UNIT, stdout=>OUTPUT_UNIT\nimplicit none\n\n!@(#) print small 2d integer scalar, vector, matrix in row-column format\n\ncharacter(len=*),parameter   :: all='(\" \",*(g0,1x))'\ncharacter(len=*),intent(in)  :: title\ncharacter(len=20)            :: row\ninteger,intent(in)           :: a(..)\ninteger                      :: i\n\n   write(*,all,advance='no')trim(title)\n   ! select rank of input\n   select rank(a)\n   rank (0); write(*,'(a)')' (a scalar)'\n      write(*,'(\" > [ \",i0,\" ]\")')a\n   rank (1); write(*,'(a)')' (a vector)'\n      ! find how many characters to use for integers\n      write(row,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(a))))))+2\n      ! use this format to write a row\n      row='(\" > [\",*(i'//trim(row)//':,\",\"))'\n      do i=1,size(a)\n         write(*,fmt=row,advance='no')a(i)\n         write(*,'(\" ]\")')\n      enddo\n   rank (2); write(*,'(a)')' (a matrix) '\n      ! find how many characters to use for integers\n      write(row,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(a))))))+2\n      ! use this format to write a row\n      row='(\" > [\",*(i'//trim(row)//':,\",\"))'\n      do i=1,size(a,dim=1)\n         write(*,fmt=row,advance='no')a(i,:)\n         write(*,'(\" ]\")')\n      enddo\n   rank default\n      write(stderr,*)'*printi* did not expect rank=', rank(a), &\n       & 'shape=', shape(a),'size=',size(a)\n      stop '*printi* unexpected rank'\n   end select\n   write(*,all) '>shape=',shape(a),',rank=',rank(a),',size=',size(a)\n   write(*,*)\n\nend subroutine printi\n\nend program demo_spread\n```\nResults:\n```text\n > TEST SPREAD(3)\n >   SPREAD(3) is a FORTRAN90 function which replicates\n >   an array by adding a dimension.\n >\n >  suppose we have a scalar S  (a scalar)\n >  > [ 99 ]\n >  >shape= ,rank= 0 ,size= 1\n >\n >  to add a new dimension (1) of extent 4 call\n >  spread( s, dim=1, ncopies=4 )  (a vector)\n >  > [  99 ]\n >  > [  99 ]\n >  > [  99 ]\n >  > [   0 ]\n >  >shape= 4 ,rank= 1 ,size= 4\n >\n >   first we will set V to  (a vector)\n >  > [  1 ]\n >  > [  2 ]\n >  > [  3 ]\n >  > [  4 ]\n >  >shape= 4 ,rank= 1 ,size= 4\n >\n >  and then do \"spread ( v, dim=2, ncopies=3 )\"\n >  uses v as a column and makes 3 columns  (a matrix)\n >  > [  1,  1,  1 ]\n >  > [  2,  2,  2 ]\n >  > [  3,  3,  3 ]\n >  > [  4,  4,  4 ]\n >  >shape= 4 3 ,rank= 2 ,size= 12\n >\n >   spread(v,1,3) uses v as a row and makes 3 rows  (a matrix)\n >  > [  1,  2,  3,  4 ]\n >  > [  1,  2,  3,  4 ]\n >  > [  1,  2,  3,  4 ]\n >  >shape= 3 4 ,rank= 2 ,size= 12\n >\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**merge**(3)](#merge),\n[**pack**(3)](#pack),\n[**unpack**(3)](#unpack)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n<!--\nwhen adding dimension 3,4,5, ... why is 15 not allowed if 16 is allowed?\n\nneed an illustration of what happens with higher dimension array\n-->\n",
     "SQRT": "## sqrt\n\n### **Name**\n\n**sqrt** - \\[MATHEMATICS\\] Square-root function\n\n### **Synopsis**\n```fortran\n    result = sqrt(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function sqrt(x)\n\n      TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **TYPE** may be _real_ or _complex_.\n - **KIND** may be any kind valid for the declared type.\n - the result has the same characteristics as **x**.\n\n### **Description**\n\n  **sqrt** computes the principal square root of **x**.\n\n  The number whose square root is being considered is known as the\n  _radicand_.\n\n  In mathematics, a square root of a radicand **x** is a number **y**\n  such that **y\\*y = x**.\n\n  Every nonnegative radicand  **x** has two square roots of the same unique\n  magnitude, one positive and one negative. The nonnegative square root\n  is called the principal square root.\n\n  The principal square root of 9 is 3, for example, even though (-3)\\*(-3)\n  is also 9.\n\n  Square roots of negative numbers are a special case of complex numbers,\n  where with **complex** input the components of the _radicand_ need\n  not be positive in order to have a valid square root.\n\n### **Options**\n\n- **x**\n  : The radicand to find the principal square root of.\n  If **x** is _real_ its value must be greater than or equal to zero.\n\n### **Result**\n\n  The principal square root of **x** is returned.\n\n  For a _complex_ result the real part is greater than or equal to zero.\n\n  When the real part of the result is zero, the imaginary part has the\n  same sign as the imaginary part of **x**.\n\n### **Examples**\n\nSample program:\n\n```fortran\nprogram demo_sqrt\nuse, intrinsic :: iso_fortran_env, only : real_kinds, &\n & real32, real64, real128\nimplicit none\nreal(kind=real64) :: x, x2\ncomplex :: z, z2\n\n  ! basics\n   x = 2.0_real64\n   ! complex\n   z = (1.0, 2.0)\n   write(*,*)'input values ',x,z\n\n   x2 = sqrt(x)\n   z2 = sqrt(z)\n   write(*,*)'output values ',x2,z2\n\n  ! elemental\n  write(*,*)'elemental',sqrt([64.0,121.0,30.0])\n\n  ! alternatives\n   x2 = x**0.5\n   z2 = z**0.5\n   write(*,*)'alternatively',x2,z2\n\nend program demo_sqrt\n```\nResults:\n```text\n    input values    2.00000000000000      (1.000000,2.000000)\n    output values    1.41421356237310      (1.272020,0.7861513)\n    elemental   8.000000       11.00000       5.477226\n    alternatively   1.41421356237310      (1.272020,0.7861513)\n```\n### **Standard**\n\nFORTRAN 77\n\n### **See also**\n\n[**exp**(3)](#exp),\n[**log**(3)](#log),\n[**log10**(3)](#log10)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "STORAGE_SIZE": "\n## storage_size\n\n### **Name**\n\n**storage_size** - \\[BIT:INQUIRY\\] Storage size in bits\n\n### **Synopsis**\n```fortran\n    result = storage_size(a [,KIND] )\n```\n```fortran\n     integer(kind=KIND) storage_size(a,KIND)\n\n      type(TYPE(kind=**)) :: a\n      integer,intent(in),optional :: KIND\n```\n### **Characteristics**\n  - a kind designated as ** may be any supported kind for the type\n\n  - **a** may be of any type and kind. If it is polymorphic it shall not\n    be an undefined pointer. If it is unlimited polymorphic or has any\n    deferred type parameters, it shall not be an unallocated allocatable\n    variable or a disassociated or undefined pointer.\n\n  - The kind type parameter of the returned value is that specified by\n    the value of **kind**; otherwise, the kind type parameter is that of\n    default integer type.\n\n  - The result is an _integer_ scalar of default kind unless **kind** is\n    specified, in which case it has the kind specified by **kind**.\n\n### **Description**\n\n**storage_size** returns the storage size of argument **a** in bits.\n\n### **Options**\n\n- **a**\n  : The entity to determine the storage size of\n\n- **kind**\n  : a scalar integer constant expression that defines the kind of the\n  output value.\n\n### **Result**\n\n  The result value is the size expressed in bits for an element of an\n  array that has the dynamic type and type parameters of **a**.\n\n  If the type and type parameters are such that storage association\n  applies, the result is consistent with the named constants\n  defined in the intrinsic module ISO_FORTRAN_ENV.\n\n  NOTE1\n\n   An array element might take \"type\" more bits to store than an isolated\n   scalar, since any hardware-imposed alignment requirements for array\n   elements might not apply to a simple scalar variable.\n\n  NOTE2\n\n   This is intended to be the size in memory that an object takes when it\n   is stored; this might differ from the size it takes during expression\n   handling (which might be the native register size) or when stored in a\n   file. If an object is never stored in memory but only in a register,\n   this function nonetheless returns the size it would take if it were\n   stored in memory.\n\n### **Examples**\n\nSample program\n```fortran\nprogram demo_storage_size\nimplicit none\n\n   ! a default real, integer, and logical are the same storage size\n   write(*,*)'size of integer       ',storage_size(0)\n   write(*,*)'size of real          ',storage_size(0.0)\n   write(*,*)'size of logical       ',storage_size(.true.)\n   write(*,*)'size of complex       ',storage_size((0.0,0.0))\n\n   ! note the size of an element of the array, not the storage size of\n   ! the entire array is returned for array arguments\n   write(*,*)'size of integer array ',storage_size([0,1,2,3,4,5,6,7,8,9])\n\nend program demo_storage_size\n```\nResults:\n```text\n    size of integer                 32\n    size of real                    32\n    size of logical                 32\n    size of complex                 64\n    size of integer array           32\n```\n### **Standard**\n\nFortran 2008\n\n### **See Also**\n\n[**c_sizeof**(3)](#c_sizeof)\n\n _fortran-lang intrinsic descriptions_\n",
     "SUM": "## sum\n\n### **Name**\n\n**sum** - \\[ARRAY:REDUCTION\\] Sum the elements of an array\n\n### **Synopsis**\n```fortran\n   result = sum(array [,dim[,mask]] | [mask] )\n```\n```fortran\n     TYPE(kind=KIND) function sum(array, dim, mask)\n\n      TYPE(kind=KIND),intent(in) :: array(..)\n      integer(kind=**),intent(in),optional :: dim\n      logical(kind=**),intent(in),optional :: mask(..)\n```\n### **Characteristics**\n\n  - a kind designated as ** may be any supported kind for the type\n  - **array** may be of any numeric type - _integer_, _real_ or _complex_.\n  - **dim** is an _integer_\n  - **mask** is _logical_ and conformable with **array**.\n  - The result is of the same type and kind as **array**. It is scalar\n    if **dim** is not present or **array** is a vector, else it is an array.\n\n### **Description**\n\n  **sum** adds the elements of **array**.\n\n  When only **array** is specified all elements are summed, but groups\n  of sums may be returned along the dimension specified by **dim**\n  and/or elements to add may be selected by a logical mask.\n\n  No method is designated for how the sum is conducted, so whether or not\n  accumulated error is compensated for is processor-dependent.\n\n### **Options**\n\n- **array**\n  : an array containing the elements to add\n\n- **dim**\n  : a value in the range from 1 to n, where n equals the rank (the number\n  of dimensions) of **array**. **dim** designates the dimension\n  along which to create sums. When absent a scalar sum of the elements\n  optionally selected by **mask** is returned.\n\n- **mask**\n  : an array of the same shape as **array** that designates\n  which elements to add. If absent all elements are used in the sum(s).\n\n### **Result**\n\n  If **dim** is absent, a scalar with the sum of all selected elements\n  in **array** is returned. Otherwise, an array of rank n-1, where n\n  equals the rank of **array**, and a shape similar to that of **array**\n  with dimension **dim** dropped is returned. Since a vector has a rank\n  of one, the result is a scalar (if n==1, n-1 is zero; and a rank of\n  zero means a scalar).\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_sum\nimplicit none\ninteger :: vector(5) , matrix(3,4), box(5,6,7)\n\n   vector = [ 1, 2, -3, 4, 5 ]\n\n   matrix(1,:)=[  -1,   2,    -3,   4    ]\n   matrix(2,:)=[  10,   -20,  30,   -40  ]\n   matrix(3,:)=[  100,  200, -300,  400  ]\n\n   box=11\n\n  ! basics\n   print *, 'sum all elements:',sum(vector)\n   print *, 'real :',sum([11.0,-5.0,20.0])\n   print *, 'complex :',sum([(1.1,-3.3),(4.0,5.0),(8.0,-6.0)])\n  ! with MASK option\n   print *, 'sum odd elements:',sum(vector, mask=mod(vector, 2)==1)\n   print *, 'sum positive values:', sum(vector, mask=vector>0)\n\n   call printi('the input array', matrix )\n   call printi('sum of all elements in matrix', sum(matrix) )\n   call printi('sum of positive elements', sum(matrix,matrix>=0) )\n  ! along dimensions\n   call printi('sum along rows', sum(matrix,dim=1) )\n   call printi('sum along columns', sum(matrix,dim=2) )\n   call printi('sum of a vector is always a scalar', sum(vector,dim=1) )\n   call printi('sum of a volume by row', sum(box,dim=1) )\n   call printi('sum of a volume by column', sum(box,dim=2) )\n   call printi('sum of a volume by depth', sum(box,dim=3) )\n\ncontains\n! CONVENIENCE ROUTINE; NOT DIRECTLY CONNECTED TO SPREAD(3)\nsubroutine printi(title,a)\nuse, intrinsic :: iso_fortran_env, only : stderr=>ERROR_UNIT,&\n & stdin=>INPUT_UNIT, stdout=>OUTPUT_UNIT\nimplicit none\n\n!@(#) print small 2d integer scalar, vector, matrix in row-column format\n\ncharacter(len=*),intent(in)  :: title\ninteger,intent(in)           :: a(..)\n\ncharacter(len=*),parameter   :: all='(\" \",*(g0,1x))'\ncharacter(len=20)            :: row\ninteger,allocatable          :: b(:,:)\ninteger                      :: i\n   write(*,all,advance='no')trim(title)\n   ! copy everything to a matrix to keep code simple\n   select rank(a)\n   rank (0); write(*,'(a)')' (a scalar)'; b=reshape([a],[1,1])\n   rank (1); write(*,'(a)')' (a vector)'; b=reshape(a,[size(a),1])\n   rank (2); write(*,'(a)')' (a matrix)'; b=a\n   rank default; stop '*printi* unexpected rank'\n   end select\n   ! find how many characters to use for integers\n   write(row,'(i0)')ceiling(log10(max(1.0,real(maxval(abs(b))))))+2\n   ! use this format to write a row\n   row='(\" > [\",*(i'//trim(row)//':,\",\"))'\n   do i=1,size(b,dim=1)\n      write(*,fmt=row,advance='no')b(i,:)\n      write(*,'(\" ]\")')\n   enddo\n   write(*,all) '>shape=',shape(a),',rank=',rank(a),',size=',size(a)\n   write(*,*)\nend subroutine printi\nend program demo_sum\n```\nResults:\n```text\n    sum all elements:           9\n    real :   26.00000\n    complex : (13.10000,-4.300000)\n    sum odd elements:           6\n    sum positive values:          12\n    the input array  (a matrix)\n    > [   -1,    2,   -3,    4 ]\n    > [   10,  -20,   30,  -40 ]\n    > [  100,  200, -300,  400 ]\n    >shape= 3 4 ,rank= 2 ,size= 12\n\n    sum of all elements in matrix  (a scalar)\n    > [  382 ]\n    >shape= ,rank= 0 ,size= 1\n\n    sum of positive elements  (a scalar)\n    > [  746 ]\n    >shape= ,rank= 0 ,size= 1\n\n    sum along rows  (a vector)\n    > [  109 ]\n    > [  182 ]\n    > [ -273 ]\n    > [  364 ]\n    >shape= 4 ,rank= 1 ,size= 4\n\n    sum along columns  (a vector)\n    > [    2 ]\n    > [  -20 ]\n    > [  400 ]\n    >shape= 3 ,rank= 1 ,size= 3\n\n    sum of a vector is always a scalar  (a scalar)\n    > [  9 ]\n    >shape= ,rank= 0 ,size= 1\n\n    sum of a volume by row  (a matrix)\n    > [  55,  55,  55,  55,  55,  55,  55 ]\n    > [  55,  55,  55,  55,  55,  55,  55 ]\n    > [  55,  55,  55,  55,  55,  55,  55 ]\n    > [  55,  55,  55,  55,  55,  55,  55 ]\n    > [  55,  55,  55,  55,  55,  55,  55 ]\n    > [  55,  55,  55,  55,  55,  55,  55 ]\n    >shape= 6 7 ,rank= 2 ,size= 42\n\n    sum of a volume by column  (a matrix)\n    > [  66,  66,  66,  66,  66,  66,  66 ]\n    > [  66,  66,  66,  66,  66,  66,  66 ]\n    > [  66,  66,  66,  66,  66,  66,  66 ]\n    > [  66,  66,  66,  66,  66,  66,  66 ]\n    > [  66,  66,  66,  66,  66,  66,  66 ]\n    >shape= 5 7 ,rank= 2 ,size= 35\n\n    sum of a volume by depth  (a matrix)\n    > [  77,  77,  77,  77,  77,  77 ]\n    > [  77,  77,  77,  77,  77,  77 ]\n    > [  77,  77,  77,  77,  77,  77 ]\n    > [  77,  77,  77,  77,  77,  77 ]\n    > [  77,  77,  77,  77,  77,  77 ]\n    >shape= 5 6 ,rank= 2 ,size= 30\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n - [**all**(3)](#all) - Determines if all the values are true\n - [**any**(3)](#any) - Determines if any of the values in the logical array are true.\n - [**count**(3)](#count) - Count true values in an array\n - [**maxval**(3)](#maxval) - Determines the maximum value in an array\n - [**minval**(3)](#minval) - Minimum value of an array\n - [**product**(3)](#product) - Product of array elements\n - [**merge**(3)](#merge) - Merge variables\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "SYSTEM_CLOCK": "## system_clock\n\n### **Name**\n\n**system_clock** - \\[SYSTEM:TIME\\] Query system clock\n\n### **Synopsis**\n```fortran\n    call system_clock([count] [,count_rate] [,count_max] )\n```\n```fortran\n     subroutine system_clock(count, count_rate, count_max)\n\n      integer(kind=**),intent(out),optional    :: count\n      type(TYPE(kind=**)),intent(out),optional :: count_rate\n      integer(kind=**),intent(out),optional    :: count_max\n```\n### **Characteristics**\n\n - **count** is an _integer_ scalar\n - **count_rate** is an _integer_ or _real_ scalar\n - **count_max** is an _integer_ scalar\n\n### **Description**\n\n  **system_clock** lets you measure durations of time with the\n  precision of the smallest time increment generally available on a\n  system by returning processor-dependent values based on the current\n  value of the processor clock.\n\n  **system_clock** is typically used to measure short time intervals\n  (system clocks may be 24-hour clocks or measure processor clock ticks\n  since boot, for example). It is most often used for measuring or\n  tracking the time spent in code blocks in lieu of using profiling tools.\n\n  **count_rate** and **count_max** are assumed constant (even though\n  CPU rates can vary on a single platform).\n\n  Whether an image has no clock, has a single clock of its own, or shares\n  a clock with another image, is processor dependent.\n\n  If there is no clock, or querying the clock fails, **count** is set to\n  **-huge(count)**, and **count_rate** and **count_max** are set to zero.\n\n  The accuracy of the measurements may depend on the kind of the\n  arguments!\n\n  Timing-related procedures are obviously processor and system-dependent.\n  More specific information may generally be found in compiler-specific\n  documentation.\n\n### **Options**\n\n- **count**\n  If there is no clock, the returned value for **count** is the negative\n  value **-huge(count)**.\n\n  Otherwise, the **clock** value is incremented by one for each clock\n  count until the value **count_max** is reached and is then reset to\n  zero at the next count. **clock** therefore is a modulo value that\n  lies in the range **0 to count_max**.\n\n- **count_rate**\n  : is assigned a processor-dependent approximation to the number of\n  processor clock counts per second, or zero if there is no clock.\n  **count_rate** is system dependent and can vary depending on the kind\n  of the arguments. Generally, a large _real_ may generate a more precise\n  interval.\n\n- **count_max**\n  : is assigned the maximum value that **COUNT** can have, or zero if\n  there is no clock.\n\n### **Examples**\n\n  If the processor clock is a 24-hour clock that registers time at\n  approximately 18.20648193 ticks per second, at 11:30 A.M. the reference\n\n```fortran\n      call system_clock (count = c, count_rate = r, count_max = m)\n```\n  defines\n```text\n      C = (11*3600+30*60)*18.20648193 = 753748,\n      R = 18.20648193, and\n      M = 24*3600*18.20648193-1 = 1573039.\n```\n\nSample program:\n```fortran\nprogram demo_system_clock\nuse, intrinsic :: iso_fortran_env, only: wp => real64, int32, int64\nimplicit none\ncharacter(len=*), parameter :: g = '(1x,*(g0,1x))'\n\ninteger(kind=int64) :: count64, count_rate64, count_max64\ninteger(kind=int64) :: start64, finish64\n\ninteger(kind=int32) :: count32, count_rate32, count_max32\ninteger(kind=int32) :: start32, finish32\n\nreal(kind=wp)       :: time_read\nreal(kind=wp)       :: sum\ninteger             :: i\n\n   print g, 'accuracy may vary with argument type!'\n\n   print g, 'query all arguments'\n\n   call system_clock(count64, count_rate64, count_max64)\n   print g, 'COUNT_MAX(64bit)=', count_max64\n   print g, 'COUNT_RATE(64bit)=', count_rate64\n   print g, 'CURRENT COUNT(64bit)=', count64\n\n   call system_clock(count32, count_rate32, count_max32)\n   print g, 'COUNT_MAX(32bit)=', count_max32\n   print g, 'COUNT_RATE(32bit)=', count_rate32\n   print g, 'CURRENT COUNT(32bit)=', count32\n\n   print g, 'time some computation'\n   call system_clock(start64)\n\n   ! some code to time\n   sum = 0.0_wp\n   do i = -0, huge(0) - 1\n      sum = sum + sqrt(real(i))\n   end do\n   print g, 'SUM=', sum\n\n   call system_clock(finish64)\n\n   time_read = (finish64 - start64)/real(count_rate64, wp)\n   write (*, '(1x,a,1x,g0,1x,a)') 'time : ', time_read, ' seconds'\n\nend program demo_system_clock\n```\nResults:\n```text\n >  accuracy may vary with argument type!\n >  query all arguments\n >  COUNT_MAX(64bit)= 9223372036854775807\n >  COUNT_RATE(64bit)= 1000000000\n >  CURRENT COUNT(64bit)= 1105422387865806\n >  COUNT_MAX(32bit)= 2147483647\n >  COUNT_RATE(32bit)= 1000\n >  CURRENT COUNT(32bit)= 1105422387\n >  time some computation\n >  SUM= 66344288183024.266\n >  time :  6.1341038460000004  seconds\n```\n### **Standard**\n\nFortran 95\n\n### **See Also**\n\n[**date_and_time**(3)](#date_and_time),\n[**cpu_time**(3)](#cpu_time)\n\n _fortran-lang intrinsic descriptions_\n",
     "TAN": "## tan\n\n### **Name**\n\n**tan** - \\[MATHEMATICS:TRIGONOMETRIC\\] Tangent function\n\n### **Synopsis**\n```fortran\nresult = tan(x)\n```\n```fortran\n elemental TYPE(kind=KIND) function tan(x)\n\n  TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n  - the **TYPE** of **x** may be _real_ or _complex_ of any supported kind\n  - The returned value will be of the same type and kind as the argument\n    **x**.\n\n### **Description**\n\n**tan** computes the tangent of **x**.\n\n### **Options**\n\n- **x**\n  : The angle in radians to compute the tangent of for _real_ input.\n    If **x** is of type _complex_, its real part is regarded as a value\n    in radians.\n\n### **Result**\n\n  The return value is the tangent of the value **x**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_tan\nuse, intrinsic :: iso_fortran_env, only : real_kinds, &\n& real32, real64, real128\nimplicit none\nreal(kind=real64) :: x = 0.165_real64\n     write(*,*)x, tan(x)\nend program demo_tan\n```\nResults:\n```text\n     0.16500000000000001       0.16651386310913616\n```\n### **Standard**\n\nFORTRAN 77 . For a complex argument, Fortran 2008 .\n\n### **See Also**\n\n[**atan**(3)](#atan),\n[**atan2**(3)](#atan2),\n[**cos**(3)](#cos),\n[**sin**(3)](#sin)\n\n _fortran-lang intrinsic descriptions (license: MIT) \\@urbanjost_\n",
     "TANH": "## tanh\n\n### **Name**\n\n**tanh** - \\[MATHEMATICS:TRIGONOMETRIC\\] Hyperbolic tangent function\n\n### **Synopsis**\n```fortran\n    result = tanh(x)\n```\n```fortran\n     elemental TYPE(kind=KIND) function tanh(x)\n\n      TYPE(kind=KIND),intent(in) :: x\n```\n### **Characteristics**\n\n - **x** may be _real_ or _complex_ and any associated kind supported by\n   the processor.\n - The returned value will be of the same type and kind as the argument.\n\n### **Description**\n\n**tanh** computes the hyperbolic tangent of **x**.\n\n### **Options**\n\n- **x**\n  : The value to compute the Hyperbolic tangent of.\n\n### **Result**\n\nReturns the hyperbolic tangent of **x**.\n\n  If **x** is _complex_, the imaginary part of the result is regarded as\n  a radian value.\n\n  If **x** is _real_, the return value lies in the range\n```\n      -1 <= tanh(x) <= 1.\n```\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_tanh\nuse, intrinsic :: iso_fortran_env, only : &\n& real_kinds, real32, real64, real128\nimplicit none\nreal(kind=real64) :: x = 2.1_real64\n   write(*,*)x, tanh(x)\nend program demo_tanh\n```\nResults:\n```text\n      2.1000000000000001       0.97045193661345386\n```\n### **Standard**\n\nFORTRAN 77 , for a complex argument Fortran 2008\n\n### **See Also**\n\n[**atanh**(3)](#atanh)\n\n### **Resources**\n\n- [Wikipedia:hyperbolic functions](https://en.wikipedia.org/wiki/Hyperbolic_functions)\n\n _fortran-lang intrinsic descriptions_\n",
     "THIS_IMAGE": "## this_image\n\n### **Name**\n\n**this_image** - \\[COLLECTIVE\\] Cosubscript index of this image\n\n### **Synopsis**\n\n```fortran\nresult = this_image() | = this_image(distance) | = this_image(coarray,dim)\n```\n```fortran\n   integer function this_image( distance ,coarray, dim )\n\n    type(TYPE(kind=**)),optional :: coarray[*]\n    integer,intent(in),optional  :: distance\n    integer,intent(in),optional  :: dim\n```\n### **Characteristics**\n\n - a kind designated as ** may be any supported kind for the type\n - **coarray** can be of any type. If **dim** is present it is required.\n - **distance** is not permitted together with **coarray**\n - if **dim** if present, coarray is required.\n\n### **Description**\n\n**this_image** returns the cosubscript for this image.\n\n### **Options**\n\n- **distance**\n  : Nonnegative scalar _integer_ (not permitted together with **coarray**).\n\n- **coarray**\n  : if **dim** present, required).\n\n- **dim**\n  : If present, **dim** shall be between one and the corank of **coarray**.\n\n### **Result**\n\nDefault integer. If **coarray** is not present, it is scalar; if **distance** is\nnot present or has value **0**, its value is the image index on the invoking\nimage for the current team, for values smaller or equal distance to the\ninitial team, it returns the image index on the ancestor team which has\na distance of **distance** from the invoking team. If **distance** is larger\nthan the distance to the initial team, the image index of the initial\nteam is returned. Otherwise when the **coarray** is present, if **dim** is not\npresent, a rank-1 array with corank elements is returned, containing the\ncosubscripts for **coarray** specifying the invoking image. If **dim** is\npresent, a scalar is returned, with the value of the **dim** element of\n**this_image(coarray)**.\n\n### **Examples**\n\nSample program:\n```fortran\nprogram demo_this_image\nimplicit none\ninteger :: value[*]\ninteger :: i\n   value = this_image()\n   sync all\n   if (this_image() == 1) then\n      do i = 1, num_images()\n         write(*,'(2(a,i0))') 'value[', i, '] is ', value[i]\n      end do\n   endif\nend program demo_this_image\n```\nResults:\n```text\n   value[1] is 1\n```\n### **Standard**\n\nFortran 2008. With DISTANCE argument, TS 18508\n\n### **See Also**\n\n[**num\\_images**(3)](#num_images),\n[**image\\_index**(3)](#image_index)\n\n _fortran-lang intrinsic descriptions_\n",
```

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/intrinsics.py` & `fortls-3.0.0rc3/fortls/parsers/internal/intrinsics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import glob
 import json
 import os
-import pathlib
+from pathlib import Path
 
 from fortls.helper_functions import fortran_md, get_placeholders, map_keywords
 
 from .ast import FortranAST
 from .base import FortranObj
 from .function import Function
 from .module import Module
@@ -267,21 +267,23 @@
 def update_m_intrinsics():
     try:
         files = glob.glob("M_intrinsics/md/*.md")
         markdown_intrinsics = {}
         for f in sorted(files):
             key = f.replace("M_intrinsics/md/", "")
             key = key.replace(".md", "").upper()  # remove md extension
-            val = pathlib.Path(f).read_text()
+            val = Path(f).read_text()
             # remove manpage tag
             val = val.replace(f"**{key.lower()}**(3)", f"**{key.lower()}**")
             val = val.replace(f"**{key.upper()}**(3)", f"**{key.upper()}**")
             markdown_intrinsics[key] = val
 
-        with open("fortls/intrinsic.procedures.markdown.json", "w") as f:
+        with open(
+            Path(__file__).parent / "intrinsic.procedures.markdown.json", "w"
+        ) as f:
             json.dump(markdown_intrinsics, f, indent=2)
             f.write("\n")  # add newline at end of file
     except Exception as e:
         print(e)
 
 
 if __name__ == "__main__":
```

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/keywords.json` & `fortls-3.0.0rc3/fortls/parsers/internal/keywords.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/method.py` & `fortls-3.0.0rc3/fortls/parsers/internal/method.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/module.py` & `fortls-3.0.0rc3/fortls/parsers/internal/module.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/parser.py` & `fortls-3.0.0rc3/fortls/parsers/internal/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1673,19 +1673,19 @@
             if len(file_ast.end_errors) > 0:
                 log.debug("\n=== Scope Errors ===\n")
                 for error in file_ast.end_errors:
                     if error[0] >= 0:
                         message = f"Unexpected end of scope at line {error[0]}"
                     else:
                         message = "Unexpected end statement: No open scopes"
-                    log.debug(f"{error[1]}: {message}")
+                    log.debug("%s: %s", error[1], message)
             if len(file_ast.parse_errors) > 0:
                 log.debug("\n=== Parsing Errors ===\n")
                 for error in file_ast.parse_errors:
-                    log.debug(f"{error['range']}: {error['message']}")
+                    log.debug("%s: %s", error["range"], error["message"])
         return file_ast
 
     def parse_imp_dim(self, line: str):
         """Parse the implicit dimension of an array e.g.
         var(3,4), var_name(size(val,1)*10)
 
         Parameters
@@ -1915,15 +1915,15 @@
                 )
             return docstr
 
         def add_line_comment(file_ast: FortranAST, docs: list[str]):
             # Handle dangling comments from previous line
             if docs:
                 file_ast.add_doc(format(docs))
-                log.debug(f"{format(docs)} !!! Doc string - Line:{ln}")
+                log.debug("%s !!! Doc string - Line:%d", format(docs), ln)
                 docs[:] = []  # empty the documentation stack
 
         # Check for comments in line
         if not self.COMMENT_LINE_MATCH.match(line):
             add_line_comment(file_ast, docs)
             return False
         # Check for documentation
@@ -1936,15 +1936,15 @@
         ln, docs[:], predocmark = self.get_docstring(ln, line, doc_match, docs)
 
         # Count the total length of all the stings in docs
         # most efficient implementation, see: shorturl.at/dfmyV
         if len("".join(docs)) > 0:
             file_ast.add_doc(format(docs), forward=predocmark)
         for i, doc_line in enumerate(docs):
-            log.debug(f"{doc_line} !!! Doc string - Line:{_ln + i}")
+            log.debug("%s !!! Doc string - Line:%d", doc_line, _ln + i)
         docs[:] = []
         return ln
 
     def get_docstring(
         self, ln: int, line: str, match: Match[str], docs: list[str]
     ) -> tuple[int, list[str], bool]:
         """Extract entire documentation strings from the current file position
@@ -2041,17 +2041,17 @@
             return expr
 
         def replace_defined(line: str):
             i0 = 0
             out_line = ""
             for match in FRegex.DEFINED.finditer(line):
                 if match.group(1) in defs:
-                    out_line += line[i0 : match.start(0)] + "($@)"
+                    out_line += line[i0 : match.start(0)] + "(@$@)"
                 else:
-                    out_line += line[i0 : match.start(0)] + "($%)"
+                    out_line += line[i0 : match.start(0)] + "(%$%)"
                 i0 = match.end(0)
             if i0 < len(line):
                 out_line += line[i0:]
             return out_line
 
         def replace_vars(line: str):
             i0 = 0
@@ -2060,29 +2060,46 @@
                 if match.group(0) in defs:
                     out_line += line[i0 : match.start(0)] + defs[match.group(0)]
                 else:
                     out_line += line[i0 : match.start(0)] + "False"
                 i0 = match.end(0)
             if i0 < len(line):
                 out_line += line[i0:]
-            out_line = out_line.replace("$@", "True")
-            out_line = out_line.replace("$%", "False")
+            out_line = out_line.replace("@$@", "True")
+            out_line = out_line.replace("%$%", "False")
             return out_line
 
         if defs is None:
             defs = {}
         out_line = replace_defined(text)
         out_line = replace_vars(out_line)
         try:
             line_res = eval(replace_ops(out_line))
         except:
             return False
         else:
             return line_res
 
+    def expand_func_macro(def_name: str, def_value: tuple[str, str]):
+        def_args, sub = def_value
+        def_args = def_args.split(",")
+        regex = re.compile(rf"\b{def_name}\s*\({','.join(['(.*)']*len(def_args))}\)")
+
+        for i, arg in enumerate(def_args, start=1):
+            sub = re.sub(rf"\b({arg.strip()})\b", rf"\\{i}", sub)
+
+        return regex, sub
+
+    def append_multiline_macro(def_value: str | tuple, line: str):
+        if isinstance(def_value, tuple):
+            def_args, def_value = def_value
+            def_value += line
+            return (def_args, def_value)
+        return def_value + line
+
     if pp_defs is None:
         pp_defs = {}
     if include_dirs is None:
         include_dirs = set()
     if file_path is not None:
         include_dirs.add(os.path.abspath(os.path.dirname(file_path)))
     pp_skips = []
@@ -2093,53 +2110,55 @@
     def_regexes = {}
     output_file = []
     def_cont_name = None
     for i, line in enumerate(contents_split):
         # Handle multiline macro continuation
         if def_cont_name is not None:
             output_file.append("")
-            if line.rstrip()[-1] != "\\":
-                defs_tmp[def_cont_name] += line.strip()
+            is_multiline = line.strip()[-1] != "\\"
+            line_to_append = line.strip() if is_multiline else line[0:-1].strip()
+            defs_tmp[def_cont_name] = append_multiline_macro(
+                defs_tmp[def_cont_name], line_to_append
+            )
+            if is_multiline:
                 def_cont_name = None
-            else:
-                defs_tmp[def_cont_name] += line[0:-1].strip()
             continue
         # Handle conditional statements
         match = FRegex.PP_REGEX.match(line)
         if match:
             output_file.append(line)
             def_name = None
             if_start = False
             # Opening conditional statements
-            if match.group(1) == "if ":
+            if match.group(1).lower() == "if ":
                 is_path = eval_pp_if(line[match.end(1) :], defs_tmp)
                 if_start = True
-            elif match.group(1) == "ifdef":
+            elif match.group(1).lower() == "ifdef":
                 if_start = True
                 def_name = line[match.end(0) :].strip()
                 is_path = def_name in defs_tmp
-            elif match.group(1) == "ifndef":
+            elif match.group(1).lower() == "ifndef":
                 if_start = True
                 def_name = line[match.end(0) :].strip()
                 is_path = not (def_name in defs_tmp)
             if if_start:
                 if is_path:
                     pp_stack.append([-1, -1])
-                    log.debug(f"{line.strip()} !!! Conditional TRUE({i + 1})")
+                    log.debug("%s !!! Conditional TRUE(%d)", line.strip(), i + 1)
                 else:
                     pp_stack.append([i + 1, -1])
-                    log.debug(f"{line.strip()} !!! Conditional FALSE({i + 1})")
+                    log.debug("%s !!! Conditional FALSE(%d)", line.strip(), i + 1)
                 continue
             if len(pp_stack) == 0:
                 continue
             # Closing/middle conditional statements
             inc_start = False
             exc_start = False
             exc_continue = False
-            if match.group(1) == "elif":
+            if match.group(1).lower() == "elif":
                 if (not pp_stack_group) or (pp_stack_group[-1][0] != len(pp_stack)):
                     # First elif statement for this elif group
                     if pp_stack[-1][0] < 0:
                         pp_stack_group.append([len(pp_stack), True])
                     else:
                         pp_stack_group.append([len(pp_stack), False])
                 if pp_stack_group[-1][1]:
@@ -2151,15 +2170,15 @@
                     pp_stack[-1][1] = i + 1
                     pp_skips.append(pp_stack.pop())
                     pp_stack_group[-1][1] = True
                     pp_stack.append([-1, -1])
                     inc_start = True
                 else:
                     exc_start = True
-            elif match.group(1) == "else":
+            elif match.group(1).lower() == "else":
                 if pp_stack[-1][0] < 0:
                     pp_stack[-1][0] = i + 1
                     exc_start = True
                 elif (
                     pp_stack_group
                     and (pp_stack_group[-1][0] == len(pp_stack))
                     and (pp_stack_group[-1][1])
@@ -2167,32 +2186,32 @@
                     # An earlier if or elif in this group has been true
                     exc_continue = True
                 else:
                     pp_stack[-1][1] = i + 1
                     pp_skips.append(pp_stack.pop())
                     pp_stack.append([-1, -1])
                     inc_start = True
-            elif match.group(1) == "endif":
+            elif match.group(1).lower() == "endif":
                 if pp_stack_group and (pp_stack_group[-1][0] == len(pp_stack)):
                     pp_stack_group.pop()
                 if pp_stack[-1][0] < 0:
                     pp_stack.pop()
-                    log.debug(f"{line.strip()} !!! Conditional TRUE/END({i + 1})")
+                    log.debug("%s !!! Conditional TRUE/END(%d)", line.strip(), i + 1)
                     continue
                 if pp_stack[-1][1] < 0:
                     pp_stack[-1][1] = i + 1
-                    log.debug(f"{line.strip()} !!! Conditional FALSE/END({i + 1})")
+                    log.debug("%s !!! Conditional FALSE/END(%d)", line.strip(), i + 1)
                 pp_skips.append(pp_stack.pop())
             if debug:
                 if inc_start:
-                    log.debug(f"{line.strip()} !!! Conditional TRUE({i + 1})")
+                    log.debug("%s !!! Conditional TRUE(%d)", line.strip(), i + 1)
                 elif exc_start:
-                    log.debug(f"{line.strip()} !!! Conditional FALSE({i + 1})")
+                    log.debug("%s !!! Conditional FALSE(%d)", line.strip(), i + 1)
                 elif exc_continue:
-                    log.debug(f"{line.strip()} !!! Conditional EXCLUDED({i + 1})")
+                    log.debug("%s !!! Conditional EXCLUDED(%d)", line.strip(), i + 1)
             continue
         # Handle variable/macro definitions files
         match = FRegex.PP_DEF.match(line)
         if (match is not None) and ((len(pp_stack) == 0) or (pp_stack[-1][0] < 0)):
             output_file.append(line)
             pp_defines.append(i + 1)
             def_name = match.group(2)
@@ -2205,28 +2224,34 @@
             # if match.group(3):
             #     def_name += match.group(3)
             if (match.group(1) == "define") and (def_name not in defs_tmp):
                 eq_ind = line[match.end(0) :].find(" ")
                 if eq_ind >= 0:
                     # Handle multiline macros
                     if line.rstrip()[-1] == "\\":
-                        defs_tmp[def_name] = line[match.end(0) + eq_ind : -1].strip()
+                        def_value = line[match.end(0) + eq_ind : -1].strip()
                         def_cont_name = def_name
                     else:
-                        defs_tmp[def_name] = line[match.end(0) + eq_ind :].strip()
+                        def_value = line[match.end(0) + eq_ind :].strip()
                 else:
-                    defs_tmp[def_name] = "True"
+                    def_value = "True"
+
+                # are there arguments to parse?
+                if match.group(3):
+                    def_value = (match.group(4), def_value)
+
+                defs_tmp[def_name] = def_value
             elif (match.group(1) == "undef") and (def_name in defs_tmp):
                 defs_tmp.pop(def_name, None)
-            log.debug(f"{line.strip()} !!! Define statement({i + 1})")
+            log.debug("%s !!! Define statement(%d)", line.strip(), i + 1)
             continue
         # Handle include files
         match = FRegex.PP_INCLUDE.match(line)
         if (match is not None) and ((len(pp_stack) == 0) or (pp_stack[-1][0] < 0)):
-            log.debug(f"{line.strip()} !!! Include statement({i + 1})")
+            log.debug("%s !!! Include statement(%d)", line.strip(), i + 1)
             include_filename = match.group(1).replace('"', "")
             include_path = None
             # Intentionally keep this as a list and not a set. There are cases
             # where projects play tricks with the include order of their headers
             # to get their codes to compile. Using a set would not permit that.
             for include_dir in include_dirs:
                 include_path_tmp = os.path.join(include_dir, include_filename)
@@ -2234,44 +2259,57 @@
                     include_path = os.path.abspath(include_path_tmp)
                     break
             if include_path is not None:
                 try:
                     include_file = FortranFile(include_path)
                     err_string, _ = include_file.load_from_disk()
                     if err_string is None:
-                        log.debug(f'\n!!! Parsing include file "{include_path}"')
+                        log.debug("\n!!! Parsing include file '%s'", include_path)
                         _, _, _, defs_tmp = preprocess_file(
                             include_file.contents_split,
                             file_path=include_path,
                             pp_defs=defs_tmp,
                             include_dirs=include_dirs,
                             debug=debug,
                         )
                         log.debug("!!! Completed parsing include file\n")
 
                     else:
-                        log.debug(f"!!! Failed to parse include file: {err_string}")
+                        log.debug("!!! Failed to parse include file: %s", err_string)
 
                 except:
                     log.debug("!!! Failed to parse include file: exception")
 
             else:
-                log.debug(f"{line.strip()} !!! Could not locate include file ({i + 1})")
+                log.debug(
+                    "%s !!! Could not locate include file (%d)", line.strip(), i + 1
+                )
 
         # Substitute (if any) read in preprocessor macros
         for def_tmp, value in defs_tmp.items():
             # Skip if the line does not contain the macro at all. This is supposed to
             # spare the expensive regex-substitution in case we do not need it at all
             if def_tmp not in line:
                 continue
             def_regex = def_regexes.get(def_tmp)
             if def_regex is None:
-                def_regex = re.compile(rf"\b{def_tmp}\b")
+                if isinstance(value, tuple):
+                    def_regex = expand_func_macro(def_tmp, value)
+                else:
+                    def_regex = re.compile(rf"\b{def_tmp}\b")
                 def_regexes[def_tmp] = def_regex
+
+            if isinstance(def_regex, tuple):
+                def_regex, value = def_regex
+
             line_new, nsubs = def_regex.subn(value, line)
             if nsubs > 0:
                 log.debug(
-                    f"{line.strip()} !!! Macro sub({i + 1}) '{def_tmp}' -> {value}"
+                    "%s !!! Macro sub(%d) '%s' -> '%s'",
+                    line.strip(),
+                    i + 1,
+                    def_tmp,
+                    value,
                 )
                 line = line_new
         output_file.append(line)
     return output_file, pp_skips, pp_defines, defs_tmp
```

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/scope.py` & `fortls-3.0.0rc3/fortls/parsers/internal/scope.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/select.py` & `fortls-3.0.0rc3/fortls/parsers/internal/select.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/statements.json` & `fortls-3.0.0rc3/fortls/parsers/internal/statements.json`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/submodule.py` & `fortls-3.0.0rc3/fortls/parsers/internal/submodule.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/subroutine.py` & `fortls-3.0.0rc3/fortls/parsers/internal/subroutine.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/type.py` & `fortls-3.0.0rc3/fortls/parsers/internal/type.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/use.py` & `fortls-3.0.0rc3/fortls/parsers/internal/use.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/utilities.py` & `fortls-3.0.0rc3/fortls/parsers/internal/utilities.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/parsers/internal/variable.py` & `fortls-3.0.0rc3/fortls/parsers/internal/variable.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/fortls/regex_patterns.py` & `fortls-3.0.0rc3/fortls/regex_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         I,
     )
     PARAMETER_VAL: Pattern = compile(r"\w*[\s\&]*=(([\s\&]*[\w\.\-\+\*\/\'\"])*)", I)
     TATTR_LIST: Pattern = compile(
         r"[ ]*,[ ]*(PUBLIC|PRIVATE|ABSTRACT|EXTENDS\(\w*\))", I
     )
     VIS: Pattern = compile(r"[ ]*\b(PUBLIC|PRIVATE)\b", I)
-    WORD: Pattern = compile(r"[a-z_]\w*", I)
+    WORD: Pattern = compile(r"[a-z_][\w\$]*", I)
     NUMBER: Pattern = compile(
         r"[\+\-]?(\b\d+\.?\d*|\.\d+)(_\w+|d[\+\-]?\d+|e[\+\-]?\d+(_\w+)?)?(?!\w)",
         I,
     )
     LOGICAL: Pattern = compile(r".true.|.false.", I)
     SUB_PAREN: Pattern = compile(r"\([\w, ]*\)", I)
     # KIND_SPEC_MATCH: Pattern = compile(r"\([\w, =*]*\)", I)
@@ -120,19 +120,22 @@
     FREE_COMMENT: Pattern = compile(r"([ ]*!)")
     FREE_CONT: Pattern = compile(r"([ ]*&)")
     FREE_DOC: Pattern = compile(r"[ ]*!([<>!])")
     FREE_OPENMP: Pattern = compile(r"[ ]*!\$OMP", I)
     FREE_FORMAT_TEST: Pattern = compile(r"[ ]{1,4}[a-z]", I)
     # Preprocessor matching rules
     DEFINED: Pattern = compile(r"defined[ ]*\(?[ ]*([a-z_]\w*)[ ]*\)?", I)
-    PP_REGEX: Pattern = compile(r"#(if |ifdef|ifndef|else|elif|endif)")
-    PP_DEF: Pattern = compile(r"#(define|undef)[ ]*([\w]+)(\((\w+(,[ ]*)?)+\))?", I)
+    PP_REGEX: Pattern = compile(r"[ ]*#[ ]*(if |ifdef|ifndef|else|elif|endif)", I)
+    PP_DEF: Pattern = compile(
+        r"[ ]*#[ ]*(define|undef|undefined)[ ]*(\w+)(\([ ]*([ \w,]*?)[ ]*\))?",
+        I,
+    )
     PP_DEF_TEST: Pattern = compile(r"(![ ]*)?defined[ ]*\([ ]*(\w*)[ ]*\)$", I)
-    PP_INCLUDE: Pattern = compile(r"#include[ ]*([\"\w\.]*)", I)
-    PP_ANY: Pattern = compile(r"(^#:?\w+)")
+    PP_INCLUDE: Pattern = compile(r"[ ]*#[ ]*include[ ]*([\"\w\.]*)", I)
+    PP_ANY: Pattern = compile(r"^[ ]*#:?[ ]*(\w+)")
     # Context matching rules
     CALL: Pattern = compile(r"[ ]*CALL[ ]+[\w%]*$", I)
     INT_STMNT: Pattern = compile(r"^[ ]*[a-z]*$", I)
     TYPE_STMNT: Pattern = compile(r"[ ]*(TYPE|CLASS)[ ]*(IS)?[ ]*$", I)
     PROCEDURE_STMNT: Pattern = compile(r"[ ]*(PROCEDURE)[ ]*$", I)
     PRO_LINK: Pattern = compile(r"[ ]*(MODULE[ ]*PROCEDURE )", I)
     SCOPE_DEF: Pattern = compile(
@@ -142,15 +145,15 @@
         r"[ ]*(END)("
         r" |MODULE|PROGRAM|SUBROUTINE|FUNCTION|PROCEDURE|TYPE|DO|IF|SELECT)?",
         I,
     )
     # Object regex patterns
     CLASS_VAR: Pattern = compile(r"(TYPE|CLASS)[ ]*\(", I)
     DEF_KIND: Pattern = compile(r"(\w*)[ ]*\((?:KIND|LEN)?[ =]*(\w*)", I)
-    OBJBREAK: Pattern = compile(r"[\/\-(.,+*<>=$: ]", I)
+    OBJBREAK: Pattern = compile(r"[\/\-(.,+*<>=: ]", I)
 
 
 # TODO: use this in the main code
 def create_src_file_exts_regex(input_exts: list[str] = []) -> Pattern[str]:
     r"""Create a REGEX for which sources the Language Server should parse.
 
     Default extensions are (case insensitive):
```

### Comparing `fortls-3.0.0rc2/fortls/schema.py` & `fortls-3.0.0rc3/fortls/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import json
 import pathlib
 
 from pydantic import Field, create_model
 
 from fortls.interface import cli
 
 
@@ -19,19 +20,19 @@
             or arg.dest == "version"
             or arg.help == "==SUPPRESS=="
             or (arg.dest.startswith("debug") and arg.dest != "debug_log")
         ):
             continue
         val = arg.default
         desc: str = arg.help.replace("%(default)s", str(val))  # type: ignore
-        only_vals[arg.dest] = Field(val, description=desc)  # type: ignore
+        only_vals[arg.dest] = (type(val), Field(val, description=desc))  # type: ignore
 
     m = create_model("fortls schema", **only_vals)
     m.__doc__ = "Schema for the fortls Fortran Language Server"
 
-    with open(str(root / "fortls.schema.json"), "w") as f:
-        print(m.schema_json(indent=2), file=f)
+    with open(str(root / "fortls.schema.json"), "w", encoding="utf-8") as f:
+        print(json.dumps(m.model_json_schema(), indent=2), file=f)
     print(f"Created schema file: {root / 'fortls.schema.json'}")
 
 
 if __name__ == "__main__":
     create_schema()
```

### Comparing `fortls-3.0.0rc2/fortls.egg-info/PKG-INFO` & `fortls-3.0.0rc3/fortls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortls
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: fortls - Fortran Language Server
 Home-page: https://fortls.fortran-lang.org
 Author: Giannis Nikiteas
 Author-email: giannis.nikiteas@gmail.com
 License: MIT
 Project-URL: Documentation, https://fortls.fortran-lang.org
 Project-URL: Changes, https://github.com/fortran-lang/fortls/blob/master/CHANGELOG.md
@@ -38,29 +38,30 @@
 Provides-Extra: dev
 Requires-Dist: pytest>=7.2.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=3.0.2; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pydantic==1.10.13; extra == "dev"
+Requires-Dist: pydantic; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=4.0.0; extra == "docs"
 Requires-Dist: sphinx-argparse; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx_design; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx-sitemap; extra == "docs"
 
 ![alt](https://raw.githubusercontent.com/fortran-lang/fortls/master/assets/logo.png)
 
 # fortls - Fortran Language Server
 
+[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat-square&colorA=E1523D&colorB=007D8A)](https://numfocus.org)
 ![PyPI](https://img.shields.io/pypi/v/fortls?style=flat-square)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fortls?style=flat-square)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/fortls?style=flat-square&label=PyPi)](https://pepy.tech/project/fortls)
 ![Conda](https://img.shields.io/conda/dn/conda-forge/fortls?label=Anaconda&style=flat-square)
 ![GitHub License](https://img.shields.io/github/license/fortran-lang/fortls?style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/main.yml?branch=master&label=CI&style=flat-square)
 ![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/fortran-lang/fortls/docs.yml?branch=master&label=Docs&style=flat-square)
@@ -115,28 +116,14 @@
   - Generate type-bound procedures and implementation templates for
     deferred procedures
 
 ### Notes/Limitations
 
 - Signature help and hover does not handle elegantly overloaded functions i.e. interfaces
 
-## `fortls` vs `fortran-language-server`
-
-This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
-
-`fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
-the original `fortran-language-server` does not.
-
-For a complete and detailed list of the differences between the two Language Servers
-see the Documentation section: [Unique fortls features (not in fortran-language-server)](https://fortls.fortran-lang.org/fortls_changes.html)
-
-The name of executable for this project has been chosen to remain `fortls`
-to allow for integration with pre-existing plugins and workflows, but it could
-change in the future.
-
 ## Future plans
 
 `fortls` has reached a point where it is feature complete and stable enough to be used in many modern Fortran projects without any issues.
 It does however still have fundamental limitations,
 namely its ability to understand all Fortran syntax and semantics that has been used throughout the 65+ years of the language. **The good news is that we have a plan to address this issue!**
 
 We are excited to announce that we are working on creating a new Fortran Language Server
@@ -226,14 +213,28 @@
 | `textDocument/rename`            | Rename a symbol across the workspace                   |
 | `textDocument/didOpen`           | Document synchronisation upon opening                  |
 | `textDocument/didSave`           | Document synchronisation upon saving                   |
 | `textDocument/didClose`          | Document synchronisation upon closing                  |
 | `textDocument/didChange`         | Document synchronisation upon changes to the document  |
 | `textDocument/codeAction`        | **Experimental** Generate code                         |
 
+## `fortls` vs `fortran-language-server`
+
+This project was originally based on `fortran-language-server` LSP implementation, but the two projects have since diverged.
+
+`fortls` (this project) is now developed independently of the upstream `hansec/fortran-language-server` project and contains numerous new features and bug fixes
+the original `fortran-language-server` does not.
+
+For a complete and detailed list of the differences between the two Language Servers
+see the Documentation section: [Unique fortls features (not in fortran-language-server)](https://fortls.fortran-lang.org/fortls_changes.html)
+
+The name of executable for this project has been chosen to remain `fortls`
+to allow for integration with pre-existing plugins and workflows, but it could
+change in the future.
+
 ## Acknowledgements
 
 This project would not have been possible without the original work of [@hansec](https://github.com/hansec/)
 in [`fortran-language-server`](https://github.com/hansec/fortran-language-server)
 
 <!-- ## Support
```

### Comparing `fortls-3.0.0rc2/fortls.egg-info/SOURCES.txt` & `fortls-3.0.0rc3/fortls.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 .github/CODEOWNERS
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/codeql-analysis.yml
 .github/workflows/docs.yml
+.github/workflows/docs_preview.yml
 .github/workflows/main.yml
 .github/workflows/python-publish.yml
 .github/workflows/update-intrinsics.yml
 assets/LICENSE
 assets/README.md
 assets/f.svg
 assets/icon.svg
@@ -54,27 +55,30 @@
 assets/lsp/symbols.png
 docs/Makefile
 docs/conf.py
 docs/contact.rst
 docs/contributing.rst
 docs/editor_integration.rst
 docs/features.rst
+docs/fortls.parsers.internal.rst
+docs/fortls.parsers.rst
 docs/fortls.rst
 docs/index.rst
 docs/make.bat
 docs/modules.rst
 docs/options.rst
 docs/quickstart.rst
 docs/html_extra/CNAME
 docs/html_extra/google3e426562ce42e98f.html
 docs/html_extra/robots.txt
 fortls/__init__.py
 fortls/__main__.py
 fortls/_version.py
 fortls/constants.py
+fortls/debug.py
 fortls/fortls.schema.json
 fortls/ftypes.py
 fortls/helper_functions.py
 fortls/interface.py
 fortls/json_templates.py
 fortls/jsonrpc.py
 fortls/langserver.py
@@ -121,14 +125,15 @@
 fortls/parsers/internal/variable.py
 fortls/parsers/internal/where.py
 licenses/fortran-language-server-license.txt
 test/setup_tests.py
 test/test_interface.py
 test/test_parser.py
 test/test_preproc.py
+test/test_preproc_parser.py
 test/test_regex_patterns.py
 test/test_server.py
 test/test_server_completion.py
 test/test_server_definitions.py
 test/test_server_diagnostics.py
 test/test_server_documentation.py
 test/test_server_hover.py
```

### Comparing `fortls-3.0.0rc2/licenses/fortran-language-server-license.txt` & `fortls-3.0.0rc3/licenses/fortran-language-server-license.txt`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/setup.cfg` & `fortls-3.0.0rc3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 dev = 
 	pytest >= 7.2.0
 	pytest-cov >= 4.0.0
 	pytest-xdist >= 3.0.2
 	black
 	isort
 	pre-commit
-	pydantic==1.10.13
+	pydantic
 docs = 
 	sphinx >= 4.0.0
 	sphinx-argparse
 	sphinx-autodoc-typehints
 	sphinx_design
 	sphinx-copybutton
 	furo
```

### Comparing `fortls-3.0.0rc2/test/setup_tests.py` & `fortls-3.0.0rc3/test/setup_tests.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_interface.py` & `fortls-3.0.0rc3/test/test_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,35 +79,36 @@
 
 
 def test_command_line_code_actions_options():
     args = parser.parse_args("--enable_code_actions".split())
     assert args.enable_code_actions
 
 
-def unittest_server_init():
+def unittest_server_init(conn=None):
     from fortls.langserver import LangServer
 
     root = (Path(__file__).parent / "test_source").resolve()
     parser = cli("fortls")
     args = parser.parse_args("-c f90_config.json".split())
 
-    server = LangServer(None, vars(args))
+    server = LangServer(conn, vars(args))
     server.root_path = root
     server._load_config_file()
 
     return server, root
 
 
 def test_config_file_general_options():
     server, root = unittest_server_init()
     assert server.nthreads == 8
     assert server.notify_init
     assert server.incremental_sync
     assert server.sort_keywords
     assert server.disable_autoupdate
+    assert server.recursion_limit == 1500
 
 
 def test_config_file_dir_parsing_options():
     server, r = unittest_server_init()
     # File parsing
     assert server.source_dirs == {"pp/**", "subdir"}
     assert server.incl_suffixes == {".FF", ".fpc", ".h", "f20"}
@@ -164,26 +165,22 @@
     assert server.enable_code_actions
 
 
 def test_version_update_pypi():
     from packaging import version
 
     from fortls.jsonrpc import JSONRPC2Connection, ReadWriter
-    from fortls.langserver import LangServer
-
-    parser = cli("fortls")
-    args = parser.parse_args("-c f90_config.json".split())
-    args = vars(args)
-    args["disable_autoupdate"] = False
 
     stdin, stdout = sys.stdin.buffer, sys.stdout.buffer
-    s = LangServer(conn=JSONRPC2Connection(ReadWriter(stdin, stdout)), settings=args)
-    s.root_path = (Path(__file__).parent / "test_source").resolve()
+    s, root = unittest_server_init(JSONRPC2Connection(ReadWriter(stdin, stdout)))
+    s.disable_autoupdate = False
+
     did_update = s._update_version_pypi(test=True)
-    assert did_update
+    isconda = os.path.exists(os.path.join(sys.prefix, "conda-meta"))
+    assert not did_update if isconda else did_update
 
     s.disable_autoupdate = True
     did_update = s._update_version_pypi()
     assert not did_update
 
     s.disable_autoupdate = False
     s._version = version.parse("999.0.0")
```

### Comparing `fortls-3.0.0rc2/test/test_parser.py` & `fortls-3.0.0rc3/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_preproc.py` & `fortls-3.0.0rc3/test/test_preproc.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 
     # Reference solution
     ref_results = (
         "```fortran90\n#define PCType character*(80)\n```",
         "```fortran90\n#define PETSC_ERR_INT_OVERFLOW 84\n```",
         "```fortran90\n#define varVar 55\n```",
         (
-            "```fortran90\n#define ewrite if (priority <= 3) write((priority),"
-            " format)\n```"
+            "```fortran90\n#define ewrite(priority, format)"
+            " if (priority <= 3) write((priority), format)\n```"
         ),
         (
-            "```fortran90\n#define ewrite2 if (priority <= 3) write((priority),"
-            " format)\n```"
+            "```fortran90\n#define ewrite2(priority, format)"
+            " if (priority <= 3) write((priority), format)\n```"
         ),
         "```fortran90\n#define SUCCESS .true.\n```",
         "```fortran90\nREAL, CONTIGUOUS, POINTER, DIMENSION(:) :: var1\n```",
         "```fortran90\nINTEGER :: var0\n```",
         "```fortran90\nREAL :: var1\n```",
         "```fortran90\nINTEGER :: var2\n```",
         "```fortran90\nINTEGER, INTENT(INOUT) :: var\n```",
```

### Comparing `fortls-3.0.0rc2/test/test_regex_patterns.py` & `fortls-3.0.0rc3/test/test_regex_patterns.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server.py` & `fortls-3.0.0rc3/test/test_server.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_completion.py` & `fortls-3.0.0rc3/test/test_server_completion.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_definitions.py` & `fortls-3.0.0rc3/test/test_server_definitions.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_diagnostics.py` & `fortls-3.0.0rc3/test/test_server_diagnostics.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_documentation.py` & `fortls-3.0.0rc3/test/test_server_documentation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_hover.py` & `fortls-3.0.0rc3/test/test_server_hover.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,25 @@
     string += hover_req(file_path, 4, 28)
     errcode, results = run_request(string, fortls_args=["--sort_keywords"])
     assert errcode == 0
     ref_results = ["```fortran90\nINTEGER, PARAMETER :: var2 = 23\n```"]
     validate_hover(results, ref_results)
 
 
+def test_hover_parameter_dollar():
+    """Test that hover parameters with dollar in name are recognized correctly"""
+    string = write_rpc_request(1, "initialize", {"rootPath": str(test_dir)})
+    file_path = test_dir / "hover" / "parameters.f90"
+    string += hover_req(file_path, 20, 31)
+    errcode, results = run_request(string, fortls_args=["--sort_keywords"])
+    assert errcode == 0
+    ref_results = ["```fortran90\nINTEGER(4), PARAMETER :: SIG$ERR = -1\n```"]
+    validate_hover(results, ref_results)
+
+
 def test_hover_parameter_eqnospace():
     """Test that hover parameters display value correctly"""
     string = write_rpc_request(1, "initialize", {"rootPath": str(test_dir)})
     file_path = test_dir / "hover" / "parameters.f90"
     string += hover_req(file_path, 11, 28)
     errcode, results = run_request(string, fortls_args=["--sort_keywords"])
     assert errcode == 0
```

### Comparing `fortls-3.0.0rc2/test/test_server_implementation.py` & `fortls-3.0.0rc3/test/test_server_implementation.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_messages.py` & `fortls-3.0.0rc3/test/test_server_messages.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_references.py` & `fortls-3.0.0rc3/test/test_server_references.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_rename.py` & `fortls-3.0.0rc3/test/test_server_rename.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_server_signature_help.py` & `fortls-3.0.0rc3/test/test_server_signature_help.py`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/completion/use_only_interface.f90` & `fortls-3.0.0rc3/test/test_source/completion/use_only_interface.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/diag/test_function_arg_list.f90` & `fortls-3.0.0rc3/test/test_source/diag/test_function_arg_list.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/diag/test_scope_overreach.f90` & `fortls-3.0.0rc3/test/test_source/diag/test_scope_overreach.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/diag/test_semicolon.f90` & `fortls-3.0.0rc3/test/test_source/diag/test_semicolon.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/docs/test_doxygen.f90` & `fortls-3.0.0rc3/test/test_source/docs/test_doxygen.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/docs/test_ford.f90` & `fortls-3.0.0rc3/test/test_source/docs/test_ford.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/excldir/sub1/tmp.f90` & `fortls-3.0.0rc3/test/test_source/excldir/sub1/tmp.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/f90_config.json` & `fortls-3.0.0rc3/test/test_source/f90_config.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'recursion_limit'": '1500'}*

```diff
@@ -35,14 +35,15 @@
         "HAVE_ZOLTAN": "",
         "Mat": "type(tMat)"
     },
     "pp_suffixes": [
         ".h",
         ".fh"
     ],
+    "recursion_limit": 1500,
     "sort_keywords": true,
     "source_dirs": [
         "subdir",
         "pp/**"
     ],
     "symbol_skip_mem": true,
     "use_signature_help": true,
```

### Comparing `fortls-3.0.0rc2/test/test_source/hover/functions.f90` & `fortls-3.0.0rc3/test/test_source/hover/functions.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/hover/parameters.f90` & `fortls-3.0.0rc3/test/test_source/hover/parameters.f90`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,9 @@
     integer, parameter :: var_sum1  = 1 + 23
     integer, parameter :: var_ex1  = 1 - 23
     integer, parameter :: var_mul1  = 1  *   23
     integer, parameter :: var_div1  = 1/1
     INTEGER, PARAMETER :: var_multi2 = 1 *   &
                                         23 + &
                                         2 /1        ! comment
+    INTEGER(4), PARAMETER :: SIG$ERR   = -1
 end program params
```

### Comparing `fortls-3.0.0rc2/test/test_source/hover/recursive.f90` & `fortls-3.0.0rc3/test/test_source/hover/recursive.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/imp/import.f90` & `fortls-3.0.0rc3/test/test_source/imp/import.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/imp/submodule.f90` & `fortls-3.0.0rc3/test/test_source/imp/submodule.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/parse/test_kinds_and_dims.f90` & `fortls-3.0.0rc3/test/test_source/parse/test_kinds_and_dims.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/pp/preproc_elif.F90` & `fortls-3.0.0rc3/test/test_source/pp/preproc_elif.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/pp/preproc_elif_elif_skip.F90` & `fortls-3.0.0rc3/test/test_source/pp/preproc_elif_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/pp/preproc_if_elif_else.F90` & `fortls-3.0.0rc3/test/test_source/pp/preproc_if_elif_else.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/pp/preproc_if_elif_skip.F90` & `fortls-3.0.0rc3/test/test_source/pp/preproc_if_elif_skip.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/rename/test_rename_intrinsic.f90` & `fortls-3.0.0rc3/test/test_source/rename/test_rename_intrinsic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/signature/help.f90` & `fortls-3.0.0rc3/test/test_source/signature/help.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/subdir/test_fixed.f` & `fortls-3.0.0rc3/test/test_source/subdir/test_fixed.f`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/subdir/test_free.f90` & `fortls-3.0.0rc3/test/test_source/subdir/test_free.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/subdir/test_generic.f90` & `fortls-3.0.0rc3/test/test_source/subdir/test_generic.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/subdir/test_select.f90` & `fortls-3.0.0rc3/test/test_source/subdir/test_select.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/subdir/test_submod.F90` & `fortls-3.0.0rc3/test/test_source/subdir/test_submod.F90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/test_diagnostic_int.f90` & `fortls-3.0.0rc3/test/test_source/test_diagnostic_int.f90`

 * *Files identical despite different names*

### Comparing `fortls-3.0.0rc2/test/test_source/test_prog.f08` & `fortls-3.0.0rc3/test/test_source/test_prog.f08`

 * *Files identical despite different names*

