# Comparing `tmp/stepup_reprep-1.0.0.tar.gz` & `tmp/stepup_reprep-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup_reprep-1.0.0.tar", last modified: Thu Apr 25 19:03:27 2024, max compression
+gzip compressed data, was "stepup_reprep-1.1.0.tar", last modified: Thu May  2 09:38:23 2024, max compression
```

## Comparing `stepup_reprep-1.0.0.tar` & `stepup_reprep-1.1.0.tar`

### file list

```diff
@@ -1,329 +1,333 @@
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:27.004144 stepup_reprep-1.0.0/
--rw-r--r--   0 toon      (1000) toon      (1000)      283 2024-02-08 02:51:50.000000 stepup_reprep-1.0.0/.editorconfig
--rw-r--r--   0 toon      (1000) toon      (1000)      181 2024-04-25 17:11:07.000000 stepup_reprep-1.0.0/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     1022 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 toon      (1000) toon      (1000)    35149 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/LICENSE
--rw-r--r--   0 toon      (1000) toon      (1000)     2425 2024-04-25 19:03:27.004144 stepup_reprep-1.0.0/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)      907 2024-04-25 16:51:28.000000 stepup_reprep-1.0.0/README.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.965144 stepup_reprep-1.0.0/docs/
--rw-r--r--   0 toon      (1000) toon      (1000)      294 2024-04-25 19:02:50.000000 stepup_reprep-1.0.0/docs/changelog.md
--rw-r--r--   0 toon      (1000) toon      (1000)       63 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/clean_stdout.sed
--rw-r--r--   0 toon      (1000) toon      (1000)      589 2024-04-25 17:36:06.000000 stepup_reprep-1.0.0/docs/development.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3820 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/index.md
--rw-r--r--   0 toon      (1000) toon      (1000)      639 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/installation.md
--rw-r--r--   0 toon      (1000) toon      (1000)      831 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/license.md
--rwxr-xr-x   0 toon      (1000) toon      (1000)      608 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.965144 stepup_reprep-1.0.0/docs/reference/
--rw-r--r--   0 toon      (1000) toon      (1000)       43 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/reference/stepup.reprep.api.md
--rw-r--r--   0 toon      (1000) toon      (1000)       53 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/reference/stepup.reprep.tile_pdf.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.966144 stepup_reprep-1.0.0/docs/tutorials/
--rw-r--r--   0 toon      (1000) toon      (1000)     3567 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/before_you_begin.md
--rw-r--r--   0 toon      (1000) toon      (1000)     4070 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/initialize_project.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2305 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/manifest_files.md
--rw-r--r--   0 toon      (1000) toon      (1000)     7232 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/template_conventions.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.967144 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)       68 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)    22692 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/figure.png
--rw-r--r--   0 toon      (1000) toon      (1000)     2183 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/hexagon.svg
--rwxr-xr-x   0 toon      (1000) toon      (1000)      114 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)     2162 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/pentagon.svg
--rwxr-xr-x   0 toon      (1000) toon      (1000)      278 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2143 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/square.svg
--rw-r--r--   0 toon      (1000) toon      (1000)     1857 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      413 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/tile.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2128 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tile_pdf/triangle.svg
--rw-r--r--   0 toon      (1000) toon      (1000)     1134 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/tiling_pdfs.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2543 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/docs/tutorials/usage.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1754 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/mkdocs.yml
--rw-r--r--   0 toon      (1000) toon      (1000)     1971 2024-04-25 17:40:36.000000 stepup_reprep-1.0.0/pyproject.toml
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2024-04-25 19:03:27.004144 stepup_reprep-1.0.0/setup.cfg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.960144 stepup_reprep-1.0.0/stepup/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.970144 stepup_reprep-1.0.0/stepup/reprep/
--rw-r--r--   0 toon      (1000) toon      (1000)      819 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/__init__.py
--rw-r--r--   0 toon      (1000) toon      (1000)      411 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup/reprep/_version.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2593 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/add_notes_pdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)    25204 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/api.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1951 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/bibtex_log.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5286 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/check_hrefs.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2946 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/check_manifest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4426 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/convert_inkscape.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4077 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/convert_markdown.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7521 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/latex.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4783 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/latex_deps.py
--rw-r--r--   0 toon      (1000) toon      (1000)     7040 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/latex_flat.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5575 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/latex_log.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4130 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/make_manifest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2129 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/normalize_pdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4776 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/nup_pdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1820 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/pytest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3191 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/raster_pdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     5081 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/render.py
--rw-r--r--   0 toon      (1000) toon      (1000)     6716 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/tile_pdf.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4415 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/stepup/reprep/zip_manifest.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:27.003144 stepup_reprep-1.0.0/stepup_reprep.egg-info/
--rw-r--r--   0 toon      (1000) toon      (1000)     2425 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup_reprep.egg-info/PKG-INFO
--rw-r--r--   0 toon      (1000) toon      (1000)    10420 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup_reprep.egg-info/SOURCES.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        1 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup_reprep.egg-info/dependency_links.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      132 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup_reprep.egg-info/entry_points.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      235 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup_reprep.egg-info/requires.txt
--rw-r--r--   0 toon      (1000) toon      (1000)        7 2024-04-25 19:03:26.000000 stepup_reprep-1.0.0/stepup_reprep.egg-info/top_level.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.972144 stepup_reprep-1.0.0/tests/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.963144 stepup_reprep-1.0.0/tests/cases/
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.973144 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)       72 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      137 2024-03-29 04:46:48.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2118 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      657 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      956 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)     1183 2024-03-29 04:51:25.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/notes.pdf
--rwxr-xr-x   0 toon      (1000) toon      (1000)      182 2024-03-29 05:35:21.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     8616 2024-03-29 04:32:13.000000 stepup_reprep-1.0.0/tests/cases/add_notes_pdf/src.pdf
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.974144 stepup_reprep-1.0.0/tests/cases/cat_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)       72 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       60 2024-03-29 04:24:07.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     4820 2024-03-29 04:28:13.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/doc1.pdf
--rw-r--r--   0 toon      (1000) toon      (1000)     4956 2024-03-29 04:28:17.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/doc2.pdf
--rw-r--r--   0 toon      (1000) toon      (1000)     2001 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      569 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      956 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      172 2024-03-29 05:35:21.000000 stepup_reprep-1.0.0/tests/cases/cat_pdf/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.975144 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-30 08:23:17.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       81 2024-03-30 08:37:53.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      106 2024-03-30 09:11:15.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/check_hrefs.yaml
--rw-r--r--   0 toon      (1000) toon      (1000)     2731 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2172 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      600 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      178 2024-03-30 08:38:38.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      612 2024-03-30 09:19:58.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_html/test.html
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.976144 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/
--rw-r--r--   0 toon      (1000) toon      (1000)       26 2024-03-30 08:23:17.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       85 2024-03-30 08:11:32.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      106 2024-03-30 09:11:15.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/check_hrefs.yaml
--rw-r--r--   0 toon      (1000) toon      (1000)     2703 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2162 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      600 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      174 2024-03-30 08:38:38.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      504 2024-03-30 09:22:56.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_md/test.md
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.977144 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)       80 2024-03-30 08:49:26.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       80 2024-03-30 08:47:53.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      106 2024-03-30 09:11:15.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/check_hrefs.yaml
--rw-r--r--   0 toon      (1000) toon      (1000)     5008 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2301 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      732 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      830 2024-03-30 09:15:37.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/main.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      202 2024-03-30 08:59:51.000000 stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.978144 stepup_reprep-1.0.0/tests/cases/convert_inkscape/
--rw-r--r--   0 toon      (1000) toon      (1000)      138 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      146 2024-03-28 13:53:11.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     4713 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1368 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3106 2024-03-28 14:16:23.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/glasses.svg
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1177 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      244 2024-03-28 19:06:54.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2918 2024-03-28 18:36:32.000000 stepup_reprep-1.0.0/tests/cases/convert_inkscape/smile.svg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.979144 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/
--rw-r--r--   0 toon      (1000) toon      (1000)       81 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      237 2024-04-21 07:23:43.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2381 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1007 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      989 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      153 2024-03-28 17:55:48.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)    13660 2024-03-28 17:48:16.000000 stepup_reprep-1.0.0/tests/cases/convert_libreoffice/slide.odp
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.981144 stepup_reprep-1.0.0/tests/cases/convert_markdown/
--rw-r--r--   0 toon      (1000) toon      (1000)       76 2024-04-24 20:49:24.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       93 2024-04-24 20:57:30.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      161 2024-03-28 17:12:18.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/demo.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1774 2024-04-24 21:04:36.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      639 2024-04-24 21:04:36.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      977 2024-04-24 20:49:24.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      151 2024-04-24 20:59:40.000000 stepup_reprep-1.0.0/tests/cases/convert_markdown/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.982144 stepup_reprep-1.0.0/tests/cases/convert_mutool/
--rw-r--r--   0 toon      (1000) toon      (1000)       80 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      146 2024-03-28 13:53:11.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     4597 2024-03-29 04:29:50.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/example.pdf
--rw-r--r--   0 toon      (1000) toon      (1000)     1747 2024-04-24 20:25:11.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      601 2024-04-24 20:25:11.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      958 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      173 2024-03-29 04:16:38.000000 stepup_reprep-1.0.0/tests/cases/convert_mutool/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.983144 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/
--rw-r--r--   0 toon      (1000) toon      (1000)       72 2024-04-24 21:00:41.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       86 2024-04-24 20:59:11.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      135 2024-04-24 20:58:53.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/doc.html
--rw-r--r--   0 toon      (1000) toon      (1000)     1553 2024-04-24 21:02:20.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      513 2024-04-24 21:02:20.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      964 2024-04-24 21:01:16.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      157 2024-04-24 21:00:15.000000 stepup_reprep-1.0.0/tests/cases/convert_weasyprint/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.984144 stepup_reprep-1.0.0/tests/cases/latex_diff/
--rw-r--r--   0 toon      (1000) toon      (1000)       74 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      124 2024-03-28 09:03:01.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2901 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1086 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      905 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       87 2024-03-28 09:03:50.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/new.tex
--rw-r--r--   0 toon      (1000) toon      (1000)       87 2024-03-28 09:03:50.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/old.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      173 2024-03-28 09:12:37.000000 stepup_reprep-1.0.0/tests/cases/latex_diff/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.986144 stepup_reprep-1.0.0/tests/cases/latex_flat/
--rw-r--r--   0 toon      (1000) toon      (1000)      104 2024-03-28 10:15:21.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      331 2024-03-28 06:37:08.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      142 2024-03-28 10:06:09.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/article_structured.tex
--rw-r--r--   0 toon      (1000) toon      (1000)        0 2024-03-28 06:43:37.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/expected_article.tex
--rw-r--r--   0 toon      (1000) toon      (1000)     3178 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/expected_graph_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     3315 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/expected_graph_02.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2330 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/expected_stdout_01.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      450 2024-04-22 16:49:13.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/expected_stdout_02.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1125 2024-04-21 12:52:42.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)       16 2024-03-28 06:41:57.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/part1.tex
--rw-r--r--   0 toon      (1000) toon      (1000)       17 2024-03-28 06:41:57.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/part2.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      210 2024-03-28 06:39:21.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/plan_01.py
--rwxr-xr-x   0 toon      (1000) toon      (1000)      249 2024-03-28 10:15:08.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/plan_02.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.986144 stepup_reprep-1.0.0/tests/cases/latex_flat/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)       50 2024-03-28 06:41:57.000000 stepup_reprep-1.0.0/tests/cases/latex_flat/sub/original.tex
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.987144 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/
--rw-r--r--   0 toon      (1000) toon      (1000)       62 2024-03-28 10:36:52.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      331 2024-03-28 06:37:08.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)      165 2024-03-28 10:36:36.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/expected_article.tex
--rw-r--r--   0 toon      (1000) toon      (1000)     3186 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      415 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      728 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      238 2024-03-28 10:34:26.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.988144 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)      168 2024-03-28 10:35:28.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/sub/article_structured.tex
--rw-r--r--   0 toon      (1000) toon      (1000)       16 2024-03-28 06:41:57.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/sub/part1.tex
--rw-r--r--   0 toon      (1000) toon      (1000)       17 2024-03-28 06:41:57.000000 stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/sub/part2.tex
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.988144 stepup_reprep-1.0.0/tests/cases/lualatex_simple/
--rw-r--r--   0 toon      (1000) toon      (1000)      115 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/lualatex_simple/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     2627 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/lualatex_simple/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      640 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/lualatex_simple/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1104 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/lualatex_simple/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      424 2024-03-18 15:02:21.000000 stepup_reprep-1.0.0/tests/cases/lualatex_simple/paper.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      134 2024-03-24 07:02:12.000000 stepup_reprep-1.0.0/tests/cases/lualatex_simple/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.989144 stepup_reprep-1.0.0/tests/cases/make_manifest_in/
--rw-r--r--   0 toon      (1000) toon      (1000)       60 2024-03-28 11:11:50.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       36 2024-03-28 05:40:43.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/MANIFEST.in
--rw-r--r--   0 toon      (1000) toon      (1000)       75 2024-03-28 05:39:46.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2084 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      331 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)       13 2024-03-28 05:40:43.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/hello.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      638 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      180 2024-03-28 05:41:55.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.990144 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/
--rw-r--r--   0 toon      (1000) toon      (1000)       60 2024-03-28 11:11:41.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      185 2024-03-28 10:49:48.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2247 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      339 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      689 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      187 2024-03-28 10:58:53.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.990144 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/sub/
--rw-r--r--   0 toon      (1000) toon      (1000)       18 2024-03-28 10:51:11.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
--rw-r--r--   0 toon      (1000) toon      (1000)       13 2024-03-28 05:40:43.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/sub/hello.txt
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.991144 stepup_reprep-1.0.0/tests/cases/make_manifest_list/
--rw-r--r--   0 toon      (1000) toon      (1000)       39 2024-03-27 23:19:37.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_list/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       69 2024-03-28 05:39:46.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_list/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1692 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_list/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      353 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_list/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      638 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_list/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      166 2024-03-27 23:12:33.000000 stepup_reprep-1.0.0/tests/cases/make_manifest_list/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.992144 stepup_reprep-1.0.0/tests/cases/nup_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)       72 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       81 2024-03-29 05:31:33.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     1823 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      617 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      926 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      162 2024-03-29 05:35:21.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     9122 2024-03-29 05:03:08.000000 stepup_reprep-1.0.0/tests/cases/nup_pdf/src.pdf
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.993144 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/
--rw-r--r--   0 toon      (1000) toon      (1000)      161 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     2878 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      588 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1072 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      170 2024-03-23 13:20:09.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/paper.bbl
--rw-r--r--   0 toon      (1000) toon      (1000)      352 2024-03-18 15:02:21.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/paper.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      172 2024-03-24 07:02:12.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.994144 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/
--rw-r--r--   0 toon      (1000) toon      (1000)      215 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      423 2024-03-16 14:39:04.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/bibsane.yaml
--rw-r--r--   0 toon      (1000) toon      (1000)     4230 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      665 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1348 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      352 2024-03-18 15:02:21.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/paper.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      190 2024-03-24 07:02:12.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      209 2024-03-16 14:36:40.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/references.bib
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.994144 stepup_reprep-1.0.0/tests/cases/pdflatex_input/
--rw-r--r--   0 toon      (1000) toon      (1000)      129 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     3780 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1715 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1114 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      308 2024-03-18 15:02:21.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/paper.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      224 2024-03-27 20:48:00.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1294 2024-03-29 04:29:22.000000 stepup_reprep-1.0.0/tests/cases/pdflatex_input/smile.pdf
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.995144 stepup_reprep-1.0.0/tests/cases/raster_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)      103 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      127 2024-03-28 18:35:22.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2569 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      736 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1005 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      181 2024-03-28 19:08:02.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1294 2024-03-29 04:29:07.000000 stepup_reprep-1.0.0/tests/cases/raster_pdf/smile.pdf
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.997144 stepup_reprep-1.0.0/tests/cases/render_basic/
--rw-r--r--   0 toon      (1000) toon      (1000)       38 2024-03-29 14:46:58.000000 stepup_reprep-1.0.0/tests/cases/render_basic/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      172 2024-04-21 07:23:44.000000 stepup_reprep-1.0.0/tests/cases/render_basic/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     2247 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/render_basic/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)      395 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/render_basic/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      700 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/render_basic/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      188 2024-03-29 17:53:00.000000 stepup_reprep-1.0.0/tests/cases/render_basic/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)      103 2024-03-29 15:01:58.000000 stepup_reprep-1.0.0/tests/cases/render_basic/template.md
--rw-r--r--   0 toon      (1000) toon      (1000)      137 2024-03-29 17:54:15.000000 stepup_reprep-1.0.0/tests/cases/render_basic/variables.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.998144 stepup_reprep-1.0.0/tests/cases/render_relpath/
--rw-r--r--   0 toon      (1000) toon      (1000)       34 2024-03-29 15:16:02.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     8244 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1826 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      935 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      270 2024-03-30 02:48:02.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/plan.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:26.999144 stepup_reprep-1.0.0/tests/cases/render_relpath/static/
--rw-r--r--   0 toon      (1000) toon      (1000)      238 2024-04-20 04:40:19.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/static/main.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      213 2024-03-29 18:32:01.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/static/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       23 2024-03-29 15:12:50.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/static/preamble.inc.tex
--rw-r--r--   0 toon      (1000) toon      (1000)       21 2024-03-29 17:51:39.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/static/variables.py
--rw-r--r--   0 toon      (1000) toon      (1000)      112 2024-03-29 17:57:08.000000 stepup_reprep-1.0.0/tests/cases/render_relpath/variables.py
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:27.001144 stepup_reprep-1.0.0/tests/cases/tile_pdf/
--rw-r--r--   0 toon      (1000) toon      (1000)      155 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)       83 2024-03-30 04:28:25.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)    14439 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2540 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/expected_stdout.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2183 2024-03-30 04:26:57.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/hexagon.svg
--rw-r--r--   0 toon      (1000) toon      (1000)     1981 2024-03-30 04:25:33.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/horizontal.svg
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1374 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)     2162 2024-03-30 04:27:09.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/pentagon.svg
--rwxr-xr-x   0 toon      (1000) toon      (1000)      227 2024-03-31 16:41:27.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2143 2024-03-30 04:27:20.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/square.svg
--rwxr-xr-x   0 toon      (1000) toon      (1000)      674 2024-03-31 16:40:50.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/tile.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2128 2024-03-30 04:27:32.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/triangle.svg
--rw-r--r--   0 toon      (1000) toon      (1000)    65932 2003-04-16 14:02:13.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/vera.ttf
--rw-r--r--   0 toon      (1000) toon      (1000)     1877 2024-03-30 04:20:20.000000 stepup_reprep-1.0.0/tests/cases/tile_pdf/vertical.svg
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:27.002144 stepup_reprep-1.0.0/tests/cases/xelatex_input/
--rw-r--r--   0 toon      (1000) toon      (1000)      162 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)     5449 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     2156 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)     1203 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/main.sh
--rw-r--r--   0 toon      (1000) toon      (1000)      500 2024-03-18 15:02:21.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/paper.tex
--rwxr-xr-x   0 toon      (1000) toon      (1000)      348 2024-03-27 20:48:00.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1294 2024-03-29 04:29:29.000000 stepup_reprep-1.0.0/tests/cases/xelatex_input/smile.pdf
-drwxr-xr-x   0 toon      (1000) toon      (1000)        0 2024-04-25 19:03:27.003144 stepup_reprep-1.0.0/tests/cases/zip_manifest/
--rw-r--r--   0 toon      (1000) toon      (1000)      101 2024-04-10 05:36:26.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/.gitignore
--rw-r--r--   0 toon      (1000) toon      (1000)      349 2024-03-28 05:35:37.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/README.md
--rw-r--r--   0 toon      (1000) toon      (1000)     3293 2024-04-24 20:23:46.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/expected_graph.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1044 2024-04-22 16:49:12.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/expected_stdout.txt
--rwxr-xr-x   0 toon      (1000) toon      (1000)      995 2024-04-21 12:39:37.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/main.sh
--rwxr-xr-x   0 toon      (1000) toon      (1000)      290 2024-03-28 05:35:37.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/plan.py
--rw-r--r--   0 toon      (1000) toon      (1000)       33 2024-03-28 05:35:37.000000 stepup_reprep-1.0.0/tests/cases/zip_manifest/static.txt
--rw-r--r--   0 toon      (1000) toon      (1000)     1041 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/conftest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1137 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/reprep_common.py
--rw-r--r--   0 toon      (1000) toon      (1000)     4395 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/test_bibtex_log.py
--rw-r--r--   0 toon      (1000) toon      (1000)     3652 2024-04-25 17:41:38.000000 stepup_reprep-1.0.0/tests/test_cases.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2113 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/test_latex_deps.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2074 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/test_latex_flat.py
--rw-r--r--   0 toon      (1000) toon      (1000)    14002 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/test_latex_log.py
--rw-r--r--   0 toon      (1000) toon      (1000)     1910 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/test_manifest.py
--rw-r--r--   0 toon      (1000) toon      (1000)     2208 2024-04-25 17:34:48.000000 stepup_reprep-1.0.0/tests/test_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.020955 stepup_reprep-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.968955 stepup_reprep-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.972955 stepup_reprep-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-02 09:38:23.020955 stepup_reprep-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.972955 stepup_reprep-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.976955 stepup_reprep-1.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/reference/stepup.reprep.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/reference/stepup.reprep.tile_pdf.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.976955 stepup_reprep-1.1.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/before_you_begin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/create_or_clone_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/manifest_files.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/template_conventions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.976955 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/figure.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/hexagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/square.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/docs/tutorials/working_on_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:38:23.020955 stepup_reprep-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.968955 stepup_reprep-1.1.0/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.980955 stepup_reprep-1.1.0/stepup/reprep/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup/reprep/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/add_notes_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25206 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/check_hrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/check_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/convert_inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/convert_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/make_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/normalize_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/nup_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/raster_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/tile_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/stepup/reprep/zip_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/stepup_reprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 09:38:22.000000 stepup_reprep-1.1.0/stepup_reprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.984955 stepup_reprep-1.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.972955 stepup_reprep-1.1.0/tests/cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.984955 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/notes.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/add_notes_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.984955 stepup_reprep-1.1.0/tests/cases/cat_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/doc1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/doc2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/cat_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.988955 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_html/test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.988955 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_md/test.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.988955 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_inkscape/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/glasses.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1179 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_inkscape/smile.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      988 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_libreoffice/slide.odp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      976 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_markdown/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.992955 stepup_reprep-1.1.0/tests/cases/convert_mutool/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_mutool/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.996955 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/convert_weasyprint/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.996955 stepup_reprep-1.1.0/tests/cases/latex_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/new.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/old.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_diff/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:22.996955 stepup_reprep-1.1.0/tests/cases/latex_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/part2.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/latex_flat/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat/sub/original.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/sub/part2.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/lualatex_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/lualatex_simple/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.000955 stepup_reprep-1.1.0/tests/cases/make_manifest_in/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/hello.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/sub/hello.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/make_manifest_list/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/make_manifest_list/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.004955 stepup_reprep-1.1.0/tests/cases/nup_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/nup_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/paper.bbl
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/bibsane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/pdflatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/pdflatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.008955 stepup_reprep-1.1.0/tests/cases/raster_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1004 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/raster_pdf/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.012955 stepup_reprep-1.1.0/tests/cases/render_basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_basic/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.012955 stepup_reprep-1.1.0/tests/cases/render_relpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      931 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.012955 stepup_reprep-1.1.0/tests/cases/render_relpath/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/preamble.inc.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/static/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/render_relpath/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/tests/cases/tile_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/hexagon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/horizontal.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/square.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/tile_pdf/vertical.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/tests/cases/xelatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/xelatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:38:23.016955 stepup_reprep-1.1.0/tests/cases/zip_manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      994 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/cases/zip_manifest/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/reprep_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-02 09:38:19.000000 stepup_reprep-1.1.0/tests/test_zip.py
```

### Comparing `stepup_reprep-1.0.0/.pre-commit-config.yaml` & `stepup_reprep-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/LICENSE` & `stepup_reprep-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/PKG-INFO` & `stepup_reprep-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.0.0
+Version: 1.1.0
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
+Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
-Project-URL: Changelog, https://github.com/reproducible-reporting/stepup-reprep/blob/main/CHANGELOG.md
+Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
@@ -24,31 +25,33 @@
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: setuptools
-Requires-Dist: stepup
+Requires-Dist: stepup>=1.2.0
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 
-[![PyPI Upload](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pypi.yaml)
-[![pytest](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml)
+[![release](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup-reprep)](https://pypi.org/project/stepup-reprep/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup-reprep)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-reprep)
 
 
 # StepUp RepRep
 
-
-StepUp RepRep is the StepUp extension for [Reproducible Reporting](https://github.com/reproducible-reporting).
+StepUp RepRep is the [StepUp](https://github.com/reproducible-reporting/stepup-core) extension for [Reproducible Reporting](https://github.com/reproducible-reporting).
 
 For more information, consult the [documentation](http://reproducible-reporting.github.io/stepup-reprep).
+
+A screen recording for a quick visual impression of StepUp RepRep in action:
+
+[![asciicast](https://asciinema.org/a/656515.svg)](https://asciinema.org/a/656515)
```

### Comparing `stepup_reprep-1.0.0/README.md` & `stepup_reprep-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-[![PyPI Upload](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pypi.yaml)
-[![pytest](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml)
+[![release](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup-reprep)](https://pypi.org/project/stepup-reprep/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup-reprep)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-reprep)
 
 
 # StepUp RepRep
 
-
-StepUp RepRep is the StepUp extension for [Reproducible Reporting](https://github.com/reproducible-reporting).
+StepUp RepRep is the [StepUp](https://github.com/reproducible-reporting/stepup-core) extension for [Reproducible Reporting](https://github.com/reproducible-reporting).
 
 For more information, consult the [documentation](http://reproducible-reporting.github.io/stepup-reprep).
+
+A screen recording for a quick visual impression of StepUp RepRep in action:
+
+[![asciicast](https://asciinema.org/a/656515.svg)](https://asciinema.org/a/656515)
```

### Comparing `stepup_reprep-1.0.0/docs/index.md` & `stepup_reprep-1.1.0/docs/index.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 # Welcome to StepUp RepRep
 
 StepUp RepRep is the publication build tool for [Reproducible Reporting](https://github.com/reproducible-reporting).
-It is a domain-specific extension of a powerful universal build tool called [StepUp Core](TODO).
+It is a domain-specific extension of a powerful universal build tool called [StepUp Core](https://reproducible-reporting.github.io/stepup-core/).
 
 To get started, follow the tutorials in this documentation:
 
-- [Before you begin](tutorials/before_you_begin.md)
-- [Create or clone a project](tutorials/initialize_project.md)
-- [Working on a project](tutorials/usage.md)
+- [Before You Begin](tutorials/before_you_begin.md)
+- [Create or Clone a Project](tutorials/create_or_clone_a_project.md)
+- [Working on a Project](tutorials/working_on_a_project.md)
 
 StepUp RepRep will be installed in your instance of the template, as part of the setup.
 
-If you want to get a more in-depth understanding of how StepUp works, the [tutorials of StepUp Core](TODO) will take you through all the basics.
+If you want to gain a more in-depth understanding of how StepUp works, the [StepUp Core tutorials](https://reproducible-reporting.github.io/stepup-core/getting_started/introduction/) will take you through all the basics.
 
 
-## Why was StepUp RepRep created?
+## Quick Demo
 
-The goal of StepUp RepRep is to facilitate the reproducibility and data management of scientific publications.
-It is targeting the *last mile* of the publication process:
-the creation of a publication from the raw research results.
+The following screen cast shows StepUp RepRep in action:
+
+[![asciicast](https://asciinema.org/a/656515.svg)](https://asciinema.org/a/656515)
+
+## Why Was StepUp RepRep Created?
+
+StepUp RepRep aims to facilitate the reproducibility and data management of scientific publications.
+It targets the *last mile* of the publication process:
+The creation of a publication from raw research results.
 
 The making of a scientific publication involves many moving parts, which are not easily connected and shared among co-authors.
-Raw results must be analyzed, tabulated, and plotted to present them in a convenient form for the reader.
-Today, such data processing is increasingly done using scripting languages (Python, R, Notebooks, ...) because they enable a more advanced analysis than spreadsheets or manual calculations.
-Too often, however, results from such scripting tools are incorporated into a publication (or a subsequent analysis tool) by tedious copy paste or manual import.
+Raw results need to be analyzed, tabulated, and plotted and presented in a convenient way to the reader.
+Today, such data processing is increasingly done using scripting languages (Python, R, Notebooks, ...) because they allow more advanced analysis than spreadsheets or manual calculations.
+Too often, however, the results of such scripting tools are incorporated into a publication (or subsequent analysis tool) by tedious copy-paste or manual import.
 While each tool can be very advanced, the transfer of information from one step to the next is often not.
 This becomes problematic in at least the following scenarios:
 
-1. When trying to reproduce the results of a paper (a long time after it was published),
-   you may not remember how to transfer of intermediate results
-   between different analysis tools and how these results were transformed into a presentable form in the publication.
+1. When trying to reproduce the results of a paper, long after it was published,
+   you may not remember how intermediate results were transferred between different analysis tools
+   and how these results were transformed into a presentable form in the publication.
    In such situations, published results are not easily reproducible.
    (They may still be formally reproducible, given an almost infinite amount of time and coffee.)
-2. If a (small) error in one of the analysis scripts is fixed,
-   you need to repeat at least a part of the analysis.
+
+2. If a small error in one of the analysis scripts is fixed,
+   at least a part of the analysis must be repeated.
    Every step after the fixed part and all data transfers between them must also be repeated.
    Especially if such fixes occur regularly in the writing process,
-   the repetitive analysis and data transfers becomes very error-prone,
+   the repetitive analysis and data transfers become very error-prone,
    which undermines the quality of the publication.
-3. Because (at least) one person needs to know how to get data into and out of an analysis tool, the raw data and scripts primarily exist on the computer or account of that person.
-   Even if the data and scripts are archived and made available, the knowledge of how to reproduce these outcomes is not easily shared.
 
-StepUp RepRep overcomes these difficulties by fully formalizing how different scripting and analysis tools interact.
+3. Because at least one person needs to know how to get data into and out of an analysis tool,
+   the raw data and scripts will primarily reside on that person's computer or account.
+   Even if the data and scripts are archived and made available,
+   the knowledge of how to reproduce these results is not easily shared.
+
+StepUp RepRep overcomes these difficulties by fully formalizing the interactions between different scripts, analysis tools and authoring software.
 Once configured, the entire process, from raw results and source files all the way to a ZIP file to be uploaded to the publisher, can be reproduced by simply running the `stepup` program once.
 
 
-## Git and virtual environments
+## Git and Virtual Environments
 
-A project created with StepUp RepRep makes use of the following technologies to further facilitate data management and reproducibility:
+A project produced with StepUp RepRep uses the following technologies
+to further facilitate data management and reproducibility:
 
-- The entire publication source, with all analysis scripts to get to the final tables and figures,
+- The entire publication source,
+  along with all analysis scripts necessary to generate final tables and figures,
   is developed in a Git repository.
-  All co-authors have access to this repository, so they can (if desired) verify every little detail that leads to the published results.
+  All co-authors have access to this repository,
+  so they can (if they wish) verify every detail that leads to the published results.
 
-- A virtual software environment (Pip or Conda) is configured, so all co-authors can locally install all the software needed to reproduce the entire publication from its sources.
+- A virtual software environment (Pip or Conda) is configured,
+  allowing all co-authors to locally install all software required to reproduce
+  the entire publication from its sources.`
```

### Comparing `stepup_reprep-1.0.0/docs/installation.md` & `stepup_reprep-1.1.0/docs/installation.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Installation
 
 Requirements:
 
-- [POSIX](https://en.wikipedia.org/wiki/POSIX) operating system: Linux, macOS or WSL. StepUp cannot not run natively on Windows.
+- [POSIX](https://en.wikipedia.org/wiki/POSIX) operating system: Linux, macOS or WSL. StepUp cannot run natively on Windows.
 - [Python](https://www.python.org/) ≥ 3.11
 - [Pip](https://pip.pypa.io/)
 
 It is assumed you know how to use [Pip](https://pip.pypa.io/).
-We recommend to perform the installation in a [Python virtual environment](https://docs.python.org/3/library/venv.html) and to activate such environments with [direnv](https://direnv.net/).
+We recommend performing the installation in a [Python virtual environment](https://docs.python.org/3/library/venv.html) and activating such environments with [direnv](https://direnv.net/).
 
 The RepRep extension (for reproducible reporting) is installed with:
 
 ```bash
 pip install stepup-reprep
 ```
```

### Comparing `stepup_reprep-1.0.0/docs/license.md` & `stepup_reprep-1.1.0/docs/license.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # License
 
 ## Source code license
 
-StepUp is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+StepUp RepRep is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
-StepUp is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+StepUp RepRep is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program. If not, see [https://www.gnu.org/licenses/](https://www.gnu.org/licenses/).
 
 
 ## Documentation license
 
-StepUp's documentation is distributed under the [Creative Commons CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
+StepUp RepRep's documentation is distributed under the [Creative Commons CC BY-SA 4.0 license](https://creativecommons.org/licenses/by-sa/4.0/).
```

### Comparing `stepup_reprep-1.0.0/docs/tutorials/before_you_begin.md` & `stepup_reprep-1.1.0/docs/tutorials/before_you_begin.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,69 @@
-# Before you begin
+# Before You Begin
 
-## Initial competences
+## Initial Competences
 
 The following competences are required (at a basic level) for this template to be useful.
 
 - Unix
 - LaTeX
 - Git
 - Python
 
 Without these competences, it is still possible to contribute to a publication
 created with StepUp RepRep, but it will be difficult to take the lead.
 
 
-## Required software and configuration
+## Required Software and Configuration
 
 It is assumed that you have installed and configured the following software,
 ideally using your operating system's software installation tool
 (app store, package manager, pip, ...).
 
-- [Python](https://www.python.org/) >= 3.11
-- [Git](https://git-scm.com/)
-- [Git LFS](https://git-lfs.com/)
-- [The cookiecutter](https://www.cookiecutter.io/)
-  (Only needed to initialize a new publication.)
-- [Inkscape](https://inkscape.org/) >= 1.2
-  (Only needed when the source contains SVG files.
-  [It must be executable as `inkscape` on the command-line](https://stackoverflow.com/a/22085247/494584).)
-- [TexLive](https://tug.org/texlive/) >= 2022
-- [direnv](https://direnv.net/)
-- A Text editor compatible with [editorconfig](https://editorconfig.org/)
+- Required:
+    - [Python](https://www.python.org/) >= 3.11
+    - [Git](https://git-scm.com/)
+    - [Git LFS](https://git-lfs.com/)
+    - [The cookiecutter](https://www.cookiecutter.io/)
+      (Only needed to initialize a new publication.)
+- Recommended:
+    - [Inkscape](https://inkscape.org/) >= 1.2
+      (Only needed when the source contains SVG files.
+      [It must be executable as `inkscape` on the command-line](https://stackoverflow.com/a/22085247/494584).)
+    - `mutool` from [MuPDF](https://mupdf.com/)
+    - [TexLive](https://tug.org/texlive/) >= 2022
+    - [direnv](https://direnv.net/)
+    - A Text editor compatible with [editorconfig](https://editorconfig.org/)
 
 Installation instructions for ...
 
-- ... Ubuntu 22:
+### Ubuntu
+
+On Ubuntu 22, the required and recommended software can be installed using the following steps:
+
+1. Install the following packages:
 
     ```bash
-    sudo apt install python3 python3.11 python3.11-venv  python3-pip python3-cookiecutter inkscape texlive-full git git-lfs direnv libreoffice
+    sudo apt install \
+      python3.11 \
+      python3.11-venv \
+      python3-pip \
+      python3-cookiecutter \
+      inkscape \
+      texlive-full \
+      git \
+      git-lfs \
+      direnv \
+      mupdf-tools \
+      libreoffice
     ```
 
-    Fira fonts (used for presentations) must be installed manually:
+2. Fira fonts (used for presentations) must be installed manually,
+   because they have not been packaged for Ubuntu yet.
+   This can be achieved as follows:
 
     ```bash
     mkdir -p ~/.local/share/fonts
     cd ~/.local/share/fonts
     wget 'https://github.com/firamath/firamath/releases/download/v0.3.4/firamath.tds.zip'
     unzip -j firamath.tds.zip fonts/opentype/public/firamath/FiraMath-Regular.otf
     rm firamath.tds.zip
@@ -56,40 +76,57 @@
     wget 'https://github.com/mozilla/Fira/archive/refs/tags/4.202.zip'
     unzip -j 4.202.zip Fira-4.202/otf/*.otf
     chmod -x *.otf
     rm 4.202.zip
     cd
     ```
 
-- ... Fedora:
+### Fedora
 
-    ```bash
-    sudo dnf install python python3-pip python3-virtualenv python3-cookiecutter inkscape texlive-scheme-full git git-lfs direnv mozilla-fira* texlive-fira*
-    ```
+On Fedora (>= 38), the required and recommended software can be installed using the following command:
+
+```bash
+sudo dnf install \
+  python \
+  python3-pip \
+  python3-virtualenv \
+  python3-cookiecutter \
+  inkscape \
+  texlive-scheme-full \
+  git \
+  git-lfs \
+  direnv \
+  mupdf \
+  libreoffice \
+  mozilla-fira* \
+  texlive-fira*
+```
+
+### Conda or Pip
 
 A new dedicated
 [pip](https://pip.pypa.io/en/stable/) or [micromamba](https://mamba.readthedocs.io/)
 software environment is created for each publication.
-It is up to each co-author which of the two they prefer:
+It is up to each co-author to decide which one they prefer:
 
 1. A virtual environment with **pip** can install the dependencies
    with low time, bandwidth and storage overheads.
-   You must already have a sufficiently recent Python version installed.
-2. A **micromamba** environment (the fastest and lightest way of using conda)
+   A sufficiently recent Python version must already be installed.
+2. A **micromamba** environment (the fastest and lightest way to use conda)
    is a bit more powerful than pip.
    In principle, you can use it on a system without (a recent version of) Python.
    It can also install non-Python dependencies.
-   The main disadvantage is the time to install it, consumed bandwidth during the installation, and the high disk usage.
-   Also, the cookiecutter requires Python >= 3.7 to work, so you will need Python when
-   initializing a new publication from the template.
+   The main drawbacks are the time it takes to install, the bandwidth consumed during installation, and the amount of diskspace used.
+   Because the cookiecutter requires Python >= 3.7, you already need a working Python version
+   before installing micromamba.
 
-The goal is to isolate this software environment from your operating system as much as possible.
-This may be hampered by your local configuration, e.g.:
+The aim is to isolate this software environment from your operating system as much as possible.
+This may be hampered by your local configuration, for example:
 
 - Another always-on pip environment (activated in your shell profile, like `.bashrc`)
   may not work well when pip is used for the publication.
 
 - Similarly, another always-on conda environment (activated in your shell profile)
   may not work well when micromamba is used for the publication.
 
-- Using pip for the publication, on top of your default conda can work well.
+- Using pip for the publication on top of your default conda can work well.
   (Needs more testing.)
```

### Comparing `stepup_reprep-1.0.0/docs/tutorials/initialize_project.md` & `stepup_reprep-1.1.0/docs/tutorials/create_or_clone_a_project.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,91 @@
-# Create or clone a project
+# Create or Clone a Project
 
 Follow route **1a + 2** OR route **1b + 2**.
 
-## 0) First-time Git users
+## 0) First-time Git Users
 
 If you have not used Git before, you probably haven't configured it yet.
 At least run the following (with correct name and email):
 
 ```bash
 git config --global init.defaultBranch main
 git config --global user.name "Your Name"
-git config --global user.email Your.Name@email.com
+git config --global user.email "Your.Name@email.com"
 git config --global core.editor nano
 ```
 
 Also, go through a [Git Tutorial](https://www.w3schools.com/git/default.asp?remote=github) to become familiar with the basic concepts.
 
-## 1a) Start a new publication
 
-- Start a new publication with the [cookiecutter](https://github.com/cookiecutter/cookiecutter):
+## 1a) Start a New Publication
+
+- Start a new publication using the [cookiecutter](https://github.com/cookiecutter/cookiecutter):
 
     ```bash
     cookiecutter https://github.com/reproducible-reporting/templates
     ```
 
-    Follow the instructions on the terminal. You will have to enter:
+    Follow the instructions on the terminal.
+    You will need to enter:
 
     - `slug`:
-      This a short name for the directory name containing all the sources and compiled outputs.
-      Use lower-case characters, digits and hyphens only.
+      This is a short name for the directory containing all sources and compiled outputs.
+      Use only lower-case characters, digits and hyphens.
     - `article`:
       The LaTeX article template you want to use.
     - `supp`:
       The LaTeX supporting of supplementary information template you want to use.
     - `cover`:
       The LaTeX template for the cover letter.
 
 - Enter the newly created directory (`slug`) and initialize the Git repository
 
     ```bash
     cd 'slug'
     git init
     ```
 
-    where `'slug'` should be replaced with the directory created by the cookiecutter.
+    Replace `'slug'` with the directory created by the cookiecutter.
 
 - Before making a first commit, define the software requirements,
-  e.g. for post-processing and plotting, in `requirements.txt` **AND** `environment.yaml`.
-  If you must use micromamba (e.g. non-Python dependencies), then you can remove `requirements.txt`
-  and `setup-venv-pip.sh`.
+  e.g., for post-processing and plotting, in `requirements.txt` **AND** `environment.yaml`.
+  If you must use micromamba, because you have non-Python dependencies,
+  then you can remove `requirements.txt`  and `setup-venv-pip.sh`.
 
 - Now you can add all the files, commit them, define a remote URL and push the initial contents online:
 
     ```bash
     git add .
     git commit -a -m "Initial commit"
     git remote add origin 'remote url'
     git push origin main -u
     ```
 
-    where you replace `'remote url'` by the correct one.
+    Replace `'remote url'` with the correct one.
     This depends on which online service is used to share the Git repository with your co-authors.
     If in doubt, create a private repository on GitHub.
 
 
-## 1b) Clone an existing publication
+## 1b) Clone an Existing Publication
 
 You need a `'remote url'` of an existing publication, which one of your co-authors created.
 Substitute this `'remote url'` in the following command, which should be executed in the terminal:
 
 ```bash
 git clone 'remote url'
 cd 'slug'
 ```
 
-where `'slug'` should be replaced with the directory created by `git clone`
+Replace `'slug'` with the directory created by `git clone`.
 
 
-## 2) Set up the software environment
+## 2) Set Up the Software Environment
 
-(It is assumed your current working directory is the `'slug'`
+(It is assumed that your current working directory is the `'slug'`
 defined in the previous section **1a** or **1b**.)
 
 - Install the software environment, using **ONE of the following** commands (**NOT more than one**):
 
     ```bash
     # Fedora
     ./setup-venv-pip.sh
@@ -105,33 +107,34 @@
 
 - Activate your software environment:
 
     ```bash
     source .envrc
     ```
 
-    This activation is needed whenever you open a new terminal.
-    It is not recommended to add publications-specific activation scripts to your `~/.bashrc`.
-    If you find it too tedious to call the activation script over and over again,
-    give [`direnv`](https://github.com/direnv/direnv) a try.
+    This activation is required each time you open a new terminal.
+    It is not recommended to add publication-specific activation scripts to your `~/.bashrc`.
+    If you find it too tedious to run the activation script over and over again,
+    try using [`direnv`](https://github.com/direnv/direnv).
     Once `direnv` is installed and configured in your shell profile,
     you only need to allow it once with `direnv allow .`,
     and the `.envrc` script is automatically sourced
     when you change to the directory of the Git repository.
 
+
 - Install `pre-commit` and `git-lfs` into the new repository:
 
     ```bash
     pre-commit install
     git-lfs install
     ```
 
-    This is needed whenever your create or clone a Git repository.
-    (Normally, that is only once per publication.)
+    This is needed each time you create or clone a Git repository.
+    Normally, that is only once per publication.
 
-- Now you should be able to build the template manuscript and related documents
+- You should now be able to build the template manuscript and related documents
   with StepUp RepRep as follows:
 
     ```bash
     cd latest-draft
     stepup -n
     ```
```

### Comparing `stepup_reprep-1.0.0/docs/tutorials/manifest_files.md` & `stepup_reprep-1.1.0/docs/tutorials/manifest_files.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # MANIFEST files
 
 `MANIFEST.txt` files are used in StepUp RepRep to prepare a ZIP archive.
 Such manifests can either be created manually (for an external dataset) or automatically (for datasets created within a StepUp workflow.)
 
 
-## File formats
+## File Formats
 
 ### `MANIFEST.txt`
 
 The `MANIFEST.txt` file contains one line per file to be archived.
-On each line, there are three values:
+Each line has three values:
 
 - the file size,
 - the [BLAKE2b](https://en.wikipedia.org/wiki/BLAKE_(hash_function)#BLAKE2) hash of the file, and
 - the relative path of the file.
 
 A fixed column width is used.
-You never create this type of file manually.
+You do not create this type of file manually.
 Instead, StepUp RepRep offers several tools to make such files.
 (See below.)
 
 
 ### `MANIFEST.in`
 
 The `MANIFEST.in` file format is borrowed from the [setuptools](https://setuptools.pypa.io/) project.
 Documentation of this format can be found [here](https://setuptools.pypa.io/en/latest/userguide/miscellaneous.html#using-manifest-in).
 
 
-## Creating `MANIFEST.txt` files.
+## Creating `MANIFEST.txt` Files.
 
-### Command-line tool: `reprep-make-manifest`
+### Command-line Tool `reprep-make-manifest`
 
-One may create manifest files with the command-line tools as follows:
+One may create manifest files with the command-line tool as follows:
 
 ```bash
 reprep-make-manifest -i MANIFEST.in -o MANIFEST.txt
 ```
 
 See `reprep-make-manifest --help` for more details.
 This tool is suitable for creating manifest files of external datasets.
 
-### StepUp RepRep function `make_manifest`
+### StepUp RepRep Function `make_manifest`
 
 One may include a [`make_manifest()`][stepup.reprep.api.make_manifest] step in `plan.py` as follows:
 
 ```python
 from stepup.reprep.api import make_manifest
 
 # Option 1: use a MANIFEST.in file
@@ -52,16 +52,16 @@
 # Option 2: list all files explicitly
 make_manifest("MANIFEST.txt", ["file1.txt", "file2.txt", ...])
 ```
 
 Such steps are mainly useful for creating manifests of datasets generated in the StepUp workflow.
 
 
-## Creating a ZIP archive with a `MANIFEST.txt` file
+## Creating a ZIP Archive From a `MANIFEST.txt` File
 
 The function [`zip_manifest()`][stepup.reprep.api.zip_manifest] takes a `MANIFEST.txt` file as input and creates a ZIP file containing all the files listed in the manifest.
 It differs from the conventional `zip` program in the following ways:
 
-- File hashes are checked before adding files to the archive.
-  (This is mostly useful for external datasets.)
-- The manifest is include in the resulting ZIP file.
+- File hashes are checked before adding files to the archive,
+  which is mostly useful for external datasets.
+- The manifest is included in the resulting ZIP file.
 - The ZIP file is reproducible: all time stamps in the ZIP file are set to January 1st, 1980.
```

### Comparing `stepup_reprep-1.0.0/docs/tutorials/template_conventions.md` & `stepup_reprep-1.1.0/docs/tutorials/template_conventions.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Template conventions
+# Template Conventions
 
 This tutorial lists some recommendations that facilitate data reuse and reproducibility.
 
 
-## General filename conventions
+## General Filename Conventions
 
 ### Must
 
 - Use semantic file and directory names to organize your data.
-- When directory or file names contain numbers, zero-pad them,
+- When directory or file names contain numbers, zero-pad them
   so all relevant information is nicely aligned and filenames are correctly
   sorted.
 
     Good example:
     ```
     pressure-000.1MPa.txt
     pressure-001.0MPa.txt
@@ -24,23 +24,23 @@
     ```
     pressure-0.1MPa.txt
     pressure-100.0MPa.txt
     pressure-10.0MPa.txt
     pressure-1.0MPa.txt
     ```
 
-- Similarly, keywords can be padded with dashes or undersores, e.g.
+- Similarly, keywords can be padded with dashes or underscores, for example:
   ```
   opt__low
   opt_high
   ```
 
 - When using a similar structure inside multiple directories, use
   exactly the same filenames within the directories.
-  This is facilitates automation.
+  This facilitates automation.
 
     Good example:
     ```
     opt__low/compute.py
     opt_high/compute.py
     ```
 
@@ -53,122 +53,126 @@
     Terrible example:
     ```
     opt__low/compute.py
     opt_high/calculate.py
     ```
 
 
-## Tex sources
+## Tex Sources
 
 ### Must
 
 - All documents are written in LaTeX.
-- Every LaTeX package you don't use, is a good package.
-- Every sentence starts on a new line in the LaTeX source.
-- To facilitate reviewing the PDF, use single-column and double line spacing.
+- Every unused LaTeX package is a good package.
+- Each sentence starts on a new line in the LaTeX source.
+- To facilitate reviewing the PDF, use single-column and double-line spacing.
 - Use [BibSane](https://github.com/reproducible-reporting/bibsane) to keep your BibTeX files sane.
-- Hint: [Quick DOI tot BIB conversion](https://www.doi2bib.org)
+- Hint: [Quick DOI to BIB conversion](https://www.doi2bib.org)
 
 ### Should
 
-- Some pakcages, like `todo` are convenient while writing.
+- Some packages, like `todo`, are convenient while writing.
   Clearly separate these from other `\usepackage` lines, so they can be easily deleted
   when finalizing the manuscript.
-- Define as little commands as possible.
+- Define as few commands as possible.
 - Avoid low-quality publisher article classes. (ACS has a decent one.)
 - Avoid `\subfigure`. Merge panels into one PDF instead. (See [Tiling PDFs](tiling_pdfs.md).)
 
 
 ## Figures
 
 ### Must
 
-- Separate the data generation or collection from the actual plotting.
-  (Do these in two separate Python scripts.)
-  This means you commit the following to Git:
-    - Data files containing the data shown in the plots.
-      Text files like CSV are preferred when possible.
-      Also commit these files when the data is auto-generated.
-      This may not seems useful, but it allows for verification of reproducibility.
-    - Scripts that generate data, if applicable.
-    - Scripts to generate the plot, using the above data as input.
-      Use matplotlib unless you have good reasons not to.
-    - A `README.md` or docstrings summarizing the scripts and the data.
-- When making drawings, use Inkscape (>= 1.2) and commit the SVG source files.
-- Use bitmap formats only as an intermediate format when the vector graphics PDF show performance issues.
-  This typically happens when a plot contains many thousands of data points.
-  Use high-resolution PNG files (not GIF, JPEG or any other format).
+- Separate data generation or collection from actual plotting:
+  Perform these two steps in separate Python scripts.
+  This means committing the following to Git:
+
+    - Data files (e.g., CSV) containing plot data, including generated data.
+      This allows for verification of reproducibility.
+
+    - Scripts generating data, if applicable.
+
+    - Scripts generating plots using the above data as input.
+      Use matplotlib unless otherwise justified.
+
+    - A `README.md` or docstrings summarizing scripts and data.
+
+- When creating drawings, use Inkscape (>= 1.2) and commit SVG source files.
+
+- Use bitmap formats only as an intermediate format
+  when vector graphics PDFs show performance issues.
+  This typically happens with plots containing many thousands of data points:
+  Use high-resolution PNG files (not GIF, JPEG or other formats).
 
 ### Avoid
 
 - Jupyter notebooks
 
 ## Tables
 
 ### Must
 
 Commit the following:
 
-- Machine-readable files containing the data shown in the table, e.g. CSV.
-- Scripts to generate the LaTeX source of table.
-- A `README.md` or docstrings summarizing the scripts and the data.
+- Machine-readable files (e.g., CSV) containing table data.
+- Scripts generating LaTeX source for tables.
+- A `README.md` or docstrings summarizing scripts and data.
 
 ### Avoid
 
 - Jupyter notebooks
 
 
-## Data sets
+## Data Sets
 
 ### Must
 
-- The `dataset-{name}` directories are appropriate when
-  the data cannot be regenerated from scratch,
-  or when it would be impractical to do so on a routine basis:
+- Use `dataset-{name}` directories for data that cannot be (easily) generated from scratch:
 
     - External data sets.
-    - Expensive calculations that you carried out separately.
+    - Expensive calculations done previously.
     - Data generated with closed-source software.
       (Avoid closed-source software when you have the choice.)
-    - Data generated with specialized hardware not generally available.
+    - Data requiring specialized hardware not generally available.
     - Manually curated data.
 
-- Add as many scripts and implementations as possible to regenerate the data.
-  Integrate these scripts as much as possible with StepUp RepRep.
+- Add scripts and implementations to regenerate the data,
+  integrating them as much as possible with StepUp RepRep.
 
-- Add a `README.md` file explaining the following:
+- Add a `README.md` file explaining:
 
-    - How the data were generated
-    - Software that was used
-    - Directory and file organization
-    - File content details
+    - How the data were generated.
+    - Software that was used.
+    - Directory and file organization.
+    - File content details.
 
-- Data sets are Zipped in the end, so store uncompressed data in the repository.
+- Data sets will be Zipped in the end, so store uncompressed data in the repository.
 
 ### Should
 
-- When data sets become large for Git (more than 500 kB), use [Git LFS](https://git-lfs.com/).
+- When data sets exceed 500 kB, use [Git LFS](https://git-lfs.com/).
   The threshold can be increased for convenience,
-  but keep in mind that most remote Git repositories have storage quota.
+  but consider remote Git repository storage quota.
   For GitHub, the maximum seems to be 5 GB at the moment (for the entire history).
+
 - When data sets become large for Git LFS (more than 50 MB), use University-provided storage.
   Check your Git LFS quota to define a sensible threshold.
   At the time of writing, this is 2 GB (all files combined) for GitHub.
   When offloading data outside the Git repository,
   document clearly where the data is stored, how to access and who has access permissions.
-- For some files, e.g. a zipped collection of data files,
+
+- For some files, such as zipped collections of data files,
   there are no concerns that the zipping itself is difficult to reproduce,
-  so you can decide not to store the zip file separately and to add it to `.gitignore` instead.
+  so you can decide not to store the zip file separately and add it to `.gitignore` instead.
 
 ### Avoid
 
 - Jupyter notebooks
-- Inventing your own file format.
-- Tar files, especially compressed ones.
-  These are prone to data loss in case of even the tiniest bit rot.
+- Inventing custom file formats.
+- Tar files, especially compressed ones, due to data loss concerns.
   Ordinary ZIP is more robust, because every file is compressed individually.
 - Compressed files inside compressed files.
 - Binary files in general, are harder to reuse in the longer term.
 - HDF5 files due to their data integrity issues.
 - Python pickle files,
   as these can only be loaded when the corresponding Python packages are around.
   This is too limiting for long-term data preservation.
@@ -176,35 +180,34 @@
 
 
 ## Software
 
 ### Must
 
 - List software dependencies in `requirements.txt` or `environment.yaml`,
-  such that they can be installed with `pip` or `conda` by all co-authors.
-  Specify the version (if relevant).
+  specifying versions where relevant,
+  to enable installation with `pip` or `conda` by all co-authors.
 
-- All software to rebuild the publication must be open source.
+- Use only open-source software to (re)build the publication.
 
-- When you have the choice, do not use closed-source software.
+- When possible, avoid using closed-source entirely.
 
 - If you generate some data with closed-source software, store it in a `dataset-<name>`
   directory and document in the `README.md` how you exactly generated the data
-  and with which versions of the software.
+  and which versions of the software were used.
 
 - If you write your own Python package and use it in a publication,
   make open-source releases of all versions used in the paper.
   In addition to `requirements.txt` or `environment.yaml`,
-  also refer to the source repository and the version of your package in the `README.md`
+  refer to the source repository and the version of your package in the `README.md`
   of the corresponding `results-<name>` or `dataset-<name>` directories.
 
-    If your Python package is highly experimental and you're not comfortable releasing it yet,
-    you can include it in the publication project repository,
-    for example, under `latest-draft/pkgs/your_package`.
-    You can then add a line `-e latest-draft/pkgs/your_package`
+    If your Python package is experimental and not ready for release yet,
+    include it in the publication project repository under `latest-draft/pkgs/your_package`.
+    Add a line `-e latest-draft/pkgs/your_package`
     to the `requirements.txt` and `environment.yaml` files as follows:
 
     **requirements.txt** (just add a line)
     ```
     -e latest-draft/pkgs/your_package
     ```
```

### Comparing `stepup_reprep-1.0.0/docs/tutorials/tile_pdf/figure.png` & `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/figure.png`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/docs/tutorials/tile_pdf/hexagon.svg` & `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/docs/tutorials/tile_pdf/pentagon.svg` & `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/docs/tutorials/tile_pdf/square.svg` & `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/docs/tutorials/tile_pdf/stdout.txt` & `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/docs/tutorials/tile_pdf/triangle.svg` & `stepup_reprep-1.1.0/docs/tutorials/tiling_pdfs/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/docs/tutorials/usage.md` & `stepup_reprep-1.1.0/docs/tutorials/working_on_a_project.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-# Working on a project
+# Working on a Project
 
-## The `stepup` program and `plan.py`
+## The `stepup` Program and `plan.py`
 
-We strongly recommend that you follow the ["Getting Started" tutorials of StepUp Core](TODO),
+We strongly recommend that you follow the [StepUp Core "Getting Started" tutorials](https://reproducible-reporting.github.io/stepup-core/getting_started/introduction/),
 to familiarize yourself with the `stepup` program.
-This is the build tool that orchestrates the processing of the results and compilation of the paper.
+This is the build tool that orchestrates the processing of results and the compilation of the paper.
 These tutorials will give you a good understanding of how StepUp works and how to use it.
 
 Now that you have gained a basic understanding of StepUp Core,
-it will become clear why there is a file `plan.py` included in the template.
+it will become clear why a `plan.py` file is included in the template.
 The off-the-shelf `plan.py` already covers quite a few use cases,
-but consider it as a good starting point for further development.
-In addition to the functions in `stepup.core.api`, StepUp RepRep provides more functionality geared towards scientific publication.
+but consider it a good starting point for further development.
+In addition to the functions in `stepup.core.api`, StepUp RepRep provides more functionality geared towards scientific publishing.
 Reference documentation for these functions can be found here:
 
 - [stepup.reprep.api][]
 - [stepup.reprep.tile_pdf][]
 
+
 ## Git
 
-Except for making small changes, working on a StepUp project can benefit greatly from some basic Git skills.
+Aside from making small changes, working on a StepUp project can greatly benefit from basic Git skills.
 If you are new to Git, start with small steps and take on bigger challenges as you gain experience.
 
-### Recommended Git tutorials
+### Recommended Git Tutorials
 
 The following sections of [GitHub's guide to Git](https://guides.github.com/) are most relevant:
 
 - [Understanding the GitHub flow](https://guides.github.com/introduction/flow/)
 - [Hello World](https://guides.github.com/activities/hello-world/)
 - [Git Handbook](https://guides.github.com/introduction/git-handbook/)
 - [Forking projects](https://guides.github.com/activities/forking/)
@@ -34,19 +35,18 @@
 More recommended visual Git resources include:
 
 - [A Visual Git Reference](https://marklodato.github.io/visual-git-guide/index-en.html)
 - [5 Git resources for visual learners](https://about.gitlab.com/blog/2022/09/14/git-resources-for-visual-learners/)
 - [Learn Git Branching](https://learngitbranching.js.org/) (an online game to learn Git)
 
 
-### Keep clean
+### Keep Clean
 
-To keep the Git repository organized and understandable by your co-authors,
-it is important to avoid messing it up.
-If in doubt, ask one of your co-authors to take a look before you make a commit.
+It is essential to keep the Git repository organized and understandable by your co-authors.
+When in doubt, ask one of your co-authors to review before making a commit.
 
-The project template uses  [`pre-commit`](https://pre-commit.com) to clean up trivial annoyances, which would otherwise result in diff noise.
-Make sure you have installed `pre-commit` and activated it on your clone of the repository.
+The project template uses  [`pre-commit`](https://pre-commit.com) to clean up trivial annoyances.
+Ensure you have installed `pre-commit` and activated it on your clone of the repository.
 
 To remove all stale files (defined in `.gitignore`), run `git clean -dfX`.
-Do not use this command before you have committed all important files,
-as it may accidentally remove work in progress.
+However, do not use this command until you have committed all important files,
+as it may inadvertently remove work in progress.
```

### Comparing `stepup_reprep-1.0.0/mkdocs.yml` & `stepup_reprep-1.1.0/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
       name: Switch to system preference
 
 nav:
   - Home: index.md
   - installation.md
   - Tutorials:
     - tutorials/before_you_begin.md
-    - tutorials/initialize_project.md
-    - tutorials/usage.md
+    - tutorials/create_or_clone_a_project.md
+    - tutorials/working_on_a_project.md
     - tutorials/template_conventions.md
     - tutorials/manifest_files.md
     - tutorials/tiling_pdfs.md
   - Reference:
     - reference/stepup.reprep.api.md
     - reference/stepup.reprep.tile_pdf.md
   - changelog.md
```

### Comparing `stepup_reprep-1.0.0/pyproject.toml` & `stepup_reprep-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "markdown_katex",
     "numpy",
     "path",
     "pymupdf",
     "pyyaml",
     "scipy",
     "setuptools",
-    "stepup",
+    "stepup>=1.2.0",
     "weasyprint",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
@@ -46,17 +46,18 @@
     "mkdocs",
     "mkdocstrings[python]",
     "mkdocs-macros-plugin",
     "mkdocs-material",
 ]
 
 [project.urls]
+Documentation = "https://reproducible-reporting.github.io/stepup-reprep/"
 Issues = "https://github.com/reproducible-reporting/stepup-reprep/issues"
 Source = "https://github.com/reproducible-reporting/stepup-reprep/"
-Changelog = "https://github.com/reproducible-reporting/stepup-reprep/blob/main/CHANGELOG.md"
+Changelog = "https://reproducible-reporting.github.io/stepup-reprep/changelog/"
 
 [project.scripts]
 reprep-make-manifest = "stepup.reprep.make_manifest:main"
 reprep-check-manifest = "stepup.reprep.check_manifest:main"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
@@ -69,11 +70,14 @@
 line-length = 100
 target-version = "py311"
 
 [tool.ruff.lint]
 select = ["E", "F", "UP", "B", "I", "PGH", "PL", "RUF", "C"]
 ignore = ["PLR0911", "PLR0912", "PLR0913", "PLR0915", "PLR2004", "PLW2901", "C901"]
 
+[tool.setuptools]
+packages = ["stepup.reprep"]
+
 [tool.setuptools_scm]
 write_to = "stepup/reprep/_version.py"
 version_scheme = "post-release"
 local_scheme = "no-local-version"
```

### Comparing `stepup_reprep-1.0.0/stepup/reprep/__init__.py` & `stepup_reprep-1.1.0/stepup/reprep/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/add_notes_pdf.py` & `stepup_reprep-1.1.0/stepup/reprep/add_notes_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/api.py` & `stepup_reprep-1.1.0/stepup/reprep/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     """Check hyper references in a Markdown, HTML or PDF file.
 
     Parameters
     ----------
     path_src
         The source Markdown, HTML or PDF to check.
     path_config
-        The confiration file.
+        The configuration file.
         Defaults to `${REPREP_CHECK_HREFS_CONFIG}` variable or `check_hrefs.yaml` if it is not set.
     block
         When `True`, the step will always remain pending.
     """
     with subs_env_vars() as subs:
         path_src = subs(path_src)
         path_config = subs(path_config)
@@ -544,15 +544,15 @@
         The diff output tex or bbl.
     latexdiff
         Path of the latexdiff  executable.
         Defaults to `${REPREP_LATEXDIFF}` variable or `latexdiff` if the variable is unset.
     latexdiff_args
         Additional arguments for latexdiff.
         Defaults to `${REPREP_LATEXDIFF_ARG}` variable.
-        if this variable is unset, the following default is used:
+        If this variable is unset, the following default is used:
 
         ```
         --append-context2cmd=abstract,supplementary,dataavailability,funding, \\
                              authorcontributions,conflictsofinterest,abbreviations
         ```
 
         The option `--no-label` is always added because it is needed to make the file reproducible.
```

### Comparing `stepup_reprep-1.0.0/stepup/reprep/bibtex_log.py` & `stepup_reprep-1.1.0/stepup/reprep/bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/check_hrefs.py` & `stepup_reprep-1.1.0/stepup/reprep/check_hrefs.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/check_manifest.py` & `stepup_reprep-1.1.0/stepup/reprep/check_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/convert_inkscape.py` & `stepup_reprep-1.1.0/stepup/reprep/convert_inkscape.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/convert_markdown.py` & `stepup_reprep-1.1.0/stepup/reprep/convert_markdown.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/latex.py` & `stepup_reprep-1.1.0/stepup/reprep/latex.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/latex_deps.py` & `stepup_reprep-1.1.0/stepup/reprep/latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/latex_flat.py` & `stepup_reprep-1.1.0/stepup/reprep/latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/latex_log.py` & `stepup_reprep-1.1.0/stepup/reprep/latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/make_manifest.py` & `stepup_reprep-1.1.0/stepup/reprep/make_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/normalize_pdf.py` & `stepup_reprep-1.1.0/stepup/reprep/normalize_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/nup_pdf.py` & `stepup_reprep-1.1.0/stepup/reprep/nup_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/pytest.py` & `stepup_reprep-1.1.0/stepup/reprep/pytest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/raster_pdf.py` & `stepup_reprep-1.1.0/stepup/reprep/raster_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/render.py` & `stepup_reprep-1.1.0/stepup/reprep/render.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup/reprep/tile_pdf.py` & `stepup_reprep-1.1.0/stepup/reprep/tile_pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         The list panels, instances of the `Panel` class.
     fontname
         A Fontname recognized by PyMyPDF or a custom name when fontfile is specified.
     fontfile
         None or the path to a ttf file.
         When used, specify a corresponding fontname (of your choice).
     fontsize
-        The fontsize to use for the labels in points.
+        The font size to use for the labels in points.
     label_height
         The height to use for the labels in mm.
     padding
         The padding added added to the panels before combining them, in mm.
         This parameter is also used as margin between the label and the figure.
     hshift
         An optional horizontal displacement of the panel label, in mm.
@@ -97,21 +97,15 @@
     def info(self):
         inp = [panel.path_in for panel in self.panels]
         if self.fontfile is not None:
             inp.append(self.fontfile)
         return {"inp": inp, "out": self.path_out}
 
     def run(self):
-        """Combine PDF figures into a single PDF with labels on top of each panel
-
-        Parameters
-        ----------
-        figure
-            A Figure instance defined the layout and contents of the panels
-        """
+        """Combine PDF figures into a single PDF with labels on top of each panel."""
         _load_pdfs(self.panels)
         for panel in self.panels:
             _add_label(panel, self)
         out = _combine_figures(self.panels)
         out.set_metadata({})
         out.del_xml_metadata()
         out.scrub()
@@ -199,22 +193,22 @@
             a_ub[ieq, col_vars[sf.icol + sf.ncol - 1]] = -1
             a_ub[ieq, col_vars[sf.icol - 1]] = 1
         b_ub[ieq] = -sf.pdf[0].rect.width
         ieq += 1
 
     # Optimize the layout
     res = optimize.linprog(c, a_ub, b_ub, method="highs")
-    rowres = np.concatenate([[0.0], res.x[:nrow]])
-    colres = np.concatenate([[0.0], res.x[nrow:]])
+    row_pos = np.concatenate([[0.0], res.x[:nrow]])
+    col_pos = np.concatenate([[0.0], res.x[nrow:]])
 
     # Put everything in one PDF
     out = fitz.open()
-    page = out.new_page(width=colres[-1], height=rowres[-1])
+    page = out.new_page(width=col_pos[-1], height=row_pos[-1])
     for sf in panels:
         dst_rect = fitz.Rect(
-            colres[sf.icol],
-            rowres[sf.irow],
-            colres[sf.icol + sf.ncol],
-            rowres[sf.irow + sf.nrow],
+            col_pos[sf.icol],
+            row_pos[sf.irow],
+            col_pos[sf.icol + sf.ncol],
+            row_pos[sf.irow + sf.nrow],
         )
         page.show_pdf_page(dst_rect, sf.pdf, 0)
     return out
```

### Comparing `stepup_reprep-1.0.0/stepup/reprep/zip_manifest.py` & `stepup_reprep-1.1.0/stepup/reprep/zip_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/stepup_reprep.egg-info/PKG-INFO` & `stepup_reprep-1.1.0/stepup_reprep.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.0.0
+Version: 1.1.0
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
+Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
-Project-URL: Changelog, https://github.com/reproducible-reporting/stepup-reprep/blob/main/CHANGELOG.md
+Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
@@ -24,31 +25,33 @@
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: setuptools
-Requires-Dist: stepup
+Requires-Dist: stepup>=1.2.0
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: mkdocs-macros-plugin; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 
-[![PyPI Upload](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pypi.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pypi.yaml)
-[![pytest](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/pytest.yaml)
+[![release](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml/badge.svg)](https://github.com/reproducible-reporting/stepup-reprep/actions/workflows/release.yaml)
 [![PyPI Version](https://img.shields.io/pypi/v/stepup-reprep)](https://pypi.org/project/stepup-reprep/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/stepup-reprep)
 ![GPL-3 License](https://img.shields.io/github/license/reproducible-reporting/stepup-reprep)
 
 
 # StepUp RepRep
 
-
-StepUp RepRep is the StepUp extension for [Reproducible Reporting](https://github.com/reproducible-reporting).
+StepUp RepRep is the [StepUp](https://github.com/reproducible-reporting/stepup-core) extension for [Reproducible Reporting](https://github.com/reproducible-reporting).
 
 For more information, consult the [documentation](http://reproducible-reporting.github.io/stepup-reprep).
+
+A screen recording for a quick visual impression of StepUp RepRep in action:
+
+[![asciicast](https://asciinema.org/a/656515.svg)](https://asciinema.org/a/656515)
```

### Comparing `stepup_reprep-1.0.0/stepup_reprep.egg-info/SOURCES.txt` & `stepup_reprep-1.1.0/stepup_reprep.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
+.github/workflows/mkdocs.yaml
+.github/workflows/pytest.yaml
+.github/workflows/release.yaml
 docs/changelog.md
 docs/clean_stdout.sed
 docs/development.md
 docs/index.md
 docs/installation.md
 docs/license.md
-docs/plan.py
 docs/reference/stepup.reprep.api.md
 docs/reference/stepup.reprep.tile_pdf.md
 docs/tutorials/before_you_begin.md
-docs/tutorials/initialize_project.md
+docs/tutorials/create_or_clone_a_project.md
 docs/tutorials/manifest_files.md
 docs/tutorials/template_conventions.md
 docs/tutorials/tiling_pdfs.md
-docs/tutorials/usage.md
-docs/tutorials/tile_pdf/.gitignore
-docs/tutorials/tile_pdf/figure.png
-docs/tutorials/tile_pdf/hexagon.svg
-docs/tutorials/tile_pdf/main.sh
-docs/tutorials/tile_pdf/pentagon.svg
-docs/tutorials/tile_pdf/plan.py
-docs/tutorials/tile_pdf/square.svg
-docs/tutorials/tile_pdf/stdout.txt
-docs/tutorials/tile_pdf/tile.py
-docs/tutorials/tile_pdf/triangle.svg
+docs/tutorials/working_on_a_project.md
+docs/tutorials/tiling_pdfs/.gitignore
+docs/tutorials/tiling_pdfs/figure.png
+docs/tutorials/tiling_pdfs/hexagon.svg
+docs/tutorials/tiling_pdfs/main.sh
+docs/tutorials/tiling_pdfs/pentagon.svg
+docs/tutorials/tiling_pdfs/plan.py
+docs/tutorials/tiling_pdfs/square.svg
+docs/tutorials/tiling_pdfs/stdout.txt
+docs/tutorials/tiling_pdfs/tile.py
+docs/tutorials/tiling_pdfs/triangle.svg
 stepup/reprep/__init__.py
 stepup/reprep/_version.py
 stepup/reprep/add_notes_pdf.py
 stepup/reprep/api.py
 stepup/reprep/bibtex_log.py
 stepup/reprep/check_hrefs.py
 stepup/reprep/check_manifest.py
```

### Comparing `stepup_reprep-1.0.0/tests/cases/add_notes_pdf/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_graph.txt`

 * *Files 11% similar despite different names*

```diff
@@ -52,13 +52,15 @@
              command = python -m stepup.reprep.add_notes_pdf src.pdf notes.pdf dst.pdf
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:notes.pdf
             consumes   file:src.pdf
              creates   file:dst.pdf
+            supplies   file:dst.pdf
 
 file:dst.pdf
                 path = dst.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.add_notes_pdf src.pdf notes.pdf dst.pdf
             consumes   file:./
+            consumes   step:python -m stepup.reprep.add_notes_pdf src.pdf notes.pdf dst.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/add_notes_pdf/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.add_notes_pdf src.pdf notes.pdf dst.pdf
    SUCCESS │ python -m stepup.reprep.add_notes_pdf src.pdf notes.pdf dst.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ dst.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/add_notes_pdf/main.sh` & `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv dst.pdf dst1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("dst.pdf")
+watch_delete("dst.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["dst.pdf", "dst1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/add_notes_pdf/notes.pdf` & `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/notes.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/add_notes_pdf/src.pdf` & `stepup_reprep-1.1.0/tests/cases/add_notes_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/cat_pdf/doc1.pdf` & `stepup_reprep-1.1.0/tests/cases/cat_pdf/doc1.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/cat_pdf/doc2.pdf` & `stepup_reprep-1.1.0/tests/cases/cat_pdf/doc2.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/cat_pdf/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_graph.txt`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,15 @@
              command = mutool merge -o cat.pdf doc1.pdf doc2.pdf
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:doc1.pdf
             consumes   file:doc2.pdf
              creates   file:cat.pdf
+            supplies   file:cat.pdf
 
 file:cat.pdf
                 path = cat.pdf
                state = BUILT
           created by   step:mutool merge -o cat.pdf doc1.pdf doc2.pdf
             consumes   file:./
+            consumes   step:mutool merge -o cat.pdf doc1.pdf doc2.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/cat_pdf/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/cat_pdf/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mutool merge -o cat.pdf doc1.pdf doc2.pdf
    SUCCESS │ mutool merge -o cat.pdf doc1.pdf doc2.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ cat.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/cat_pdf/main.sh` & `stepup_reprep-1.1.0/tests/cases/cat_pdf/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv cat.pdf cat1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("cat.pdf")
+watch_delete("cat.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["cat.pdf", "cat1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_html/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_html/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/expected_stdout.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.check_hrefs test.html
 RESCHEDULE │ python -m stepup.reprep.check_hrefs test.html
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.check_hrefs test.html
 Return code           1
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 BROKEN.md
 ──────────────────────────────── Standard error ────────────────────────────────
-FAILED LINK: https://www.speedtest.net/
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               python -m stepup.reprep.check_hrefs test.html
 Working directory     ./
 Inputs        STATIC  ./
              PENDING  (BROKEN.md)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_html/main.sh` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_html/test.html` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_html/test.html`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_md/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_md/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_md/expected_stdout.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.check_hrefs test.md
 RESCHEDULE │ python -m stepup.reprep.check_hrefs test.md
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.check_hrefs test.md
 Return code           1
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 BROKEN.md
 ──────────────────────────────── Standard error ────────────────────────────────
-FAILED LINK: https://www.speedtest.net/
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               python -m stepup.reprep.check_hrefs test.md
 Working directory     ./
 Inputs        STATIC  ./
              PENDING  (BROKEN.md)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_md/main.sh` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_md/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_graph.txt`

 * *Files 14% similar despite different names*

```diff
@@ -65,45 +65,54 @@
             consumes   file:./
             supplies   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 step:python -m stepup.reprep.latex main.tex --run-bibtex
              workdir = ./
              command = python -m stepup.reprep.latex main.tex --run-bibtex
                state = SUCCEEDED
-   creates (amended) = file:main.log
+  supplies (amended) = file:main.log
                      = file:main.out
                      = file:main.sh
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:main.tex
              creates   file:main.MANIFEST.txt
              creates   file:main.aux
              creates   file:main.log
              creates   file:main.out
              creates   file:main.pdf
              creates   file:main.sh
+            supplies   file:main.MANIFEST.txt
+            supplies   file:main.aux
+            supplies   file:main.log
+            supplies   file:main.out
+            supplies   file:main.pdf
+            supplies   file:main.sh
 
 file:main.MANIFEST.txt
                 path = main.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 file:main.aux
                 path = main.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 file:main.pdf
                 path = main.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
             supplies   step:python -m stepup.reprep.check_hrefs main.pdf
 
 step:python -m stepup.reprep.check_hrefs main.pdf
              workdir = ./
              command = python -m stepup.reprep.check_hrefs main.pdf
                state = PENDING
   consumes (amended) = file:BROKEN.md
@@ -121,25 +130,28 @@
             consumes   file:plan.py
 
 file:main.log
                 path = main.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 file:main.out
                 path = main.out
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 file:main.sh
                 path = main.sh
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex
 
 (file:BROKEN.md)
                 path = BROKEN.md
                state = PENDING
             consumes   file:./
             supplies   step:python -m stepup.reprep.check_hrefs main.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/expected_stdout.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex main.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex main.tex --run-bibtex
      START │ python -m stepup.reprep.check_hrefs main.pdf
 RESCHEDULE │ python -m stepup.reprep.check_hrefs main.pdf
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.check_hrefs main.pdf
 Return code           1
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 BROKEN.md
 ──────────────────────────────── Standard error ────────────────────────────────
-FAILED LINK: https://www.speedtest.net/
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               python -m stepup.reprep.check_hrefs main.pdf
 Working directory     ./
 Inputs        STATIC  ./
              PENDING  (BROKEN.md)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/main.sh` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/check_hrefs_pdf/main.tex` & `stepup_reprep-1.1.0/tests/cases/check_hrefs_pdf/main.tex`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_inkscape/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_graph.txt`

 * *Files 4% similar despite different names*

```diff
@@ -82,31 +82,35 @@
                state = SUCCEEDED
            mandatory = IMPLIED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
             consumes   file:./
             consumes   file:glasses.svg
              creates   file:glasses.png
+            supplies   file:glasses.png
 
 file:glasses.png
                 path = glasses.png
                state = BUILT
           created by   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
             consumes   file:./
+            consumes   step:inkscape glasses.svg  --export-filename=glasses.png --export-type=png
             supplies   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
 step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
              workdir = ./
              command = inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
             consumes   file:./
             consumes   file:glasses.png
             consumes   file:smile.svg
              creates   file:final.pdf
+            supplies   file:final.pdf
 
 file:final.pdf
                 path = final.pdf
                state = BUILT
           created by   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_inkscape/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/convert_inkscape/expected_stdout.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
    SUCCESS │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
      START │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
      START │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
    SUCCESS │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
      START │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
    SUCCESS │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
+   UPDATED │ glasses.svg
+   UPDATED │ smile.svg
      PHASE │ watch
    DELETED │ final.pdf
    DELETED │ glasses.png
      PHASE │ run
+      SKIP │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
+      SKIP │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
      START │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
    SUCCESS │ inkscape glasses.svg  --export-filename=glasses.png --export-type=png
      START │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
    SUCCESS │ inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_inkscape/glasses.svg` & `stepup_reprep-1.1.0/tests/cases/convert_inkscape/glasses.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_inkscape/main.sh` & `stepup_reprep-1.1.0/tests/cases/convert_inkscape/main.sh`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv final.pdf final1.pdf
 mv glasses.png glasses1.png
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("final.pdf")
-watch_del("glasses.png")
+watch_delete("final.pdf")
+watch_delete("glasses.png")
 run()
 join()
 write_manifest("reproducibility_png_manifest.txt", ["glasses.png", "glasses1.png"])
 write_manifest("reproducibility_pdf_manifest.txt", ["final.pdf", "final1.pdf"])
 EOD
 
 # Wait for background processes, if any.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_inkscape/smile.svg` & `stepup_reprep-1.1.0/tests/cases/convert_inkscape/smile.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_libreoffice/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -44,13 +44,15 @@
              command = WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
                state = SUCCEEDED
                 pool = libreoffice
           created by   step:./plan.py
             consumes   file:./
             consumes   file:slide.odp
              creates   file:slide.pdf
+            supplies   file:slide.pdf
 
 file:slide.pdf
                 path = slide.pdf
                state = BUILT
           created by   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
             consumes   file:./
+            consumes   step:WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_libreoffice/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
    SUCCESS │ WORK=`mktemp -d --suffix=reprep` && libreoffice --convert-to pdf slide.odp --outdir ${WORK} > /dev/null && cp ${WORK}/*.pdf slide.pdf && rm -r ${WORK}
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ slide.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_libreoffice/main.sh` & `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/main.sh`

 * *Files 11% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv slide.pdf slide1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("slide.pdf")
+watch_delete("slide.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest_skip.txt", ["slide.pdf", "slide1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_libreoffice/slide.odp` & `stepup_reprep-1.1.0/tests/cases/convert_libreoffice/slide.odp`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_markdown/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_graph.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,13 +43,15 @@
              command = python -m stepup.reprep.convert_markdown demo.md demo.html
                state = SUCCEEDED
                 pool = markdown
           created by   step:./plan.py
             consumes   file:./
             consumes   file:demo.md
              creates   file:demo.html
+            supplies   file:demo.html
 
 file:demo.html
                 path = demo.html
                state = BUILT
           created by   step:python -m stepup.reprep.convert_markdown demo.md demo.html
             consumes   file:./
+            consumes   step:python -m stepup.reprep.convert_markdown demo.md demo.html
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_markdown/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/convert_markdown/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.convert_markdown demo.md demo.html
    SUCCESS │ python -m stepup.reprep.convert_markdown demo.md demo.html
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ demo.html
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_markdown/main.sh` & `stepup_reprep-1.1.0/tests/cases/convert_markdown/main.sh`

 * *Files 9% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv demo.html demo1.html
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("demo.html")
+watch_delete("demo.html")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["demo.html", "demo1.html"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_mutool/example.pdf` & `stepup_reprep-1.1.0/tests/cases/convert_mutool/example.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_mutool/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -43,13 +43,15 @@
              workdir = ./
              command = mutool draw -q -o example.png -r 100 example.pdf
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:example.pdf
              creates   file:example.png
+            supplies   file:example.png
 
 file:example.png
                 path = example.png
                state = BUILT
           created by   step:mutool draw -q -o example.png -r 100 example.pdf
             consumes   file:./
+            consumes   step:mutool draw -q -o example.png -r 100 example.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_mutool/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/convert_mutool/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mutool draw -q -o example.png -r 100 example.pdf
    SUCCESS │ mutool draw -q -o example.png -r 100 example.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ example.png
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_mutool/main.sh` & `stepup_reprep-1.1.0/tests/cases/convert_mutool/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv example.png example1.png
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("example.png")
+watch_delete("example.png")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["example.png", "example1.png"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_weasyprint/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -42,13 +42,15 @@
              workdir = ./
              command = weasyprint doc.html doc.pdf
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:doc.html
              creates   file:doc.pdf
+            supplies   file:doc.pdf
 
 file:doc.pdf
                 path = doc.pdf
                state = BUILT
           created by   step:weasyprint doc.html doc.pdf
             consumes   file:./
+            consumes   step:weasyprint doc.html doc.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_weasyprint/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/convert_weasyprint/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ weasyprint doc.html doc.pdf
    SUCCESS │ weasyprint doc.html doc.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ doc.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/convert_weasyprint/main.sh` & `stepup_reprep-1.1.0/tests/cases/nup_pdf/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
-mv doc.pdf doc1.pdf
+mv dst.pdf dst1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("doc.pdf")
+watch_delete("dst.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["doc.pdf", "doc1.pdf"])
+write_manifest("reproducibility_manifest.txt", ["dst.pdf", "dst1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f doc.html ]] || exit -1
-[[ -f doc.pdf ]] || exit -1
-[[ -f doc1.pdf ]] || exit -1
+[[ -f src.pdf ]] || exit -1
+[[ -f dst.pdf ]] || exit -1
+[[ -f dst1.pdf ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_diff/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/latex_diff/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,15 @@
              command = latexdiff --append-context2cmd=abstract,supplementary,dataavailability,funding,authorcontributions,conflictsofinterest,abbreviations old.tex new.tex --no-label > diff.tex
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:new.tex
             consumes   file:old.tex
              creates   file:diff.tex
+            supplies   file:diff.tex
 
 file:diff.tex
                 path = diff.tex
                state = BUILT
           created by   step:latexdiff --append-context2cmd=abstract,supplementary,dataavailability,funding,authorcontributions,conflictsofinterest,abbreviations old.tex new.tex --no-label > diff.tex
             consumes   file:./
+            consumes   step:latexdiff --append-context2cmd=abstract,supplementary,dataavailability,funding,authorcontributions,conflictsofinterest,abbreviations old.tex new.tex --no-label > diff.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_diff/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/latex_diff/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ latexdiff --append-context2cmd=abstract,supplementary,dataavailability,funding,authorcontributions,conflictsofinterest,abbreviations old.tex new.tex --no-label > diff.tex
    SUCCESS │ latexdiff --append-context2cmd=abstract,supplementary,dataavailability,funding,authorcontributions,conflictsofinterest,abbreviations old.tex new.tex --no-label > diff.tex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ diff.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_diff/main.sh` & `stepup_reprep-1.1.0/tests/cases/latex_diff/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv diff.tex diff1.tex
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("diff.tex")
+watch_delete("diff.tex")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["diff.tex", "diff1.tex"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_flat/expected_graph_01.txt` & `stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_01.txt`

 * *Files 5% similar despite different names*

```diff
@@ -67,20 +67,22 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:article_structured.tex
             consumes   file:part1.tex
             consumes   file:part2.tex
             consumes   (file:sub/other.tex)
              creates   file:article.tex
+            supplies   file:article.tex
 
 file:article.tex
                 path = article.tex
                state = PENDING
           created by   step:python -m stepup.reprep.latex_flat article_structured.tex article.tex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex_flat article_structured.tex article.tex
 
 (file:sub/other.tex)
                 path = sub/other.tex
                state = PENDING
             consumes   (file:sub/)
             supplies   step:python -m stepup.reprep.latex_flat article_structured.tex article.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_flat/expected_graph_02.txt` & `stepup_reprep-1.1.0/tests/cases/latex_flat/expected_graph_02.txt`

 * *Files 2% similar despite different names*

```diff
@@ -69,20 +69,22 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:article_structured.tex
             consumes   file:part1.tex
             consumes   file:part2.tex
             consumes   file:sub/other.tex
              creates   file:article.tex
+            supplies   file:article.tex
 
 file:article.tex
                 path = article.tex
                state = BUILT
           created by   step:python -m stepup.reprep.latex_flat article_structured.tex article.tex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex_flat article_structured.tex article.tex
 
 file:sub/other.tex
                 path = sub/other.tex
                state = STATIC
           created by   step:./plan.py
             consumes   file:sub/
             supplies   step:python -m stepup.reprep.latex_flat article_structured.tex article.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_flat/expected_stdout_01.txt` & `stepup_reprep-1.1.0/tests/cases/latex_flat/expected_stdout_01.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex_flat article_structured.tex article.tex
 RESCHEDULE │ python -m stepup.reprep.latex_flat article_structured.tex article.tex
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.latex_flat article_structured.tex article.tex
 Return code           255
 ──────────────── Rescheduling due to unavailable amended inputs ────────────────
 sub/other.tex
 ──────────────────────────────── Standard error ────────────────────────────────
-Could not locate input file 'sub/other.tex' on line 6 in 'article_structured.tex'
+(stripped)
 ────────────────────────────────────────────────────────────────────────────────
    WARNING │ 1 step remains pending due to incomplete requirements
 ───────────────────────────────── PENDING Step ─────────────────────────────────
 Command               python -m stepup.reprep.latex_flat article_structured.tex article.tex
 Working directory     ./
 Inputs        STATIC  ./
               STATIC  article_structured.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_flat/main.sh` & `stepup_reprep-1.1.0/tests/cases/latex_flat/main.sh`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 stepup -w 1 plan.py & # > current_stdout_01.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 print("HERE")
 wait()
-graph("current_graph_01.txt")
+graph("current_graph_01")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f article_structured.tex ]] || exit -1
 [[ ! -f article.tex ]] || exit -1
@@ -28,15 +28,15 @@
 # Add the missing file and run again
 cp plan_02.py plan.py
 cp sub/original.tex sub/other.tex
 stepup -w 1 plan.py & # > current_stdout_02.txt &
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph_02.txt")
+graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f article_structured.tex ]] || exit -1
 [[ -f article.tex ]] || exit -1
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/expected_graph.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,13 +74,15 @@
           created by   step:./plan.py
             consumes   file:./
             consumes   file:sub/
             consumes   file:sub/article_structured.tex
             consumes   file:sub/part1.tex
             consumes   file:sub/part2.tex
              creates   file:sub/article.tex
+            supplies   file:sub/article.tex
 
 file:sub/article.tex
                 path = sub/article.tex
                state = BUILT
           created by   step:python -m stepup.reprep.latex_flat sub/article_structured.tex sub/article.tex
             consumes   file:sub/
+            consumes   step:python -m stepup.reprep.latex_flat sub/article_structured.tex sub/article.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/latex_flat_subdir/main.sh` & `stepup_reprep-1.1.0/tests/cases/latex_flat_subdir/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f sub/article_structured.tex ]] || exit -1
 [[ -f sub/part1.tex ]] || exit -1
```

### Comparing `stepup_reprep-1.0.0/tests/cases/lualatex_simple/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_graph.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,40 +41,48 @@
             consumes   file:./
             supplies   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 step:python -m stepup.reprep.latex paper.tex --run-bibtex
              workdir = ./
              command = python -m stepup.reprep.latex paper.tex --run-bibtex
                state = SUCCEEDED
-   creates (amended) = file:paper.log
+  supplies (amended) = file:paper.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:paper.tex
              creates   file:paper.MANIFEST.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.pdf
+            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper.aux
+            supplies   file:paper.log
+            supplies   file:paper.pdf
 
 file:paper.MANIFEST.txt
                 path = paper.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.pdf
                 path = paper.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.log
                 path = paper.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/lualatex_simple/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/lualatex_simple/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ paper.aux
```

### Comparing `stepup_reprep-1.0.0/tests/cases/lualatex_simple/main.sh` & `stepup_reprep-1.1.0/tests/cases/pdflatex_input/main.sh`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
-export REPREP_LATEX="lualatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log
+rm paper.aux paper.log generated.tex
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("paper.pdf")
+watch_delete("paper.pdf")
+watch_delete("generated.tex")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/make_manifest_in/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/make_manifest_in/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,13 +58,15 @@
              workdir = ./
              command = reprep-make-manifest -i MANIFEST.in
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:MANIFEST.in
              creates   file:MANIFEST.txt
+            supplies   file:MANIFEST.txt
 
 file:MANIFEST.txt
                 path = MANIFEST.txt
                state = BUILT
           created by   step:reprep-make-manifest -i MANIFEST.in
             consumes   file:./
+            consumes   step:reprep-make-manifest -i MANIFEST.in
```

### Comparing `stepup_reprep-1.0.0/tests/cases/make_manifest_in/main.sh` & `stepup_reprep-1.1.0/tests/cases/make_manifest_in/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/expected_graph.txt`

 * *Files 13% similar despite different names*

```diff
@@ -60,13 +60,15 @@
              command = reprep-make-manifest -i sub/MANIFEST.in
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:sub/
             consumes   file:sub/MANIFEST.in
              creates   file:sub/MANIFEST.txt
+            supplies   file:sub/MANIFEST.txt
 
 file:sub/MANIFEST.txt
                 path = sub/MANIFEST.txt
                state = BUILT
           created by   step:reprep-make-manifest -i sub/MANIFEST.in
             consumes   file:sub/
+            consumes   step:reprep-make-manifest -i sub/MANIFEST.in
```

### Comparing `stepup_reprep-1.0.0/tests/cases/make_manifest_in_sub/main.sh` & `stepup_reprep-1.1.0/tests/cases/make_manifest_list/main.sh`

 * *Files 17% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f sub/hello.txt ]] || exit -1
-[[ -f sub/MANIFEST.txt ]] || exit -1
-reprep-check-manifest sub/MANIFEST.txt
-mv sub/MANIFEST.txt current_manifest.txt
+[[ -f README.md ]] || exit -1
+[[ -f MANIFEST.txt ]] || exit -1
+mv MANIFEST.txt current_manifest.txt
```

### Comparing `stepup_reprep-1.0.0/tests/cases/make_manifest_list/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/make_manifest_list/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -42,13 +42,15 @@
              workdir = ./
              command = reprep-make-manifest README.md -o MANIFEST.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:README.md
              creates   file:MANIFEST.txt
+            supplies   file:MANIFEST.txt
 
 file:MANIFEST.txt
                 path = MANIFEST.txt
                state = BUILT
           created by   step:reprep-make-manifest README.md -o MANIFEST.txt
             consumes   file:./
+            consumes   step:reprep-make-manifest README.md -o MANIFEST.txt
```

### Comparing `stepup_reprep-1.0.0/tests/cases/make_manifest_list/main.sh` & `stepup_reprep-1.1.0/tests/cases/make_manifest_in_sub/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f README.md ]] || exit -1
-[[ -f MANIFEST.txt ]] || exit -1
-mv MANIFEST.txt current_manifest.txt
+[[ -f sub/hello.txt ]] || exit -1
+[[ -f sub/MANIFEST.txt ]] || exit -1
+reprep-check-manifest sub/MANIFEST.txt
+mv sub/MANIFEST.txt current_manifest.txt
```

### Comparing `stepup_reprep-1.0.0/tests/cases/nup_pdf/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,13 +45,15 @@
    env_var (amended) = REPREP_NUP_MARGIN
                      = REPREP_NUP_NCOL
                      = REPREP_NUP_NROW
           created by   step:./plan.py
             consumes   file:./
             consumes   file:src.pdf
              creates   file:dst.pdf
+            supplies   file:dst.pdf
 
 file:dst.pdf
                 path = dst.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.nup_pdf src.pdf dst.pdf -p A4
             consumes   file:./
+            consumes   step:python -m stepup.reprep.nup_pdf src.pdf dst.pdf -p A4
```

### Comparing `stepup_reprep-1.0.0/tests/cases/nup_pdf/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/nup_pdf/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.nup_pdf src.pdf dst.pdf -p A4
    SUCCESS │ python -m stepup.reprep.nup_pdf src.pdf dst.pdf -p A4
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ dst.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/nup_pdf/main.sh` & `stepup_reprep-1.1.0/tests/cases/convert_weasyprint/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
-mv dst.pdf dst1.pdf
+mv doc.pdf doc1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("dst.pdf")
+watch_delete("doc.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["dst.pdf", "dst1.pdf"])
+write_manifest("reproducibility_manifest.txt", ["doc.pdf", "doc1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f src.pdf ]] || exit -1
-[[ -f dst.pdf ]] || exit -1
-[[ -f dst1.pdf ]] || exit -1
+[[ -f doc.html ]] || exit -1
+[[ -f doc.pdf ]] || exit -1
+[[ -f doc1.pdf ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.0.0/tests/cases/nup_pdf/src.pdf` & `stepup_reprep-1.1.0/tests/cases/nup_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_graph.txt`

 * *Files 8% similar despite different names*

```diff
@@ -51,41 +51,49 @@
             supplies   step:python -m stepup.reprep.latex paper.tex
 
 step:python -m stepup.reprep.latex paper.tex
              workdir = ./
              command = python -m stepup.reprep.latex paper.tex
                state = SUCCEEDED
   consumes (amended) = file:paper.bbl
-   creates (amended) = file:paper.log
+  supplies (amended) = file:paper.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:paper.bbl
             consumes   file:paper.tex
              creates   file:paper.MANIFEST.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.pdf
+            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper.aux
+            supplies   file:paper.log
+            supplies   file:paper.pdf
 
 file:paper.MANIFEST.txt
                 path = paper.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
 
 file:paper.aux
                 path = paper.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
 
 file:paper.pdf
                 path = paper.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
 
 file:paper.log
                 path = paper.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex
    SUCCESS │ python -m stepup.reprep.latex paper.tex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ paper.aux
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_bbl/main.sh` & `stepup_reprep-1.1.0/tests/cases/pdflatex_bbl/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 export SOURCE_DATE_EPOCH"315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 rm paper.aux paper.log
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("paper.pdf")
+watch_delete("paper.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_graph.txt`

 * *Files 10% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 step:python -m stepup.reprep.latex paper.tex --run-bibtex
              workdir = ./
              command = python -m stepup.reprep.latex paper.tex --run-bibtex
                state = SUCCEEDED
   consumes (amended) = file:bibsane.yaml
                      = file:references.bib
-   creates (amended) = file:paper.bbl
+  supplies (amended) = file:paper.bbl
                      = file:paper.blg
                      = file:paper.log
    env_var (amended) = REPREP_BIBSANE
                      = REPREP_BIBSANE_CONFIG
                      = REPREP_BIBTEX
                      = REPREP_LATEX
                      = ROOT
@@ -83,43 +83,55 @@
             consumes   file:references.bib
              creates   file:paper.MANIFEST.txt
              creates   file:paper.aux
              creates   file:paper.bbl
              creates   file:paper.blg
              creates   file:paper.log
              creates   file:paper.pdf
+            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper.aux
+            supplies   file:paper.bbl
+            supplies   file:paper.blg
+            supplies   file:paper.log
+            supplies   file:paper.pdf
 
 file:paper.MANIFEST.txt
                 path = paper.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.pdf
                 path = paper.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.bbl
                 path = paper.bbl
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.blg
                 path = paper.blg
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.log
                 path = paper.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ paper.aux
-   DELETED │ paper.bbl
    DELETED │ paper.pdf
+   DELETED │ paper.bbl
      PHASE │ run
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_bibtex/main.sh` & `stepup_reprep-1.1.0/tests/cases/pdflatex_bibtex/main.sh`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 export LATEX_MAIN="paper"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 rm paper.aux paper.log
 mv paper.pdf paper1.pdf
 mv paper.bbl paper1.bbl
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("paper.pdf")
-watch_del("paper.bbl")
+watch_delete("paper.pdf")
+watch_delete("paper.bbl")
 run()
 join()
 write_manifest("reproducibility_pdf_manifest.txt", ["paper.pdf", "paper1.pdf"])
 write_manifest("reproducibility_bbl_manifest.txt", ["paper.bbl", "paper1.bbl"])
 EOD
 
 # Wait for background processes, if any.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_input/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_graph.txt`

 * *Files 19% similar despite different names*

```diff
@@ -55,57 +55,67 @@
 
 step:python -m stepup.reprep.latex paper.tex --run-bibtex
              workdir = ./
              command = python -m stepup.reprep.latex paper.tex --run-bibtex
                state = SUCCEEDED
   consumes (amended) = file:generated.tex
                      = file:smile.pdf
-   creates (amended) = file:paper.log
+  supplies (amended) = file:paper.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:generated.tex
             consumes   file:paper.tex
             consumes   file:smile.pdf
              creates   file:paper.MANIFEST.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.pdf
+            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper.aux
+            supplies   file:paper.log
+            supplies   file:paper.pdf
 
 file:paper.MANIFEST.txt
                 path = paper.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.pdf
                 path = paper.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 step:echo 'Hi there!' > generated.tex
              workdir = ./
              command = echo 'Hi there!' > generated.tex
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:generated.tex
+            supplies   file:generated.tex
 
 file:generated.tex
                 path = generated.tex
                state = BUILT
           created by   step:echo 'Hi there!' > generated.tex
             consumes   file:./
+            consumes   step:echo 'Hi there!' > generated.tex
             supplies   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.log
                 path = paper.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_input/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/pdflatex_input/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
 RESCHEDULE │ python -m stepup.reprep.latex paper.tex --run-bibtex
 ────────────────────────────────── Step info ───────────────────────────────────
 Command               python -m stepup.reprep.latex paper.tex --run-bibtex
 Return code           0
@@ -12,16 +12,16 @@
 ────────────────────────────────────────────────────────────────────────────────
      START │ echo 'Hi there!' > generated.tex
    SUCCESS │ echo 'Hi there!' > generated.tex
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
-   DELETED │ generated.tex
    DELETED │ paper.aux
+   DELETED │ generated.tex
    DELETED │ paper.pdf
      PHASE │ run
      START │ echo 'Hi there!' > generated.tex
    SUCCESS │ echo 'Hi there!' > generated.tex
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_input/main.sh` & `stepup_reprep-1.1.0/tests/cases/xelatex_input/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
+export REPREP_LATEX="xelatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log generated.tex
+rm paper.aux
+rm paper.log
+rm subdir/generated.tex
+rm subdir/code.txt
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("paper.pdf")
-watch_del("generated.tex")
+watch_delete("paper.pdf")
+watch_delete("subdir/generated.tex")
+watch_delete("subdir/code.txt")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/pdflatex_input/smile.pdf` & `stepup_reprep-1.1.0/tests/cases/pdflatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/raster_pdf/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_graph.txt`

 * *Files 11% similar despite different names*

```diff
@@ -43,33 +43,37 @@
 step:mkdir -p rastered/
              workdir = ./
              command = mkdir -p rastered/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:rastered/
+            supplies   file:rastered/
 
 file:rastered/
                 path = rastered/
                state = BUILT
           created by   step:mkdir -p rastered/
             consumes   file:./
+            consumes   step:mkdir -p rastered/
             supplies   file:rastered/smile.pdf
             supplies   step:python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
 
 step:python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
              workdir = ./
              command = python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_RASTER_QUALITY
                      = REPREP_RASTER_RESOLUTION
           created by   step:./plan.py
             consumes   file:./
             consumes   file:rastered/
             consumes   file:smile.pdf
              creates   file:rastered/smile.pdf
+            supplies   file:rastered/smile.pdf
 
 file:rastered/smile.pdf
                 path = rastered/smile.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
             consumes   file:rastered/
+            consumes   step:python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
```

### Comparing `stepup_reprep-1.0.0/tests/cases/raster_pdf/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/raster_pdf/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mkdir -p rastered/
    SUCCESS │ mkdir -p rastered/
      START │ python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
    SUCCESS │ python -m stepup.reprep.raster_pdf smile.pdf rastered/smile.pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
```

### Comparing `stepup_reprep-1.0.0/tests/cases/raster_pdf/main.sh` & `stepup_reprep-1.1.0/tests/cases/raster_pdf/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv rastered/smile.pdf rastered/smile1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("rastered/smile.pdf")
+watch_delete("rastered/smile.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["rastered/smile.pdf", "rastered/smile1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/raster_pdf/smile.pdf` & `stepup_reprep-1.1.0/tests/cases/raster_pdf/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/render_basic/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/render_basic/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -53,13 +53,15 @@
                state = SUCCEEDED
    env_var (amended) = ENV_VAR_TEST_STEPUP_RENDER
           created by   step:./plan.py
             consumes   file:./
             consumes   file:template.md
             consumes   file:variables.py
              creates   file:rendered.md
+            supplies   file:rendered.md
 
 file:rendered.md
                 path = rendered.md
                state = BUILT
           created by   step:python -m stepup.reprep.render template.md variables.py rendered.md
             consumes   file:./
+            consumes   step:python -m stepup.reprep.render template.md variables.py rendered.md
```

### Comparing `stepup_reprep-1.0.0/tests/cases/render_basic/main.sh` & `stepup_reprep-1.1.0/tests/cases/render_basic/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 export ENV_VAR_TEST_STEPUP_RENDER="cool"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/render_relpath/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/render_relpath/expected_graph.txt`

 * *Files 9% similar despite different names*

```diff
@@ -56,20 +56,22 @@
 step:mkdir -p public/
              workdir = ./
              command = mkdir -p public/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:public/
+            supplies   file:public/
 
 file:public/
                 path = public/
                state = BUILT
           created by   step:mkdir -p public/
             consumes   file:./
+            consumes   step:mkdir -p public/
             supplies   file:public/main.MANIFEST.txt
             supplies   file:public/main.aux
             supplies   file:public/main.log
             supplies   file:public/main.pdf
             supplies   file:public/main.tex
             supplies   file:public/preamble.inc.tex
             supplies   step:cp -aT static/preamble.inc.tex public/preamble.inc.tex
@@ -82,14 +84,15 @@
                state = SUCCEEDED
            mandatory = IMPLIED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:public/
             consumes   file:static/preamble.inc.tex
              creates   file:public/preamble.inc.tex
+            supplies   file:public/preamble.inc.tex
 
 file:static/preamble.inc.tex
                 path = static/preamble.inc.tex
                state = STATIC
           created by   dg:'static/**'
             consumes   file:static/
             supplies   step:cp -aT static/preamble.inc.tex public/preamble.inc.tex
@@ -107,14 +110,15 @@
             supplies   step:python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
 
 file:public/preamble.inc.tex
                 path = public/preamble.inc.tex
                state = BUILT
           created by   step:cp -aT static/preamble.inc.tex public/preamble.inc.tex
             consumes   file:public/
+            consumes   step:cp -aT static/preamble.inc.tex public/preamble.inc.tex
             supplies   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 
 step:./plan.py  # wd=static/
              workdir = static/
              command = ./plan.py
                state = SUCCEEDED
    env_var (amended) = PUBLIC
@@ -141,14 +145,15 @@
           created by   step:./plan.py  # wd=static/
             consumes   file:public/
             consumes   file:static/
             consumes   file:static/main.tex
             consumes   file:static/variables.py
             consumes   file:variables.py
              creates   file:public/main.tex
+            supplies   file:public/main.tex
 
 file:static/main.tex
                 path = static/main.tex
                state = STATIC
           created by   dg:'static/**'
             consumes   file:static/
             supplies   step:python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
@@ -161,48 +166,57 @@
             supplies   step:python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
 
 file:public/main.tex
                 path = public/main.tex
                state = BUILT
           created by   step:python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
             consumes   file:public/
+            consumes   step:python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
             supplies   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 
 step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
              workdir = public/
              command = python -m stepup.reprep.latex main.tex --run-bibtex
                state = SUCCEEDED
   consumes (amended) = file:public/preamble.inc.tex
-   creates (amended) = file:public/main.log
+  supplies (amended) = file:public/main.log
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py  # wd=static/
             consumes   file:public/
             consumes   file:public/main.tex
             consumes   file:public/preamble.inc.tex
              creates   file:public/main.MANIFEST.txt
              creates   file:public/main.aux
              creates   file:public/main.log
              creates   file:public/main.pdf
+            supplies   file:public/main.MANIFEST.txt
+            supplies   file:public/main.aux
+            supplies   file:public/main.log
+            supplies   file:public/main.pdf
 
 file:public/main.MANIFEST.txt
                 path = public/main.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
             consumes   file:public/
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 
 file:public/main.aux
                 path = public/main.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
             consumes   file:public/
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 
 file:public/main.pdf
                 path = public/main.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
             consumes   file:public/
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
 
 file:public/main.log
                 path = public/main.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
             consumes   file:public/
+            consumes   step:python -m stepup.reprep.latex main.tex --run-bibtex  # wd=public/
```

### Comparing `stepup_reprep-1.0.0/tests/cases/render_relpath/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/render_relpath/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mkdir -p public/
    SUCCESS │ mkdir -p public/
      START │ ./plan.py  # wd=static/
    SUCCESS │ ./plan.py  # wd=static/
      START │ python -m stepup.reprep.render main.tex ../variables.py variables.py ../public/main.tex  # wd=static/
```

### Comparing `stepup_reprep-1.0.0/tests/cases/render_relpath/main.sh` & `stepup_reprep-1.1.0/tests/cases/render_relpath/main.sh`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 export PUBLIC="public/"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
 
 # Check files that are expected to be present and/or missing.
```

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -214,105 +214,117 @@
              command = inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
             consumes   file:./
             consumes   file:hexagon.svg
              creates   file:hexagon.pdf
+            supplies   file:hexagon.pdf
 
 file:hexagon.pdf
                 path = hexagon.pdf
                state = BUILT
           created by   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
              workdir = ./
              command = inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
             consumes   file:./
             consumes   file:horizontal.svg
              creates   file:horizontal.pdf
+            supplies   file:horizontal.pdf
 
 file:horizontal.pdf
                 path = horizontal.pdf
                state = BUILT
           created by   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
              workdir = ./
              command = inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
             consumes   file:./
             consumes   file:pentagon.svg
              creates   file:pentagon.pdf
+            supplies   file:pentagon.pdf
 
 file:pentagon.pdf
                 path = pentagon.pdf
                state = BUILT
           created by   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
              workdir = ./
              command = inkscape square.svg  --export-filename=square.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
             consumes   file:./
             consumes   file:square.svg
              creates   file:square.pdf
+            supplies   file:square.pdf
 
 file:square.pdf
                 path = square.pdf
                state = BUILT
           created by   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
              workdir = ./
              command = inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
             consumes   file:./
             consumes   file:triangle.svg
              creates   file:triangle.pdf
+            supplies   file:triangle.pdf
 
 file:triangle.pdf
                 path = triangle.pdf
                state = BUILT
           created by   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
              workdir = ./
              command = inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
                state = SUCCEEDED
                 pool = inkscape
           created by   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
             consumes   file:./
             consumes   file:vertical.svg
              creates   file:vertical.pdf
+            supplies   file:vertical.pdf
 
 file:vertical.pdf
                 path = vertical.pdf
                state = BUILT
           created by   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             consumes   file:./
+            consumes   step:inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:./tile.py run
              workdir = ./
              command = ./tile.py run
                state = SUCCEEDED
           created by   step:./tile.py plan
@@ -322,13 +334,15 @@
             consumes   file:pentagon.pdf
             consumes   file:square.pdf
             consumes   file:tile.py
             consumes   file:triangle.pdf
             consumes   file:vera.ttf
             consumes   file:vertical.pdf
              creates   file:figure.pdf
+            supplies   file:figure.pdf
 
 file:figure.pdf
                 path = figure.pdf
                state = BUILT
           created by   step:./tile.py run
             consumes   file:./
+            consumes   step:./tile.py run
```

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/expected_stdout.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
      START │ inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
    SUCCESS │ inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
      START │ python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
@@ -27,16 +27,34 @@
      START │ inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
    SUCCESS │ inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
      START │ ./tile.py plan
    SUCCESS │ ./tile.py plan
      START │ ./tile.py run
    SUCCESS │ ./tile.py run
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
+   UPDATED │ hexagon.svg
+   UPDATED │ horizontal.svg
+   UPDATED │ pentagon.svg
+   UPDATED │ square.svg
+   UPDATED │ triangle.svg
+   UPDATED │ vertical.svg
      PHASE │ watch
    DELETED │ figure.pdf
      PHASE │ run
+      SKIP │ python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
+      SKIP │ python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
+      SKIP │ python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
+      SKIP │ python -m stepup.reprep.convert_inkscape square.svg square.pdf
+      SKIP │ python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
+      SKIP │ python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
+      SKIP │ inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+      SKIP │ inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+      SKIP │ inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+      SKIP │ inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+      SKIP │ inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+      SKIP │ inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
      START │ ./tile.py run
    SUCCESS │ ./tile.py run
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/hexagon.svg` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/horizontal.svg` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/horizontal.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/main.sh` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 export PUBLIC="public/"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 mv figure.pdf figure1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("figure.pdf")
+watch_delete("figure.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["figure.pdf", "figure1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/pentagon.svg` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/square.svg` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/tile.py` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/tile.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/triangle.svg` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/vera.ttf` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/vera.ttf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/tile_pdf/vertical.svg` & `stepup_reprep-1.1.0/tests/cases/tile_pdf/vertical.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/xelatex_input/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_graph.txt`

 * *Files 14% similar despite different names*

```diff
@@ -52,99 +52,115 @@
 step:mkdir -p subdir/
              workdir = ./
              command = mkdir -p subdir/
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:subdir/
+            supplies   file:subdir/
 
 file:subdir/
                 path = subdir/
                state = BUILT
           created by   step:mkdir -p subdir/
             consumes   file:./
+            consumes   step:mkdir -p subdir/
             supplies   file:subdir/code.txt
             supplies   file:subdir/generated.tex
             supplies   step:echo '2 + 2' > subdir/code.txt
             supplies   step:echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
 
 step:python -m stepup.reprep.latex paper.tex --run-bibtex
              workdir = ./
              command = python -m stepup.reprep.latex paper.tex --run-bibtex
                state = SUCCEEDED
   consumes (amended) = file:subdir/code.txt
                      = file:subdir/generated.tex
-   creates (amended) = file:paper.log
+  supplies (amended) = file:paper.log
                      = file:paper.out
    env_var (amended) = REPREP_LATEX
           created by   step:./plan.py
             consumes   file:./
             consumes   file:paper.tex
             consumes   file:subdir/code.txt
             consumes   file:subdir/generated.tex
              creates   file:paper.MANIFEST.txt
              creates   file:paper.aux
              creates   file:paper.log
              creates   file:paper.out
              creates   file:paper.pdf
+            supplies   file:paper.MANIFEST.txt
+            supplies   file:paper.aux
+            supplies   file:paper.log
+            supplies   file:paper.out
+            supplies   file:paper.pdf
 
 file:paper.MANIFEST.txt
                 path = paper.MANIFEST.txt
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.aux
                 path = paper.aux
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.pdf
                 path = paper.pdf
                state = BUILT
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 step:echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
              workdir = ./
              command = echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:subdir/
              creates   file:subdir/generated.tex
+            supplies   file:subdir/generated.tex
 
 file:subdir/generated.tex
                 path = subdir/generated.tex
                state = BUILT
           created by   step:echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
             consumes   file:subdir/
+            consumes   step:echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
             supplies   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 step:echo '2 + 2' > subdir/code.txt
              workdir = ./
              command = echo '2 + 2' > subdir/code.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:subdir/
              creates   file:subdir/code.txt
+            supplies   file:subdir/code.txt
 
 file:subdir/code.txt
                 path = subdir/code.txt
                state = BUILT
           created by   step:echo '2 + 2' > subdir/code.txt
             consumes   file:subdir/
+            consumes   step:echo '2 + 2' > subdir/code.txt
             supplies   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.log
                 path = paper.log
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
 
 file:paper.out
                 path = paper.out
                state = VOLATILE
           created by   step:python -m stepup.reprep.latex paper.tex --run-bibtex
             consumes   file:./
+            consumes   step:python -m stepup.reprep.latex paper.tex --run-bibtex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/xelatex_input/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/xelatex_input/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ mkdir -p subdir/
    SUCCESS │ mkdir -p subdir/
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
 RESCHEDULE │ python -m stepup.reprep.latex paper.tex --run-bibtex
 ────────────────────────────────── Step info ───────────────────────────────────
@@ -17,17 +17,17 @@
      START │ echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
    SUCCESS │ echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ paper.aux
-   DELETED │ paper.pdf
-   DELETED │ subdir/code.txt
    DELETED │ subdir/generated.tex
+   DELETED │ subdir/code.txt
+   DELETED │ paper.pdf
      PHASE │ run
      START │ echo '2 + 2' > subdir/code.txt
    SUCCESS │ echo '2 + 2' > subdir/code.txt
      START │ echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
    SUCCESS │ echo 'Verbatim input:\verbatiminput{code.txt}' > subdir/generated.tex
      START │ python -m stepup.reprep.latex paper.tex --run-bibtex
    SUCCESS │ python -m stepup.reprep.latex paper.tex --run-bibtex
```

### Comparing `stepup_reprep-1.0.0/tests/cases/xelatex_input/main.sh` & `stepup_reprep-1.1.0/tests/cases/lualatex_simple/main.sh`

 * *Files 17% similar despite different names*

```diff
@@ -2,33 +2,31 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
-export REPREP_LATEX="xelatex"
+export REPREP_LATEX="lualatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log subdir/generated.tex subdir/code.txt
+rm paper.aux paper.log
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("paper.pdf")
-watch_del("subdir/generated.tex")
-watch_del("subdir/code.txt")
+watch_delete("paper.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/cases/xelatex_input/smile.pdf` & `stepup_reprep-1.1.0/tests/cases/xelatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/cases/zip_manifest/expected_graph.txt` & `stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_graph.txt`

 * *Files 2% similar despite different names*

```diff
@@ -47,46 +47,52 @@
 step:echo hello > built.txt
              workdir = ./
              command = echo hello > built.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
              creates   file:built.txt
+            supplies   file:built.txt
 
 file:built.txt
                 path = built.txt
                state = BUILT
           created by   step:echo hello > built.txt
             consumes   file:./
+            consumes   step:echo hello > built.txt
             supplies   step:reprep-make-manifest static.txt built.txt -o MANIFEST.txt
 
 step:reprep-make-manifest static.txt built.txt -o MANIFEST.txt
              workdir = ./
              command = reprep-make-manifest static.txt built.txt -o MANIFEST.txt
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:built.txt
             consumes   file:static.txt
              creates   file:MANIFEST.txt
+            supplies   file:MANIFEST.txt
 
 file:MANIFEST.txt
                 path = MANIFEST.txt
                state = BUILT
           created by   step:reprep-make-manifest static.txt built.txt -o MANIFEST.txt
             consumes   file:./
+            consumes   step:reprep-make-manifest static.txt built.txt -o MANIFEST.txt
             supplies   step:python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
 
 step:python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
              workdir = ./
              command = python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:MANIFEST.txt
              creates   file:upload.zip
+            supplies   file:upload.zip
 
 file:upload.zip
                 path = upload.zip
                state = BUILT
           created by   step:python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
             consumes   file:./
+            consumes   step:python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
```

### Comparing `stepup_reprep-1.0.0/tests/cases/zip_manifest/expected_stdout.txt` & `stepup_reprep-1.1.0/tests/cases/zip_manifest/expected_stdout.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-     PHASE │ run
   DIRECTOR │ Launched worker 0
+     PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ echo hello > built.txt
    SUCCESS │ echo hello > built.txt
      START │ reprep-make-manifest static.txt built.txt -o MANIFEST.txt
    SUCCESS │ reprep-make-manifest static.txt built.txt -o MANIFEST.txt
      START │ python -m stepup.reprep.zip_manifest MANIFEST.txt upload.zip
```

### Comparing `stepup_reprep-1.0.0/tests/cases/zip_manifest/main.sh` & `stepup_reprep-1.1.0/tests/cases/zip_manifest/main.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
-graph("current_graph.txt")
+graph("current_graph")
 EOD
 
 # Reproducibility test
 rm built.txt
 mv upload.zip upload1.zip
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_del("upload.zip")
+watch_delete("upload.zip")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["upload.zip", "upload1.zip"])
 EOD
 
 # Wait for background processes, if any.
 wait $(jobs -p)
```

### Comparing `stepup_reprep-1.0.0/tests/conftest.py` & `stepup_reprep-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/reprep_common.py` & `stepup_reprep-1.1.0/tests/reprep_common.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/test_bibtex_log.py` & `stepup_reprep-1.1.0/tests/test_bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/test_cases.py` & `stepup_reprep-1.1.0/tests/test_cases.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 @pytest.mark.parametrize(
     "name",
     [
         "add_notes_pdf",
         "check_hrefs_html",
         "check_hrefs_md",
-        "check_hrefs_pdf",
         "convert_markdown",
         "convert_weasyprint",
         "latex_flat",
         "latex_flat_subdir",
         "make_manifest_in",
         "make_manifest_in_sub",
         "make_manifest_list",
@@ -84,14 +83,15 @@
     return True
 
 
 @pytest.mark.skipif(not has_texlive_2023(), reason="No TeX Live 2023")
 @pytest.mark.parametrize(
     "name",
     [
+        "check_hrefs_pdf",
         "latex_diff",
         "lualatex_simple",
         "pdflatex_bbl",
         "pdflatex_bibtex",
         "pdflatex_input",
         "render_relpath",
         "xelatex_input",
```

### Comparing `stepup_reprep-1.0.0/tests/test_latex_deps.py` & `stepup_reprep-1.1.0/tests/test_latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/test_latex_flat.py` & `stepup_reprep-1.1.0/tests/test_latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/test_latex_log.py` & `stepup_reprep-1.1.0/tests/test_latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/test_manifest.py` & `stepup_reprep-1.1.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.0.0/tests/test_zip.py` & `stepup_reprep-1.1.0/tests/test_zip.py`

 * *Files identical despite different names*

