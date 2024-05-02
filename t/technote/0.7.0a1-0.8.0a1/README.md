# Comparing `tmp/technote-0.7.0a1.tar.gz` & `tmp/technote-0.8.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "technote-0.7.0a1.tar", last modified: Mon Jan 29 21:13:35 2024, max compression
+gzip compressed data, was "technote-0.8.0a1.tar", last modified: Thu May  2 18:50:04 2024, max compression
```

## Comparing `technote-0.7.0a1.tar` & `technote-0.8.0a1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.683463 technote-0.7.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.659462 technote-0.7.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-01-29 21:13:14.000000 technote-0.7.0a1/.github/CODE_OF_CONDUCT
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-01-29 21:13:14.000000 technote-0.7.0a1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-01-29 21:13:14.000000 technote-0.7.0a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.659462 technote-0.7.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-01-29 21:13:14.000000 technote-0.7.0a1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-29 21:13:14.000000 technote-0.7.0a1/.github/workflows/dependencies.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-29 21:13:14.000000 technote-0.7.0a1/.github/workflows/periodic-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-01-29 21:13:14.000000 technote-0.7.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-29 21:13:14.000000 technote-0.7.0a1/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-29 21:13:14.000000 technote-0.7.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-29 21:13:14.000000 technote-0.7.0a1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-29 21:13:14.000000 technote-0.7.0a1/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.659462 technote-0.7.0a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-29 21:13:14.000000 technote-0.7.0a1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-01-29 21:13:14.000000 technote-0.7.0a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-29 21:13:14.000000 technote-0.7.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-29 21:13:14.000000 technote-0.7.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-29 21:13:14.000000 technote-0.7.0a1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-01-29 21:13:35.683463 technote-0.7.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-29 21:13:14.000000 technote-0.7.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.659462 technote-0.7.0a1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-29 21:13:14.000000 technote-0.7.0a1/changelog.d/20240129_154947_jsick_DM_42705.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-29 21:13:14.000000 technote-0.7.0a1/changelog.d/_template.md.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.651462 technote-0.7.0a1/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.659462 technote-0.7.0a1/demo/md/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.659462 technote-0.7.0a1/demo/md/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/_static/technote-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/_static/technote-logo-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/index.md
--rw-r--r--   0 runner    (1001) docker     (127)   199011 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/rubin-watermark.png
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/md/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.663462 technote-0.7.0a1/demo/rst/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.663462 technote-0.7.0a1/demo/rst/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/_static/technote-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/_static/technote-logo-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18134 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)   199011 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/rubin-watermark.png
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-29 21:13:14.000000 technote-0.7.0a1/demo/rst/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.663462 technote-0.7.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.663462 technote-0.7.0a1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/documenteer.toml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.667462 technote-0.7.0a1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/configuration-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/configure-authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/configure-sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/configure-status.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/technote-toml.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs/user-guide/theming-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-29 21:13:14.000000 technote-0.7.0a1/docs-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)   198626 2024-01-29 21:13:24.000000 technote-0.7.0a1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-01-29 21:13:14.000000 technote-0.7.0a1/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-29 21:13:14.000000 technote-0.7.0a1/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-01-29 21:13:14.000000 technote-0.7.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 21:13:35.683463 technote-0.7.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.651462 technote-0.7.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.667462 technote-0.7.0a1/src/technote/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.667462 technote-0.7.0a1/src/technote/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/insertposttitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/pygmentscss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.667462 technote-0.7.0a1/src/technote/ext/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/templates/post-title.html.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/toc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/ext/wraptables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.671462 technote-0.7.0a1/src/technote/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   218216 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/orcid.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/ror.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/spdx.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/metadata/zenodo.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.671462 technote-0.7.0a1/src/technote/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/sources/tomlsettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/sphinxconf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.671462 technote-0.7.0a1/src/technote/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/templating/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/templating/highwire.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/templating/metatagbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/templating/opengraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.671462 technote-0.7.0a1/src/technote/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.671462 technote-0.7.0a1/src/technote/theme/components/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/sidebar-authors.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/sidebar-logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/sidebar-source.html
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/sidebar-toc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/sidebar-version.html
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/toggle-sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/components/toggle-sidebar-secondary.html
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.671462 technote-0.7.0a1/src/technote/theme/partials/
--rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/partials/octicons.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.675463 technote-0.7.0a1/src/technote/theme/sections/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/announcement.html
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/article.html
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/footer-article.html
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/header-content.html
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/header-secondary.html
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/header.html
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/sections/sidebar-secondary.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.675463 technote-0.7.0a1/src/technote/theme/static/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/static/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.675463 technote-0.7.0a1/src/technote/theme/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-01-29 21:13:26.000000 technote-0.7.0a1/src/technote/theme/static/scripts/technote.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.675463 technote-0.7.0a1/src/technote/theme/static/styles/
--rw-r--r--   0 runner    (1001) docker     (127)    25016 2024-01-29 21:13:26.000000 technote-0.7.0a1/src/technote/theme/static/styles/technote.css
--rw-r--r--   0 runner    (1001) docker     (127)    58263 2024-01-29 21:13:26.000000 technote-0.7.0a1/src/technote/theme/static/styles/technote.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-01-29 21:13:14.000000 technote-0.7.0a1/src/technote/theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/src/technote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-01-29 21:13:35.000000 technote-0.7.0a1/src/technote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-01-29 21:13:35.000000 technote-0.7.0a1/src/technote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:13:35.000000 technote-0.7.0a1/src/technote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-01-29 21:13:35.000000 technote-0.7.0a1/src/technote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-29 21:13:35.000000 technote-0.7.0a1/src/technote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-29 21:13:35.000000 technote-0.7.0a1/src/technote.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.675463 technote-0.7.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.675463 technote-0.7.0a1/tests/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/ext/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/ext/toc_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/metadata/orcid_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/metadata/ror_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/metadata/spdx_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/packaging_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.655462 technote-0.7.0a1/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/roots/test-abstract-basic/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-abstract-basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-abstract-basic/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-abstract-basic/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/roots/test-metadata-basic/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-metadata-basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-metadata-basic/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-metadata-basic/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/roots/test-toc-basic/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-toc-basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-toc-basic/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-toc-basic/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/roots/test-toc-no-sections/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-toc-no-sections/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-toc-no-sections/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/roots/test-toc-no-sections/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/sources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/sources/tomlsettings_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:35.679463 technote-0.7.0a1/tests/templating/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-29 21:13:14.000000 technote-0.7.0a1/tests/templating/context_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-29 21:13:14.000000 technote-0.7.0a1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-29 21:13:14.000000 technote-0.7.0a1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.996261 technote-0.8.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 18:49:38.000000 technote-0.8.0a1/.github/CODE_OF_CONDUCT
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 18:49:38.000000 technote-0.8.0a1/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-02 18:49:38.000000 technote-0.8.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-02 18:49:38.000000 technote-0.8.0a1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-02 18:49:38.000000 technote-0.8.0a1/.github/workflows/dependencies.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-02 18:49:38.000000 technote-0.8.0a1/.github/workflows/periodic-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-02 18:49:38.000000 technote-0.8.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 18:49:38.000000 technote-0.8.0a1/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-02 18:49:38.000000 technote-0.8.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-02 18:49:38.000000 technote-0.8.0a1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 18:49:38.000000 technote-0.8.0a1/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-02 18:49:38.000000 technote-0.8.0a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-02 18:49:38.000000 technote-0.8.0a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-02 18:49:38.000000 technote-0.8.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-02 18:49:38.000000 technote-0.8.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 18:49:38.000000 technote-0.8.0a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-02 18:50:03.996261 technote-0.8.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-02 18:49:38.000000 technote-0.8.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-02 18:49:38.000000 technote-0.8.0a1/changelog.d/20240501_170745_jsick_DM_43638.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-02 18:49:38.000000 technote-0.8.0a1/changelog.d/_template.md.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.968261 technote-0.8.0a1/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/demo/md/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/demo/md/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/_static/technote-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/_static/technote-logo-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)   199011 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/rubin-watermark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/md/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.976261 technote-0.8.0a1/demo/rst/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.980261 technote-0.8.0a1/demo/rst/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/_static/technote-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/_static/technote-logo-light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19285 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   199011 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/rubin-watermark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-02 18:49:38.000000 technote-0.8.0a1/demo/rst/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.980261 technote-0.8.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.980261 technote-0.8.0a1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/documenteer.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.980261 technote-0.8.0a1/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/configuration-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/configure-authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/configure-sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/configure-status.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/technote-toml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs/user-guide/theming-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-02 18:49:38.000000 technote-0.8.0a1/docs-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   198626 2024-05-02 18:49:47.000000 technote-0.8.0a1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-02 18:49:38.000000 technote-0.8.0a1/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 18:49:38.000000 technote-0.8.0a1/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7278 2024-05-02 18:49:38.000000 technote-0.8.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:50:03.996261 technote-0.8.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.968261 technote-0.8.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.984261 technote-0.8.0a1/src/technote/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.984261 technote-0.8.0a1/src/technote/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/insertposttitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/pygmentscss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.984261 technote-0.8.0a1/src/technote/ext/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/templates/post-title.html.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/toc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/ext/wraptables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.984261 technote-0.8.0a1/src/technote/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   218216 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/orcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/ror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/spdx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/metadata/zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.984261 technote-0.8.0a1/src/technote/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13318 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/sources/tomlsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/sphinxconf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.988261 technote-0.8.0a1/src/technote/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7064 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/templating/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/templating/highwire.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/templating/metatagbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/templating/opengraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.988261 technote-0.8.0a1/src/technote/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.988261 technote-0.8.0a1/src/technote/theme/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/sidebar-authors.html
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/sidebar-logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/sidebar-source.html
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/sidebar-toc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/sidebar-version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/toggle-sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/components/toggle-sidebar-secondary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.988261 technote-0.8.0a1/src/technote/theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/partials/octicons.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/src/technote/theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/announcement.html
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/article.html
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/footer-article.html
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/footer-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/header-content.html
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/header-secondary.html
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/sections/sidebar-secondary.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/src/technote/theme/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/static/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/src/technote/theme/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-05-02 18:49:49.000000 technote-0.8.0a1/src/technote/theme/static/scripts/technote.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/src/technote/theme/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)    25631 2024-05-02 18:49:49.000000 technote-0.8.0a1/src/technote/theme/static/styles/technote.css
+-rw-r--r--   0 runner    (1001) docker     (127)    59679 2024-05-02 18:49:49.000000 technote-0.8.0a1/src/technote/theme/static/styles/technote.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-02 18:49:38.000000 technote-0.8.0a1/src/technote/theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.996261 technote-0.8.0a1/src/technote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-05-02 18:50:03.000000 technote-0.8.0a1/src/technote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-02 18:50:03.000000 technote-0.8.0a1/src/technote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:50:03.000000 technote-0.8.0a1/src/technote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 18:50:03.000000 technote-0.8.0a1/src/technote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 18:50:03.000000 technote-0.8.0a1/src/technote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-02 18:50:03.000000 technote-0.8.0a1/src/technote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/tests/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/ext/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/ext/toc_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/tests/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/metadata/orcid_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/metadata/ror_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/metadata/spdx_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/packaging_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.972261 technote-0.8.0a1/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/tests/roots/test-abstract-basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-abstract-basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-abstract-basic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-abstract-basic/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.992261 technote-0.8.0a1/tests/roots/test-metadata-basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-metadata-basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-metadata-basic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-metadata-basic/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.996261 technote-0.8.0a1/tests/roots/test-toc-basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-toc-basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-toc-basic/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-toc-basic/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.996261 technote-0.8.0a1/tests/roots/test-toc-no-sections/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-toc-no-sections/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-toc-no-sections/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/roots/test-toc-no-sections/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.996261 technote-0.8.0a1/tests/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/sources/tomlsettings_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:50:03.996261 technote-0.8.0a1/tests/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-02 18:49:38.000000 technote-0.8.0a1/tests/templating/context_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-02 18:49:38.000000 technote-0.8.0a1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-02 18:49:38.000000 technote-0.8.0a1/webpack.config.js
```

### Comparing `technote-0.7.0a1/.github/CONTRIBUTING.md` & `technote-0.8.0a1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/.github/workflows/ci.yaml` & `technote-0.8.0a1/.github/workflows/ci.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 jobs:
   lint:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          python-version: '3.11'
+          python-version: '3.12'
 
       - name: Run pre-commit
-        uses: pre-commit/action@v3.0.0
+        uses: pre-commit/action@v3.0.1
 
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python:
           - '3.11'
+          - '3.12'
 
     steps:
       - uses: actions/checkout@v4
 
       - uses: actions/setup-node@v4
         with:
           cache: 'npm'
@@ -78,15 +79,15 @@
         run: |
           npm install
           npm run build
 
       - name: Run tox
         uses: lsst-sqre/run-tox@v1
         with:
-          python-version: '3.11'
+          python-version: '3.12'
           tox-envs: 'demo,docs'
           # tox-envs: "docs,docs-linkcheck"
 
       # Only attempt documentation uploads for tagged releases and pull
       # requests from ticket branches in the same repository.  This avoids
       # version clutter in the docs and failures when a PR doesn't have access
       # to secrets.
@@ -109,15 +110,15 @@
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
       - name: Build and publish
         uses: lsst-sqre/build-and-publish-to-pypi@v2
         with:
-          python-version: '3.11'
+          python-version: '3.12'
           upload: false
 
   pypi:
     # This job requires set up:
     # 1. Set up a trusted publisher for PyPI
     # 2. Set up a "pypi" environment in the repository
     # See https://github.com/lsst-sqre/build-and-publish-to-pypi
@@ -145,8 +146,8 @@
         run: |
           npm install
           npm run build
 
       - name: Build and publish
         uses: lsst-sqre/build-and-publish-to-pypi@v2
         with:
-          python-version: '3.11'
+          python-version: '3.12'
```

### Comparing `technote-0.7.0a1/.github/workflows/dependencies.yaml` & `technote-0.8.0a1/.github/workflows/dependencies.yaml`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/.github/workflows/periodic-ci.yaml` & `technote-0.8.0a1/.github/workflows/periodic-ci.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
   test:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
         python:
           - '3.11'
+          - '3.12'
 
     steps:
       - uses: actions/checkout@v4
 
       - uses: actions/setup-node@v4
         with:
           cache: 'npm'
@@ -42,15 +43,15 @@
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Build docs in tox
         uses: lsst-sqre/run-tox@v1
         with:
-          python-version: '3.11'
+          python-version: '3.12'
           tox-envs: 'demo,docs,docs-linkcheck'
           use-cache: false
 
   test-packaging:
     name: Test packaging
     runs-on: ubuntu-latest
 
@@ -58,9 +59,9 @@
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0 # full history for setuptools_scm
 
       - name: Build and publish
         uses: lsst-sqre/build-and-publish-to-pypi@v2
         with:
-          python-version: '3.11'
+          python-version: '3.12'
           upload: false
```

### Comparing `technote-0.7.0a1/.gitignore` & `technote-0.8.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/.pre-commit-config.yaml` & `technote-0.8.0a1/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: check-yaml
       - id: check-toml
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.1.0
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.278
+    rev: v0.4.2
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.11.0
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.16.0
     hooks:
       - id: blacken-docs
```

### Comparing `technote-0.7.0a1/.vscode/tasks.json` & `technote-0.8.0a1/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/CHANGELOG.md` & `technote-0.8.0a1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Change log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-0.7.0'></a>
+## 0.7.0 (2024-01-30)
+
+### New features
+
+- When the `technote.date_updated` field in `technote.toml` is not set, the update date internally defaults to "now" (the build time). This ensures that documents always carry some form of metadata about when they were modified.
+
+- Code samples without captions (unwrapped `.highlight` divs) now have borders and are protected against x-overflow. This matches the behavior of code samples with captions.
+- All code samples have negative left margin equal to their content padding so that the code lines up with the text column.
+- The content (`div.sb-container`) now has bottom margin to give content breathing room.
+
 <a id='changelog-0.6.2'></a>
 ## 0.6.2 (2023-12-14)
 
 ### Bug fixes
 
 - Fix the `technote.ext.pygmentsscss` extension to handle cases where the HTML builder isn't being run.
```

### Comparing `technote-0.7.0a1/LICENSE` & `technote-0.8.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/PKG-INFO` & `technote-0.8.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: technote
-Version: 0.7.0a1
+Version: 0.8.0a1
 Summary: Rubin Observatory's framework for Sphinx-based technote documents.
 License: MIT License
         
         Copyright (c) 2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,19 +46,20 @@
 Requires-Dist: beautifulsoup4
 Requires-Dist: pygments
 Requires-Dist: accessible-pygments
 Requires-Dist: myst-parser
 Requires-Dist: markdown-it-py[linkify]
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest<8.0; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-docutils; extra == "dev"
+Requires-Dist: defusedxml; extra == "dev"
 Requires-Dist: lxml; extra == "dev"
 Requires-Dist: cssselect; extra == "dev"
 Requires-Dist: mf2py; extra == "dev"
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10385500.svg)](https://doi.org/10.5281/zenodo.10385500)
 [![Python CI](https://github.com/lsst-sqre/technote/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/technote/actions/workflows/ci.yaml)
```

### Comparing `technote-0.7.0a1/README.md` & `technote-0.8.0a1/README.md`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/md/_static/technote-logo-dark.svg` & `technote-0.8.0a1/demo/md/_static/technote-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/md/_static/technote-logo-light.svg` & `technote-0.8.0a1/demo/md/_static/technote-logo-light.svg`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/md/rubin-watermark.png` & `technote-0.8.0a1/demo/md/rubin-watermark.png`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/md/technote.toml` & `technote-0.8.0a1/demo/md/technote.toml`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/rst/_static/technote-logo-dark.svg` & `technote-0.8.0a1/demo/rst/_static/technote-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/rst/_static/technote-logo-light.svg` & `technote-0.8.0a1/demo/rst/_static/technote-logo-light.svg`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/rst/index.rst` & `technote-0.8.0a1/demo/rst/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,16 @@
    :caption: hello.py
 
    print("Hello world")
 
 Code cells
 ==========
 
+Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin facilisis pharetra neque, at semper nulla mattis auctor. ``inline code`` to test line height behaviour. Proin ``hello world`` facilisis pharetra neque, at semper nulla mattis auctor. `pathlib.Path`. Proin facilisis pharetra neque, at semper nulla mattis auctor.
+
 This is a long code cell:
 
 .. code-block:: Makefile
    :caption: Makefile
 
    .PHONY: update-deps
    update-deps:
@@ -90,14 +92,36 @@
    .PHONY: update
    update: update-deps init
 
    .PHONY: run
    run:
    	cd server && tox run -e=run
 
+A code cell without a caption:
+
+.. code-block:: python
+
+   print("Hello world")
+
+A code sample with no language set::
+
+   Hello world
+
+A wide code sample with no caption:
+
+.. code-block:: Makefile
+
+   .PHONY: update-deps
+   update-deps:
+   	pip install --upgrade pip-tools pip setuptools
+   	pip-compile --upgrade --build-isolation --generate-hashes --output-file server/requirements/main.hashed.txt server/requirements/main.in
+   	pip-compile --upgrade --build-isolation --generate-hashes --output-file server/requirements/dev.hashed.txt server/requirements/dev.in
+   	pip-compile --upgrade --build-isolation --allow-unsafe --output-file server/requirements/main.txt server/requirements/main.in
+   	pip-compile --upgrade --build-isolation --allow-unsafe --output-file server/requirements/dev.txt server/requirements/dev.in
+
 Admonitions
 ===========
 
 Some content.
 
 .. attention::
```

### Comparing `technote-0.7.0a1/demo/rst/rubin-watermark.png` & `technote-0.8.0a1/demo/rst/rubin-watermark.png`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/demo/rst/technote.toml` & `technote-0.8.0a1/demo/rst/technote.toml`

 * *Files 18% similar despite different names*

```diff
@@ -24,7 +24,10 @@
 
 [[technote.status.supersceding_urls]]
 url = "https://sqr-000.lsst.io/"
 title = "The technical note system"
 
 [[technote.status.supersceding_urls]]
 url = "https://sqr-006.lsst.io/"
+
+[technote.sphinx.intersphinx.projects]
+python = "https://docs.python.org/3/"
```

### Comparing `technote-0.7.0a1/docs/_rst_epilog.rst` & `technote-0.8.0a1/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/api.rst` & `technote-0.8.0a1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/changelog.md` & `technote-0.8.0a1/docs/changelog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Change log
 
 <!-- scriv-insert-here -->
 
+<a id='changelog-0.7.0'></a>
+## 0.7.0 (2024-01-30)
+
+### New features
+
+- When the `technote.date_updated` field in `technote.toml` is not set, the update date internally defaults to "now" (the build time). This ensures that documents always carry some form of metadata about when they were modified.
+
+- Code samples without captions (unwrapped `.highlight` divs) now have borders and are protected against x-overflow. This matches the behavior of code samples with captions.
+- All code samples have negative left margin equal to their content padding so that the code lines up with the text column.
+- The content (`div.sb-container`) now has bottom margin to give content breathing room.
+
 <a id='changelog-0.6.2'></a>
 ## 0.6.2 (2023-12-14)
 
 ### Bug fixes
 
 - Fix the `technote.ext.pygmentsscss` extension to handle cases where the HTML builder isn't being run.
```

### Comparing `technote-0.7.0a1/docs/dev/development.rst` & `technote-0.8.0a1/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/dev/release.rst` & `technote-0.8.0a1/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/documenteer.toml` & `technote-0.8.0a1/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/index.rst` & `technote-0.8.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/user-guide/configuration-overview.rst` & `technote-0.8.0a1/docs/user-guide/configuration-overview.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/user-guide/configure-authors.rst` & `technote-0.8.0a1/docs/user-guide/configure-authors.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/user-guide/configure-sphinx.rst` & `technote-0.8.0a1/docs/user-guide/configure-sphinx.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 Intersphinx_ is a built-in Sphinx extension that helps you link to other sphinx projects (including other technotes and many Python project documentation sites including `docs.astropy.org <https://docs.astropy.org/en/stable/>`__ and `docs.python.org <https://docs.python.org/3/>`__.)
 
 To add a site to the Intersphinx_ configuration, add items to the ``[technote.sphinx.intersphinx]`` table:
 
 .. code-block:: toml
    :caption: technote.toml
 
-   [technote.sphinx.intersphinx]
+   [technote.sphinx.intersphinx.projects]
    astropy = "https://docs.astropy.org/en/stable/"
    python = "https://docs.python.org/3/"
 
 Keys are the names of projects, and also become prefixes for ``ref`` directives to that project.
 
 For information on using Intersphinx_ to make cross-project links, see the `Sphinx documentation <https://www.sphinx-doc.org/en/master/usage/extensions/intersphinx.html>`__.
```

### Comparing `technote-0.7.0a1/docs/user-guide/configure-status.rst` & `technote-0.8.0a1/docs/user-guide/configure-status.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/user-guide/metadata.rst` & `technote-0.8.0a1/docs/user-guide/metadata.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/user-guide/technote-toml.rst` & `technote-0.8.0a1/docs/user-guide/technote-toml.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/docs/user-guide/theming-overview.rst` & `technote-0.8.0a1/docs/user-guide/theming-overview.rst`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/package-lock.json` & `technote-0.8.0a1/package-lock.json`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/pyproject.toml` & `technote-0.8.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,20 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     # Testing
     "coverage[toml]",
-    "pytest",
+    "pytest<8.0",
     "pytest-asyncio",
     "pre-commit",
     "mypy",
     "types-docutils",
+    "defusedxml", # used by Sphinx, but not a direct dependency
     # Test depedendencies for analyzing HTML output
     "lxml",
     "cssselect",
     "mf2py",
 ]
 
 [project.urls]
```

### Comparing `technote-0.7.0a1/src/technote/__init__.py` & `technote-0.8.0a1/src/technote/__init__.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/__init__.py` & `technote-0.8.0a1/src/technote/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/abstract.py` & `technote-0.8.0a1/src/technote/ext/abstract.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/insertposttitle.py` & `technote-0.8.0a1/src/technote/ext/insertposttitle.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/metadata.py` & `technote-0.8.0a1/src/technote/ext/metadata.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/pygmentscss.py` & `technote-0.8.0a1/src/technote/ext/pygmentscss.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/templates/post-title.html.jinja` & `technote-0.8.0a1/src/technote/ext/templates/post-title.html.jinja`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/toc.py` & `technote-0.8.0a1/src/technote/ext/toc.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/ext/wraptables.py` & `technote-0.8.0a1/src/technote/ext/wraptables.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/factory.py` & `technote-0.8.0a1/src/technote/factory.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/main.py` & `technote-0.8.0a1/src/technote/main.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/metadata/licenses.json` & `technote-0.8.0a1/src/technote/metadata/licenses.json`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/metadata/model.py` & `technote-0.8.0a1/src/technote/metadata/model.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/metadata/orcid.py` & `technote-0.8.0a1/src/technote/metadata/orcid.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/metadata/ror.py` & `technote-0.8.0a1/src/technote/metadata/ror.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/metadata/spdx.py` & `technote-0.8.0a1/src/technote/metadata/spdx.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/metadata/zenodo.py` & `technote-0.8.0a1/src/technote/metadata/zenodo.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/sources/tomlsettings.py` & `technote-0.8.0a1/src/technote/sources/tomlsettings.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/sphinxconf.py` & `technote-0.8.0a1/src/technote/sphinxconf.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/templating/context.py` & `technote-0.8.0a1/src/technote/templating/context.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/templating/highwire.py` & `technote-0.8.0a1/src/technote/templating/highwire.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/templating/metatagbase.py` & `technote-0.8.0a1/src/technote/templating/metatagbase.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/templating/opengraph.py` & `technote-0.8.0a1/src/technote/templating/opengraph.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/components/sidebar-authors.html` & `technote-0.8.0a1/src/technote/theme/components/sidebar-authors.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/components/sidebar-source.html` & `technote-0.8.0a1/src/technote/theme/components/sidebar-source.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/components/sidebar-version.html` & `technote-0.8.0a1/src/technote/theme/components/sidebar-version.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/components/toggle-sidebar-primary.html` & `technote-0.8.0a1/src/technote/theme/components/toggle-sidebar-primary.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/components/toggle-sidebar-secondary.html` & `technote-0.8.0a1/src/technote/theme/components/toggle-sidebar-secondary.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/page.html` & `technote-0.8.0a1/src/technote/theme/page.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/partials/octicons.html` & `technote-0.8.0a1/src/technote/theme/partials/octicons.html`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/static/scripts/technote.js` & `technote-0.8.0a1/src/technote/theme/static/scripts/technote.js`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/src/technote/theme/static/styles/technote.css` & `technote-0.8.0a1/src/technote/theme/static/styles/technote.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 /*!********************************************************************************************************************************************************************************************************************************************************!*\
   !*** css ./node_modules/css-loader/dist/cjs.js??ruleSet[1].rules[0].use[1]!./node_modules/postcss-loader/dist/cjs.js??ruleSet[1].rules[0].use[2]!./node_modules/sass-loader/dist/cjs.js??ruleSet[1].rules[0].use[3]!./src/assets/styles/technote.scss ***!
   \********************************************************************************************************************************************************************************************************************************************************/
 html {
   box-sizing: border-box;
+  /*
+   * Maintain the user's default font size. Rems are relative to this.
+   */
+  font-size: 100%;
 }
 
 /*
  * Inherit border-box sizing from html
  * https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/
  */
 *,
 *:before,
 *:after {
   box-sizing: inherit;
 }
 
 :root {
   /*
-   * Reinforce that we're respecting the user's ability to set a default
-   * font size. The rem unit now becomes relative to this.
-   * Flexible Typesetting, Tim Brown, ch 2 and 4
-   */
-  font-size: 1.1rem;
-}
-
-:root {
-  /*
    * Color design tokens.
    *
    * These are based on GitHub Primer.
    * https://primer.style/prism/local/a4751264-de23-430e-a2fc-669488065638/scale/c2a0938a-e1dc-4b20-a07b-e2778ae57f41
    */
   --tn-color-black: #1b1f24;
   --tn-color-white: #ffffff;
@@ -179,29 +174,31 @@
   /*
    * Typographic design tokens.
    */
   --tn-component-h1-size: 3.052rem;
   --tn-component-h2-size: 2.441rem;
   --tn-component-h3-size: 1.563rem;
   --tn-component-h4-size: 1.25rem;
-  --tn-component-h5-size: 1rem;
-  --tn-component-h6-size: 0.8rem;
+  --tn-component-h5-size: 1.1rem;
+  --tn-component-h6-size: 1rem;
   --tn-component-h1-weight: normal;
   --tn-component-h2-weight: normal;
   --tn-component-h3-weight: bold;
   --tn-component-h4-weight: bold;
   --tn-component-h5-weight: bold;
   --tn-component-h6-weight: bold;
+  --tn-component-text-font-size: 1.1rem;
   --tn-component-text-color: var(--tn-color-black);
   --tn-component-link-color: var(--tn-color-blue-500);
   --tn-component-text-background-color: var(--tn-color-white);
-  --tn-component-text-font-family: -apple-system, BlinkMacSystemFont, Segoe UI,
-    Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue,
-    sans-serif;
+  --tn-component-text-font-family: -apple-system, ui-sans-serif,
+    BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans,
+    Droid Sans, Helvetica Neue, sans-serif;
   --tn-component-text-line-height: 1.5;
+  --tn-component-code-font-family: ui-monospace, monospace;
 }
 
 html[data-theme=dark] {
   --tn-component-text-color: var(--tn-color-white);
   --tn-component-link-color: var(--tn-color-blue-300);
   --tn-component-text-background-color: var(--tn-color-black);
 }
@@ -230,14 +227,15 @@
 /*
  * Styles that affect the overall layout. Since Technote is built on
  * sphinx-basic-ng as the base theme, these styles primarily work with
  * the base theme's sb- classes.
  */
 .sb-container {
   margin-top: var(--tn-space-md-fixed);
+  margin-bottom: var(--tn-space-xxl-fixed);
 }
 
 /* Style the prmary sidebar when it's a popover. */
 #sb-sidebar-toggle--primary:checked ~ .sb-container .sb-sidebar-primary {
   background-color: white;
   box-shadow: 10px 5px 5px rgb(161, 161, 161);
   border-right: 1px solid black;
@@ -279,153 +277,153 @@
 .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
   /* reset skeleton.css. Using 100vw means we get horizontal scrollbars. */
   width: auto;
 }
 
-@media (max-width: 42rem) {
+@media (max-width: 42em) {
   .sb-article-container,
 .sb-footer-content__inner {
     width: 100vw;
   }
   body {
     -webkit-hyphens: auto;
             hyphens: auto;
   }
 }
-@media (min-width: 42rem) {
+@media (min-width: 42em) {
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 38rem;
+    width: 38em;
   }
   .sb-article,
 .match-content-width {
-    width: 38rem;
+    width: 38em;
   }
 }
-@media (min-width: 46rem) {
+@media (min-width: 46em) {
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-article,
 .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
 }
-@media (min-width: 50rem) {
+@media (min-width: 50em) {
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-article,
 .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   /* h1::after {
     content: ' 50';
   } */
 }
-@media (min-width: 59rem) {
+@media (min-width: 59em) {
   /* secondary sidebar appears, width is 17rem. */
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-article,
 .match-content-width {
-    width: 36rem;
+    width: 36em;
   }
   /* h1::after {
     content: ' 59';
   } */
 }
-@media (min-width: 63rem) {
+@media (min-width: 63em) {
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-article,
 .match-content-width {
-    width: 36rem;
+    width: 36em;
   }
   /* h1::after {
     content: ' 63';
   } */
 }
-@media (min-width: 67rem) {
+@media (min-width: 67em) {
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-article,
 .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   /* h1::after {
     content: ' 67';
   } */
 }
-@media (min-width: 76rem) {
+@media (min-width: 76em) {
   /* The primary sidebar appears */
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-article,
 .match-content-width {
-    width: 32rem;
+    width: 32em;
   }
   .sb-sidebar-primary {
     box-shadow: none;
     border-right: none;
   }
   /* h1::after {
     content: ' 76';
   } */
 }
-@media (min-width: 80rem) {
+@media (min-width: 80em) {
   .sb-article,
 .match-content-width {
-    width: 34rem;
+    width: 34em;
   }
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   /* h1::after {
     content: ' 80';
   } */
 }
-@media (min-width: 84rem) {
+@media (min-width: 84em) {
   .sb-article,
 .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   /* h1::after {
     content: ' 84';
   } */
 }
-@media (min-width: 88rem) {
+@media (min-width: 88em) {
   .sb-footer-content__inner,
 .drop-secondary-sidebar-for-full-width-content .sb-article,
 .drop-secondary-sidebar-for-full-width-content .match-content-width {
-    width: 40rem;
+    width: 40em;
   }
   .sb-page-width {
-    width: 86rem;
+    width: 86em;
   }
   /* h1::after {
     content: ' 88';
   } */
 }
 /*
  * Primary sidebar
@@ -436,14 +434,15 @@
 
 /*
  * Typography.
  */
 body {
   font-family: var(--tn-component-text-font-family);
   line-height: var(--tn-component-text-line-height);
+  font-size: var(--tn-component-text-font-size);
   color: var(--tn-component-text-color);
   background: var(--tn-component-text-background-color);
 }
 
 h1,
 h2,
 h3,
@@ -506,14 +505,33 @@
   visibility: visible;
 }
 
 a {
   color: var(--tn-component-link-color);
 }
 
+pre,
+xmp,
+plaintext,
+listing {
+  font-family: var(--tn-component-code-font-family);
+  font-size: 1rem;
+}
+
+tt,
+code,
+kbd,
+samp {
+  font-family: var(--tn-component-code-font-family);
+  /* Making inline code slightly smaller seems to help with baseline alignment
+   * some monospace fonts seems bigger that Source Sans.
+   */
+  font-size: 0.9em;
+}
+
 /* Styles Sphinx-generated content classes */
 a.headerlink {
   opacity: 0;
   font-size: 0.9em;
   margin-left: var(--tn-space-xxs);
   text-decoration: none;
   transition: all 0.2s ease-out;
@@ -532,38 +550,40 @@
   opacity: 0.5;
 }
 
 a.headerlink:hover {
   opacity: 1;
 }
 
-pre {
-  font-size: 0.85rem;
-}
-
-.literal-block-wrapper .highlight pre {
+.highlight {
   margin: 0;
+  margin-left: calc(-1 * var(--tn-space-xs-fixed));
   padding: var(--tn-space-xs-fixed);
   overflow-x: auto;
+  border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);
+  border-radius: var(--tn-sphinx-code-block-border-radius);
 }
 
 .literal-block-wrapper {
+  margin-left: calc(-1 * var(--tn-space-xs-fixed));
+  padding-left: var(--tn-space-xs-fixed);
   border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);
   border-radius: var(--tn-sphinx-code-block-border-radius);
 }
 
 .literal-block-wrapper .highlight {
-  border-radius: 0 0 var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius);
+  border: none;
 }
 
 .code-block-caption {
   background-color: var(--tn-sphinx-code-block-caption-background-color);
   border-bottom: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);
   border-radius: var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius) 0 0;
   padding: var(--tn-space-xxxs-fixed) var(--tn-space-xs-fixed);
+  margin-left: calc(-1 * var(--tn-space-xs-fixed));
 }
 
 .admonition {
   border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);
   border-radius: var(--tn-sphinx-code-block-border-radius);
   padding: var(--tn-space-xs-fixed);
   margin-bottom: 1rem;
```

### Comparing `technote-0.7.0a1/src/technote/theme/static/styles/technote.css.map` & `technote-0.8.0a1/src/technote/theme/static/styles/technote.css.map`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8968253968253969%*

 * *Differences: {"'mappings'": "';;;AAAA;EACE;EAEA;;IAAA;EAGA;ACAF;;ADGA;;;EAAA;AAIA;;;EAGE;ACAF;;AChBA;EACE;;;;;IAAA;EAMA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA; […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "styles/technote.css",
-    "mappings": ";;;AAAA;EACE;ACCF;;ADEA;;;EAAA;AAIA;;;EAGE;ACCF;;ADEA;EACE;;;;IAAA;EAKA;ACCF;;ACrBA;EACE;;;;;IAAA;EAMA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAGA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;ADaF;;AErIA;EACE;;IAAA;EAGA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;;;KAAA;EAIA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;AFuIF;;AGnKA;EACE;;IAAA;EAGA;EACA;EACA;AHsKF;;AI5KA;EACE;;IAAA;EAGA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EAEA;;cAAA;EAGA;AJ4KF;;AIzKA;EACE;EACA;EACA;AJ4KF;;AK3MA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;AL6MF;;AK1MA;EACE;EACA;EACA;EACA;EACA;EACA;AL6MF;;AMhOA;;;;EAAA;AAMA;EACE;ANkOF;;AM/NA;AACA;EACE;EACA;EACA;ANkOF;;AM/NA;EACE;EACA;EACA;EACA;ANkOF;;AM/NA;EACE;ANkOF;;AM/NA;EAEE;UAAA;EACA;ANiOF;;AM7NA;EACE;EACA;ANgOF;;AM7NA;EACE;ANgOF;;AM7NA;AAWA;;;;EAAA;AAKA;;;;EAIE;EACA;ANsNF;;AMnNA;EACE;;IAEE;ENsNF;EMnNA;IAEE;YAAA;ENoNF;AACF;AMjNA;EACE;;;IAGE;ENmNF;EMjNA;;IAEE;ENmNF;AACF;AM9MA;EACE;;;IAGE;ENgNF;EM9MA;;IAEE;ENgNF;AACF;AM3MA;EACE;;;IAGE;EN6MF;EM3MA;;IAEE;EN6MF;EM3MA;;KAAA;AN+MF;AM3MA;EACE;EACA;;;IAGE;EN6MF;EM3MA;;IAEE;EN6MF;EM3MA;;KAAA;AN+MF;AM3MA;EACE;;;IAGE;EN6MF;EM3MA;;IAEE;EN6MF;EM3MA;;KAAA;AN+MF;AM3MA;EACE;;;IAGE;EN6MF;EM3MA;;IAEE;EN6MF;EM3MA;;KAAA;AN+MF;AM3MA;EACE;EACA;;;IAGE;EN6MF;EM3MA;;IAEE;EN6MF;EMzMA;IACE;IACA;EN2MF;EMzMA;;KAAA;AN6MF;AMzMA;EACE;;IAEE;EN2MF;EMzMA;;;IAGE;EN2MF;EMzMA;;KAAA;AN6MF;AMzMA;EACE;;IAEE;EN2MF;EMzMA;;KAAA;AN6MF;AMzMA;EACE;;;IAGE;EN2MF;EMzMA;IACE;EN2MF;EMzMA;;KAAA;AN6MF;AMxMA;;EAAA;AAGA;EACE;AN0MF;;AO7aA;;EAAA;AAGA;EACE;EACA;EACA;EACA;APgbF;;AO7aA;;;;;;EAME;EACA;EACA;APgbF;;AO7aA;EACE;EACA;EACA;APgbF;;AO7aA;EACE;EACA;APgbF;;AO7aA;EACE;EACA;APgbF;;AO7aA;EACE;EACA;APgbF;;AO7aA;EACE;EACA;APgbF;;AO7aA;EACE;EACA;APgbF;;AO7aA;AACA;;;;;;EAME;EACA;APgbF;;AO9aA;;;;;;EAME;APibF;;AO9aA;EACE;APibF;;AQzfA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;KAAA;UAAA;AR2fF;;AQxfA;;;;;;;EASE;ARyfF;;AQtfA;EACE;ARyfF;;AQtfA;EACE;ARyfF;;AQtfA;EACE;EACA;EACA;ARyfF;;AQtfA;EACE;EAEA;ARwfF;;AQrfA;EAGE;ARsfF;;AQlfA;EACE;EACA;EAEA;EAEA;ARmfF;;AQhfA;EACE;EAEA;EACA;EACA;ARkfF;;AQ/eA;EACE;ARkfF;;AQ/eA;EACE;EACA;EACA;EACA;EAEA;ARifF;;AQ9eA;;;;EAIE;ARifF;;AQ9eA;;;;EAIE;ARifF;;AQ9eA;;EAEE;ARifF;;AQ9eA;;EAEE;ARifF;;AQ9eA;;;EAGE;ARifF;;AQ9eA;;;EAGE;ARifF;;AQ9eA;EACE;EACA;EACA;EACA;EACA;ARifF;;AQ9eA;EACE;EACA;ARifF;;AQ9eA;;EAEE;EACA;EACA;EACA;EACA;EACA;ARifF;;AQ9eA;;EAEE;EACA;ARifF;;AQ9eA;;EAEE;ARifF;;AQ9eA;EAEE;ARgfF;;AQ7eA;EACE;EACA;ARgfF;;AQ7eA;EACE;ARgfF;;AQ7eA;EACE;EACA;EACA;ARgfF;;AQ7eA;EACE;ARgfF;;AQ7eA;EACE;EACA;ARgfF;;AQ7eA;EACE;EACA;ARgfF;;AQ7eA;EACE;ARgfF;;AQ7eA;EACE;ARgfF;;AQ7eA;EACE;ARgfF;;AQ5eA;EACE;AR+eF;;AQ5eA;EACE;EACA;AR+eF;;AQ5eA;EACE;AR+eF;;AQ5eA;EACE;EACA;EACA;EACA;EACA;EACA;AR+eF;;AQ3eA;EACE;EACA;EACA;AR8eF;;AQ3eA;EACE;AR8eF;;AQreA;EACE;EACA;ARweF;;AQreA;EACE;EAAA;EACA;EACA;EAEA;EACA;EACA;ARueF;;AQpeA;EACE;ARueF;;AQpeA;EACE;ARueF;;AQpeA;;EAEE;EACA;EACA;ARueF;;AQpeA;EAEE;ARseF;;AQneA;EACE;ARseF;;AStvBA;EACE;EACA;ATyvBF;;AU3vBA;;;;EAAA;AAMA;EACE;EACA;EACA;EACA;EACA;AV6vBF;;AU1vBA;EACE;EACA;EACA;EACA;AV6vBF;;AU1vBA;EACE;EACA;AV6vBF;;AWpxBA;;EAAA;AAIA;EACE;AXsxBF;;AY3xBA;AAEA;EACE;IAGE;IACA;IAGA;IACA;EZyxBF;AACF;AaryBA;EACE;AbuyBF;;AapyBA;EACE;AbuyBF;;AapyBA;EACE;AbuyBF;;AapyBA;EAGE;AbqyBF;;AalyBA;EACE;EACA;EACA;EACA;AbqyBF;;AalyBA;EACE;AbqyBF;;AalyBA;EACE;AbqyBF;;AalyBA;EACE;EACA;EACA;EACA;AbqyBF;;Ac10BA;;EAAA;AAIA;EACE;Ad40BF;;Aej1BA;AAEA;EACE;EACA;EACA;Afm1BF;;Aeh1BA;EACE;Afm1BF;;Aeh1BA;EACE;Afm1BF;;Aeh1BA;EACE;Afm1BF;;AgBp2BA;EACE;EACA;EACA;EACA;AhBu2BF;;AgBp2BA;EAEE;AhBs2BF;;AiB/2BA;;EAAA;AAIA;EACE;EACA;AjBi3BF;;AiB92BA;EACE;EACA;AjBi3BF;;AiB92BA;EAEE;EACA;AjBg3BF;;AiB72BA;EAEE;IAEE;IACA;IAIA;IAGA;EjBy2BF;AACF;AiBt2BA;EACE;EACA;EACA;EACA;AjBw2BF;;AiBr2BA;EACE;EACA;EACA;AjBw2BF;;AiBr2BA;EACE;AjBw2BF;;AiBr2BA;EACE;AjBw2BF;;AiBr2BA;EACE;EACA;EACA;EACA;EACA;AjBw2BF;;AiBr2BA;AACA;EACE;EACA;EACA;EACA;AjBw2BF;;AiBr2BA;EACE;AjBw2BF;;AkBl7BA;;EAAA;AAIA;EACE;AlBo7BF;;AkBj7BA;EACE;AlBo7BF;;AmB37BA;EACE;EACA;EACA;AnB87BF;;AmB37BA;;;EAAA;AAIA;EACE;EACA;EACA;AnB87BF;;AmB37BA;EACE;AnB87BF;;AmB37BA;EACE;AnB87BF;;AmB37BA;EACE;AnB87BF;;AmB37BA;EACE;AnB87BF;;AmB37BA;EACE;AnB87BF;;AmB37BA;;;;EAAA;AAKA;EACE;EACA;UAAA;EACA;EACA;EACA;EACA;EACA;AnB87BF,C",
+    "mappings": ";;;AAAA;EACE;EAEA;;IAAA;EAGA;ACAF;;ADGA;;;EAAA;AAIA;;;EAGE;ACAF;;AChBA;EACE;;;;;IAAA;EAMA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAGA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;ADQF;;AEhIA;EACE;;IAAA;EAGA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;;;KAAA;EAIA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;AFkIF;;AG9JA;EACE;;IAAA;EAGA;EACA;EACA;AHiKF;;AIvKA;EACE;;IAAA;EAGA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;EACA;EACA;EAEA;;0CAAA;EAGA;EAEA;AJsKF;;AInKA;EACE;EACA;EACA;AJsKF;;AKxMA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;AL0MF;;AKvMA;EACE;EACA;EACA;EACA;EACA;EACA;AL0MF;;AM7NA;;;;EAAA;AAMA;EACE;EACA;AN+NF;;AM5NA;AACA;EACE;EACA;EACA;AN+NF;;AM5NA;EACE;EACA;EACA;EACA;AN+NF;;AM5NA;EACE;AN+NF;;AM5NA;EAEE;UAAA;EACA;AN8NF;;AM1NA;EACE;EACA;AN6NF;;AM1NA;EACE;AN6NF;;AM1NA;AAWA;;;;EAAA;AAKA;;;;EAIE;EACA;ANmNF;;AMhNA;EACE;;IAEE;ENmNF;EMhNA;IAEE;YAAA;ENiNF;AACF;AM9MA;EACE;;;IAGE;ENgNF;EM9MA;;IAEE;ENgNF;AACF;AM3MA;EACE;;;IAGE;EN6MF;EM3MA;;IAEE;EN6MF;AACF;AMxMA;EACE;;;IAGE;EN0MF;EMxMA;;IAEE;EN0MF;EMxMA;;KAAA;AN4MF;AMxMA;EACE;EACA;;;IAGE;EN0MF;EMxMA;;IAEE;EN0MF;EMxMA;;KAAA;AN4MF;AMxMA;EACE;;;IAGE;EN0MF;EMxMA;;IAEE;EN0MF;EMxMA;;KAAA;AN4MF;AMxMA;EACE;;;IAGE;EN0MF;EMxMA;;IAEE;EN0MF;EMxMA;;KAAA;AN4MF;AMxMA;EACE;EACA;;;IAGE;EN0MF;EMxMA;;IAEE;EN0MF;EMtMA;IACE;IACA;ENwMF;EMtMA;;KAAA;AN0MF;AMtMA;EACE;;IAEE;ENwMF;EMtMA;;;IAGE;ENwMF;EMtMA;;KAAA;AN0MF;AMtMA;EACE;;IAEE;ENwMF;EMtMA;;KAAA;AN0MF;AMtMA;EACE;;;IAGE;ENwMF;EMtMA;IACE;ENwMF;EMtMA;;KAAA;AN0MF;AMrMA;;EAAA;AAGA;EACE;ANuMF;;AO3aA;;EAAA;AAGA;EACE;EACA;EACA;EACA;EACA;AP8aF;;AO3aA;;;;;;EAME;EACA;EACA;AP8aF;;AO3aA;EACE;EACA;EACA;AP8aF;;AO3aA;EACE;EACA;AP8aF;;AO3aA;EACE;EACA;AP8aF;;AO3aA;EACE;EACA;AP8aF;;AO3aA;EACE;EACA;AP8aF;;AO3aA;EACE;EACA;AP8aF;;AO3aA;AACA;;;;;;EAME;EACA;AP8aF;;AO5aA;;;;;;EAME;AP+aF;;AO5aA;EACE;AP+aF;;AO5aA;;;;EAIE;EACA;AP+aF;;AO5aA;;;;EAIE;EAEA;;IAAA;EAGA;AP8aF;;AQ3gBA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;KAAA;UAAA;AR6gBF;;AQ1gBA;;;;;;;EASE;AR2gBF;;AQxgBA;EACE;AR2gBF;;AQxgBA;EACE;EACA;EACA;EACA;EACA;EAEA;AR0gBF;;AQvgBA;EACE;EACA;EACA;EAEA;ARygBF;;AQtgBA;EAGE;ARugBF;;AQpgBA;EACE;EACA;EAEA;EAEA;EACA;ARqgBF;;AQlgBA;EACE;EAEA;EACA;EACA;ARogBF;;AQjgBA;EACE;ARogBF;;AQjgBA;EACE;EACA;EACA;EACA;EAEA;ARmgBF;;AQhgBA;;;;EAIE;ARmgBF;;AQhgBA;;;;EAIE;ARmgBF;;AQhgBA;;EAEE;ARmgBF;;AQhgBA;;EAEE;ARmgBF;;AQhgBA;;;EAGE;ARmgBF;;AQhgBA;;;EAGE;ARmgBF;;AQhgBA;EACE;EACA;EACA;EACA;EACA;ARmgBF;;AQhgBA;EACE;EACA;ARmgBF;;AQhgBA;;EAEE;EACA;EACA;EACA;EACA;EACA;ARmgBF;;AQhgBA;;EAEE;EACA;ARmgBF;;AQhgBA;;EAEE;ARmgBF;;AQhgBA;EAEE;ARkgBF;;AQ/fA;EACE;EACA;ARkgBF;;AQ/fA;EACE;ARkgBF;;AQ/fA;EACE;EACA;EACA;ARkgBF;;AQ/fA;EACE;ARkgBF;;AQ/fA;EACE;EACA;ARkgBF;;AQ/fA;EACE;EACA;ARkgBF;;AQ/fA;EACE;ARkgBF;;AQ/fA;EACE;ARkgBF;;AQ/fA;EACE;ARkgBF;;AQ9fA;EACE;ARigBF;;AQ9fA;EACE;EACA;ARigBF;;AQ9fA;EACE;ARigBF;;AQ9fA;EACE;EACA;EACA;EACA;EACA;EACA;ARigBF;;AQ7fA;EACE;EACA;EACA;ARggBF;;AQ7fA;EACE;ARggBF;;AQvfA;EACE;EACA;AR0fF;;AQvfA;EACE;EAAA;EACA;EACA;EAEA;EACA;EACA;ARyfF;;AQtfA;EACE;ARyfF;;AQtfA;EACE;ARyfF;;AQtfA;;EAEE;EACA;EACA;ARyfF;;AQtfA;EAEE;ARwfF;;AQrfA;EACE;ARwfF;;AS1wBA;EACE;EACA;AT6wBF;;AU/wBA;;;;EAAA;AAMA;EACE;EACA;EACA;EACA;EACA;AVixBF;;AU9wBA;EACE;EACA;EACA;EACA;AVixBF;;AU9wBA;EACE;EACA;AVixBF;;AWxyBA;;EAAA;AAIA;EACE;AX0yBF;;AY/yBA;AAEA;EACE;IAGE;IACA;IAGA;IACA;EZ6yBF;AACF;AazzBA;EACE;Ab2zBF;;AaxzBA;EACE;Ab2zBF;;AaxzBA;EACE;Ab2zBF;;AaxzBA;EAGE;AbyzBF;;AatzBA;EACE;EACA;EACA;EACA;AbyzBF;;AatzBA;EACE;AbyzBF;;AatzBA;EACE;AbyzBF;;AatzBA;EACE;EACA;EACA;EACA;AbyzBF;;Ac91BA;;EAAA;AAIA;EACE;Adg2BF;;Aer2BA;AAEA;EACE;EACA;EACA;Afu2BF;;Aep2BA;EACE;Afu2BF;;Aep2BA;EACE;Afu2BF;;Aep2BA;EACE;Afu2BF;;AgBx3BA;EACE;EACA;EACA;EACA;AhB23BF;;AgBx3BA;EAEE;AhB03BF;;AiBn4BA;;EAAA;AAIA;EACE;EACA;AjBq4BF;;AiBl4BA;EACE;EACA;AjBq4BF;;AiBl4BA;EAEE;EACA;AjBo4BF;;AiBj4BA;EAEE;IAEE;IACA;IAIA;IAGA;EjB63BF;AACF;AiB13BA;EACE;EACA;EACA;EACA;AjB43BF;;AiBz3BA;EACE;EACA;EACA;AjB43BF;;AiBz3BA;EACE;AjB43BF;;AiBz3BA;EACE;AjB43BF;;AiBz3BA;EACE;EACA;EACA;EACA;EACA;AjB43BF;;AiBz3BA;AACA;EACE;EACA;EACA;EACA;AjB43BF;;AiBz3BA;EACE;AjB43BF;;AkBt8BA;;EAAA;AAIA;EACE;AlBw8BF;;AkBr8BA;EACE;AlBw8BF;;AmB/8BA;EACE;EACA;EACA;AnBk9BF;;AmB/8BA;;;EAAA;AAIA;EACE;EACA;EACA;AnBk9BF;;AmB/8BA;EACE;AnBk9BF;;AmB/8BA;EACE;AnBk9BF;;AmB/8BA;EACE;AnBk9BF;;AmB/8BA;EACE;AnBk9BF;;AmB/8BA;EACE;AnBk9BF;;AmB/8BA;;;;EAAA;AAKA;EACE;EACA;UAAA;EACA;EACA;EACA;EACA;EACA;AnBk9BF,C",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/assets/styles/_reset.scss",
         "webpack:///./src/assets/styles/technote.scss",
         "webpack:///./src/assets/styles/properties/_colors.scss",
         "webpack:///./src/assets/styles/properties/_spacing.scss",
@@ -23,24 +23,24 @@
         "webpack:///./src/assets/styles/components/_status.scss",
         "webpack:///./src/assets/styles/components/_svg-icon.scss",
         "webpack:///./src/assets/styles/components/_toc.scss",
         "webpack:///./src/assets/styles/utilities/_theme.scss",
         "webpack:///./src/assets/styles/utilities/_index.scss"
     ],
     "sourcesContent": [
-        "html {\n  box-sizing: border-box;\n}\n\n/*\n * Inherit border-box sizing from html\n * https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/\n */\n*,\n*:before,\n*:after {\n  box-sizing: inherit;\n}\n\n:root {\n  /*\n   * Reinforce that we're respecting the user's ability to set a default\n   * font size. The rem unit now becomes relative to this.\n   * Flexible Typesetting, Tim Brown, ch 2 and 4\n   */\n  font-size: 1.1rem;\n}\n",
-        "html {\n  box-sizing: border-box;\n}\n\n/*\n * Inherit border-box sizing from html\n * https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/\n */\n*,\n*:before,\n*:after {\n  box-sizing: inherit;\n}\n\n:root {\n  /*\n   * Reinforce that we're respecting the user's ability to set a default\n   * font size. The rem unit now becomes relative to this.\n   * Flexible Typesetting, Tim Brown, ch 2 and 4\n   */\n  font-size: 1.1rem;\n}\n\n:root {\n  /*\n   * Color design tokens.\n   *\n   * These are based on GitHub Primer.\n   * https://primer.style/prism/local/a4751264-de23-430e-a2fc-669488065638/scale/c2a0938a-e1dc-4b20-a07b-e2778ae57f41\n   */\n  --tn-color-black: #1b1f24;\n  --tn-color-white: #ffffff;\n  --tn-color-neutral-000: #f6f8fa;\n  --tn-color-neutral-100: #eaeef2;\n  --tn-color-neutral-200: #d0d7de;\n  --tn-color-neutral-300: #afb8c1;\n  --tn-color-neutral-400: #8c959f;\n  --tn-color-neutral-500: #6e7781;\n  --tn-color-neutral-600: #57606a;\n  --tn-color-neutral-700: #424a53;\n  --tn-color-neutral-800: #32383f;\n  --tn-color-neutral-900: #24292f;\n  --tn-color-blue-000: #ddf4ff;\n  --tn-color-blue-100: #b6e3ff;\n  --tn-color-blue-200: #80ccff;\n  --tn-color-blue-300: #54aeff;\n  --tn-color-blue-400: #218bff;\n  --tn-color-blue-500: #0969da;\n  --tn-color-blue-600: #0550ae;\n  --tn-color-blue-700: #033d8b;\n  --tn-color-blue-800: #0a3069;\n  --tn-color-blue-900: #002155;\n  --tn-color-green-000: #dafbe1;\n  --tn-color-green-100: #aceebb;\n  --tn-color-green-200: #6fdd8b;\n  --tn-color-green-300: #4ac26b;\n  --tn-color-green-400: #2da44e;\n  --tn-color-green-500: #1a7f37;\n  --tn-color-green-600: #116329;\n  --tn-color-green-700: #044f1e;\n  --tn-color-green-800: #003d16;\n  --tn-color-green-900: #002d11;\n  --tn-color-yellow-000: #fff8c5;\n  --tn-color-yellow-100: #fae17d;\n  --tn-color-yellow-200: #eac54f;\n  --tn-color-yellow-300: #d4a72c;\n  --tn-color-yellow-400: #bf8700;\n  --tn-color-yellow-500: #9a6700;\n  --tn-color-yellow-600: #7d4e00;\n  --tn-color-yellow-700: #633c01;\n  --tn-color-yellow-800: #4d2d00;\n  --tn-color-yellow-900: #3b2300;\n  --tn-color-orange-000: #fff1e5;\n  --tn-color-orange-100: #ffd8b5;\n  --tn-color-orange-200: #ffb77c;\n  --tn-color-orange-300: #fb8f44;\n  --tn-color-orange-400: #e16f24;\n  --tn-color-orange-500: #bc4c00;\n  --tn-color-orange-600: #953800;\n  --tn-color-orange-700: #762c00;\n  --tn-color-orange-800: #5c2200;\n  --tn-color-orange-900: #471700;\n  --tn-color-red-000: #ffebe9;\n  --tn-color-red-100: #ffcecb;\n  --tn-color-red-200: #ffaba8;\n  --tn-color-red-300: #ff8182;\n  --tn-color-red-400: #fa4549;\n  --tn-color-red-500: #cf222e;\n  --tn-color-red-600: #a40e26;\n  --tn-color-red-700: #82071e;\n  --tn-color-red-800: #660018;\n  --tn-color-red-900: #4c0014;\n  --tn-color-purple-000: #fbefff;\n  --tn-color-purple-100: #ecd8ff;\n  --tn-color-purple-200: #d8b9ff;\n  --tn-color-purple-300: #c297ff;\n  --tn-color-purple-400: #a475f9;\n  --tn-color-purple-500: #8250df;\n  --tn-color-purple-600: #6639ba;\n  --tn-color-purple-700: #512a97;\n  --tn-color-purple-800: #3e1f79;\n  --tn-color-purple-900: #2e1461;\n  --tn-color-pink-000: #ffeff7;\n  --tn-color-pink-100: #ffd3eb;\n  --tn-color-pink-200: #ffadda;\n  --tn-color-pink-300: #ff80c8;\n  --tn-color-pink-400: #e85aad;\n  --tn-color-pink-500: #bf3989;\n  --tn-color-pink-600: #99286e;\n  --tn-color-pink-700: #772057;\n  --tn-color-pink-800: #611347;\n  --tn-color-pink-900: #4d0336;\n  --tn-color-coral-000: #fff0eb;\n  --tn-color-coral-100: #ffd6cc;\n  --tn-color-coral-200: #ffb4a1;\n  --tn-color-coral-300: #fd8c73;\n  --tn-color-coral-400: #ec6547;\n  --tn-color-coral-500: #c4432b;\n  --tn-color-coral-600: #9e2f1c;\n  --tn-color-coral-700: #801f0f;\n  --tn-color-coral-800: #691105;\n  --tn-color-coral-900: #510901;\n  --tn-color-primary: var(--tn-color-neutral-900);\n  --tn-color-primary-000: var(--tn-color-neutral-000);\n  --tn-color-primary-100: var(--tn-color-neutral-100);\n  --tn-color-primary-200: var(--tn-color-neutral-200);\n  --tn-color-primary-300: var(--tn-color-neutral-300);\n  --tn-color-primary-400: var(--tn-color-neutral-400);\n  --tn-color-primary-500: var(--tn-color-neutral-500);\n  --tn-color-primary-600: var(--tn-color-neutral-600);\n  --tn-color-primary-700: var(--tn-color-neutral-700);\n  --tn-color-primary-800: var(--tn-color-neutral-800);\n  --tn-color-primary-900: var(--tn-color-neutral-900);\n}\n\n:root {\n  /*\n   * Spacing values in em units\n   */\n  --tn-space-unit: 1em;\n  --tn-space-xxxs: calc(0.25 * var(--tn-space-unit));\n  --tn-space-xxs: calc(0.375 * var(--tn-space-unit));\n  --tn-space-xs: calc(0.5 * var(--tn-space-unit));\n  --tn-space-sm: calc(0.75 * var(--tn-space-unit));\n  --tn-space-md: calc(1.25 * var(--tn-space-unit));\n  --tn-space-lg: calc(2 * var(--tn-space-unit));\n  --tn-space-xl: calc(3.25 * var(--tn-space-unit));\n  --tn-space-xxl: calc(5.25 * var(--tn-space-unit));\n  --tn-space-xxxl: calc(8.5 * var(--tn-space-unit));\n  /*\n    * Fixed spacing\n    * These aren't affected by --space-unit or the root font size\n    */\n  --tn-space-unit-fixed: 1rem;\n  --tn-space-xxxs-fixed: calc(0.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxs-fixed: calc(0.375 * var(--tn-space-unit-fixed));\n  --tn-space-xs-fixed: calc(0.5 * var(--tn-space-unit-fixed));\n  --tn-space-sm-fixed: calc(0.75 * var(--tn-space-unit-fixed));\n  --tn-space-md-fixed: calc(1.25 * var(--tn-space-unit-fixed));\n  --tn-space-lg-fixed: calc(2 * var(--tn-space-unit-fixed));\n  --tn-space-xl-fixed: calc(3.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxl-fixed: calc(5.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxxl-fixed: calc(8.5 * var(--tn-space-unit-fixed));\n}\n\n:root {\n  /*\n   * Border radius\n   */\n  --tn-border-radius-0: 0px;\n  --tn-border-radius-1: 4px;\n  --tn-border-radius-2: 7px;\n}\n\n:root {\n  /*\n   * Typographic design tokens.\n   */\n  --tn-component-h1-size: 3.052rem;\n  --tn-component-h2-size: 2.441rem;\n  --tn-component-h3-size: 1.563rem;\n  --tn-component-h4-size: 1.25rem;\n  --tn-component-h5-size: 1rem;\n  --tn-component-h6-size: 0.8rem;\n  --tn-component-h1-weight: normal;\n  --tn-component-h2-weight: normal;\n  --tn-component-h3-weight: bold;\n  --tn-component-h4-weight: bold;\n  --tn-component-h5-weight: bold;\n  --tn-component-h6-weight: bold;\n  --tn-component-text-color: var(--tn-color-black);\n  --tn-component-link-color: var(--tn-color-blue-500);\n  --tn-component-text-background-color: var(--tn-color-white);\n  --tn-component-text-font-family: -apple-system, BlinkMacSystemFont, Segoe UI,\n    Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue,\n    sans-serif;\n  --tn-component-text-line-height: 1.5;\n}\n\nhtml[data-theme=dark] {\n  --tn-component-text-color: var(--tn-color-white);\n  --tn-component-link-color: var(--tn-color-blue-300);\n  --tn-component-text-background-color: var(--tn-color-black);\n}\n\n/* Properties for Sphinx components. */\n:root {\n  --tn-sphinx-code-block-border-color: var(--tn-color-primary);\n  --tn-sphinx-code-block-border-thickness: 1px;\n  --tn-sphinx-code-block-border-radius: var(--tn-border-radius-1);\n  --tn-sphinx-code-block-caption-background-color: var(--tn-color-primary-000);\n  --tn-sphinx-footnote-label-background-color: var(--tn-color-blue-000);\n  --tn-sphinx-footnote-label-border-color: var(--tn-color-blue-100);\n  --tn-sphinx-footnote-label-background-hover-color: var(--tn-color-blue-100);\n  --tn-sphinx-footnote-label-border-hover-color: var(--tn-color-blue-200);\n}\n\nhtml[data-theme=dark] {\n  --tn-sphinx-code-block-border-color: var(--tn-color-primary-700);\n  --tn-sphinx-code-block-caption-background-color: var(--tn-color-primary-900);\n  --tn-sphinx-footnote-label-background-color: var(--tn-color-blue-900);\n  --tn-sphinx-footnote-label-border-color: var(--tn-color-blue-800);\n  --tn-sphinx-footnote-label-background-hover-color: var(--tn-color-blue-800);\n  --tn-sphinx-footnote-label-border-hover-color: var(--tn-color-blue-700);\n}\n\n/*\n * Styles that affect the overall layout. Since Technote is built on\n * sphinx-basic-ng as the base theme, these styles primarily work with\n * the base theme's sb- classes.\n */\n.sb-container {\n  margin-top: var(--tn-space-md-fixed);\n}\n\n/* Style the prmary sidebar when it's a popover. */\n#sb-sidebar-toggle--primary:checked ~ .sb-container .sb-sidebar-primary {\n  background-color: white;\n  box-shadow: 10px 5px 5px rgb(161, 161, 161);\n  border-right: 1px solid black;\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .sb-sidebar-secondary {\n  background-color: white;\n  box-shadow: -5px 0 5px rgb(161, 161, 161);\n  border-left: 1px solid black;\n  padding-left: var(--tn-space-md-fixed);\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .technote-toc-header {\n  margin-top: var(--tn-space-md-fixed);\n}\n\n.sb-sidebar-overlay {\n  backdrop-filter: blur(1.5px) opacity(0.7) brightness(150%);\n  background-color: rgba(0, 0, 0, 0);\n}\n\n.sb-header__inner {\n  display: flex;\n  justify-content: space-between;\n}\n\n.sb-header__inner label {\n  margin: var(--tn-space-xs-fixed);\n}\n\n/* Highlight key containers for debugging. */\n/*\n * Content container width.\n * Goal is to have a content width <= 80 characters. These override\n * breakpoint settings from sphinx-basic-ng's skeleton.css\n */\n.sb-article-container,\n.sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n  /* reset skeleton.css. Using 100vw means we get horizontal scrollbars. */\n  width: auto;\n}\n\n@media (max-width: 42rem) {\n  .sb-article-container,\n.sb-footer-content__inner {\n    width: 100vw;\n  }\n  body {\n    hyphens: auto;\n  }\n}\n@media (min-width: 42rem) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 38rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 38rem;\n  }\n}\n@media (min-width: 46rem) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 40rem;\n  }\n}\n@media (min-width: 50rem) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 50';\n  } */\n}\n@media (min-width: 59rem) {\n  /* secondary sidebar appears, width is 17rem. */\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 36rem;\n  }\n  /* h1::after {\n    content: ' 59';\n  } */\n}\n@media (min-width: 63rem) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 36rem;\n  }\n  /* h1::after {\n    content: ' 63';\n  } */\n}\n@media (min-width: 67rem) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 67';\n  } */\n}\n@media (min-width: 76rem) {\n  /* The primary sidebar appears */\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n.match-content-width {\n    width: 32rem;\n  }\n  .sb-sidebar-primary {\n    box-shadow: none;\n    border-right: none;\n  }\n  /* h1::after {\n    content: ' 76';\n  } */\n}\n@media (min-width: 80rem) {\n  .sb-article,\n.match-content-width {\n    width: 34rem;\n  }\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 80';\n  } */\n}\n@media (min-width: 84rem) {\n  .sb-article,\n.match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 84';\n  } */\n}\n@media (min-width: 88rem) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-page-width {\n    width: 86rem;\n  }\n  /* h1::after {\n    content: ' 88';\n  } */\n}\n/*\n * Primary sidebar\n */\n.sb-sidebar-primary {\n  padding: var(--tn-space-md-fixed);\n}\n\n/*\n * Typography.\n */\nbody {\n  font-family: var(--tn-component-text-font-family);\n  line-height: var(--tn-component-text-line-height);\n  color: var(--tn-component-text-color);\n  background: var(--tn-component-text-background-color);\n}\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n  /* Put header vertically closer to its own section. */\n  margin: 1.5em 0 0.8em;\n  line-height: 1.2;\n}\n\nh1 {\n  font-size: var(--tn-component-h1-size);\n  font-weight: var(--tn-component-h1-weight);\n  margin: 0 0 1em;\n}\n\nh2 {\n  font-size: var(--tn-component-h2-size);\n  font-weight: var(--tn-component-h2-weight);\n}\n\nh3 {\n  font-size: var(--tn-component-h3-size);\n  font-weight: var(--tn-component-h3-weight);\n}\n\nh4 {\n  font-size: var(--tn-component-h4-size);\n  font-weight: var(--tn-component-h4-weight);\n}\n\nh5 {\n  font-size: var(--tn-component-h5-size);\n  font-weight: var(--tn-component-h5-weight);\n}\n\nh6 {\n  font-size: var(--tn-component-h6-size);\n  font-weight: var(--tn-component-h6-weight);\n}\n\n/* Handle Sphinx's built-in permalink icon. */\nh1 .headerlink,\nh2 .headerlink,\nh3 .headerlink,\nh4 .headerlink,\nh5 .headerlink,\nh6 .headerlink {\n  visibility: hidden;\n  text-decoration: none;\n}\n\nh1:hover .headerlink,\nh2:hover .headerlink,\nh3:hover .headerlink,\nh4:hover .headerlink,\nh5:hover .headerlink,\nh6:hover .headerlink {\n  visibility: visible;\n}\n\na {\n  color: var(--tn-component-link-color);\n}\n\n/* Styles Sphinx-generated content classes */\na.headerlink {\n  opacity: 0;\n  font-size: 0.9em;\n  margin-left: var(--tn-space-xxs);\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n  user-select: none;\n}\n\nh1:hover a.headlink,\nh2:hover a.headerlink,\nh3:hover a.headerlink,\nh4:hover a.headerlink,\nh5:hover a.headerlink,\nh6:hover a.headerlink,\n.code-block-caption:hover a.headerlink {\n  opacity: 0.5;\n}\n\na.headerlink:hover {\n  opacity: 1;\n}\n\npre {\n  font-size: 0.85rem;\n}\n\n.literal-block-wrapper .highlight pre {\n  margin: 0;\n  padding: var(--tn-space-xs-fixed);\n  overflow-x: auto;\n}\n\n.literal-block-wrapper {\n  border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n\n.literal-block-wrapper .highlight {\n  border-radius: 0 0 var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius);\n}\n\n.code-block-caption {\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-bottom: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius) 0 0;\n  padding: var(--tn-space-xxxs-fixed) var(--tn-space-xs-fixed);\n}\n\n.admonition {\n  border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n  padding: var(--tn-space-xs-fixed);\n  margin-bottom: 1rem;\n}\n\n.admonition :last-child {\n  margin-bottom: 0;\n}\n\n.admonition-title {\n  font-weight: bold;\n  margin: calc(-1 * var(--tn-space-xs-fixed));\n  padding: var(--tn-space-xs-fixed);\n  border-radius: var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius) 0 0;\n  font-size: 0.9rem;\n}\n\n.admonition.attention .admonition-title,\n.admonition.caution .admonition-title,\n.admonition.warning .admonition-title,\n.admonition.important .admonition-title {\n  background-color: var(--tn-color-yellow-100);\n}\n\n.admonition.attention,\n.admonition.caution,\n.admonition.warning,\n.admonition.important {\n  border-color: var(--tn-color-yellow-500);\n}\n\n.admonition.danger .admonition-title,\n.admonition.error .admonition-title {\n  background-color: var(--tn-color-red-100);\n}\n\n.admonition.danger,\n.admonition.error {\n  border-color: var(--tn-color-red-500);\n}\n\n.admonition.tip .admonition-title,\n.admonition.note .admonition-title,\n.admonition.hint .admonition-title {\n  background-color: var(--tn-color-blue-100);\n}\n\n.admonition.tip,\n.admonition.note,\n.admonition.hint {\n  border-color: var(--tn-color-blue-500);\n}\n\n.footnote-list .footnote {\n  font-size: 0.9rem;\n  margin-bottom: 0.5rem;\n  display: flex;\n  flex-direction: row;\n  align-items: baseline;\n}\n\n.footnote-list .footnote .label {\n  display: block;\n  min-width: 1.5rem;\n}\n\n.footnote-list .footnote .label a,\n.footnote-reference {\n  background-color: var(--tn-sphinx-footnote-label-background-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-color);\n  border-radius: 4px;\n  padding: 2px 4px;\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.footnote-list .footnote .label a:hover,\n.footnote-reference:hover {\n  background-color: var(--tn-sphinx-footnote-label-background-hover-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-hover-color);\n}\n\n.footnote .fn-bracket,\n.footnote-reference .fn-bracket {\n  display: none;\n}\n\n.citation p {\n  display: inline;\n}\n\n.citation .label a {\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.citation .label a:hover {\n  text-decoration: underline;\n}\n\nblockquote {\n  border-left: 0.25rem solid var(--tn-color-primary);\n  margin-left: 0;\n  padding-left: 1rem;\n}\n\nblockquote .attribution {\n  font-style: italic;\n}\n\nmain li p {\n  margin-top: 0;\n  margin-bottom: 0;\n}\n\n.block-list p {\n  margin-top: 1rem;\n  margin-bottom: 1rem;\n}\n\ndt {\n  font-weight: bold;\n}\n\ndd {\n  margin-left: 2rem;\n}\n\ndd p:first-of-type {\n  margin-top: 0.2rem;\n}\n\nimg {\n  max-width: 100%;\n}\n\nfigure {\n  margin-left: 0;\n  margin-right: 0;\n}\n\nfigure img {\n  max-width: 100%;\n}\n\nfigcaption {\n  width: 100%;\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-radius: 4px;\n  padding: 0.5rem 1rem;\n  margin: 0;\n  border: none;\n}\n\nfigcaption p {\n  margin-top: 0;\n  margin-bottom: 1em;\n  padding: 0;\n}\n\nfigcaption p:last-child {\n  margin-bottom: 0;\n}\n\n.technote-table {\n  max-width: 100%;\n  overflow-x: auto;\n}\n\ntable {\n  max-width: fit-content;\n  margin: 0 auto 0 0;\n  white-space: nowrap;\n  font-size: 0.9rem;\n  font-variant-numeric: lining-nums tabular-nums;\n  border-collapse: collapse;\n}\n\nth {\n  font-weight: normal;\n}\n\nthead {\n  border-bottom: 1px solid var(--tn-component-text-color);\n}\n\ntd,\nth {\n  padding: 0.125em 0.5em 0.25em 0.5em;\n  line-height: 1;\n  text-align: inherit;\n}\n\ntd {\n  text-align: \".\" center;\n}\n\ntable caption {\n  caption-side: bottom;\n}\n\n.technote-article-header-id {\n  font-size: var(--tn-component-h4-size);\n  font-weight: bold;\n}\n\n/*\n * Icon Metadata Lists consist of a an icon paired with a metadata value.\n * The value can span multiple lines, but will always be indented beside\n * the icon.\n */\n.technote-icon-metadata {\n  display: flex;\n  flex-direction: row;\n  justify-content: flex-start;\n  align-items: baseline;\n  gap: var(--tn-space-xxs-fixed);\n}\n\n.technote-icon-metadata__icon {\n  width: 1em;\n  flex-grow: 0;\n  flex-shrink: 0;\n  margin: 0;\n}\n\n.technote-icon-metadata__value {\n  flex-grow: 1;\n  margin: 0;\n}\n\n/*\n * Styles for the author list that appears below the title.\n */\n.technote-status + .technote-inline-authors {\n  margin-top: 2rem;\n}\n\n/* The container for the primary sidebar */\n@media (min-width: 76rem) {\n  .technote-sidebar-container {\n    position: sticky;\n    top: 1rem;\n    overflow-y: auto;\n    max-height: 100vh;\n  }\n}\n:root {\n  --tn-component-sidebar-header-color: var(--tn-color-neutral-600);\n}\n\nhtml[data-theme=dark] {\n  --tn-component-sidebar-header-color: var(--tn-color-neutral-200);\n}\n\n.technote-sidebar-section {\n  margin: 0 0 var(--tn-space-lg-fixed);\n}\n\n.technote-sidebar-section:first-of-type {\n  margin-top: var(--tn-space-lg-fixed);\n}\n\n.technote-sidebar-section__heading {\n  font-size: var(--tn-component-h6-size);\n  font-weight: bold;\n  color: var(--tn-component-sidebar-header-color);\n  margin-bottom: 0.5rem;\n}\n\n.technote-sidebar-section__heading + * {\n  margin-top: var(--tn-space-xs-fixed);\n}\n\n.technote-sidebar-author-list {\n  margin-top: var(--tn-space-xs-fixed);\n}\n\n.technote-sidebar-metadata-list {\n  margin-top: var(--tn-space-xs-fixed);\n  margin-bottom: var(--tn-space-xs-fixed);\n  list-style-type: none;\n  padding: 0;\n}\n\n/*\n * Styles for the sidebar-logo component.\n */\n.technote-sidebar-logo__picture {\n  max-width: 12rem;\n}\n\n/* Styles for the document status aside */\n.technote-status {\n  border: 1px solid var(--tn-component-text-color);\n  padding: 1rem;\n  border-radius: var(--tn-border-radius-1);\n}\n\n.technote-status--deprecated {\n  border-color: var(--tn-color-red-500);\n}\n\n.technote-status p:first-of-type {\n  margin-top: 0;\n}\n\n.technote-status *:last-child {\n  margin-bottom: 0;\n}\n\n.technote-svg-icon {\n  width: 0.85em;\n  height: 0.85em;\n  display: inline;\n  fill: currentColor;\n}\n\na .technote-svg-icon {\n  fill: var(--tn-component-text-color);\n}\n\n/*\n * Local TOC styling.\n */\n:root {\n  --tn-component-toc-header-color: var(--tn-color-neutral-600);\n  --tn-component-toc-level-border-color: var(--tn-color-neutral-600);\n}\n\nhtml[data-theme=dark] {\n  --tn-component-toc-header-color: var(--tn-color-neutral-200);\n  --tn-component-toc-level-border-color: var(--tn-color-neutral-200);\n}\n\n.technote-toc {\n  overflow-y: auto;\n  max-height: 100vh;\n}\n\n@media (min-width: 59rem) {\n  .technote-toc {\n    position: sticky;\n    top: 1rem;\n    margin-top: 20vh;\n    margin-left: 2rem;\n  }\n}\n.technote-toc-header {\n  margin: 0 0 1rem;\n  font-size: var(--tn-component-h4-size);\n  font-weight: bold;\n  color: var(--tn-component-toc-header-color);\n}\n\n.technote-toc-container {\n  line-height: 1.2;\n  /* Spacing between items in the toc */\n  --technote-toc-container-spacing: var(--tn-space-xs-fixed);\n}\n\n.technote-toc-container a {\n  text-decoration: none;\n}\n\n.technote-toc-container a:hover {\n  text-decoration: underline;\n}\n\n.technote-toc-container ul {\n  list-style-type: none;\n  padding-left: var(--tn-space-xs-fixed);\n  margin-left: var(--tn-space-xxs-fixed);\n  border-left: 2px solid var(--tn-component-toc-level-border-color);\n  margin-top: var(--technote-toc-container-spacing);\n}\n\n/* Root-level sections aren't indented */\n.technote-toc-container > ul {\n  margin-left: 0;\n  padding-left: 0;\n  border-left: none;\n  margin-top: 0;\n}\n\n.technote-toc-container li {\n  margin-bottom: var(--technote-toc-container-spacing);\n}\n\n/*\n * Utilities for displaying different elements based on the current theme.\n */\nhtml[data-theme=light] .technote-themed-dark {\n  display: none;\n}\n\nhtml[data-theme=dark] .technote-themed-light {\n  display: none;\n}\n\n.technote-icon-pair-list {\n  list-style: none;\n  margin-left: 0;\n  padding-left: 0;\n}\n\n/*\n * comma-list makes a ul an inline list with grammatical comma separated\n * items.\n */\n.technote-inline-comma-list {\n  list-style: none;\n  margin-left: 0;\n  padding-left: 0;\n}\n\n.technote-inline-comma-list li {\n  display: inline;\n}\n\n.technote-inline-comma-list li:after {\n  content: \", \";\n}\n\n.technote-inline-comma-list li:last-child:after {\n  content: \"\";\n}\n\n.technote-inline-comma-list li:nth-last-child(2):after {\n  content: \" and \";\n}\n\n.technote-inline-comma-list li:nth-last-child(3) ~ li:nth-last-child(2):after {\n  content: \", and \";\n}\n\n/*\n * Hiding class, making content visible only to screen readers but not visually\n * \"sr\" meaning \"screen-reader\"\n * https://css-tricks.com/inclusively-hidden/\n */\n.sr-only:not(:focus):not(:active) {\n  clip: rect(0 0 0 0);\n  clip-path: inset(50%);\n  height: 1px;\n  overflow: hidden;\n  position: absolute;\n  white-space: nowrap;\n  width: 1px;\n}",
+        "html {\n  box-sizing: border-box;\n\n  /*\n   * Maintain the user's default font size. Rems are relative to this.\n   */\n  font-size: 100%;\n}\n\n/*\n * Inherit border-box sizing from html\n * https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/\n */\n*,\n*:before,\n*:after {\n  box-sizing: inherit;\n}\n",
+        "html {\n  box-sizing: border-box;\n  /*\n   * Maintain the user's default font size. Rems are relative to this.\n   */\n  font-size: 100%;\n}\n\n/*\n * Inherit border-box sizing from html\n * https://css-tricks.com/inheriting-box-sizing-probably-slightly-better-best-practice/\n */\n*,\n*:before,\n*:after {\n  box-sizing: inherit;\n}\n\n:root {\n  /*\n   * Color design tokens.\n   *\n   * These are based on GitHub Primer.\n   * https://primer.style/prism/local/a4751264-de23-430e-a2fc-669488065638/scale/c2a0938a-e1dc-4b20-a07b-e2778ae57f41\n   */\n  --tn-color-black: #1b1f24;\n  --tn-color-white: #ffffff;\n  --tn-color-neutral-000: #f6f8fa;\n  --tn-color-neutral-100: #eaeef2;\n  --tn-color-neutral-200: #d0d7de;\n  --tn-color-neutral-300: #afb8c1;\n  --tn-color-neutral-400: #8c959f;\n  --tn-color-neutral-500: #6e7781;\n  --tn-color-neutral-600: #57606a;\n  --tn-color-neutral-700: #424a53;\n  --tn-color-neutral-800: #32383f;\n  --tn-color-neutral-900: #24292f;\n  --tn-color-blue-000: #ddf4ff;\n  --tn-color-blue-100: #b6e3ff;\n  --tn-color-blue-200: #80ccff;\n  --tn-color-blue-300: #54aeff;\n  --tn-color-blue-400: #218bff;\n  --tn-color-blue-500: #0969da;\n  --tn-color-blue-600: #0550ae;\n  --tn-color-blue-700: #033d8b;\n  --tn-color-blue-800: #0a3069;\n  --tn-color-blue-900: #002155;\n  --tn-color-green-000: #dafbe1;\n  --tn-color-green-100: #aceebb;\n  --tn-color-green-200: #6fdd8b;\n  --tn-color-green-300: #4ac26b;\n  --tn-color-green-400: #2da44e;\n  --tn-color-green-500: #1a7f37;\n  --tn-color-green-600: #116329;\n  --tn-color-green-700: #044f1e;\n  --tn-color-green-800: #003d16;\n  --tn-color-green-900: #002d11;\n  --tn-color-yellow-000: #fff8c5;\n  --tn-color-yellow-100: #fae17d;\n  --tn-color-yellow-200: #eac54f;\n  --tn-color-yellow-300: #d4a72c;\n  --tn-color-yellow-400: #bf8700;\n  --tn-color-yellow-500: #9a6700;\n  --tn-color-yellow-600: #7d4e00;\n  --tn-color-yellow-700: #633c01;\n  --tn-color-yellow-800: #4d2d00;\n  --tn-color-yellow-900: #3b2300;\n  --tn-color-orange-000: #fff1e5;\n  --tn-color-orange-100: #ffd8b5;\n  --tn-color-orange-200: #ffb77c;\n  --tn-color-orange-300: #fb8f44;\n  --tn-color-orange-400: #e16f24;\n  --tn-color-orange-500: #bc4c00;\n  --tn-color-orange-600: #953800;\n  --tn-color-orange-700: #762c00;\n  --tn-color-orange-800: #5c2200;\n  --tn-color-orange-900: #471700;\n  --tn-color-red-000: #ffebe9;\n  --tn-color-red-100: #ffcecb;\n  --tn-color-red-200: #ffaba8;\n  --tn-color-red-300: #ff8182;\n  --tn-color-red-400: #fa4549;\n  --tn-color-red-500: #cf222e;\n  --tn-color-red-600: #a40e26;\n  --tn-color-red-700: #82071e;\n  --tn-color-red-800: #660018;\n  --tn-color-red-900: #4c0014;\n  --tn-color-purple-000: #fbefff;\n  --tn-color-purple-100: #ecd8ff;\n  --tn-color-purple-200: #d8b9ff;\n  --tn-color-purple-300: #c297ff;\n  --tn-color-purple-400: #a475f9;\n  --tn-color-purple-500: #8250df;\n  --tn-color-purple-600: #6639ba;\n  --tn-color-purple-700: #512a97;\n  --tn-color-purple-800: #3e1f79;\n  --tn-color-purple-900: #2e1461;\n  --tn-color-pink-000: #ffeff7;\n  --tn-color-pink-100: #ffd3eb;\n  --tn-color-pink-200: #ffadda;\n  --tn-color-pink-300: #ff80c8;\n  --tn-color-pink-400: #e85aad;\n  --tn-color-pink-500: #bf3989;\n  --tn-color-pink-600: #99286e;\n  --tn-color-pink-700: #772057;\n  --tn-color-pink-800: #611347;\n  --tn-color-pink-900: #4d0336;\n  --tn-color-coral-000: #fff0eb;\n  --tn-color-coral-100: #ffd6cc;\n  --tn-color-coral-200: #ffb4a1;\n  --tn-color-coral-300: #fd8c73;\n  --tn-color-coral-400: #ec6547;\n  --tn-color-coral-500: #c4432b;\n  --tn-color-coral-600: #9e2f1c;\n  --tn-color-coral-700: #801f0f;\n  --tn-color-coral-800: #691105;\n  --tn-color-coral-900: #510901;\n  --tn-color-primary: var(--tn-color-neutral-900);\n  --tn-color-primary-000: var(--tn-color-neutral-000);\n  --tn-color-primary-100: var(--tn-color-neutral-100);\n  --tn-color-primary-200: var(--tn-color-neutral-200);\n  --tn-color-primary-300: var(--tn-color-neutral-300);\n  --tn-color-primary-400: var(--tn-color-neutral-400);\n  --tn-color-primary-500: var(--tn-color-neutral-500);\n  --tn-color-primary-600: var(--tn-color-neutral-600);\n  --tn-color-primary-700: var(--tn-color-neutral-700);\n  --tn-color-primary-800: var(--tn-color-neutral-800);\n  --tn-color-primary-900: var(--tn-color-neutral-900);\n}\n\n:root {\n  /*\n   * Spacing values in em units\n   */\n  --tn-space-unit: 1em;\n  --tn-space-xxxs: calc(0.25 * var(--tn-space-unit));\n  --tn-space-xxs: calc(0.375 * var(--tn-space-unit));\n  --tn-space-xs: calc(0.5 * var(--tn-space-unit));\n  --tn-space-sm: calc(0.75 * var(--tn-space-unit));\n  --tn-space-md: calc(1.25 * var(--tn-space-unit));\n  --tn-space-lg: calc(2 * var(--tn-space-unit));\n  --tn-space-xl: calc(3.25 * var(--tn-space-unit));\n  --tn-space-xxl: calc(5.25 * var(--tn-space-unit));\n  --tn-space-xxxl: calc(8.5 * var(--tn-space-unit));\n  /*\n    * Fixed spacing\n    * These aren't affected by --space-unit or the root font size\n    */\n  --tn-space-unit-fixed: 1rem;\n  --tn-space-xxxs-fixed: calc(0.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxs-fixed: calc(0.375 * var(--tn-space-unit-fixed));\n  --tn-space-xs-fixed: calc(0.5 * var(--tn-space-unit-fixed));\n  --tn-space-sm-fixed: calc(0.75 * var(--tn-space-unit-fixed));\n  --tn-space-md-fixed: calc(1.25 * var(--tn-space-unit-fixed));\n  --tn-space-lg-fixed: calc(2 * var(--tn-space-unit-fixed));\n  --tn-space-xl-fixed: calc(3.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxl-fixed: calc(5.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxxl-fixed: calc(8.5 * var(--tn-space-unit-fixed));\n}\n\n:root {\n  /*\n   * Border radius\n   */\n  --tn-border-radius-0: 0px;\n  --tn-border-radius-1: 4px;\n  --tn-border-radius-2: 7px;\n}\n\n:root {\n  /*\n   * Typographic design tokens.\n   */\n  --tn-component-h1-size: 3.052rem;\n  --tn-component-h2-size: 2.441rem;\n  --tn-component-h3-size: 1.563rem;\n  --tn-component-h4-size: 1.25rem;\n  --tn-component-h5-size: 1.1rem;\n  --tn-component-h6-size: 1rem;\n  --tn-component-h1-weight: normal;\n  --tn-component-h2-weight: normal;\n  --tn-component-h3-weight: bold;\n  --tn-component-h4-weight: bold;\n  --tn-component-h5-weight: bold;\n  --tn-component-h6-weight: bold;\n  --tn-component-text-font-size: 1.1rem;\n  --tn-component-text-color: var(--tn-color-black);\n  --tn-component-link-color: var(--tn-color-blue-500);\n  --tn-component-text-background-color: var(--tn-color-white);\n  --tn-component-text-font-family: -apple-system, ui-sans-serif,\n    BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans,\n    Droid Sans, Helvetica Neue, sans-serif;\n  --tn-component-text-line-height: 1.5;\n  --tn-component-code-font-family: ui-monospace, monospace;\n}\n\nhtml[data-theme=dark] {\n  --tn-component-text-color: var(--tn-color-white);\n  --tn-component-link-color: var(--tn-color-blue-300);\n  --tn-component-text-background-color: var(--tn-color-black);\n}\n\n/* Properties for Sphinx components. */\n:root {\n  --tn-sphinx-code-block-border-color: var(--tn-color-primary);\n  --tn-sphinx-code-block-border-thickness: 1px;\n  --tn-sphinx-code-block-border-radius: var(--tn-border-radius-1);\n  --tn-sphinx-code-block-caption-background-color: var(--tn-color-primary-000);\n  --tn-sphinx-footnote-label-background-color: var(--tn-color-blue-000);\n  --tn-sphinx-footnote-label-border-color: var(--tn-color-blue-100);\n  --tn-sphinx-footnote-label-background-hover-color: var(--tn-color-blue-100);\n  --tn-sphinx-footnote-label-border-hover-color: var(--tn-color-blue-200);\n}\n\nhtml[data-theme=dark] {\n  --tn-sphinx-code-block-border-color: var(--tn-color-primary-700);\n  --tn-sphinx-code-block-caption-background-color: var(--tn-color-primary-900);\n  --tn-sphinx-footnote-label-background-color: var(--tn-color-blue-900);\n  --tn-sphinx-footnote-label-border-color: var(--tn-color-blue-800);\n  --tn-sphinx-footnote-label-background-hover-color: var(--tn-color-blue-800);\n  --tn-sphinx-footnote-label-border-hover-color: var(--tn-color-blue-700);\n}\n\n/*\n * Styles that affect the overall layout. Since Technote is built on\n * sphinx-basic-ng as the base theme, these styles primarily work with\n * the base theme's sb- classes.\n */\n.sb-container {\n  margin-top: var(--tn-space-md-fixed);\n  margin-bottom: var(--tn-space-xxl-fixed);\n}\n\n/* Style the prmary sidebar when it's a popover. */\n#sb-sidebar-toggle--primary:checked ~ .sb-container .sb-sidebar-primary {\n  background-color: white;\n  box-shadow: 10px 5px 5px rgb(161, 161, 161);\n  border-right: 1px solid black;\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .sb-sidebar-secondary {\n  background-color: white;\n  box-shadow: -5px 0 5px rgb(161, 161, 161);\n  border-left: 1px solid black;\n  padding-left: var(--tn-space-md-fixed);\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .technote-toc-header {\n  margin-top: var(--tn-space-md-fixed);\n}\n\n.sb-sidebar-overlay {\n  backdrop-filter: blur(1.5px) opacity(0.7) brightness(150%);\n  background-color: rgba(0, 0, 0, 0);\n}\n\n.sb-header__inner {\n  display: flex;\n  justify-content: space-between;\n}\n\n.sb-header__inner label {\n  margin: var(--tn-space-xs-fixed);\n}\n\n/* Highlight key containers for debugging. */\n/*\n * Content container width.\n * Goal is to have a content width <= 80 characters. These override\n * breakpoint settings from sphinx-basic-ng's skeleton.css\n */\n.sb-article-container,\n.sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n  /* reset skeleton.css. Using 100vw means we get horizontal scrollbars. */\n  width: auto;\n}\n\n@media (max-width: 42em) {\n  .sb-article-container,\n.sb-footer-content__inner {\n    width: 100vw;\n  }\n  body {\n    hyphens: auto;\n  }\n}\n@media (min-width: 42em) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 38em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 38em;\n  }\n}\n@media (min-width: 46em) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 40em;\n  }\n}\n@media (min-width: 50em) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 50';\n  } */\n}\n@media (min-width: 59em) {\n  /* secondary sidebar appears, width is 17rem. */\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 36em;\n  }\n  /* h1::after {\n    content: ' 59';\n  } */\n}\n@media (min-width: 63em) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 36em;\n  }\n  /* h1::after {\n    content: ' 63';\n  } */\n}\n@media (min-width: 67em) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 67';\n  } */\n}\n@media (min-width: 76em) {\n  /* The primary sidebar appears */\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n.match-content-width {\n    width: 32em;\n  }\n  .sb-sidebar-primary {\n    box-shadow: none;\n    border-right: none;\n  }\n  /* h1::after {\n    content: ' 76';\n  } */\n}\n@media (min-width: 80em) {\n  .sb-article,\n.match-content-width {\n    width: 34em;\n  }\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 80';\n  } */\n}\n@media (min-width: 84em) {\n  .sb-article,\n.match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 84';\n  } */\n}\n@media (min-width: 88em) {\n  .sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-page-width {\n    width: 86em;\n  }\n  /* h1::after {\n    content: ' 88';\n  } */\n}\n/*\n * Primary sidebar\n */\n.sb-sidebar-primary {\n  padding: var(--tn-space-md-fixed);\n}\n\n/*\n * Typography.\n */\nbody {\n  font-family: var(--tn-component-text-font-family);\n  line-height: var(--tn-component-text-line-height);\n  font-size: var(--tn-component-text-font-size);\n  color: var(--tn-component-text-color);\n  background: var(--tn-component-text-background-color);\n}\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n  /* Put header vertically closer to its own section. */\n  margin: 1.5em 0 0.8em;\n  line-height: 1.2;\n}\n\nh1 {\n  font-size: var(--tn-component-h1-size);\n  font-weight: var(--tn-component-h1-weight);\n  margin: 0 0 1em;\n}\n\nh2 {\n  font-size: var(--tn-component-h2-size);\n  font-weight: var(--tn-component-h2-weight);\n}\n\nh3 {\n  font-size: var(--tn-component-h3-size);\n  font-weight: var(--tn-component-h3-weight);\n}\n\nh4 {\n  font-size: var(--tn-component-h4-size);\n  font-weight: var(--tn-component-h4-weight);\n}\n\nh5 {\n  font-size: var(--tn-component-h5-size);\n  font-weight: var(--tn-component-h5-weight);\n}\n\nh6 {\n  font-size: var(--tn-component-h6-size);\n  font-weight: var(--tn-component-h6-weight);\n}\n\n/* Handle Sphinx's built-in permalink icon. */\nh1 .headerlink,\nh2 .headerlink,\nh3 .headerlink,\nh4 .headerlink,\nh5 .headerlink,\nh6 .headerlink {\n  visibility: hidden;\n  text-decoration: none;\n}\n\nh1:hover .headerlink,\nh2:hover .headerlink,\nh3:hover .headerlink,\nh4:hover .headerlink,\nh5:hover .headerlink,\nh6:hover .headerlink {\n  visibility: visible;\n}\n\na {\n  color: var(--tn-component-link-color);\n}\n\npre,\nxmp,\nplaintext,\nlisting {\n  font-family: var(--tn-component-code-font-family);\n  font-size: 1rem;\n}\n\ntt,\ncode,\nkbd,\nsamp {\n  font-family: var(--tn-component-code-font-family);\n  /* Making inline code slightly smaller seems to help with baseline alignment\n   * some monospace fonts seems bigger that Source Sans.\n   */\n  font-size: 0.9em;\n}\n\n/* Styles Sphinx-generated content classes */\na.headerlink {\n  opacity: 0;\n  font-size: 0.9em;\n  margin-left: var(--tn-space-xxs);\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n  user-select: none;\n}\n\nh1:hover a.headlink,\nh2:hover a.headerlink,\nh3:hover a.headerlink,\nh4:hover a.headerlink,\nh5:hover a.headerlink,\nh6:hover a.headerlink,\n.code-block-caption:hover a.headerlink {\n  opacity: 0.5;\n}\n\na.headerlink:hover {\n  opacity: 1;\n}\n\n.highlight {\n  margin: 0;\n  margin-left: calc(-1 * var(--tn-space-xs-fixed));\n  padding: var(--tn-space-xs-fixed);\n  overflow-x: auto;\n  border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n\n.literal-block-wrapper {\n  margin-left: calc(-1 * var(--tn-space-xs-fixed));\n  padding-left: var(--tn-space-xs-fixed);\n  border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n\n.literal-block-wrapper .highlight {\n  border: none;\n}\n\n.code-block-caption {\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-bottom: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius) 0 0;\n  padding: var(--tn-space-xxxs-fixed) var(--tn-space-xs-fixed);\n  margin-left: calc(-1 * var(--tn-space-xs-fixed));\n}\n\n.admonition {\n  border: var(--tn-sphinx-code-block-border-thickness) solid var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n  padding: var(--tn-space-xs-fixed);\n  margin-bottom: 1rem;\n}\n\n.admonition :last-child {\n  margin-bottom: 0;\n}\n\n.admonition-title {\n  font-weight: bold;\n  margin: calc(-1 * var(--tn-space-xs-fixed));\n  padding: var(--tn-space-xs-fixed);\n  border-radius: var(--tn-sphinx-code-block-border-radius) var(--tn-sphinx-code-block-border-radius) 0 0;\n  font-size: 0.9rem;\n}\n\n.admonition.attention .admonition-title,\n.admonition.caution .admonition-title,\n.admonition.warning .admonition-title,\n.admonition.important .admonition-title {\n  background-color: var(--tn-color-yellow-100);\n}\n\n.admonition.attention,\n.admonition.caution,\n.admonition.warning,\n.admonition.important {\n  border-color: var(--tn-color-yellow-500);\n}\n\n.admonition.danger .admonition-title,\n.admonition.error .admonition-title {\n  background-color: var(--tn-color-red-100);\n}\n\n.admonition.danger,\n.admonition.error {\n  border-color: var(--tn-color-red-500);\n}\n\n.admonition.tip .admonition-title,\n.admonition.note .admonition-title,\n.admonition.hint .admonition-title {\n  background-color: var(--tn-color-blue-100);\n}\n\n.admonition.tip,\n.admonition.note,\n.admonition.hint {\n  border-color: var(--tn-color-blue-500);\n}\n\n.footnote-list .footnote {\n  font-size: 0.9rem;\n  margin-bottom: 0.5rem;\n  display: flex;\n  flex-direction: row;\n  align-items: baseline;\n}\n\n.footnote-list .footnote .label {\n  display: block;\n  min-width: 1.5rem;\n}\n\n.footnote-list .footnote .label a,\n.footnote-reference {\n  background-color: var(--tn-sphinx-footnote-label-background-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-color);\n  border-radius: 4px;\n  padding: 2px 4px;\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.footnote-list .footnote .label a:hover,\n.footnote-reference:hover {\n  background-color: var(--tn-sphinx-footnote-label-background-hover-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-hover-color);\n}\n\n.footnote .fn-bracket,\n.footnote-reference .fn-bracket {\n  display: none;\n}\n\n.citation p {\n  display: inline;\n}\n\n.citation .label a {\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.citation .label a:hover {\n  text-decoration: underline;\n}\n\nblockquote {\n  border-left: 0.25rem solid var(--tn-color-primary);\n  margin-left: 0;\n  padding-left: 1rem;\n}\n\nblockquote .attribution {\n  font-style: italic;\n}\n\nmain li p {\n  margin-top: 0;\n  margin-bottom: 0;\n}\n\n.block-list p {\n  margin-top: 1rem;\n  margin-bottom: 1rem;\n}\n\ndt {\n  font-weight: bold;\n}\n\ndd {\n  margin-left: 2rem;\n}\n\ndd p:first-of-type {\n  margin-top: 0.2rem;\n}\n\nimg {\n  max-width: 100%;\n}\n\nfigure {\n  margin-left: 0;\n  margin-right: 0;\n}\n\nfigure img {\n  max-width: 100%;\n}\n\nfigcaption {\n  width: 100%;\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-radius: 4px;\n  padding: 0.5rem 1rem;\n  margin: 0;\n  border: none;\n}\n\nfigcaption p {\n  margin-top: 0;\n  margin-bottom: 1em;\n  padding: 0;\n}\n\nfigcaption p:last-child {\n  margin-bottom: 0;\n}\n\n.technote-table {\n  max-width: 100%;\n  overflow-x: auto;\n}\n\ntable {\n  max-width: fit-content;\n  margin: 0 auto 0 0;\n  white-space: nowrap;\n  font-size: 0.9rem;\n  font-variant-numeric: lining-nums tabular-nums;\n  border-collapse: collapse;\n}\n\nth {\n  font-weight: normal;\n}\n\nthead {\n  border-bottom: 1px solid var(--tn-component-text-color);\n}\n\ntd,\nth {\n  padding: 0.125em 0.5em 0.25em 0.5em;\n  line-height: 1;\n  text-align: inherit;\n}\n\ntd {\n  text-align: \".\" center;\n}\n\ntable caption {\n  caption-side: bottom;\n}\n\n.technote-article-header-id {\n  font-size: var(--tn-component-h4-size);\n  font-weight: bold;\n}\n\n/*\n * Icon Metadata Lists consist of a an icon paired with a metadata value.\n * The value can span multiple lines, but will always be indented beside\n * the icon.\n */\n.technote-icon-metadata {\n  display: flex;\n  flex-direction: row;\n  justify-content: flex-start;\n  align-items: baseline;\n  gap: var(--tn-space-xxs-fixed);\n}\n\n.technote-icon-metadata__icon {\n  width: 1em;\n  flex-grow: 0;\n  flex-shrink: 0;\n  margin: 0;\n}\n\n.technote-icon-metadata__value {\n  flex-grow: 1;\n  margin: 0;\n}\n\n/*\n * Styles for the author list that appears below the title.\n */\n.technote-status + .technote-inline-authors {\n  margin-top: 2rem;\n}\n\n/* The container for the primary sidebar */\n@media (min-width: 76rem) {\n  .technote-sidebar-container {\n    position: sticky;\n    top: 1rem;\n    overflow-y: auto;\n    max-height: 100vh;\n  }\n}\n:root {\n  --tn-component-sidebar-header-color: var(--tn-color-neutral-600);\n}\n\nhtml[data-theme=dark] {\n  --tn-component-sidebar-header-color: var(--tn-color-neutral-200);\n}\n\n.technote-sidebar-section {\n  margin: 0 0 var(--tn-space-lg-fixed);\n}\n\n.technote-sidebar-section:first-of-type {\n  margin-top: var(--tn-space-lg-fixed);\n}\n\n.technote-sidebar-section__heading {\n  font-size: var(--tn-component-h6-size);\n  font-weight: bold;\n  color: var(--tn-component-sidebar-header-color);\n  margin-bottom: 0.5rem;\n}\n\n.technote-sidebar-section__heading + * {\n  margin-top: var(--tn-space-xs-fixed);\n}\n\n.technote-sidebar-author-list {\n  margin-top: var(--tn-space-xs-fixed);\n}\n\n.technote-sidebar-metadata-list {\n  margin-top: var(--tn-space-xs-fixed);\n  margin-bottom: var(--tn-space-xs-fixed);\n  list-style-type: none;\n  padding: 0;\n}\n\n/*\n * Styles for the sidebar-logo component.\n */\n.technote-sidebar-logo__picture {\n  max-width: 12rem;\n}\n\n/* Styles for the document status aside */\n.technote-status {\n  border: 1px solid var(--tn-component-text-color);\n  padding: 1rem;\n  border-radius: var(--tn-border-radius-1);\n}\n\n.technote-status--deprecated {\n  border-color: var(--tn-color-red-500);\n}\n\n.technote-status p:first-of-type {\n  margin-top: 0;\n}\n\n.technote-status *:last-child {\n  margin-bottom: 0;\n}\n\n.technote-svg-icon {\n  width: 0.85em;\n  height: 0.85em;\n  display: inline;\n  fill: currentColor;\n}\n\na .technote-svg-icon {\n  fill: var(--tn-component-text-color);\n}\n\n/*\n * Local TOC styling.\n */\n:root {\n  --tn-component-toc-header-color: var(--tn-color-neutral-600);\n  --tn-component-toc-level-border-color: var(--tn-color-neutral-600);\n}\n\nhtml[data-theme=dark] {\n  --tn-component-toc-header-color: var(--tn-color-neutral-200);\n  --tn-component-toc-level-border-color: var(--tn-color-neutral-200);\n}\n\n.technote-toc {\n  overflow-y: auto;\n  max-height: 100vh;\n}\n\n@media (min-width: 59rem) {\n  .technote-toc {\n    position: sticky;\n    top: 1rem;\n    margin-top: 20vh;\n    margin-left: 2rem;\n  }\n}\n.technote-toc-header {\n  margin: 0 0 1rem;\n  font-size: var(--tn-component-h4-size);\n  font-weight: bold;\n  color: var(--tn-component-toc-header-color);\n}\n\n.technote-toc-container {\n  line-height: 1.2;\n  /* Spacing between items in the toc */\n  --technote-toc-container-spacing: var(--tn-space-xs-fixed);\n}\n\n.technote-toc-container a {\n  text-decoration: none;\n}\n\n.technote-toc-container a:hover {\n  text-decoration: underline;\n}\n\n.technote-toc-container ul {\n  list-style-type: none;\n  padding-left: var(--tn-space-xs-fixed);\n  margin-left: var(--tn-space-xxs-fixed);\n  border-left: 2px solid var(--tn-component-toc-level-border-color);\n  margin-top: var(--technote-toc-container-spacing);\n}\n\n/* Root-level sections aren't indented */\n.technote-toc-container > ul {\n  margin-left: 0;\n  padding-left: 0;\n  border-left: none;\n  margin-top: 0;\n}\n\n.technote-toc-container li {\n  margin-bottom: var(--technote-toc-container-spacing);\n}\n\n/*\n * Utilities for displaying different elements based on the current theme.\n */\nhtml[data-theme=light] .technote-themed-dark {\n  display: none;\n}\n\nhtml[data-theme=dark] .technote-themed-light {\n  display: none;\n}\n\n.technote-icon-pair-list {\n  list-style: none;\n  margin-left: 0;\n  padding-left: 0;\n}\n\n/*\n * comma-list makes a ul an inline list with grammatical comma separated\n * items.\n */\n.technote-inline-comma-list {\n  list-style: none;\n  margin-left: 0;\n  padding-left: 0;\n}\n\n.technote-inline-comma-list li {\n  display: inline;\n}\n\n.technote-inline-comma-list li:after {\n  content: \", \";\n}\n\n.technote-inline-comma-list li:last-child:after {\n  content: \"\";\n}\n\n.technote-inline-comma-list li:nth-last-child(2):after {\n  content: \" and \";\n}\n\n.technote-inline-comma-list li:nth-last-child(3) ~ li:nth-last-child(2):after {\n  content: \", and \";\n}\n\n/*\n * Hiding class, making content visible only to screen readers but not visually\n * \"sr\" meaning \"screen-reader\"\n * https://css-tricks.com/inclusively-hidden/\n */\n.sr-only:not(:focus):not(:active) {\n  clip: rect(0 0 0 0);\n  clip-path: inset(50%);\n  height: 1px;\n  overflow: hidden;\n  position: absolute;\n  white-space: nowrap;\n  width: 1px;\n}",
         ":root {\n  /*\n   * Color design tokens.\n   *\n   * These are based on GitHub Primer.\n   * https://primer.style/prism/local/a4751264-de23-430e-a2fc-669488065638/scale/c2a0938a-e1dc-4b20-a07b-e2778ae57f41\n   */\n  --tn-color-black: #1b1f24;\n  --tn-color-white: #ffffff;\n\n  --tn-color-neutral-000: #f6f8fa;\n  --tn-color-neutral-100: #eaeef2;\n  --tn-color-neutral-200: #d0d7de;\n  --tn-color-neutral-300: #afb8c1;\n  --tn-color-neutral-400: #8c959f;\n  --tn-color-neutral-500: #6e7781;\n  --tn-color-neutral-600: #57606a;\n  --tn-color-neutral-700: #424a53;\n  --tn-color-neutral-800: #32383f;\n  --tn-color-neutral-900: #24292f;\n\n  --tn-color-blue-000: #ddf4ff;\n  --tn-color-blue-100: #b6e3ff;\n  --tn-color-blue-200: #80ccff;\n  --tn-color-blue-300: #54aeff;\n  --tn-color-blue-400: #218bff;\n  --tn-color-blue-500: #0969da;\n  --tn-color-blue-600: #0550ae;\n  --tn-color-blue-700: #033d8b;\n  --tn-color-blue-800: #0a3069;\n  --tn-color-blue-900: #002155;\n\n  --tn-color-green-000: #dafbe1;\n  --tn-color-green-100: #aceebb;\n  --tn-color-green-200: #6fdd8b;\n  --tn-color-green-300: #4ac26b;\n  --tn-color-green-400: #2da44e;\n  --tn-color-green-500: #1a7f37;\n  --tn-color-green-600: #116329;\n  --tn-color-green-700: #044f1e;\n  --tn-color-green-800: #003d16;\n  --tn-color-green-900: #002d11;\n\n  --tn-color-yellow-000: #fff8c5;\n  --tn-color-yellow-100: #fae17d;\n  --tn-color-yellow-200: #eac54f;\n  --tn-color-yellow-300: #d4a72c;\n  --tn-color-yellow-400: #bf8700;\n  --tn-color-yellow-500: #9a6700;\n  --tn-color-yellow-600: #7d4e00;\n  --tn-color-yellow-700: #633c01;\n  --tn-color-yellow-800: #4d2d00;\n  --tn-color-yellow-900: #3b2300;\n\n  --tn-color-orange-000: #fff1e5;\n  --tn-color-orange-100: #ffd8b5;\n  --tn-color-orange-200: #ffb77c;\n  --tn-color-orange-300: #fb8f44;\n  --tn-color-orange-400: #e16f24;\n  --tn-color-orange-500: #bc4c00;\n  --tn-color-orange-600: #953800;\n  --tn-color-orange-700: #762c00;\n  --tn-color-orange-800: #5c2200;\n  --tn-color-orange-900: #471700;\n\n  --tn-color-red-000: #ffebe9;\n  --tn-color-red-100: #ffcecb;\n  --tn-color-red-200: #ffaba8;\n  --tn-color-red-300: #ff8182;\n  --tn-color-red-400: #fa4549;\n  --tn-color-red-500: #cf222e;\n  --tn-color-red-600: #a40e26;\n  --tn-color-red-700: #82071e;\n  --tn-color-red-800: #660018;\n  --tn-color-red-900: #4c0014;\n\n  --tn-color-purple-000: #fbefff;\n  --tn-color-purple-100: #ecd8ff;\n  --tn-color-purple-200: #d8b9ff;\n  --tn-color-purple-300: #c297ff;\n  --tn-color-purple-400: #a475f9;\n  --tn-color-purple-500: #8250df;\n  --tn-color-purple-600: #6639ba;\n  --tn-color-purple-700: #512a97;\n  --tn-color-purple-800: #3e1f79;\n  --tn-color-purple-900: #2e1461;\n\n  --tn-color-pink-000: #ffeff7;\n  --tn-color-pink-100: #ffd3eb;\n  --tn-color-pink-200: #ffadda;\n  --tn-color-pink-300: #ff80c8;\n  --tn-color-pink-400: #e85aad;\n  --tn-color-pink-500: #bf3989;\n  --tn-color-pink-600: #99286e;\n  --tn-color-pink-700: #772057;\n  --tn-color-pink-800: #611347;\n  --tn-color-pink-900: #4d0336;\n\n  --tn-color-coral-000: #fff0eb;\n  --tn-color-coral-100: #ffd6cc;\n  --tn-color-coral-200: #ffb4a1;\n  --tn-color-coral-300: #fd8c73;\n  --tn-color-coral-400: #ec6547;\n  --tn-color-coral-500: #c4432b;\n  --tn-color-coral-600: #9e2f1c;\n  --tn-color-coral-700: #801f0f;\n  --tn-color-coral-800: #691105;\n  --tn-color-coral-900: #510901;\n\n  // Primary color\n  --tn-color-primary: var(--tn-color-neutral-900);\n  --tn-color-primary-000: var(--tn-color-neutral-000);\n  --tn-color-primary-100: var(--tn-color-neutral-100);\n  --tn-color-primary-200: var(--tn-color-neutral-200);\n  --tn-color-primary-300: var(--tn-color-neutral-300);\n  --tn-color-primary-400: var(--tn-color-neutral-400);\n  --tn-color-primary-500: var(--tn-color-neutral-500);\n  --tn-color-primary-600: var(--tn-color-neutral-600);\n  --tn-color-primary-700: var(--tn-color-neutral-700);\n  --tn-color-primary-800: var(--tn-color-neutral-800);\n  --tn-color-primary-900: var(--tn-color-neutral-900);\n}\n",
         ":root {\n  /*\n   * Spacing values in em units\n   */\n  --tn-space-unit: 1em;\n  --tn-space-xxxs: calc(0.25 * var(--tn-space-unit));\n  --tn-space-xxs: calc(0.375 * var(--tn-space-unit));\n  --tn-space-xs: calc(0.5 * var(--tn-space-unit));\n  --tn-space-sm: calc(0.75 * var(--tn-space-unit));\n  --tn-space-md: calc(1.25 * var(--tn-space-unit));\n  --tn-space-lg: calc(2 * var(--tn-space-unit));\n  --tn-space-xl: calc(3.25 * var(--tn-space-unit));\n  --tn-space-xxl: calc(5.25 * var(--tn-space-unit));\n  --tn-space-xxxl: calc(8.5 * var(--tn-space-unit));\n\n  /*\n    * Fixed spacing\n    * These aren't affected by --space-unit or the root font size\n    */\n  --tn-space-unit-fixed: 1rem;\n  --tn-space-xxxs-fixed: calc(0.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxs-fixed: calc(0.375 * var(--tn-space-unit-fixed));\n  --tn-space-xs-fixed: calc(0.5 * var(--tn-space-unit-fixed));\n  --tn-space-sm-fixed: calc(0.75 * var(--tn-space-unit-fixed));\n  --tn-space-md-fixed: calc(1.25 * var(--tn-space-unit-fixed));\n  --tn-space-lg-fixed: calc(2 * var(--tn-space-unit-fixed));\n  --tn-space-xl-fixed: calc(3.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxl-fixed: calc(5.25 * var(--tn-space-unit-fixed));\n  --tn-space-xxxl-fixed: calc(8.5 * var(--tn-space-unit-fixed));\n}\n",
         ":root {\n  /*\n   * Border radius\n   */\n  --tn-border-radius-0: 0px;\n  --tn-border-radius-1: 4px;\n  --tn-border-radius-2: 7px;\n}\n",
-        ":root {\n  /*\n   * Typographic design tokens.\n   */\n  --tn-component-h1-size: 3.052rem;\n  --tn-component-h2-size: 2.441rem;\n  --tn-component-h3-size: 1.563rem;\n  --tn-component-h4-size: 1.25rem;\n  --tn-component-h5-size: 1rem;\n  --tn-component-h6-size: 0.8rem;\n\n  --tn-component-h1-weight: normal;\n  --tn-component-h2-weight: normal;\n  --tn-component-h3-weight: bold;\n  --tn-component-h4-weight: bold;\n  --tn-component-h5-weight: bold;\n  --tn-component-h6-weight: bold;\n\n  --tn-component-text-color: var(--tn-color-black);\n  --tn-component-link-color: var(--tn-color-blue-500);\n  --tn-component-text-background-color: var(--tn-color-white);\n\n  --tn-component-text-font-family: -apple-system, BlinkMacSystemFont, Segoe UI,\n    Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans, Droid Sans, Helvetica Neue,\n    sans-serif;\n  --tn-component-text-line-height: 1.5;\n}\n\nhtml[data-theme='dark'] {\n  --tn-component-text-color: var(--tn-color-white);\n  --tn-component-link-color: var(--tn-color-blue-300);\n  --tn-component-text-background-color: var(--tn-color-black);\n}\n",
+        ":root {\n  /*\n   * Typographic design tokens.\n   */\n  --tn-component-h1-size: 3.052rem;\n  --tn-component-h2-size: 2.441rem;\n  --tn-component-h3-size: 1.563rem;\n  --tn-component-h4-size: 1.25rem;\n  --tn-component-h5-size: 1.1rem;\n  --tn-component-h6-size: 1rem;\n\n  --tn-component-h1-weight: normal;\n  --tn-component-h2-weight: normal;\n  --tn-component-h3-weight: bold;\n  --tn-component-h4-weight: bold;\n  --tn-component-h5-weight: bold;\n  --tn-component-h6-weight: bold;\n\n  --tn-component-text-font-size: 1.1rem;\n  --tn-component-text-color: var(--tn-color-black);\n  --tn-component-link-color: var(--tn-color-blue-500);\n  --tn-component-text-background-color: var(--tn-color-white);\n\n  --tn-component-text-font-family: -apple-system, ui-sans-serif,\n    BlinkMacSystemFont, Segoe UI, Roboto, Oxygen, Ubuntu, Cantarell, Fira Sans,\n    Droid Sans, Helvetica Neue, sans-serif;\n  --tn-component-text-line-height: 1.5;\n\n  --tn-component-code-font-family: ui-monospace, monospace;\n}\n\nhtml[data-theme='dark'] {\n  --tn-component-text-color: var(--tn-color-white);\n  --tn-component-link-color: var(--tn-color-blue-300);\n  --tn-component-text-background-color: var(--tn-color-black);\n}\n",
         "/* Properties for Sphinx components. */\n\n:root {\n  --tn-sphinx-code-block-border-color: var(--tn-color-primary);\n  --tn-sphinx-code-block-border-thickness: 1px;\n  --tn-sphinx-code-block-border-radius: var(--tn-border-radius-1);\n  --tn-sphinx-code-block-caption-background-color: var(--tn-color-primary-000);\n  --tn-sphinx-footnote-label-background-color: var(--tn-color-blue-000);\n  --tn-sphinx-footnote-label-border-color: var(--tn-color-blue-100);\n  --tn-sphinx-footnote-label-background-hover-color: var(--tn-color-blue-100);\n  --tn-sphinx-footnote-label-border-hover-color: var(--tn-color-blue-200);\n}\n\nhtml[data-theme='dark'] {\n  --tn-sphinx-code-block-border-color: var(--tn-color-primary-700);\n  --tn-sphinx-code-block-caption-background-color: var(--tn-color-primary-900);\n  --tn-sphinx-footnote-label-background-color: var(--tn-color-blue-900);\n  --tn-sphinx-footnote-label-border-color: var(--tn-color-blue-800);\n  --tn-sphinx-footnote-label-background-hover-color: var(--tn-color-blue-800);\n  --tn-sphinx-footnote-label-border-hover-color: var(--tn-color-blue-700);\n}\n",
-        "/*\n * Styles that affect the overall layout. Since Technote is built on\n * sphinx-basic-ng as the base theme, these styles primarily work with\n * the base theme's sb- classes.\n */\n\n.sb-container {\n  margin-top: var(--tn-space-md-fixed);\n}\n\n/* Style the prmary sidebar when it's a popover. */\n#sb-sidebar-toggle--primary:checked ~ .sb-container .sb-sidebar-primary {\n  background-color: white;\n  box-shadow: 10px 5px 5px rgb(161, 161, 161);\n  border-right: 1px solid black;\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .sb-sidebar-secondary {\n  background-color: white;\n  box-shadow: -5px 0 5px rgb(161, 161, 161);\n  border-left: 1px solid black;\n  padding-left: var(--tn-space-md-fixed);\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .technote-toc-header {\n  margin-top: var(--tn-space-md-fixed);\n}\n\n.sb-sidebar-overlay {\n  // Fuzz out the content slightly\n  backdrop-filter: blur(1.5px) opacity(0.7) brightness(150%);\n  background-color: rgba(0, 0, 0, 0);\n}\n\n// The \"primary\" header contains the controls for the sidebars\n.sb-header__inner {\n  display: flex;\n  justify-content: space-between;\n}\n\n.sb-header__inner label {\n  margin: var(--tn-space-xs-fixed);\n}\n\n/* Highlight key containers for debugging. */\n// .sb-article {\n//   border: 1px solid red;\n// }\n// .sb-sidebar-secondary {\n//   border: 1px solid blue;\n// }\n// .sb-sidebar-primary {\n//   border: 1px solid green;\n// }\n\n/*\n * Content container width.\n * Goal is to have a content width <= 80 characters. These override\n * breakpoint settings from sphinx-basic-ng's skeleton.css\n */\n.sb-article-container,\n.sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n  /* reset skeleton.css. Using 100vw means we get horizontal scrollbars. */\n  width: auto;\n}\n\n@media (max-width: 42rem) {\n  .sb-article-container,\n  .sb-footer-content__inner {\n    width: 100vw;\n  }\n\n  body {\n    // experiment with using hyphens on phones\n    hyphens: auto;\n  }\n}\n\n@media (min-width: 42rem) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 38rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 38rem;\n  }\n  // h1::after {\n  //   content: ' 42';\n  // }\n}\n@media (min-width: 46rem) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 40rem;\n  }\n  // h1::after {\n  //   content: ' 46';\n  // }\n}\n@media (min-width: 50rem) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 50';\n  } */\n}\n@media (min-width: 59rem) {\n  /* secondary sidebar appears, width is 17rem. */\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 36rem;\n  }\n  /* h1::after {\n    content: ' 59';\n  } */\n}\n@media (min-width: 63rem) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 36rem;\n  }\n  /* h1::after {\n    content: ' 63';\n  } */\n}\n@media (min-width: 67rem) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 67';\n  } */\n}\n@media (min-width: 76rem) {\n  /* The primary sidebar appears */\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 32rem;\n  }\n\n  // Reset the pop-over specific styling for the sidebar.\n  .sb-sidebar-primary {\n    box-shadow: none;\n    border-right: none;\n  }\n  /* h1::after {\n    content: ' 76';\n  } */\n}\n@media (min-width: 80rem) {\n  .sb-article,\n  .match-content-width {\n    width: 34rem;\n  }\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 80';\n  } */\n}\n@media (min-width: 84rem) {\n  .sb-article,\n  .match-content-width {\n    width: 40rem;\n  }\n  /* h1::after {\n    content: ' 84';\n  } */\n}\n@media (min-width: 88rem) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40rem;\n  }\n  .sb-page-width {\n    width: 86rem;\n  }\n  /* h1::after {\n    content: ' 88';\n  } */\n}\n\n/*\n * Primary sidebar\n */\n.sb-sidebar-primary {\n  padding: var(--tn-space-md-fixed);\n}\n",
-        "/*\n * Typography.\n */\nbody {\n  font-family: var(--tn-component-text-font-family);\n  line-height: var(--tn-component-text-line-height);\n  color: var(--tn-component-text-color);\n  background: var(--tn-component-text-background-color);\n}\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n  /* Put header vertically closer to its own section. */\n  margin: 1.5em 0 0.8em;\n  line-height: 1.2;\n}\n\nh1 {\n  font-size: var(--tn-component-h1-size);\n  font-weight: var(--tn-component-h1-weight);\n  margin: 0 0 1em;\n}\n\nh2 {\n  font-size: var(--tn-component-h2-size);\n  font-weight: var(--tn-component-h2-weight);\n}\n\nh3 {\n  font-size: var(--tn-component-h3-size);\n  font-weight: var(--tn-component-h3-weight);\n}\n\nh4 {\n  font-size: var(--tn-component-h4-size);\n  font-weight: var(--tn-component-h4-weight);\n}\n\nh5 {\n  font-size: var(--tn-component-h5-size);\n  font-weight: var(--tn-component-h5-weight);\n}\n\nh6 {\n  font-size: var(--tn-component-h6-size);\n  font-weight: var(--tn-component-h6-weight);\n}\n\n/* Handle Sphinx's built-in permalink icon. */\nh1 .headerlink,\nh2 .headerlink,\nh3 .headerlink,\nh4 .headerlink,\nh5 .headerlink,\nh6 .headerlink {\n  visibility: hidden;\n  text-decoration: none;\n}\nh1:hover .headerlink,\nh2:hover .headerlink,\nh3:hover .headerlink,\nh4:hover .headerlink,\nh5:hover .headerlink,\nh6:hover .headerlink {\n  visibility: visible;\n}\n\na {\n  color: var(--tn-component-link-color);\n}\n",
-        "/* Styles Sphinx-generated content classes */\n\na.headerlink {\n  opacity: 0; // Hide the anchor link unless hovered over.\n  font-size: 0.9em;\n  margin-left: var(--tn-space-xxs);\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n  user-select: none;\n}\n\nh1:hover a.headlink,\nh2:hover a.headerlink,\nh3:hover a.headerlink,\nh4:hover a.headerlink,\nh5:hover a.headerlink,\nh6:hover a.headerlink,\n.code-block-caption:hover a.headerlink {\n  // If the user hovers over the caption/header, then begin to show the anchor\n  // link.\n  opacity: 0.5;\n}\n\na.headerlink:hover {\n  opacity: 1;\n}\n\npre {\n  font-size: 0.85rem;\n}\n\n.literal-block-wrapper .highlight pre {\n  margin: 0;\n  padding: var(--tn-space-xs-fixed);\n  overflow-x: auto;\n}\n\n.literal-block-wrapper {\n  border: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n\n.literal-block-wrapper .highlight {\n  // This border radius ensures the pygments background on .highlight doesn't\n  // interfere with the border radius of the .literal-block-wrapper.\n  border-radius: 0 0 var(--tn-sphinx-code-block-border-radius)\n    var(--tn-sphinx-code-block-border-radius);\n}\n\n.code-block-caption {\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-bottom: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius)\n    var(--tn-sphinx-code-block-border-radius) 0 0;\n  padding: var(--tn-space-xxxs-fixed) var(--tn-space-xs-fixed);\n}\n\n.admonition {\n  border: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n  padding: var(--tn-space-xs-fixed);\n  margin-bottom: 1rem;\n}\n\n.admonition :last-child {\n  margin-bottom: 0;\n}\n\n.admonition-title {\n  font-weight: bold;\n  margin: calc(-1 * var(--tn-space-xs-fixed));\n  padding: var(--tn-space-xs-fixed);\n  border-radius: var(--tn-sphinx-code-block-border-radius)\n    var(--tn-sphinx-code-block-border-radius) 0 0;\n  font-size: 0.9rem;\n}\n\n.admonition.attention .admonition-title,\n.admonition.caution .admonition-title,\n.admonition.warning .admonition-title,\n.admonition.important .admonition-title {\n  background-color: var(--tn-color-yellow-100);\n}\n\n.admonition.attention,\n.admonition.caution,\n.admonition.warning,\n.admonition.important {\n  border-color: var(--tn-color-yellow-500);\n}\n\n.admonition.danger .admonition-title,\n.admonition.error .admonition-title {\n  background-color: var(--tn-color-red-100);\n}\n\n.admonition.danger,\n.admonition.error {\n  border-color: var(--tn-color-red-500);\n}\n\n.admonition.tip .admonition-title,\n.admonition.note .admonition-title,\n.admonition.hint .admonition-title {\n  background-color: var(--tn-color-blue-100);\n}\n\n.admonition.tip,\n.admonition.note,\n.admonition.hint {\n  border-color: var(--tn-color-blue-500);\n}\n\n.footnote-list .footnote {\n  font-size: 0.9rem;\n  margin-bottom: 0.5rem;\n  display: flex;\n  flex-direction: row;\n  align-items: baseline;\n}\n\n.footnote-list .footnote .label {\n  display: block;\n  min-width: 1.5rem;\n}\n\n.footnote-list .footnote .label a,\n.footnote-reference {\n  background-color: var(--tn-sphinx-footnote-label-background-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-color);\n  border-radius: 4px;\n  padding: 2px 4px;\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.footnote-list .footnote .label a:hover,\n.footnote-reference:hover {\n  background-color: var(--tn-sphinx-footnote-label-background-hover-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-hover-color);\n}\n\n.footnote .fn-bracket,\n.footnote-reference .fn-bracket {\n  display: none;\n}\n\n.citation p {\n  // put the citation on the same line as the backlink.\n  display: inline;\n}\n\n.citation .label a {\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.citation .label a:hover {\n  text-decoration: underline;\n}\n\nblockquote {\n  border-left: 0.25rem solid var(--tn-color-primary);\n  margin-left: 0;\n  padding-left: 1rem;\n}\n\nblockquote .attribution {\n  font-style: italic;\n}\n\nmain li p {\n  margin-top: 0;\n  margin-bottom: 0;\n}\n\n.block-list p {\n  margin-top: 1rem;\n  margin-bottom: 1rem;\n}\n\ndt {\n  font-weight: bold;\n}\n\ndd {\n  margin-left: 2rem;\n}\n\ndd p:first-of-type {\n  margin-top: 0.2rem;\n}\n\n// Ensure bare img elements don't extend beyond the column\nimg {\n  max-width: 100%;\n}\n\nfigure {\n  margin-left: 0;\n  margin-right: 0;\n}\n\nfigure img {\n  max-width: 100%;\n}\n\nfigcaption {\n  width: 100%;\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-radius: 4px;\n  padding: 0.5rem 1rem;\n  margin: 0;\n  border: none;\n  // margin-top: -7px; // where does this extra margin come from?\n}\n\nfigcaption p {\n  margin-top: 0;\n  margin-bottom: 1em;\n  padding: 0;\n}\n\nfigcaption p:last-child {\n  margin-bottom: 0;\n}\n\n// The .technote-table class is associated with figure elements that wrap\n// tables. This figure is added by the warptables Sphinx extension in\n// technote. It allows us to make a table with overflow-x while avoiding\n// setting the display property of table itself to block, which is bad for\n// accessibility.\n// https://www.tpgi.com/short-note-on-what-css-display-properties-do-to-table-semantics/\n.technote-table {\n  max-width: 100%;\n  overflow-x: auto;\n}\n\ntable {\n  max-width: fit-content;\n  margin: 0 auto 0 0;\n  white-space: nowrap;\n\n  font-size: 0.9rem;\n  font-variant-numeric: lining-nums tabular-nums;\n  border-collapse: collapse;\n}\n\nth {\n  font-weight: normal;\n}\n\nthead {\n  border-bottom: 1px solid var(--tn-component-text-color);\n}\n\ntd,\nth {\n  padding: 0.125em 0.5em 0.25em 0.5em;\n  line-height: 1;\n  text-align: inherit;\n}\n\ntd {\n  // Attempt to align numbers on decimal points; this probably isn't supported?\n  text-align: '.' center;\n}\n\ntable caption {\n  caption-side: bottom;\n}\n",
+        "/*\n * Styles that affect the overall layout. Since Technote is built on\n * sphinx-basic-ng as the base theme, these styles primarily work with\n * the base theme's sb- classes.\n */\n\n.sb-container {\n  margin-top: var(--tn-space-md-fixed);\n  margin-bottom: var(--tn-space-xxl-fixed);\n}\n\n/* Style the prmary sidebar when it's a popover. */\n#sb-sidebar-toggle--primary:checked ~ .sb-container .sb-sidebar-primary {\n  background-color: white;\n  box-shadow: 10px 5px 5px rgb(161, 161, 161);\n  border-right: 1px solid black;\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .sb-sidebar-secondary {\n  background-color: white;\n  box-shadow: -5px 0 5px rgb(161, 161, 161);\n  border-left: 1px solid black;\n  padding-left: var(--tn-space-md-fixed);\n}\n\n#sb-sidebar-toggle--secondary:checked ~ .sb-container .technote-toc-header {\n  margin-top: var(--tn-space-md-fixed);\n}\n\n.sb-sidebar-overlay {\n  // Fuzz out the content slightly\n  backdrop-filter: blur(1.5px) opacity(0.7) brightness(150%);\n  background-color: rgba(0, 0, 0, 0);\n}\n\n// The \"primary\" header contains the controls for the sidebars\n.sb-header__inner {\n  display: flex;\n  justify-content: space-between;\n}\n\n.sb-header__inner label {\n  margin: var(--tn-space-xs-fixed);\n}\n\n/* Highlight key containers for debugging. */\n// .sb-article {\n//   border: 1px solid red;\n// }\n// .sb-sidebar-secondary {\n//   border: 1px solid blue;\n// }\n// .sb-sidebar-primary {\n//   border: 1px solid green;\n// }\n\n/*\n * Content container width.\n * Goal is to have a content width <= 80 characters. These override\n * breakpoint settings from sphinx-basic-ng's skeleton.css\n */\n.sb-article-container,\n.sb-footer-content__inner,\n.drop-secondary-sidebar-for-full-width-content .sb-article,\n.drop-secondary-sidebar-for-full-width-content .match-content-width {\n  /* reset skeleton.css. Using 100vw means we get horizontal scrollbars. */\n  width: auto;\n}\n\n@media (max-width: 42em) {\n  .sb-article-container,\n  .sb-footer-content__inner {\n    width: 100vw;\n  }\n\n  body {\n    // experiment with using hyphens on phones\n    hyphens: auto;\n  }\n}\n\n@media (min-width: 42em) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 38em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 38em;\n  }\n  // h1::after {\n  //   content: ' 42';\n  // }\n}\n@media (min-width: 46em) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 40em;\n  }\n  // h1::after {\n  //   content: ' 46';\n  // }\n}\n@media (min-width: 50em) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 50';\n  } */\n}\n@media (min-width: 59em) {\n  /* secondary sidebar appears, width is 17rem. */\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 36em;\n  }\n  /* h1::after {\n    content: ' 59';\n  } */\n}\n@media (min-width: 63em) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 36em;\n  }\n  /* h1::after {\n    content: ' 63';\n  } */\n}\n@media (min-width: 67em) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 67';\n  } */\n}\n@media (min-width: 76em) {\n  /* The primary sidebar appears */\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-article,\n  .match-content-width {\n    width: 32em;\n  }\n\n  // Reset the pop-over specific styling for the sidebar.\n  .sb-sidebar-primary {\n    box-shadow: none;\n    border-right: none;\n  }\n  /* h1::after {\n    content: ' 76';\n  } */\n}\n@media (min-width: 80em) {\n  .sb-article,\n  .match-content-width {\n    width: 34em;\n  }\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 80';\n  } */\n}\n@media (min-width: 84em) {\n  .sb-article,\n  .match-content-width {\n    width: 40em;\n  }\n  /* h1::after {\n    content: ' 84';\n  } */\n}\n@media (min-width: 88em) {\n  .sb-footer-content__inner,\n  .drop-secondary-sidebar-for-full-width-content .sb-article,\n  .drop-secondary-sidebar-for-full-width-content .match-content-width {\n    width: 40em;\n  }\n  .sb-page-width {\n    width: 86em;\n  }\n  /* h1::after {\n    content: ' 88';\n  } */\n}\n\n/*\n * Primary sidebar\n */\n.sb-sidebar-primary {\n  padding: var(--tn-space-md-fixed);\n}\n",
+        "/*\n * Typography.\n */\nbody {\n  font-family: var(--tn-component-text-font-family);\n  line-height: var(--tn-component-text-line-height);\n  font-size: var(--tn-component-text-font-size);\n  color: var(--tn-component-text-color);\n  background: var(--tn-component-text-background-color);\n}\n\nh1,\nh2,\nh3,\nh4,\nh5,\nh6 {\n  /* Put header vertically closer to its own section. */\n  margin: 1.5em 0 0.8em;\n  line-height: 1.2;\n}\n\nh1 {\n  font-size: var(--tn-component-h1-size);\n  font-weight: var(--tn-component-h1-weight);\n  margin: 0 0 1em;\n}\n\nh2 {\n  font-size: var(--tn-component-h2-size);\n  font-weight: var(--tn-component-h2-weight);\n}\n\nh3 {\n  font-size: var(--tn-component-h3-size);\n  font-weight: var(--tn-component-h3-weight);\n}\n\nh4 {\n  font-size: var(--tn-component-h4-size);\n  font-weight: var(--tn-component-h4-weight);\n}\n\nh5 {\n  font-size: var(--tn-component-h5-size);\n  font-weight: var(--tn-component-h5-weight);\n}\n\nh6 {\n  font-size: var(--tn-component-h6-size);\n  font-weight: var(--tn-component-h6-weight);\n}\n\n/* Handle Sphinx's built-in permalink icon. */\nh1 .headerlink,\nh2 .headerlink,\nh3 .headerlink,\nh4 .headerlink,\nh5 .headerlink,\nh6 .headerlink {\n  visibility: hidden;\n  text-decoration: none;\n}\nh1:hover .headerlink,\nh2:hover .headerlink,\nh3:hover .headerlink,\nh4:hover .headerlink,\nh5:hover .headerlink,\nh6:hover .headerlink {\n  visibility: visible;\n}\n\na {\n  color: var(--tn-component-link-color);\n}\n\npre,\nxmp,\nplaintext,\nlisting {\n  font-family: var(--tn-component-code-font-family);\n  font-size: 1rem;\n}\n\ntt,\ncode,\nkbd,\nsamp {\n  font-family: var(--tn-component-code-font-family);\n\n  /* Making inline code slightly smaller seems to help with baseline alignment\n   * some monospace fonts seems bigger that Source Sans.\n   */\n  font-size: 0.9em;\n}\n",
+        "/* Styles Sphinx-generated content classes */\n\na.headerlink {\n  opacity: 0; // Hide the anchor link unless hovered over.\n  font-size: 0.9em;\n  margin-left: var(--tn-space-xxs);\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n  user-select: none;\n}\n\nh1:hover a.headlink,\nh2:hover a.headerlink,\nh3:hover a.headerlink,\nh4:hover a.headerlink,\nh5:hover a.headerlink,\nh6:hover a.headerlink,\n.code-block-caption:hover a.headerlink {\n  // If the user hovers over the caption/header, then begin to show the anchor\n  // link.\n  opacity: 0.5;\n}\n\na.headerlink:hover {\n  opacity: 1;\n}\n\n.highlight {\n  margin: 0;\n  margin-left: calc(-1 * var(--tn-space-xs-fixed));\n  padding: var(--tn-space-xs-fixed);\n  overflow-x: auto;\n  border: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n\n.literal-block-wrapper {\n  margin-left: calc(-1 * var(--tn-space-xs-fixed));\n  padding-left: var(--tn-space-xs-fixed);\n  border: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n}\n\n.literal-block-wrapper .highlight {\n  // If the code sample has a caption, then turn off its border so that the\n  // border comes from the overall wrapper (.literal-block-wrapper).\n  border: none;\n}\n\n.code-block-caption {\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-bottom: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius)\n    var(--tn-sphinx-code-block-border-radius) 0 0;\n  padding: var(--tn-space-xxxs-fixed) var(--tn-space-xs-fixed);\n  margin-left: calc(-1 * var(--tn-space-xs-fixed));\n}\n\n.admonition {\n  border: var(--tn-sphinx-code-block-border-thickness) solid\n    var(--tn-sphinx-code-block-border-color);\n  border-radius: var(--tn-sphinx-code-block-border-radius);\n  padding: var(--tn-space-xs-fixed);\n  margin-bottom: 1rem;\n}\n\n.admonition :last-child {\n  margin-bottom: 0;\n}\n\n.admonition-title {\n  font-weight: bold;\n  margin: calc(-1 * var(--tn-space-xs-fixed));\n  padding: var(--tn-space-xs-fixed);\n  border-radius: var(--tn-sphinx-code-block-border-radius)\n    var(--tn-sphinx-code-block-border-radius) 0 0;\n  font-size: 0.9rem;\n}\n\n.admonition.attention .admonition-title,\n.admonition.caution .admonition-title,\n.admonition.warning .admonition-title,\n.admonition.important .admonition-title {\n  background-color: var(--tn-color-yellow-100);\n}\n\n.admonition.attention,\n.admonition.caution,\n.admonition.warning,\n.admonition.important {\n  border-color: var(--tn-color-yellow-500);\n}\n\n.admonition.danger .admonition-title,\n.admonition.error .admonition-title {\n  background-color: var(--tn-color-red-100);\n}\n\n.admonition.danger,\n.admonition.error {\n  border-color: var(--tn-color-red-500);\n}\n\n.admonition.tip .admonition-title,\n.admonition.note .admonition-title,\n.admonition.hint .admonition-title {\n  background-color: var(--tn-color-blue-100);\n}\n\n.admonition.tip,\n.admonition.note,\n.admonition.hint {\n  border-color: var(--tn-color-blue-500);\n}\n\n.footnote-list .footnote {\n  font-size: 0.9rem;\n  margin-bottom: 0.5rem;\n  display: flex;\n  flex-direction: row;\n  align-items: baseline;\n}\n\n.footnote-list .footnote .label {\n  display: block;\n  min-width: 1.5rem;\n}\n\n.footnote-list .footnote .label a,\n.footnote-reference {\n  background-color: var(--tn-sphinx-footnote-label-background-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-color);\n  border-radius: 4px;\n  padding: 2px 4px;\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.footnote-list .footnote .label a:hover,\n.footnote-reference:hover {\n  background-color: var(--tn-sphinx-footnote-label-background-hover-color);\n  border: 1px solid var(--tn-sphinx-footnote-label-border-hover-color);\n}\n\n.footnote .fn-bracket,\n.footnote-reference .fn-bracket {\n  display: none;\n}\n\n.citation p {\n  // put the citation on the same line as the backlink.\n  display: inline;\n}\n\n.citation .label a {\n  text-decoration: none;\n  transition: all 0.2s ease-out;\n}\n\n.citation .label a:hover {\n  text-decoration: underline;\n}\n\nblockquote {\n  border-left: 0.25rem solid var(--tn-color-primary);\n  margin-left: 0;\n  padding-left: 1rem;\n}\n\nblockquote .attribution {\n  font-style: italic;\n}\n\nmain li p {\n  margin-top: 0;\n  margin-bottom: 0;\n}\n\n.block-list p {\n  margin-top: 1rem;\n  margin-bottom: 1rem;\n}\n\ndt {\n  font-weight: bold;\n}\n\ndd {\n  margin-left: 2rem;\n}\n\ndd p:first-of-type {\n  margin-top: 0.2rem;\n}\n\n// Ensure bare img elements don't extend beyond the column\nimg {\n  max-width: 100%;\n}\n\nfigure {\n  margin-left: 0;\n  margin-right: 0;\n}\n\nfigure img {\n  max-width: 100%;\n}\n\nfigcaption {\n  width: 100%;\n  background-color: var(--tn-sphinx-code-block-caption-background-color);\n  border-radius: 4px;\n  padding: 0.5rem 1rem;\n  margin: 0;\n  border: none;\n  // margin-top: -7px; // where does this extra margin come from?\n}\n\nfigcaption p {\n  margin-top: 0;\n  margin-bottom: 1em;\n  padding: 0;\n}\n\nfigcaption p:last-child {\n  margin-bottom: 0;\n}\n\n// The .technote-table class is associated with figure elements that wrap\n// tables. This figure is added by the warptables Sphinx extension in\n// technote. It allows us to make a table with overflow-x while avoiding\n// setting the display property of table itself to block, which is bad for\n// accessibility.\n// https://www.tpgi.com/short-note-on-what-css-display-properties-do-to-table-semantics/\n.technote-table {\n  max-width: 100%;\n  overflow-x: auto;\n}\n\ntable {\n  max-width: fit-content;\n  margin: 0 auto 0 0;\n  white-space: nowrap;\n\n  font-size: 0.9rem;\n  font-variant-numeric: lining-nums tabular-nums;\n  border-collapse: collapse;\n}\n\nth {\n  font-weight: normal;\n}\n\nthead {\n  border-bottom: 1px solid var(--tn-component-text-color);\n}\n\ntd,\nth {\n  padding: 0.125em 0.5em 0.25em 0.5em;\n  line-height: 1;\n  text-align: inherit;\n}\n\ntd {\n  // Attempt to align numbers on decimal points; this probably isn't supported?\n  text-align: '.' center;\n}\n\ntable caption {\n  caption-side: bottom;\n}\n",
         ".technote-article-header-id {\n  font-size: var(--tn-component-h4-size);\n  font-weight: bold;\n}\n",
         "/*\n * Icon Metadata Lists consist of a an icon paired with a metadata value.\n * The value can span multiple lines, but will always be indented beside\n * the icon.\n */\n\n.technote-icon-metadata {\n  display: flex;\n  flex-direction: row;\n  justify-content: flex-start;\n  align-items: baseline;\n  gap: var(--tn-space-xxs-fixed);\n}\n\n.technote-icon-metadata__icon {\n  width: 1em;\n  flex-grow: 0;\n  flex-shrink: 0;\n  margin: 0;\n}\n\n.technote-icon-metadata__value {\n  flex-grow: 1;\n  margin: 0;\n}\n",
         "/*\n * Styles for the author list that appears below the title.\n */\n\n.technote-status + .technote-inline-authors {\n  margin-top: 2rem;\n}\n",
         "/* The container for the primary sidebar */\n\n@media (min-width: 76rem) {\n  .technote-sidebar-container {\n    // Make the primary sidebar's content's sticky to the top of the page\n    // when visible.\n    position: sticky;\n    top: 1rem;\n\n    // Allow the sidebar content to scroll when necessary\n    overflow-y: auto;\n    max-height: 100vh;\n  }\n}\n",
         ":root {\n  --tn-component-sidebar-header-color: var(--tn-color-neutral-600);\n}\n\nhtml[data-theme='dark'] {\n  --tn-component-sidebar-header-color: var(--tn-color-neutral-200);\n}\n\n.technote-sidebar-section {\n  margin: 0 0 var(--tn-space-lg-fixed);\n}\n\n.technote-sidebar-section:first-of-type {\n  // Ensure the top spacing to the logo matches the spacing between\n  // sidebar section components.\n  margin-top: var(--tn-space-lg-fixed);\n}\n\n.technote-sidebar-section__heading {\n  font-size: var(--tn-component-h6-size);\n  font-weight: bold;\n  color: var(--tn-component-sidebar-header-color);\n  margin-bottom: 0.5rem;\n}\n\n.technote-sidebar-section__heading + * {\n  margin-top: var(--tn-space-xs-fixed);\n}\n\n.technote-sidebar-author-list {\n  margin-top: var(--tn-space-xs-fixed);\n}\n\n.technote-sidebar-metadata-list {\n  margin-top: var(--tn-space-xs-fixed);\n  margin-bottom: var(--tn-space-xs-fixed);\n  list-style-type: none;\n  padding: 0;\n}\n",
         "/*\n * Styles for the sidebar-logo component.\n */\n\n.technote-sidebar-logo__picture {\n  max-width: 12rem;\n}\n",
         "/* Styles for the document status aside */\n\n.technote-status {\n  border: 1px solid var(--tn-component-text-color);\n  padding: 1rem;\n  border-radius: var(--tn-border-radius-1);\n}\n\n.technote-status--deprecated {\n  border-color: var(--tn-color-red-500);\n}\n\n.technote-status p:first-of-type {\n  margin-top: 0;\n}\n\n.technote-status *:last-child {\n  margin-bottom: 0;\n}\n",
```

### Comparing `technote-0.7.0a1/src/technote.egg-info/PKG-INFO` & `technote-0.8.0a1/src/technote.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: technote
-Version: 0.7.0a1
+Version: 0.8.0a1
 Summary: Rubin Observatory's framework for Sphinx-based technote documents.
 License: MIT License
         
         Copyright (c) 2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -46,19 +46,20 @@
 Requires-Dist: beautifulsoup4
 Requires-Dist: pygments
 Requires-Dist: accessible-pygments
 Requires-Dist: myst-parser
 Requires-Dist: markdown-it-py[linkify]
 Provides-Extra: dev
 Requires-Dist: coverage[toml]; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest<8.0; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: types-docutils; extra == "dev"
+Requires-Dist: defusedxml; extra == "dev"
 Requires-Dist: lxml; extra == "dev"
 Requires-Dist: cssselect; extra == "dev"
 Requires-Dist: mf2py; extra == "dev"
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10385500.svg)](https://doi.org/10.5281/zenodo.10385500)
 [![Python CI](https://github.com/lsst-sqre/technote/actions/workflows/ci.yaml/badge.svg)](https://github.com/lsst-sqre/technote/actions/workflows/ci.yaml)
```

### Comparing `technote-0.7.0a1/src/technote.egg-info/SOURCES.txt` & `technote-0.8.0a1/src/technote.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 .github/CODE_OF_CONDUCT
 .github/CONTRIBUTING.md
 .github/dependabot.yml
 .github/workflows/ci.yaml
 .github/workflows/dependencies.yaml
 .github/workflows/periodic-ci.yaml
 .vscode/tasks.json
-changelog.d/20240129_154947_jsick_DM_42705.md
+changelog.d/20240501_170745_jsick_DM_43638.md
 changelog.d/_template.md.jinja
 demo/md/.gitignore
 demo/md/Makefile
 demo/md/conf.py
 demo/md/index.md
 demo/md/rubin-watermark.png
 demo/md/technote.toml
```

### Comparing `technote-0.7.0a1/tests/conftest.py` & `technote-0.8.0a1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Pytest configuration and fixtures."""
 
-
 import pytest
 from sphinx.testing.path import path
 
 pytest_plugins = ("sphinx.testing.fixtures",)
 
 # Exclude 'roots' dirs for pytest test collector
 collect_ignore: list[str] = ["roots"]
```

### Comparing `technote-0.7.0a1/tests/ext/abstract_test.py` & `technote-0.8.0a1/tests/ext/abstract_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/ext/toc_test.py` & `technote-0.8.0a1/tests/ext/toc_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/metadata/orcid_test.py` & `technote-0.8.0a1/tests/metadata/orcid_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/metadata/ror_test.py` & `technote-0.8.0a1/tests/metadata/ror_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/metadata/spdx_test.py` & `technote-0.8.0a1/tests/metadata/spdx_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/metadata_test.py` & `technote-0.8.0a1/tests/metadata_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/sources/tomlsettings_test.py` & `technote-0.8.0a1/tests/sources/tomlsettings_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tests/templating/context_test.py` & `technote-0.8.0a1/tests/templating/context_test.py`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/tox.ini` & `technote-0.8.0a1/tox.ini`

 * *Files identical despite different names*

### Comparing `technote-0.7.0a1/webpack.config.js` & `technote-0.8.0a1/webpack.config.js`

 * *Files identical despite different names*

